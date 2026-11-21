# Network Addressing and Basic Troubleshooting - Módulo 3   <img src="../0-aux/logo_course.png" alt="sfp_009" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">sfp_009 (Network Addressing and Basic Troubleshooting)   <img src="../0-aux/logo_course.png" alt="sfp_009" width="auto" height="25"></a>
### Module: 3. Roteamento na camada de rede

---

### Theme:
- Network

### Used Tools:
- Operating System (OS): 
  - Windows 11 <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/windows11.png" alt="windows11" width="auto" height="25">
- Cloud Services:
  - Google Drive <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/google_drive.png" alt="google_drive" width="auto" height="25">
- Language:
  - HTML   <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" alt="html" width="auto" height="25">
  - Markdown   <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/markdown/markdown-original.svg" alt="markdown" width="auto" height="25">
- Integrated Development Environment (IDE) and Text Editor:
  - Visual Studio Code (VS Code)   <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" alt="vscode" width="auto" height="25">
- Versioning: 
  - Git   <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" alt="git" width="auto" height="25">
- Repository:
  - GitHub   <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="github" width="auto" height="25">

---

### Course Module 3 Structure:
3. <a name="item03">Roteamento na camada de rede</a><br>
  3.1 <a href="#item03.01">Introdução</a><br>
  3.2 <a href="#item03.02">Como um Host Roteia</a><br>
  3.3 <a href="#item03.03">Tabelas de Roteamento</a><br>
  3.4 <a href="#item03.04">Resumo da Roteamento na camada de rede</a><br>
  3.5 Exame de ponto de verificação: Camadas físicas, de enlace de dados e de rede<br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item03.01"><h4>3.1 Introdução</h4></a>[Back to summary](#item03)

🧭 Mecanismos de Encaminhamento e Tabelas de Roteamento   
A interconexão de múltiplas filiais e edifícios em uma infraestrutura corporativa unificada depende diretamente das decisões tomadas na camada de rede. Para que ocorra a comunicação de ponta a ponta — permitindo o tráfego de e-mails, acessos a servidores e transferências de arquivos entre localidades distantes —, os dispositivos finais e os roteadores precisam processar informações geográficas lógicas. Esse direcionamento estruturado garante que cada pacote de dados encontre a saída adequada e navegue pelo caminho correto até o seu destino final.

🎯 Objetivo do módulo:   
- Explicar os critérios técnicos utilizados por hosts e roteadores para processar e encaminhar pacotes de dados através de redes interconectadas.

📘 Tópicos do módulo:   
- Como um Host Roteia: Análise do comportamento dos dispositivos de origem ao utilizarem suas tabelas de decisão internas para discriminar entre tráfego local e tráfego destinado a redes remotas.
- Tabela de Roteamento: Estudo detalhado dos parâmetros, métricas e campos estruturais que compõem o banco de dados de um roteador, decodificando como o sistema operacional escolhe a melhor interface de saída.

<a name="item03.02"><h4>3.2 Como um Host Roteia</h4></a>[Back to summary](#item03)

🗺️ Escopos de Destino e Mecanismos de Decisão do Host   
Independentemente da infraestrutura operar sob o protocolo IPv4 ou IPv6, os pacotes de dados são estruturados na origem. Para viabilizar a entrega, o host emissor precisa determinar com precisão a localização do destinatário. Esse processo de triagem baseia-se na classificação do destino em três cenários lógicos:
- A Própria Interface (Loopback): Ocorre quando um host envia dados para si mesmo. Essa operação utiliza endereços lógicos reservados, sendo o 127.0.0.1 no IPv4 e o ::1 no IPv6 (representado também pela sub-rede ::/1). Disparar um teste de ping contra a interface de loopback serve para atestar que o subsistema de software da pilha de protocolos TCP/IP está instalado e respondendo corretamente no sistema operacional.
- Host Local (Mesma Sub-rede): Aplica-se quando a estação de destino reside no mesmo segmento físico e lógico da estação emissora. Nesse cenário, o dispositivo de origem e o de destino compartilham obrigatoriamente a mesma identidade de rede.
- Host Remoto (Redes Distantes): Caracteriza-se quando o destinatário encontra-se alocado em uma sub-rede externa. Nessa situação, as identidades de rede da origem e do destino são divergentes.

A responsabilidade por classificar o destino como local ou remoto recai sobre o próprio host de origem. O algoritmo de decisão varia conforme a versão do protocolo IP:
- No IPv4: O host realiza uma operação lógica bit a bit (AND) combinando o seu próprio endereço IPv4 com a sua máscara de sub-rede. Em seguida, ele aplica o mesmo cálculo ao IP de destino. Se os resultados forem idênticos, o destino é classificado como local.
- No IPv6: O processo é simplificado através das mensagens de anúncio de roteamento. Os roteadores locais propagam periodicamente o prefixo da rede local para todos os hosts conectados, permitindo que as estações identifiquem imediatamente se o IP de destino pertence ou não ao mesmo escopo.

Quando o destino é identificado como local, o tráfego flui sem a necessidade de intervenção de um roteador. Em redes residenciais ou corporativas, switches LAN e pontos de acesso sem fio realizam o encaminhamento direto dos quadros entre as interfaces locais. O pacote é despachado pela placa de rede da origem, transita pelo ativo intermediário de Camada 2 e alcança o alvo final diretamente.

🚪 O Gateway Padrão e o Roteamento de Saída   
Para viabilizar a comunicação além das fronteiras da rede local — permitindo o acesso à internet ou a outras filiais —, o host exige a intermediação de um roteador (ou switch de Camada 3). O dispositivo encarregado de interconectar a LAN local a segmentos externos recebe o nome de gateway padrão. Ele funciona como a porta de saída da rede: se um pacote precisa alcançar outro segmento, ele deve obrigatoriamente ser direcionado a essa interface.

As propriedades técnicas que qualificam um ativo para atuar como gateway padrão envolvem:
- Possuir um endereço IP local configurado obrigatoriamente na mesma faixa e sub-rede que os demais hosts da LAN.
- Estar apto a receber o tráfego vindo da rede interna e processá-lo para encaminhamento externo.
- Dispor de uma tabela de roteamento capaz de identificar o melhor caminho para guiar os dados até as redes de destino.

A ausência ou falha do gateway padrão paralisa o tráfego inter-redes. Caso o endereço do gateway não esteja configurado nas estações, esteja incorreto ou a interface do roteador fique inativa, o host permanecerá restrito à comunicação local, ficando impossibilitado de enviar dados para redes externas.

A distribuição desse parâmetro lógico para os hosts pode ocorrer de forma automatizada ou manual. No ambiente IPv4, as estações herdam o IP do gateway dinamicamente por meio do protocolo DHCP ou via inserção estática. No ecossistema IPv6, os hosts aprendem a rota de saída capturando as mensagens de anúncio dos roteadores presentes na rede, embora também aceitem a fixação manual. A definição do gateway cria automaticamente um caminho especial na tabela de encaminhamento do host, conhecido como rota padrão, que serve como o destino universal para onde todo o tráfego direcionado a redes remotas deve ser enviado.

🔍 Inspeção da Tabela de Roteamento do Host no Windows   
Os sistemas operacionais dos computadores mantêm tabelas de roteamento internas para gerenciar o destino dos pacotes criados pelas aplicações. Em plataformas Windows, o administrador pode inspecionar esse mapa lógico executando os comandos `route print` ou `netstat -r` no prompt de comando. Ambos os utilitários extraem as mesmas informações do sistema.

A saída gerada por esses comandos é estruturada em três seções principais:
- Lista de Interfaces: Catálogo que mapeia todos os adaptadores de rede físicos e virtuais instalados no hardware (como placas Ethernet, chips Wi-Fi e conexões Bluetooth). A lista associa o número de índice atribuído pelo sistema operacional ao respectivo endereço físico MAC de cada interface.
- Tabela de Rotas IPv4: Exibe todos os caminhos conhecidos para o tráfego IPv4. Essa seção discrimina as conexões diretas da placa, os escopos de rede local e a rota padrão vinculada ao gateway.
- Tabela de Rotas IPv6: Apresenta a listagem análoga de caminhos estruturados para o endereçamento de nova geração, mapeando os prefixos locais, endereços de link local e as rotas de saída padrão do IPv6.

<a name="item03.03"><h4>3.3 Tabelas de Roteamento</h4></a>[Back to summary](#item03)

⚙️ O Processo de Encaminhamento de Pacotes no Roteador   
Quando as estações de trabalho identificam que um destinatário reside em uma rede externa, elas direcionam os pacotes para o seu gateway padrão, que é a interface do roteador local. Ao receber o pacote em uma de suas portas (como a Gigabit Ethernet 0/0/0), o roteador assume o processamento do tráfego na Camada 3 operando através do seguinte fluxo:
- Desencapsulamento: O hardware inspeciona o quadro recebido, remove o cabeçalho e o trailer de Camada 2 (Ethernet) e extrai o pacote IP.
- Análise do Destino: O sistema examina o endereço IP de destino gravado no pacote e realiza uma busca em sua tabela de roteamento interna para encontrar a rota com a maior correspondência de prefixo (a correspondência mais longa).
- Encapsulamento e Envio: Ao localizar a entrada correspondente (que pode apontar para um roteador vizinho ou para uma interface local), o dispositivo reinsere o pacote em um novo cabeçalho e trailer de Camada 2 apropriados para o próximo link e o despacha pela interface de saída.

🗂️ Tipos de Entradas na Tabela de Roteamento   
A tabela de roteamento atua como o mapa de navegação do dispositivo intermediário. Ela armazena os prefixos conhecidos organizados em três categorias de rotas:
- Redes Diretamente Conectadas: São os segmentos lógicos ligados diretamente às interfaces físicas ativas do próprio roteador. Quando uma interface recebe um endereço IP e é ligada, o sistema operacional do roteador (Cisco IOS) adiciona automaticamente duas entradas na tabela: uma com o código C (indicando a sub-rede conectada) e outra com o código L (mapeando o IP local exato atribuído àquela porta).
- Redes Remotas: Representam os escopos lógicos que estão distantes do roteador, vinculados a outros ativos de rede. O roteador preenche essas entradas por meio de inserção manual feita pelo administrador ou assimilando os dados de forma automatizada via protocolos de roteamento.
- Rota Padrão (Gateway de Último Recurso): Configurada com um endereço de zeros (0.0.0.0/0 no IPv4). Essa rota serve como um destino coringa: caso o IP de destino do pacote não possua nenhuma correspondência específica na tabela de roteamento, o dispositivo envia o tráfego para o parceiro definido nesta regra (como o roteador da operadora de internet).

📍 Características do Roteamento Estático   
O roteamento estático baseia-se na alimentação manual da tabela de encaminhamento. O analista de redes precisa registrar explicitamente cada rede remota e associá-la ao IP do roteador de próximo salto (next-hop) ou à interface de saída correspondente.

Esse modelo possui propriedades operacionais rígidas:
- Configuração Manual: Cada caminho exige intervenção humana para passar a existir.
- Rigidez Perante Falhas: Caso ocorra uma queda de link ou mudança física na topologia, a rota estática permanece inalterada na tabela e continuará tentando enviar dados pelo caminho quebrado. O administrador deve intervir e reconfigurar manualmente as rotas para desviar o tráfego por caminhos redundantes (como redirecionar o tráfego através de um roteador alternativo).
- Cenário Ideal: É uma abordagem eficiente para infraestruturas de pequeno porte, redes que possuem links únicos de saída (stub) ou locais onde não existem caminhos redundantes que justifiquem o processamento de protocolos dinâmicos.

🔄 Funcionamento do Roteamento Dinâmico   
Os protocolos de roteamento dinâmico automatizam por completo a gerência e o aprendizado das redes remotas. Sob esse regime, o administrador precisa apenas ativar o protocolo nas interfaces diretamente conectadas; a partir disso, os próprios roteadores vizinhos passam a conversar entre si e trocar atualizações sobre suas tabelas de encaminhamento.

A operação dinâmica executa quatro tarefas essenciais de forma automatizada:
- Descobrir novos prefixos e redes remotas na infraestrutura.
- Manter o mapa de rotas permanentemente atualizado.
- Calcular e eleger o melhor caminho para guiar os dados até o destino com base em métricas técnicas.
- Detectar quedas de links na rede e recalcular de forma imediata um novo trajeto alternativo, ajustando as tabelas de todos os roteadores sem exigir nenhuma ação do administrador.

Tecnologias consagradas do mercado, como o OSPF e o EIGRP, executam essa automação compartilhando informações de topologia constantemente. Vale ressaltar que a maioria dos cenários de produção mescla as duas técnicas: os roteadores usam protocolos dinâmicos para mapear as redes internas da empresa e adotam uma rota estática padrão (S*) apontando para o roteador de internet da operadora.

🔍 Comandos de Exibição e Códigos do Cisco IOS   
Para auditar e visualizar o mapa de encaminhamento IPv4 em um roteador Cisco, utiliza-se o comando `show ip route` a partir do modo executivo privilegiado. A saída gerada lista todos os destinos conhecidos precedidos por letras que funcionam como uma legenda explicativa sobre a origem daquela rota.

Os códigos mais comuns encontrados nos prompts do Cisco IOS são:
- L: Identifica o endereço IP individual da interface local do roteador.
- C: Identifica uma rede diretamente conectada ao dispositivo.
- S: Identifica rotas estáticas criadas manualmente pelo administrador.
- S*: Identifica a presença de uma rota estática padrão (gateway de último recurso).
- O: Identifica caminhos aprendidos dinamicamente por meio do protocolo OSPF.
- D: Identifica caminhos assimilados dinamicamente através do protocolo EIGRP.

<a name="item03.04"><h4>3.4 Resumo da Roteamento na camada de rede</h4></a>[Back to summary](#item03)

🚀 Destinos do Fluxo de Dados   
Um dispositivo conectado à rede possui a capacidade de direcionar pacotes para três cenários distintos: para si próprio, para um parceiro na mesma sub-rede ou para uma máquina externa. No ambiente IPv4, a origem cruza seu IP e máscara com o IP de destino para identificar a localização do alvo; já no ecossistema IPv6, essa verificação baseia-se nos anúncios de prefixo local transmitidos periodicamente pelo roteador da rede.

🚪 A Função do Gateway Padrão   
O gateway padrão atua como o ponto de conexão obrigatório para que os dados consigam sair da vizinhança local e alcançar outras sub-redes. Esse papel é desempenhado por um roteador que possui uma interface física com um endereço IP contido na mesma faixa dos hosts locais, tornando-o apto a receber o tráfego interno da LAN e encaminhá-lo para o ambiente externo através de suas tabelas de decisão.

🗺️ Tabelas de Roteamento no Computador   
Os sistemas operacionais dos computadores mantêm um mapa interno para registrar suas saídas de rede, incluindo a rota para o gateway. No IPv4, esse endereço chega de forma automática via DHCP ou por inserção manual; no IPv6, o próprio roteador informa sua presença na rede. Em sistemas operacionais Windows, o analista pode auditar esse mapa local utilizando os comandos de linha de comando `route print` ou `netstat -r`.

🚦 Encaminhamento de Pacotes no Host   
Sempre que inicia o envio de uma informação, o sistema operacional realiza uma consulta imediata em sua tabela de rotas interna para definir o destino físico do pacote. Caso essa verificação aponte que o destinatário final reside em um segmento remoto, o computador interrompe a busca local e despacha o pacote diretamente para o endereço do gateway cadastrado.

🔍 Processamento Interno do Roteador   
Ao receber um quadro em sua interface, o roteador abre o cabeçalho para ler o endereço IP de destino e inicia uma busca em sua própria tabela de roteamento. Essa base de dados abriga um índice com todas as redes conhecidas (prefixos); o equipamento compara os bits do endereço e seleciona a rota que possuir o maior nível de especificidade, técnica conhecida como a correspondência de prefixo mais longa.

🗂️ Categorias de Rotas do Roteador   
A memória de caminhos de um roteador organiza-se em três grandes grupos de registros de rede:
- Redes Conectadas: Links físicos diretamente associados às interfaces do equipamento.
- Redes Remotas: Caminhos distantes aprendidos manualmente através de rotas estáticas criadas pelo administrador — que especificam o IP do próximo salto —, ou de forma automatizada por protocolos de roteamento dinâmico como OSPF e EIGRP.
- Rota Padrão: Uma diretiva genérica utilizada para escoar o tráfego quando o destino não consta em nenhuma outra parte da tabela.

📊 Inspeção de Rotas no Cisco IOS   
Para analisar o mapa de encaminhamento IPv4 em dispositivos da linha Cisco, utiliza-se a diretiva `show ip route` a partir do prompt de privilégios elevados. A tabela gerada exibe uma legenda detalhada no cabeçalho contendo códigos de letras que revelam a origem de cada caminho, permitindo ao administrador rastrear a topologia lógica do ambiente.

🔤 Legenda de Origem das Rotas   
- L (Local): Indica o endereço IP específico configurado na interface física do próprio roteador.
- C (Connected): Representa a faixa de rede inteira que está ligada diretamente àquela porta.
- S (Static): Sinaliza um caminho inserido de forma manual e fixa por um analista de infraestrutura.
- O (OSPF): Identifica uma rota mapeada de forma dinâmica pelo protocolo Open Shortest Path First.
- D (EIGRP): Aponta um trajeto descoberto de forma automatizada através do protocolo proprietário aprimorado da Cisco.
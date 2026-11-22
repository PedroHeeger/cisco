# Network Addressing and Basic Troubleshooting - Módulo 6   <img src="../0-aux/logo_course.png" alt="sfp_009" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">sfp_009 (Network Addressing and Basic Troubleshooting)   <img src="../0-aux/logo_course.png" alt="sfp_009" width="auto" height="25"></a>
### Module: 6. Switches e Roteadores Cisco

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

### Course Module 6 Structure:
6. <a name="item06">Switches e Roteadores Cisco</a><br>
  6.1 <a href="#item06.01">Introdução</a><br>
  6.2 <a href="#item06.02">Switches Cisco</a><br>
  6.3 <a href="#item06.03">Velocidades do Switch e Métodos de Encaminhamento</a><br>
  6.4 <a href="#item06.04">Processo de inicialização do switch</a><br>
  6.5 <a href="#item06.05">Roteadores Cisco</a><br>
  6.6 <a href="#item06.06">Processo de inicialização do roteador</a><br>
  6.7 <a href="#item06.07">Resumo Switches e roteadores Cisco</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item06.01"><h4>6.1 Introdução</h4></a>[Back to summary](#item06)

🏢 Arquitetura e Inicialização de Ativos de Rede Cisco   
O projeto e a implementação de novas filiais corporativas exigem a seleção e a parametrização adequada de switches e roteadores. Compreender o funcionamento interno desses ativos de rede — desde o momento em que são energizados até a forma como processam e distribuem o tráfego de dados — é fundamental para garantir a estabilidade da infraestrutura. Dispositivos de nível empresarial oferecem recursos avançados de hardware e software que otimizam a velocidade de comutação e garantem o isolamento seguro do tráfego corporativo.

🎯 Objetivo do módulo:   
- Descrever as características estruturais, métodos de encaminhamento e os processos de inicialização de switches e roteadores Cisco.

📘 Tópicos do módulo:   
- Switches Cisco: Visão geral sobre os comutadores de rede local (LAN) da Cisco, suas aplicações na infraestrutura e o papel que desempenham na conectividade dos hosts.
- Métodos de encaminhamento e velocidades de switches: Análise técnica dos modos de comutação da Camada 2 (como Store-and-Forward e Cut-Through), além do gerenciamento de largura de banda e configurações de duplex nas portas físicas.
- Processo de inicialização do switch: Detalhamento das etapas de boot de um switch Cisco LAN, incluindo a execução do POST (Power-On Self-Test) e o carregamento do sistema operacional.
- Roteadores Cisco: Apresentação das linhas de roteadores Cisco voltadas para ambientes empresariais e de pequenas filiais, destacando suas funções de interconexão.
- Processo de inicialização do roteador: Estudo da sequência de inicialização de um roteador, mapeando a busca e a carga do microcódigo de boot, do Cisco IOS e dos arquivos de configuração ativa.

<a name="item06.02"><h4>6.2 Switches Cisco</h4></a>[Back to summary](#item06)

🏠 Redes Domésticas vs. Estruturas Corporativas   
Em cenários residenciais e de escritórios de pequeno porte (SOHO), a demanda por infraestrutura é simplificada, exigindo poucos ativos para operar com eficiência. Geralmente, um único roteador sem fio — que integra internamente um switch de poucas portas cabeadas e um ponto de acesso — é suficiente para suprir a demanda de conectividade do grupo. A gerência desse dispositivo é feita de forma intuitiva por meio de navegadores web, utilizando interfaces gráficas (GUI) amigáveis que guiam o usuário pelas configurações básicas.

No entanto, esses equipamentos domésticos não possuem a robustez necessária para sustentar redes corporativas de grande escala, que lidam com uma densidade massiva de usuários e fluxos concorrentes. As redes empresariais modernas dependem de múltiplos ativos especializados, onde cada equipamento possui inteligência dedicada para ditar o comportamento e o fluxo dos dados.

Na arquitetura de redes, aplica-se uma regra fundamental: quanto mais alta for a camada de operação de um ativo no modelo OSI, maior será a sua inteligência. Dispositivos que operam em níveis superiores possuem capacidade computacional para analisar o tráfego de forma profunda, tomando decisões de encaminhamento baseadas em critérios complexos que são invisíveis para as camadas inferiores. Um switch tradicional de Camada 2, por exemplo, limita-se a inspecionar os endereços físicos MAC para filtrar e direcionar os quadros estritamente para a porta onde o destino se encontra.

🔀 A Distinção Funcional entre Switches e Roteadores   
Com a evolução tecnológica e o surgimento de switches avançados que executam funções de roteamento, as fronteiras entre esses dois ativos podem parecer sobrepostas. Contudo, a engenharia de redes preserva uma linha de separação conceitual clara:
- Switches LAN: São ativos projetados para fornecer conectividade interna e concentrar os dispositivos dentro do mesmo segmento ou rede local corporativa. Eles interconectam os nós de uma mesma LAN.
- Roteadores: São os dispositivos encarregados de estabelecer pontes e interconectar diferentes redes lógicas distantes, sendo indispensáveis para viabilizar o tráfego em redes de longa distância (WANs).

Em suma, o switch atua ligando os equipamentos pertencentes à mesma rede local, enquanto o roteador realiza a comunicação entre redes distintas.

Para agregar valor a essa infraestrutura local, as corporações implantam outras soluções de conectividade. Os pontos de acesso sem fio (Access Points) empresariais expandem a área de cobertura, permitindo que estações móveis e telefones IP conectem-se ao barramento cabeado. Em paralelo, a segurança do perímetro e o controle de conformidade do tráfego são gerenciados por firewalls, que protegem a organização contra ameaças cibernéticas externas e realizam a contenção de riscos.

🏗️ Fatores de Escolha para a Expansão com Switches LAN   
Quando a infraestrutura de uma empresa expande e as poucas portas integradas de um roteador básico tornam-se insuficientes, adiciona-se um switch LAN dedicado. Ele atua na camada de acesso da rede, permitindo o acoplamento de novas estações e o crescimento modular da topologia sem a necessidade de substituir os ativos centrais da rede.

A seleção de um switch de nível comercial deve ser balizada por quatro critérios de engenharia:

🔌 Tipo de Portas   
É mandatório dimensionar a quantidade e a tecnologia das interfaces físicas. Modelos de entrada trazem conectores baseados em par trançado de cobre (RJ-45). Equipamentos de maior desempenho incorporam interfaces ópticas para transceptores de fibra, utilizadas para interconectar switches geograficamente distantes ou realizar a subida de tráfego (uplink) para o núcleo da rede. Equipamentos como a série Cisco Catalyst 9300 entregam flexibilidade de portas adaptáveis ao ambiente.

⚡ Velocidade Requerida   
As portas operam sob taxas de transmissão padronizadas. Uma interface do tipo Fast Ethernet (10/100) limita-se a negociar transmissões em 10 Mbps ou 100 Mbps. Se um servidor com placa Gigabit for conectado a essa porta, a comunicação sofrerá um gargalo, ficando restrita ao teto de 100 Mbps.

Switches modernos trazem portas Gigabit Ethernet (1000 Mbps) para aproveitar links de alta velocidade. A largura de banda real estabelecida em um link será sempre determinada pelo maior denominador comum (a maior velocidade suportada simultaneamente pela placa de rede do host e pela porta do switch). Para evitar o estrangulamento do tráfego corporativo, modelos avançados como o Cisco Catalyst 9300 48S trazem portas de uplink de alta performance (como conexões de 40 Gbps) para dar vazão ao tráfego acumulado das 48 portas locais em direção ao núcleo ou à internet.

🧱 Capacidade de Expansão (Escalabilidade)   
O hardware dos ativos pode ser classificado em duas arquiteturas físicas:
- Configuração Fixa: O switch possui um número imutável e predefinido de portas de fábrica, não aceitando modificações de hardware.
- Configuração Modular: O equipamento é estruturado em um gabinete que possui slots vazios para a inserção de módulos de expansão (placas de linha), permitindo que o administrador adicione novas portas de cobre, fibra ou interfaces de velocidades superiores conforme a demanda cresce. Um exemplo desse modelo é o gabinete Cisco Catalyst 9600.

🎛️ Capacidade de Gerenciamento   
Switches de baixo custo voltados ao mercado residencial operam de forma autônoma e não aceitam customizações (unmanaged). Em contrapartida, as redes de negócios exigem switches gerenciáveis equipados com sistemas operacionais (como o Cisco IOS).

O gerenciamento permite que o administrador acesse o equipamento (utilizando um cabo de console conectado diretamente à porta de gerência) para configurar individualmente o comportamento de cada porta, implementar políticas de segurança (como o bloqueio de MACs desconhecidos) e monitorar métricas de desempenho em tempo real.

Modelos como o Cisco Catalyst 9300 atendem com eficiência ao segmento de pequenas e médias empresas, fornecendo 24 portas de 1 Gbps dotadas de tecnologia PoE (Power over Ethernet) — recurso que injeta alimentação elétrica diretamente pelo cabo de rede para ligar dispositivos como câmeras IP e telefones sem a necessidade de fontes externas —, além de trazerem portas de uplink modulares de 40 Gbps e LEDs de diagnóstico de status no painel frontal.

<a name="item06.03"><h4>6.3 Velocidades do Switch e Métodos de Encaminhamento</h4></a>[Back to summary](#item06)

🕹️ Mecanismos de Comutação de Quadros na Camada 2   
Os switches Ethernet operam na Camada de Enlace processando e encaminhando os quadros de dados com base em seus endereços físicos MAC. Para realizar esse transporte entre as portas, o sistema operacional do ativo adota dois métodos de engenharia de switching, cada um priorizando um aspecto diferente do desempenho da rede:

📦 Método Store-and-Forward (Armazenar e Encaminhar)   
Esta abordagem prioriza a integridade absoluta dos dados. O switch aguarda o recebimento completo de todos os bits do quadro para armazená-lo temporariamente em sua memória buffer. Antes de tomar qualquer decisão de envio, o hardware aplica o cálculo do algoritmo CRC (Verificação de Redundância Cíclica) sobre o bloco de dados.

O CRC realiza uma fórmula matemática comparativa para validar se o pacote sofreu distorções ou corrupções elétricas durante o tráfego pelo cabo. Se o resultado for válido, o switch inspeciona a tabela MAC para localizar a interface de saída correspondente e despacha os dados. Caso o CRC aponte inconsistências, o quadro corrompido é descartado imediatamente na origem.

O descarte preventivo traz vantagens nítidas:
- Evita o desperdício de largura de banda com o tráfego de pacotes inválidos.
- Fornece a base mandatória para a aplicação de políticas de QoS (Qualidade de Serviço) em redes convergentes, permitindo ler e classificar o cabeçalho completo para dar prioridade a tráfegos sensíveis (como pacotes de Voz sobre IP - VoIP) sobre dados comuns de navegação web.

⚡ Método Cut-Through (Corte Direto)   
Este modelo foca em entregar a menor latência possível para o link. O switch não aguarda o recebimento total do quadro para iniciar o encaminhamento; ele começa a transmitir os bits para a interface de destino assim que lê os primeiros 6 bytes do pacote posicionados logo após o preâmbulo — trecho exato onde fica gravado o endereço MAC de destino.

Como o switch não executa nenhuma verificação de erro (CRC) antes do reenvio, dados inválidos podem acabar se propagando pela topologia, sendo descartados apenas na placa de rede do host final. 

O switching por corte direto subdivide-se em duas técnicas operacionais:
- Fast-Forward (Avanço Rápido): É a forma padrão e mais veloz do corte direto. O switch lê unicamente os dados de endereçamento e inicia o repasse do primeiro bit de saída antes mesmo de ter recebido o corpo ou o final do pacote, registrando os menores índices de latência da rede.
- Fragment-Free (Livre de Fragmentos): Atua como um modelo intermediário de equilíbrio. O switch realiza a leitura e o armazenamento estrito dos 64 bytes iniciais do quadro antes de dispará-lo. O motivo técnico para essa escolha geométrica é que as leis de colisão e a maioria dos erros de hardware manifestam-se nos primeiros 64 bytes da transmissão. O método valida essa janela inicial para garantir que o quadro não seja fruto de um choque de colisão, unindo a velocidade do corte direto com um filtro mínimo de integridade.

Mecanismo Adaptativo: Roteadores e switches modernos de nível comercial possuem inteligência para operar nativamente em modo Cut-Through, mas monitoram o comportamento das portas. Se o índice de erros de uma interface ultrapassar um teto limite customizado pelo administrador, a porta migra automaticamente para o modo Store-and-Forward. Assim que o ruído cessa e a taxa de falhas retorna ao nível seguro, o hardware restabelece a operação em corte direto.

💾 Modelos de Buffer de Memória para Armazenamento   
Quando ocorre o congestionamento de uma interface devido ao alto volume de tráfego simultâneo voltado para um mesmo destino, o switch armazena temporariamente os quadros excedentes em buffers de memória até que o canal seja liberado. O hardware pode estruturar essa memória de duas maneiras:

🧩 Memória Baseada em Portas   
Nessa arquitetura, a memória total é segmentada em filas rígidas e exclusivas vinculadas a cada porta física de entrada e saída. Um quadro armazenado em uma fila de saída precisa aguardar de forma sequencial que todos os pacotes posicionados à sua frente sejam transmitidos com sucesso.

A desvantagem crítica desse design é que o travamento ou saturação de uma única porta de destino pode congelar o tráfego de toda a fila, impedindo que outros quadros guardados na mesma memória sejam enviados para portas que se encontram totalmente livres e ociosas.

🔄 Memória Compartilhada   
Deposita todas as transmissões recebidas em um grande pool ou buffer de memória comum compartilhado dinamicamente por todas as interfaces do switch. Os pacotes guardados nesse bloco comum não ficam presos a filas físicas; eles recebem links virtuais dinâmicos apontando diretamente para as suas respectivas portas de destino.

Esse design entrega maior flexibilidade computacional, pois permite que um pacote seja recebido por uma interface e despachado por outra sem a necessidade de movimentação interna de memória. A memória compartilhada reduz drasticamente a taxa de descarte de quadros e viabiliza a comutação assimétrica, permitindo o fluxo eficiente de dados entre portas de velocidades discrepantes (como balancear o tráfego quando PCs de 1 Gbps requisitam dados simultaneamente de um servidor acoplado a um link de 10 Gbps).

⚡ Alinhamento de Links e Resolução de Conflitos Duplex   
O estabelecimento de um canal de comunicação de alta performance exige a correta paridade nos parâmetros de velocidade e duplexação entre a porta do switch e o dispositivo conectado.

A transmissão Ethernet classifica o tráfego físico em dois regimes de operação:
- Full-Duplex: Ambas as pontas do link conseguem transmitir e receber dados em regime estritamente simultâneo.
- Half-Duplex: Apenas um dispositivo pode falar por vez; o uso compartilhado do canal proíbe transmissões síncronas.

🤝 Negociação Automática (Auto-Negotiation)   
A grande maioria das placas de rede atuais e das portas de switches Cisco traz ativado por padrão o recurso de negociação automática. Essa função executa uma sondagem elétrica inicial onde os dois dispositivos conectados anunciam suas capacidades máximas de hardware e escolhem o melhor cenário comum. Se um computador que suporta velocidades de até 100 Mbps em Full-Duplex conectar-se a um switch Gigabit (10/100/1000 Mbps), o link irá travar na maior configuração suportada por ambos: 100 Mbps em modo Full-Duplex.

Regra Gigabit: Conexões configuradas para operar em velocidades de Gigabit Ethernet (1000 Mbps) ou superiores funcionam exclusivamente em modo Full-Duplex, rejeitando retrocessos para Half-Duplex.

⚠️ Incompatibilidade de Duplex (Duplex Mismatch)   
Trata-se de uma das falhas mais recorrentes no diagnóstico de lentidão e perda de pacotes na Camada 1 e 2. O problema ocorre quando uma ponta do cabo assume o modo Full-Duplex e a ponta oposta opera fixada em Half-Duplex.

Esse desalinhamento quebra as regras de tráfego: o dispositivo configurado em Full-Duplex assume que o meio está sempre disponível e envia quadros continuamente, ignorando o tráfego que chega. A ponta configurada em Half-Duplex interpreta esse fluxo simultâneo como uma colisão contínua de sinais, interrompendo suas próprias transmissões de forma intermitente. O resultado direto dessa anomalia é a perda massiva de vazão, erros de CRC e degradação severa da performance do link.

Essa falha é provocada tipicamente quando a negociação automática falha após a reincialização de uma interface ou quando um analista de redes fixa os parâmetros manualmente em apenas um lado da conexão, esquecendo de replicar a configuração no dispositivo parceiro. Como regra de engenharia, ambos os lados do cabo devem adotar o mesmo regime: ou ambos operam com a negociação automática ligada, ou ambos operam com ela desligada. A melhor prática de infraestrutura determina a fixação manual de ambas as portas em Full-Duplex sempre que possível.

🔌 Detecção de Cabeamento via Recurso Auto-MDIX   
No passado, a infraestrutura física de rede exigia o emprego rigoroso de cabos específicos baseados na natureza dos dispositivos conectados para alinhar os pinos de transmissão (TX) e recepção (RX):
- Cabos Cruzados (Crossover): Utilizados para conectar componentes de mesma categoria (ex: switch para switch, computador para computador ou roteador conectado direto a um host).
- Cabos Diretos (Straight-Through): Utilizados para interconectar equipamentos de categorias distintas (ex: computador conectado a um switch ou switch ligado a um roteador).

Para extinguir a dependência desse controle rígido de cabos em campo, a engenharia de hardware desenvolveu a funcionalidade Auto-MDIX (Automatic Medium-Dependent Interface Crossover). Quando esse recurso encontra-se em execução, os circuitos integrados da porta do switch realizam uma leitura eletrônica do cabo conectado e rearranjam internamente as funções dos pinos para fechar o circuito elétrico corretamente, tornando indiferente o uso de cabos diretos ou cruzados na rede local.

Nos switches Cisco equipados com o sistema operacional Cisco IOS a partir da versão 12.2(18)SE, o Auto-MDIX vem habilitado e ativo por padrão de fábrica em todas as portas de cobre de 10/100/1000 Mbps. Caso o recurso tenha sido desativado em uma auditoria anterior, o administrador pode restabelecer a automação acessando o prompt de configuração da interface e aplicando a diretiva `mdix auto`. Contudo, como boas práticas de gerenciamento de riscos, os engenheiros orientam que as equipes técnicas realizem o lançamento físico da rede utilizando as regras de cabeamento corretas, evitando a dependência exclusiva da automação de hardware para o funcionamento da rede.

<a name="item06.04"><h4>6.4 Processo de inicialização do switch</h4></a>[Back to summary](#item06)

🚀 Inicialização Operacional de Ativos Cisco   
Os switches da linha Cisco saem de fábrica pré-configurados em modo plug-and-play para operar em uma rede local (LAN). Ao ligar o equipamento, todas as portas físicas de interface encontram-se ativas e iniciam o encaminhamento de quadros de dados imediatamente após o acoplamento dos cabos dos hosts.

No entanto, é vital que o analista de infraestrutura compreenda que nenhum parâmetro de segurança vem ativado por padrão de fábrica. Lançar o ativo diretamente em um ambiente de produção sem as devidas salvaguardas cria vulnerabilidades críticas. Portanto, é uma diretriz mandatória aplicar configurações de segurança básicas antes de integrar definitivamente o switch à topologia da empresa.

O procedimento padrão para colocar um switch em operação divide-se em três etapas físicas e logísticas:
- Etapa 1 - Inventário e Verificação de Componentes: Antes de iniciar a montagem, deve-se auditar o kit de acessórios fornecido com o equipamento (como na linha Catalyst 2960). O inventário básico deve conter o cabo de console (para gerência local), o cabo de alimentação CA, os patch cords Ethernet e os manuais de documentação oficial do switch.
- Etapa 2 - Interconexão de Cabos de Controle: Fixa-se o conector do cabo de console na porta correspondente do switch e a outra extremidade no terminal de gerenciamento (PC do administrador), iniciando um software emulador de terminal (como PuTTY ou Tera Term) com os parâmetros de transmissão adequados para abrir a interface de linha de comando (CLI).
- Etapa 3 - Energização e Boot do Chassi: A grande maioria dos switches corporativos da Cisco — incluindo modelos avançados como a série Catalyst 9300 — dispensa chaves físicas ou botões de liga/desliga. Para iniciar o equipamento, basta acoplar o cabo de força no conector traseiro do chassi e ligá-lo a uma tomada aterrada. Modelos de alta disponibilidade trazem fontes de alimentação redundantes e trocáveis em operação (hot-swappable), garantindo que o ativo continue funcionando mesmo em caso de falha elétrica de uma das fontes.

🚦 O Processo POST e Diagnóstico por LEDs   
Ao receber energia elétrica, o hardware do switch inicia de forma autônoma o procedimento de POST (Power On Self Test - Autoteste de Inicialização). Esse mecanismo executa uma varredura interna nos circuitos integrados, memórias e barramentos para validar a integridade física do hardware.

Durante a execução do POST, o status do teste é sinalizado visualmente através dos LEDs do painel frontal:
- POST Concluído com Sucesso: Os LEDs piscam em sequência e o indicador SYST (Sistema) assume a cor verde, piscando rapidamente. Esse comportamento indica que o hardware está íntegro e o sistema operacional iniciará o carregamento.
- Falha no Hardware: Caso algum componente crítico falhe no diagnóstico, o LED SYST assume a cor âmbar (laranja) fixa. Sob essa condição, o processo de boot é interrompido e o equipamento deve ser encaminhado para manutenção ou substituição por defeito físico.

💾 Gestão de Memória e Arquivos de Inicialização   
Assim que o autoteste POST valida o hardware, o carregador de inicialização (bootloader) assume o controle do dispositivo e transfere dois arquivos vitais para a memória volátil RAM para colocar o switch em estado operacional:

🎞️ Imagem do Sistema Operacional (Cisco IOS)   
É o software binário que gerencia as funções lógicas do ativo, viabilizando o controle das interfaces, protocolos e algoritmos de comutação. A imagem do IOS fica guardada permanentemente em um chip de memória de armazenamento não volátil conhecido como Flash. Durante o boot, o código do IOS é descompactado e copiado para a RAM para execução em alta velocidade.

⚙️ Arquivo de Configuração de Inicialização (startup-config)   
Contém todo o histórico de comandos e parametrizações customizadas pelo administrador (como senhas, nomes de hosts e IPs de gerência). Este arquivo fica salvo na memória NVRAM (Non-Volatile RAM), um armazenamento que preserva as informações mesmo se o switch for completamente desligado.

Quando o IOS é carregado, ele lê o conteúdo da NVRAM e o joga para a RAM, criando o arquivo de trabalho ativo, batizado de configuração em execução (running-config). Todas as alterações que o analista realiza na linha de comando afetam de forma imediata e exclusiva o arquivo running-config na RAM.

Por residir na memória volátil RAM, qualquer modificação feita na configuração ativa se perderá caso ocorra uma queda brusca de energia ou um comando de reinicialização. Por essa razão, após concluir um ajuste na rede, o administrador deve salvar manualmente as alterações, copiando o arquivo da RAM de volta para a NVRAM (atualizando o startup-config). Esse backup garante que o switch retorne com as mesmas configurações personalizadas após passar por um ciclo de desligamento.

<a name="item06.05"><h4>6.5 Roteadores Cisco</h4></a>[Back to summary](#item06)

💻 A Natureza Computacional dos Roteadores   
Independentemente do seu porte, fabricante ou complexidade na topologia, um roteador opera fundamentalmente como um computador especializado em engenharia de tráfego. Assim como um servidor ou um smartphone, ele depende de uma arquitetura de hardware integrada para processar instruções lógicas e gerenciar recursos.

Os componentes vitais que sustentam essa infraestrutura digital incluem:
- Unidade Central de Processamento (CPU): O cérebro do dispositivo. A CPU executa as linhas de instrução do sistema operacional, processa os algoritmos de inicialização, calcula as tabelas de encaminhamento e gerencia as funções de switching entre as interfaces.
- Memória RAM (Volátil): Funciona como a área de trabalho temporária de alta velocidade. Armazena o sistema operacional em execução, a tabela de roteamento ativa, as filas de pacotes em buffer e o arquivo de configuração de trabalho (running-config).
- Memória ROM (Não Volátil): Chip de leitura que armazena o código básico de inicialização (Bootstrap) e softwares de diagnóstico de hardware para garantir que o roteador consiga ligar com segurança.
- Memória NVRAM (Não Volátil): Armazenamento magnético permanente de tamanho reduzido que guarda estritamente o arquivo de configuração de inicialização (startup-config).
- Memória Flash (Não Volátil): Funciona como o "disco rígido" do roteador, sendo o local onde fica armazenada a imagem binária completa do sistema operacional.

Para orquestrar esse hardware e habilitar as capacidades de roteamento e comutação, a CPU exige um sistema operacional robusto. No ecossistema da Cisco, essa função é desempenhada pelo Cisco IOS (Internetwork Operating System). Esse software de sistema possui arquitetura modular e é empregado de forma transversal em toda a linha de produtos da marca, equipando desde pequenos pontos de acesso sem fio residenciais até switches de borda e roteadores de altíssimo desempenho com dezenas de interfaces.

🔌 Interfaces e Conexões Físicas de Hardware   
Embora o mercado ofereça uma ampla variedade de modelos voltados a diferentes nichos, os roteadores Cisco mantêm um arranjo padrão de conexões em seu painel traseiro para viabilizar o controle e o tráfego.

Tomando como referência um modelo comercial como o roteador de serviços integrados Cisco ISR 4321, identificam-se as seguintes interfaces de comunicação:
- Portas de Console: Conexões dedicadas exclusivamente ao gerenciamento local, configuração inicial do ativo e acesso à Interface de Linha de Comando (CLI). O hardware disponibiliza duas opções de conectores para essa função: uma porta tradicional no padrão RJ-45 e uma interface moderna baseada em conexões USB Tipo-B (mini-USB).
- Interfaces LAN de Alta Velocidade: Portas destinadas a integrar o roteador aos switches das redes locais, geralmente representadas por duas interfaces Gigabit Ethernet (GE 0/0/0 e GE 0/0/1). Em designs flexíveis, a porta principal pode aceitar tanto o conector RJ-45 para cabos de cobre quanto adaptadores do tipo SFP, permitindo o acoplamento direto de transceptores de fibra óptica para conexões de longa distância.
- Slots de Expansão NIM (Network Interface Modules): Baias vazias modulares que conferem flexibilidade ao hardware. Elas permitem que o administrador insira placas de expansão específicas para adaptar o roteador às necessidades da empresa, adicionando portas seriais para conexões WAN antigas, links de telefonia digital (DSL), portas extras de switch ou interfaces de rádio sem fio.
- O painel do roteador incorpora ainda conexões de suporte, como portas USB convencionais utilizadas para a transferência rápida de arquivos de configuração e atualização de firmwares.
- O equipamento traz também uma interface de gerência dedicada externa para acessos remotos de emergência e uma porta auxiliar (AUX), que representa um recurso legado projetado para conectar modems de linha discada (dial-up) para administração remota via telefone — uma tecnologia que se encontra praticamente em desuso nas arquiteturas de redes modernas.

<a name="item06.06"><h4>6.6 Processo de inicialização do roteador</h4></a>[Back to summary](#item06)

🛠️ Procedimento Físico de Instalação e Ativação do Roteador   
O processo de implantação de um roteador de nível corporativo na infraestrutura de TI exige o cumprimento rigoroso de etapas físicas de montagem e segurança elétrica. Antes de manipular o equipamento, o técnico deve consultar os guias oficiais fornecidos pelo fabricante para se ambientar com as diretivas de conformidade específicas do hardware.

O roteiro sequencial de montagem e ativação do dispositivo compreende seis etapas fundamentais:
- Etapa 1 (Fixação Estrutural): O roteador deve ser acomodado e parafusado de forma firme em um rack padrão de telecomunicações de 19 polegadas. Utilizam-se suportes metálicos laterais (orelhas de rack) para garantir que o peso do equipamento fique distribuído adequadamente, evitando quedas ou trepidações.
- Etapa 2 (Aterramento Elétrico): Fixa-se o cabo de aterramento da carcaça metálica do roteador diretamente na barra de terra (grounding busbar) do rack corporativo. Essa conexão é mandatória para dissipar correntes de surto elétrico e proteger tanto a integridade dos circuitos eletrônicos internos quanto o operador do sistema.
- Etapa 3 (Conexão de Energia): Insere-se o cabo de força adequado na fonte do roteador, conectando a outra ponta a uma tomada protegida por um sistema de energia ininterrupta (Nobreak/UPS).
- Etapa 4 (Acoplamento do Console): Conecta-se um cabo de gerenciamento dedicado entre a porta de console física do roteador e o computador do administrador de redes. Nesse momento, o técnico abre e configura o software de emulação de terminal na máquina para abrir o console local.
- Etapa 5 (Energização do Hardware): Aciona-se o sistema conectando a alimentação ou ligando a chave seletora, se disponível.
- Etapa 6 (Monitoramento do Boot): O analista acompanha visualmente o fluxo das mensagens de inicialização do sistema operacional carregadas na janela do emulador de terminal no computador, validando se o autoteste de hardware e o boot do kernel ocorreram sem falhas estruturais.

🖥️ Métodos de Acesso e Gerenciamento da CLI   
O sistema operacional Cisco IOS disponibiliza três vias principais para que o administrador abra o prompt da interface de linha de comando (CLI) do dispositivo, dividindo-se em conexões de controle local ou remoto:
- Porta de Console: Apresenta-se como uma interface física nativa fixada no painel traseiro do roteador. Ela fornece um acesso de gerenciamento classificado como fora de banda (out-of-band), o que significa que o canal de controle corre por uma via física exclusiva e isolada do tráfego de dados padrão da rede. Utiliza conexões seriais clássicas (como o padrão RJ-45) ou conexões modernas via cabo mini-USB, dispensando que o roteador possua qualquer configuração lógica de IP ou link de rede ativo para aceitar comandos.
- Protocolo SSH (Secure Shell): É o método recomendado para que os engenheiros abram sessões remotas de CLI na infraestrutura através da rede de dados (gerenciamento em banda). O tráfego do SSH é totalmente criptografado, protegendo as credenciais de acesso contra interceptações. Para que essa conexão funcione, o roteador deve possuir pelo menos uma interface de rede física (ou porta de gerência dedicada) devidamente ativada, configurada com um endereço IP válido e operando em plena comunicação com o terminal do analista.
- Porta Auxiliar (AUX): Interface física focada em gerência remota legada. Esse barramento foi desenhado para ligar modems analógicos de linha telefônica discada diretamente ao roteador. Caso a rede da empresa sofresse uma queda geral e as conexões SSH fossem perdidas, o técnico conseguia efetuar uma ligação telefônica para o modem acoplado à porta AUX e assumir o controle do equipamento de forma remota. Nas arquiteturas de redes contemporâneas, essa modalidade é raramente empregada.

🔌 Interfaces de Rede e Diversidade de Mídias   
Além de dispor das portas exclusivas de controle e gerência descritas anteriormente, os roteadores são dotados de interfaces de tráfego de dados projetadas para receber, processar e despachar os pacotes IP.

Como a função principal de um roteador é realizar a interconexão de múltiplas sub-redes distintas e distantes entre si, o hardware deve suportar uma ampla pluralidade de meios físicos. Isso significa que, em um único dispositivo, o administrador encontrará portas Gigabit Ethernet para cabos de cobre de par trançado voltadas para a rede local interna (LAN), portas ópticas baseadas em transceptores SFP para cabeamentos de fibra de longa distância e conexões de cartões WAN modulares, exigindo o conhecimento e o manuseio técnico de diferentes tipos de conectores e cabos para cada topologia de rede.

<a name="item06.07"><h4>6.7 Resumo Switches e roteadores Cisco</h4></a>[Back to summary](#item06)

🏢 Papel dos Switches e Roteadores   
O switch atua como o ponto de convergência que interliga os computadores e servidores dentro de um mesmo segmento local. O roteador, por sua vez, opera em um nível hierárquico superior, sendo o responsável por conectar essas diferentes redes entre si. No planejamento de uma LAN, a escolha do switch deve considerar o volume e a tecnologia das portas: modelos de entrada utilizam conectores de cobre, enquanto equipamentos avançados trazem interfaces de fibra óptica para realizar conexões de longa distância com outros switches.

⚡ Alinhamento de Largura de Banda   
As placas de rede (NICs) dos computadores e as portas dos switches trabalham em velocidades padronizadas, como 10/100 Mbps ou o padrão Gigabit (10/100/1000 Mbps). A taxa de transmissão real de um link será sempre definida pela maior velocidade suportada em comum por ambas as pontas. Além disso, o hardware pode adotar designs de portas fixas ou estruturas modulares expansíveis, sendo que switches gerenciados com o sistema operacional Cisco dão controle total ao administrador sobre o comportamento de cada interface.

🔀 Métodos de Comutação e Memória   
Para movimentar os quadros de dados entre suas portas, os switches utilizam duas abordagens de encaminhamento:
- Store-and-Forward (Armazenar e Encaminhar): O switch recebe o quadro inteiro, valida o código de erro e só então o repassa.
- Cut-Through (Corte Direto): O switch lê apenas os endereços iniciais e já direciona o pacote. Suas variantes incluem o Fast-Forward (encaminhamento imediato) e o Fragment-Free (que lê os primeiros 64 bytes para evitar fragmentos de colisões).

Para gerenciar esse fluxo, o hardware aloca buffers de memória, que podem ser dedicados por porta ou compartilhados globalmente entre todas as interfaces.

🤝 Automação com Negociação e Auto-MDIX   
O recurso de negociação automática permite que a placa de rede e o switch conversem para estabelecer de forma transparente a melhor velocidade e o modo duplex (preferencialmente full-duplex) suportados por ambos. Complementando essa automação, a tecnologia Auto-MDIX identifica eletricamente se o cabo inserido é do tipo direto ou cruzado, reconfigurando os pinos internos da porta automaticamente para garantir a conexão sem a necessidade de trocar o cabo físico.

🔌 Inicialização e Segurança do Switch   
Embora os switches saiam de fábrica prontos para encaminhar pacotes assim que são ligados na tomada, é uma prática crítica de infraestrutura aplicar parâmetros de segurança antes de conectá-los ao ambiente de produção. O processo físico de ativação resume-se em inspecionar os módulos, acoplar o cabeamento e ligar a fonte de energia, momento em que o hardware inicia o POST (Power On Self Test) para testar seus circuitos internos.

🕹️ Gerenciamento Em Banda e Fora da Banda   
A administração de um ativo de rede divide-se em duas metodologias de acesso:
- Gerenciamento Fora da Banda (Out-of-Band): Exige uma conexão física direta entre o computador do técnico e a porta de console do equipamento, sendo usada para configurações iniciais ou quando a rede está fora do ar.
- Gerenciamento Em Banda (In-Band): Utiliza a própria estrutura da rede local ou da internet através de protocolos como SSH, permitindo monitorar e alterar o sistema remotamente.

💾 Arquivos de Inicialização na Memória   
Ao ser ligado, um dispositivo Cisco carrega dois arquivos essenciais para a memória RAM: a imagem do sistema operacional (IOS), que fica armazenada de forma permanente na memória Flash, e o arquivo de configuração de inicialização (startup-config), guardado na NVRAM. Esse arquivo armazena todas as diretrizes de segurança e redes salvas pelo administrador.

🏗️ Anatomia de Hardware do Roteador   
Para processar o tráfego de Camada 3, o roteador funciona como um computador especializado, equipado com processador (CPU), memória RAM (execução), ROM (inicialização básica) e NVRAM. Seu chassi oferece portas de console para gerência, interfaces LAN para conectar as redes internas, portas auxiliares (AUX) e slots de expansão modulares para receber placas seriais, modems DSL ou conexões sem fio adicionais.

📋 Roteiro de Instalação do Roteador   
A ativação física de um roteador corporativo segue um protocolo rigoroso de engenharia:
- Fixar o equipamento com segurança nos trilhos do rack.
- Conectar o cabo de aterramento para proteção elétrica do chassi.
- Plugar o cabo de alimentação na tomada.
- Conectar o cabo de console à estação de trabalho.
- Ligar a chave de energia do aparelho.
- Acompanhar a leitura dos códigos de boot na tela do terminal.
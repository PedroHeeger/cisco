# Networking Devices and Initial Configuration - Módulo 12   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_003 (Networking Devices and Initial Configuration)   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="25"></a>
### Module: 12. ICMP

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

### Course Module 12 Structure:
12. <a name="item12">ICMP</a><br>
  12.1 <a href="#item12.01">Introdução</a><br>
  12.2 <a href="#item12.02">Mensagens ICMP</a><br>
  12.3 <a href="#item12.03">Teste de Ping e Traceroute</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;12.3.1 <a href="../../../pkt/files/pkt_040/">Packet Tracer - Verifique o endereçamento IPv4 e IPv6</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;12.3.2 <a href="../../../pkt/files/pkt_041/">Packet Tracer - Use Ping e Traceroute para testar a conectividade de rede</a><br>
  12.4 <a href="#item12.04">Resumo ICMP</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;12.4.1 <a href="../../../pkt/files/pkt_042/">Packet Tracer - Use ICMP para testar e corrigir a conectividade de rede</a><br>
  12.5 Exame de ponto de verificação: serviços de endereçamento e protocolos da camada de transporte<br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item12.01"><h4>12.1 Introdução</h4></a>[Back to summary](#item12)

🔍 Verificação de Conectividade e Diagnóstico de Redes   
A validação operacional de uma infraestrutura de rede recém-configurada exige a aplicação de métodos de teste que comprovem o fluxo adequado dos dados e a acessibilidade dos nós. Esse processo de auditoria e diagnóstico fundamenta-se em protocolos de controle que emitem notificações sobre o estado do tráfego e em utilitários práticos que mapeiam o caminho percorrido pelas informações, permitindo a localização exata de eventuais falhas de comunicação ou pontos de lentidão no sistema.

🎯 Objetivo do módulo:   
- Empregar ferramentas e protocolos de diagnóstico para analisar a conectividade estrutural e validar o funcionamento de uma rede de computadores.

📘 Tópicos do módulo:   
- Mensagens ICMP: Análise da operação do Internet Control Message Protocol no fornecimento de relatórios de erro e feedbacks operacionais durante o tráfego de pacotes.
- Teste de ping e traceroute: Utilização prática de ferramentas de varredura para mensurar a latência de ponta a ponta e rastrear as etapas do roteamento na infraestrutura física e lógica.

<a name="item12.02"><h4>12.2 Mensagens ICMP</h4></a>[Back to summary](#item12)

📢 O Protocolo ICMP e o Feedback de Controle na Camada de Rede   
O protocolo IP opera sob o princípio de melhor esforço, o que significa que ele não possui mecanismos nativos para garantir o sucesso das entregas. Para mitigar essa característica e fornecer relatórios operacionais, a arquitetura TCP/IP utiliza o ICMP (Internet Control Message Protocol).

O propósito central do ICMP é gerar mensagens informativas e relatórios de erro sobre o processamento de pacotes sob condições específicas. Suas mensagens não alteram a natureza não confiável do protocolo IP, servindo apenas como uma ferramenta de diagnóstico. Vale ressaltar que, por questões de endurecimento de segurança e para evitar o mapeamento da topologia por agentes maliciosos, administradores frequentemente bloqueiam o tráfego ICMP nas bordas da rede através de firewalls.

O protocolo apresenta duas variantes correspondentes às versões da camada de rede:
- ICMPv4: Encarregado das mensagens operacionais estruturadas para o ecossistema IPv4.
- ICMPv6: Desenvolvido para o ambiente IPv6. Esta versão executa todas as funções de diagnóstico de seu antecessor, mas agrega novos recursos integrados que substituem outros protocolos de infraestrutura da Camada 2.

Tanto no ambiente IPv4 quanto no IPv6, existem três categorias fundamentais de mensagens compartilhadas que monitoram a atividade dos fluxos:

🟢 Acessibilidade do Host (Echo Request e Echo Reply)   
Utilizada para validar se uma estação remota está ativa e respondendo na camada de rede. O host local dispara uma solicitação de eco (ICMP Echo Request) em direção ao destino. Caso o dispositivo parceiro esteja operacional e com o tráfego liberado, ele devolve uma resposta de eco (ICMP Echo Reply). Essa interação síncrona constitui a base lógica de funcionamento do utilitário de teste de conectividade conhecido como ping.

🔴 Destino ou Serviço Inalcançável (Destination Unreachable)   
Emitida por um roteador intermediário ou pelo próprio host de destino quando um pacote recebido não pode ser processado ou entregue com sucesso. A mensagem carrega códigos numéricos padronizados que apontam a causa exata da falha de entrega.

No ecossistema do ICMPv4, os códigos de falha mais comuns são:
- Código 0: Rede de destino inalcançável.
- Código 1: Host de destino inalcançável.
- Código 2: Protocolo solicitado indisponível no destino.
- Código 3: Porta de destino inalcançável.

No ecossistema do ICMPv6, a nomenclatura e as funções dos códigos sofrem ligeiras adaptações estruturais:
- Código 0: Ausência de rota para o destino na tabela de roteamento.
- Código 1: Comunicação administrativamente proibida (barrada por regras de firewall).
- Código 2: Escopo do endereço de origem incompatível com o destino.
- Código 3: Endereço de destino inacessível.
- Código 4: Porta de aplicação inalcançável.

⏳ Tempo Excedido (Time Exceeded)   
Garante que pacotes perdidos em loops de roteamento não fiquem circulando indefinidamente na infraestrutura, consumindo banda. No IPv4, cada roteador que encaminha o pacote reduz em uma unidade o campo de Vida Útil (TTL - Time to Live) contido no cabeçalho IP. Se o TTL atingir o valor zero, o roteador descarta o pacote e envia uma mensagem de tempo excedido (ICMP Type 11) de volta para o host de origem.

No IPv6, o comportamento operacional é idêntico, porém o ICMPv6 monitora o campo de Limite de Saltos (Hop Limit), descartando o pacote e gerando o alerta quando este contador é zerado. Esse mecanismo de controle por estouro de tempo é a base de funcionamento da ferramenta de mapeamento de caminhos traceroute.

🌐 Recursos Exclusivos e Protocolos do ICMPv6   
Diferente do modelo clássico, o ICMPv6 possui maior relevância na arquitetura da rede por encapsular as funções do NDP (Neighbor Discovery Protocol - Protocolo de Descoberta de Vizinhos). O NDP substitui mecanismos antigos (como o ARP em broadcast do IPv4) e introduz quatro novas mensagens lógicas que governam a autoconfiguração e a convivência dos dispositivos no meio físico:

🗺️ Interações entre Roteadores e Dispositivos Finais   
- Mensagem de Anúncio de Roteador (RA - Router Advertisement): Emitida periodicamente por roteadores IPv6 ativos a cada 200 segundos, ou enviada sob demanda em resposta a uma solicitação. O RA propaga dados essenciais de endereçamento para o segmento local, incluindo o prefixo de rede, o comprimento desse prefixo, o servidor DNS e os nomes de domínio. Dispositivos que operam sob o mecanismo de autoconfiguração automática sem estado (SLAAC) interceptam essa mensagem, utilizam o prefixo para autogerar seu endereço unicast global e definem o endereço de link local (Link-Local) do próprio roteador emissor como seu gateway padrão.
- Mensagem de Solicitação de Roteador (RS - Router Solicitation): Disparada por um host IPv6 imediatamente após a sua inicialização na rede. A estação envia a mensagem RS para consultar se existem roteadores ativos no segmento, agilizando o recebimento dos parâmetros dinâmicos de endereçamento sem precisar aguardar o intervalo padrão do anúncio do roteador.

👥 Interações de Vizinhança entre Dispositivos Locais   
- Mensagem de Solicitação de Vizinho (NS - Neighbor Solicitation): Atua em duas frentes operacionais distintas na rede local: a resolução de endereços e a validação de exclusividade de IPs. Na resolução de endereços, quando um host conhece o IP unicast do destino, mas necessita descobrir seu endereço físico MAC de Camada 2, ele envia uma mensagem NS perguntando pelo endereço MAC do detentor daquele IP. A outra função ocorre no processo de Detecção de Endereço Duplicado (DAD). Ao adquirir um novo IP na rede (seja via SLAAC ou estático), o dispositivo dispara uma mensagem NS tendo como destino o seu próprio IP recém-adquirido. O objetivo é checar se alguma outra interface já está utilizando aquela identidade lógica na LAN.
- Mensagem de Anúncio de Vizinho (NA - Neighbor Advertisement): Funciona como a resposta direta às solicitações NS. No processo de resolução de endereços, o dispositivo que possui o IP consultado responde enviando uma mensagem NA contendo o seu respectivo endereço MAC Ethernet, permitindo que a origem monte o quadro física e complete a transmissão. Na dinâmica do processo DAD, caso outra máquina intercepte a mensagem NS e constate que o IP testado já pertence à sua interface, ela devolve um anúncio NA para notificar o emissor original de que a identidade está ocupada, forçando-o a rejeitar o endereço para evitar conflitos de IP na rede. Se o tempo limite expirar sem que nenhum anúncio NA de contestação retorne, o host assume que o endereço é exclusivo e valida seu uso.

<a name="item12.03"><h4>12.3 Teste de Ping e Traceroute</h4></a>[Back to summary](#item12)

🛠️ Diagnóstico de Conectividade com o Utilitário Ping   
O ping é uma ferramenta de diagnóstico compatível com os protocolos IPv4 e IPv6, desenvolvida para testar a conectividade de Camada 3 entre dois dispositivos. Seu funcionamento baseia-se no envio de mensagens de solicitação de eco ICMP (Echo Request) em direção a um endereço específico. Caso o destino receba o pacote e esteja operacional, ele devolve uma mensagem de resposta de eco (Echo Reply).

Durante a execução, o utilitário calcula e exibe o tempo transcorrido entre o disparo da solicitação e a chegada da resposta. Essa métrica serve como um indicador do desempenho e da latência da infraestrutura. O programa opera associado a um temporizador de limite de espera (timeout). Se uma resposta não retornar dentro desse prazo, o sistema exibe uma notificação de falha.

O esgotamento do tempo limite pode apontar falhas físicas ou lógicas no trajeto, mas também pode ser gerado por políticas de segurança que bloqueiam o tráfego ICMP. Adicionalmente, é comum que a primeira solicitação de uma sequência sofra timeout caso o dispositivo local precise realizar o processo de resolução de endereços na Camada 2 (via ARP no IPv4 ou Neighbor Discovery no IPv6) antes de conseguir disparar o pacote de eco.

Ao término do procedimento, o utilitário exibe um relatório consolidado contendo o percentual de sucesso e o tempo médio de ida e volta (Round-Trip Time). O isolamento de falhas por meio do ping estrutura-se em três níveis de testes:

🔄 1. Teste de Loopback Local   
Consiste em direcionar o comando para o endereço de loopback interno do host, utilizando o IP 127.0.0.1 no IPv4 ou ::1 no IPv6. Uma resposta bem-sucedida atesta que a pilha de protocolos TCP/IP está instalada e funcionando na camada de rede da máquina local, fazendo com que o dispositivo envie um pacote para si mesmo. Contudo, o sucesso desse teste não garante que os parâmetros de máscara, gateway ou o hardware da placa de rede estejam operando corretamente; ele valida apenas o subsistema de software da Camada 3.

🚪 2. Teste do Gateway Padrão   
Realizado ao disparar o comando para o endereço IP da interface local do roteador. O sucesso desse teste confirma que a placa de rede do host, o meio físico da rede local, o switch intermediário e a interface do roteador que serve de saída estão totalmente operacionais na LAN.

Se o gateway padrão não responder, o técnico pode testar o IP de outra estação da mesma rede que sabidamente esteja ativa:
- Caso o outro host responda, mas o gateway permaneça inativo, o problema reside na interface do roteador ou em uma falha de parametrização no host, como a configuração de um IP incorreto para o gateway.
- Outra causa provável é a presença de regras de controle de acesso ou firewalls na interface do roteador, impedindo o processamento de pacotes ICMP.

🌐 3. Teste de Host Remoto   
Consiste em efetuar o ping apontando para o endereço lógico de um dispositivo localizado em um segmento de rede externo. A validação desse fluxo atesta o funcionamento de uma grande parcela da infraestrutura interconectada. O sucesso do teste confirma a comunicação interna na LAN, a integridade operacional do gateway local, o funcionamento de todos os roteadores que compõem o caminho de trânsito até o destino e, por fim, a atividade da própria estação remota. Caso o host remoto possua restrições de saída ou esteja desligado, nenhuma resposta será devolvida.

🚦 Rastreamento de Caminhos e Mapeamento de Saltos via Traceroute   
Enquanto o ping limita-se a atestar a conectividade fim a fim, o utilitário traceroute (executado como tracert em sistemas Windows) mapeia o trajeto percorrido pelos pacotes, gerando uma listagem sequencial de todos os roteadores intermediários (saltos) alcançados ao longo do percurso.

Essa ferramenta é crucial para localizar pontos de falha ou gargalos na infraestrutura de tráfego. Se os pacotes deixarem de alcançar o destino final, o relatório do traceroute exibirá o endereço do último roteador que respondeu ao processo, indicando a localização aproximada do problema ou o ponto onde barreiras de segurança interceptaram o fluxo.

🕒 O Tempo de Ida e Volta (RTT) no Rastreamento   
O traceroute mede o RTT individual para cada um dos saltos ao longo do caminho. Caso um roteador intermediário falhe em responder a uma das sondagens, o programa sinaliza a perda exibindo um caractere asterisco (*). A amostragem de latências elevadas ou perdas intermitentes em um determinado salto indica que o hardware daquele roteador específico ou seus links de comunicação adjacentes encontram-se sobrecarregados.

⏳ A Dinâmica de Funcionamento com TTL e Limite de Saltos   
O traceroute explora de forma intencional os mecanismos de proteção contra loops contidos no cabeçalho de Camada 3: o campo de Vida Útil (TTL) no IPv4 e o campo de Limite de Saltos (Hop Limit) no IPv6, operando em conjunto com as mensagens de erro de tempo excedido do ICMP.

O processo de mapeamento ocorre por meio do seguinte ciclo de mensagens:
- Sondagem Inicial: O traceroute dispara a primeira sequência de pacotes configurando o campo TTL ou Limite de Saltos com o valor inicial igual a 1.
- Intercepção no Primeiro Salto: Ao receber o pacote, o primeiro roteador da rota reduz o valor do campo em uma unidade, zerando o contador. O roteador descarta o pacote e devolve uma mensagem ICMP de tempo excedido (Time Exceeded) para a origem. O traceroute coleta o IP do remetente desse alerta, catalogando o endereço do primeiro salto.
- Progressão Linear: O utilitário incrementa progressivamente o valor do campo para 2, 3, 4 e assim por diante nas rajadas subsequentes. Cada incremento permite que o pacote avance um salto a mais na topologia antes de expirar e forçar o próximo roteador a devolver o aviso de tempo excedido.
- Finalização no Destino: Esse avanço gradual estende-se até que o pacote alcance o host de destino final ou atinja um limite máximo configurado no programa. Ao interceptar o pacote, o host de destino constata que a mensagem chegou ao seu destino real. Em vez de descartar o pacote por tempo excedido, o dispositivo final encerra o rastreamento devolvendo uma mensagem ICMP de resposta de eco ou um alerta de porta inalcançável, sinalizando o término do mapeamento da rota.

<a name="item12.04"><h4>12.4 Resumo ICMP</h4></a>[Back to summary](#item12)

📢 O Papel do Protocolo ICMP   
Como o protocolo IP opera de forma agnóstica sob o modelo de melhor esforço, a arquitetura TCP/IP utiliza o ICMP para emitir notificações de erro e relatórios operacionais durante a comunicação entre ativos. O objetivo dessas mensagens não é injetar confiabilidade ou garantir a entrega do tráfego IP, mas sim fornecer um feedback técnico sobre anomalias no processamento dos pacotes, estando disponível tanto no ecossistema IPv4 quanto no IPv6.

🎯 Mecanismo de Verificação de Eco   
A ferramenta primária para checar a acessibilidade de um dispositivo baseia-se no envio de uma mensagem de solicitação de eco ICMP (Echo Request). Quando o dispositivo transmissor despacha esse pacote para um alvo específico, o host de destino, caso esteja ligado e operacional na rede, processa a demanda e devolve obrigatoriamente uma resposta de eco (Echo Reply), confirmando o canal de comunicação.

🚫 Notificação de Destino Inacessível   
Sempre que um computador ou roteador intermediário se depara com um pacote que não pode ser entregue ao destinatário final, ele gera uma mensagem de destino inalcançável direcionada ao host de origem. Esse aviso carrega códigos numéricos padronizados que especificam a causa exata do problema, detalhando se a falha decorre de uma rede inexistente, host desligado ou porta de serviço bloqueada.

⏱️ Efeito do Tempo Excedido (TTL)   
Os roteadores utilizam a mensagem ICMP Time Exceeded para conter o tráfego órfão na rede. No IPv4, se um roteador recebe um pacote e, ao processá-lo, reduz o campo TTL (Tempo de Vida) para zero, o dado é descartado e um alerta de tempo esgotado é enviado ao emissor. O ICMPv6 desempenha exatamente a mesma função de descarte e aviso quando o campo Limite de Saltos do cabeçalho IPv6 atinge o valor zero.

🔄 Inovações do Protocolo ICMPv6 e NDP   
Embora o ICMPv6 herde as funções clássicas de diagnóstico do seu antecessor, ele incorpora capacidades exclusivas para gerenciar a descoberta de vizinhos (NDP) em redes de nova geração. Essa evolução elimina a necessidade de transmissões em broadcast através de quatro mensagens específicas: as solicitações e anúncios de roteadores (RS e RA) e as consultas e avisos de vizinhos físicos (NS e NA).

📊 Auditoria de Desempenho com Ping   
A execução do comando ping ativa o ciclo de eco do ICMP e monitora o intervalo cronometrado entre o envio do pedido e a chegada da resposta. Essa métrica de tempo serve como indicador de desempenho e latência da infraestrutura. O utilitário possui também um limite de tolerância temporal; caso a resposta exceda esse prazo de espera, o sistema notifica a perda do pacote.

🧪 Escala de Testes com Ping   
O isolamento de falhas através do ping ocorre de forma progressiva, dividindo-se em três etapas lógicas de testes:
- Validação da Loopback: Realizar o ping no endereço de loopback testa a integridade interna da pilha de protocolos do próprio sistema operacional, confirmando que o software de rede está inicializado.
- Teste do Gateway: Disparar contra o IP do roteador local valida se a placa física do computador e a interface interna do roteador estão conversando corretamente dentro da rede local.
- Alvo Remoto: Um teste bem-sucedido contra um IP externo atesta o funcionamento de toda a cadeia: a LAN local, o encaminhamento do gateway e o roteamento através das redes intermediárias da internet.

🛣️ Rastreamento de Rotas com Tracert   
O utilitário tracert mapeia o caminho físico percorrido pelos dados, listando sequencialmente cada interface de roteador alcançada até o destino final. Se o fluxo sofrer uma interrupção no meio do trajeto, o endereço do último nó que respondeu ao comando aponta com precisão a localização do problema técnico ou a presença de um bloqueio de segurança na infraestrutura.

⏱️ Diagnóstico por Salto e Manipulação do TTL   
Para descobrir o nome dos roteadores no caminho, o traceroute manipula deliberadamente o campo TTL (ou Limite de Saltos no IPv6), iniciando o primeiro pacote com valor igual a um e incrementando essa métrica a cada novo disparo. Esse processo força cada roteador do trajeto a descartar o pacote e devolver uma mensagem de tempo excedido. O comando calcula o tempo de ida e volta de cada tentativa e exibe um asterisco (*) sempre que uma resposta é perdida.
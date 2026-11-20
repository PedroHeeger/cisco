# Networking Devices and Initial Configuration - Módulo 7   <img src="../0-aux/logo_course.png" alt="sfp_008" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">sfp_008 (Networking Devices and Initial Configuration)   <img src="../0-aux/logo_course.png" alt="sfp_008" width="auto" height="25"></a>
### Module: 7. Resolução de Endereços

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

### Course Module 7 Structure:
7. <a name="item07">Resolução de Endereços</a><br>
  7.1 <a href="#item07.01">Introdução</a><br>
  7.2 <a href="#item07.02">ARP</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;7.2.1 <a href="../../../pkt/files/pkt_024/">Packet Tracer – Exame da Tabela ARP</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;7.2.2 <a href="../../../labs/files/lab_060/">Laboratório - Visualizar tráfego ARP no Wireshark</a><br>
  7.3 <a href="#item07.03">Resumo da Resolução de Endereço</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item07.01"><h4>7.1 Introdução</h4></a>[Back to summary](#item07)

🔍 Resolução de Endereços em Redes Locais   
A transmissão de dados dentro de um mesmo segmento de rede exige a associação direta entre o endereçamento lógico da camada de rede e o endereçamento físico da camada de enlace. Para que um dispositivo envie um pacote a outro host local, é necessário mapear o identificador IP ao respectivo identificador de hardware (MAC). Esse processo de tradução e descoberta é essencial para que os quadros de dados sejam estruturados corretamente e alcancem as interfaces físicas de destino na infraestrutura local.

🎯 Objetivo do módulo:   
- Explicar o funcionamento e a importância do protocolo ARP nos processos de comunicação interna de uma rede de área local.

📘 Tópicos do módulo:   
- ARP: Descrição detalhada da finalidade do Address Resolution Protocol, analisando seus mecanismos de requisição, resposta e armazenamento em tabelas locais para a localização de dispositivos.

<a name="item07.02"><h4>7.2 ARP</h4></a>[Back to summary](#item07)

🔍 O Papel do Protocolo ARP na Rede Local   
Dentro de uma infraestrutura baseada no protocolo IPv4, a comunicação na Camada 2 (Enlace) depende exclusivamente do conhecimento dos endereços físicos. Embora os nomes de dispositivos e os endereços lógicos (IP) facilitem a localização na Camada 3, as placas de rede (NICs) só conseguem despachar quadros Ethernet se souberem o destino físico exato.

A função do protocolo ARP (Address Resolution Protocol) é preencher essa lacuna através de duas tarefas básicas:
- Mapear e traduzir endereços IPv4 conhecidos em seus respectivos endereços MAC.
- Construir e gerenciar uma tabela de indexação na memória do dispositivo para armazenar esses vínculos.

Sempre que um host inicia uma transmissão, ele analisa a localização do destino. Se o alvo residir no mesmo segmento local, o emissor busca o MAC do próprio nó de destino. Caso o alvo esteja em uma sub-rede remota, o pacote precisa sair do perímetro local; portanto, o host busca o endereço MAC do seu gateway padrão (a interface do roteador local).

💾 A Tabela ou Cache ARP   
Para evitar a busca constante de identidades na rede, cada dispositivo mantém um banco de dados temporário na memória RAM conhecido como tabela ARP ou cache ARP. Cada linha dessa estrutura atua como um mapa, vinculando um IP específico ao seu respectivo endereço físico. Se o mapeamento pretendido já constar na tabela, o dispositivo extrai o endereço MAC e o insere diretamente no campo de destino do quadro Ethernet. Se o registro não existir, a pilha de protocolos inicia o processo de descoberta ativa através do tráfego de requisições.

📢 O Mecanismo de Busca: Requisição e Resposta ARP   
O processo de descoberta de um endereço físico ocorre em duas etapas consecutivas e envolve comportamentos distintos dos ativos de rede:

1. A Requisição ARP (Solicitação):
- Quando o endereço MAC correspondente a um IP é desconhecido, o host gera uma mensagem de requisição. Esta estrutura é injetada diretamente no quadro Ethernet, sem conter um cabeçalho IPv4.
- Identificação de Destino: O quadro adota o endereço de broadcast FF-FF-FF-FF-FF-FF. Isso força todas as placas de rede da LAN a coletar e encaminhar o quadro para a análise de seus respectivos sistemas operacionais.
- Encaminhamento no Switch: O switch recebe o broadcast e o replica por todas as suas portas ativas, exceto pela interface onde o tráfego entrou. Os roteadores barram o broadcast, impedindo-o de afetar outras sub-redes.
- Identificação de Tipo: O campo EtherType do quadro recebe o código hexadecimal 0x806, alertando a interface receptora de que os dados internos pertencem ao processo ARP.

2. A Resposta ARP: 
- Embora todos os computadores da LAN processem a requisição para verificar o IP solicitado, apenas o dispositivo que detém a identidade IPv4 idêntica à da busca gerará um retorno. As demais máquinas descartam o pacote silenciosamente.
- Tipo de Tráfego: O dispositivo correspondente envia uma resposta configurada como unicast. O endereço MAC de destino deste novo quadro aponta diretamente para a placa de rede do host que iniciou a busca.
- Finalização do Processo: Ao receber a resposta unicast, o host original lê o MAC de origem, associa-o ao IP correspondente e grava as informações na tabela cache ARP, viabilizando o envio dos quadros de dados represados. Se nenhum dispositivo responder à requisição, o pacote é descartado por impossibilidade de montagem do quadro.

⏳ Manutenção, Ciclo de Vida e Comandos da Tabela   
Os registros armazenados na cache ARP possuem natureza dinâmica. Cada entrada recebe uma marcação de tempo (timestamp); caso a interface não registre tráfego vindo daquele dispositivo antes da expiração do temporizador, o mapeamento é removido da memória. O tempo de permanência varia conforme o sistema operacional. Versões modernas do Windows, por exemplo, renovam a tabela em intervalos curtos que oscilam entre 15 e 45 segundos. Embora seja possível inserir mapas estáticos manuais que nunca expiram, tal configuração é rara na rotina operacional.

Para inspecionar ou gerenciar essas informações via linha de comando, utilizam-se os seguintes utilitários:
- No Windows 10: O comando `arp -a` exibe os mapeamentos vigentes. Parâmetros adicionais via CLI também permitem forçar a limpeza manual da cache.
- Em Roteadores Cisco: A tabela de equivalências é consultada por meio do comando `show ip arp`.

No ambiente IPv6, esse ecossistema de descoberta foi totalmente reformulado. O protocolo ARP foi substituído pelo mecanismo de ND (Neighbor Discovery), que opera através de mensagens estruturadas de solicitação e anúncio de vizinhos sobre o protocolo ICMPv6.

⚡ Impacto no Desempenho e Riscos de Segurança   
Sob condições normais em redes corporativas, o tráfego gerado por broadcasts ARP possui impacto irrelevante na largura de banda. Contudo, anomalias de desempenho conhecidas como tempestades de broadcast podem ocorrer temporariamente se centenas de equipamentos forem inicializados simultaneamente, gerando requisições síncronas. O tráfego estabiliza assim que as caches locais são preenchidas.

O maior desafio associado ao protocolo ARP reside na sua ausência nativa de mecanismos de validação, o que abre margem para vulnerabilidades de segurança:
- Falsificação ARP (ARP Spoofing / Poisoning): Um agente malicioso pode injetar respostas ARP falsas na rede local, associando o seu próprio endereço MAC ao IP de outro ativo legítimo, como o gateway padrão.
- Consequência: Os computadores da rede passam a preencher suas tabelas ARP com informações corrompidas, direcionando o tráfego de dados para a máquina do atacante em vez de enviá-lo ao roteador.
- Mitigação: Para conter essa ameaça, switches de categoria corporativa dispõem de ferramentas de proteção ativa chamadas DAI (Dynamic ARP Inspection), encarregadas de validar e filtrar mensagens ARP suspeitas antes de sua propagação.

<a name="item07.03"><h4>7.3 Resumo da Resolução de Endereço</h4></a>[Back to summary](#item07)

🔍 Funções Fundamentais do ARP   
Para transmitir dados em uma rede local, um computador precisa associar o endereço IP de destino ao seu respectivo endereço físico MAC. Quando o hardware conhece o IP mas carece do dado físico, ele aciona o protocolo ARP, que desempenha o papel duplo de traduzir os endereços IPv4 em endereços MAC e gerenciar dinamicamente esse mapeamento em uma tabela temporária.

🗺️ Lógica de Busca na Tabela   
Antes de enviar um pacote, o host consulta seu mapa interno para localizar o IP alvo. Se o destinatário residir no mesmo segmento local, o dispositivo busca o MAC correspondente ao IP do próprio host final; caso o destino pertença a uma rede externa, o computador altera a estratégia e pesquisa pelo endereço físico do seu gateway padrão para conseguir despachar a informação.

📦 Estrutura do Quadro de Requisição   
As mensagens ARP possuem a particularidade de serem envelopadas diretamente na Camada 2, dispensando o uso de um cabeçalho IPv4. O quadro de solicitação é montado com o endereço MAC de origem do remetente, o código identificador 0x806 no campo tipo — que sinaliza à placa de rede que o conteúdo pertence ao processo ARP — e o endereço físico de destino configurado em broadcast total.

📢 Inundação e Resposta Unicast   
Por ser uma mensagem de broadcast, o switch replica a requisição ARP por todas as suas saídas, exceto pela interface onde o sinal entrou. Embora todas as placas de rede da LAN recebam e processem o pacote, apenas o dispositivo que possuir o endereço IPv4 idêntico ao solicitado gerará uma resposta, enviando seus dados físicos de volta para que o emissor atualize sua tabela.

🚪 Resolução para o Gateway   
Quando a comunicação é destinada a outra sub-rede, a tabela ARP é utilizada para descobrir especificamente o endereço físico da interface do roteador local. Se o host não possuir o MAC do gateway em sua memória cache, ele inicia o ciclo de solicitação ARP focado no IP do roteador, obtendo o dado necessário para direcionar os quadros para fora da rede local de forma correta.

⏱️ Gerenciamento e Limpeza da Cache   
As informações armazenadas na tabela ARP não são permanentes e possuem um tempo de vida controlado por um temporizador interno, cujo prazo varia conforme o sistema operacional. Entradas que permanecem inativas por muito tempo são limpas automaticamente para evitar o acúmulo de dados obsoletos, mas o administrador de rede também pode realizar essa exclusão manualmente através da linha de comando.

💻 Comandos de Diagnóstico   
Para auditar as associações de endereços gravadas nos equipamentos, utilizam-se comandos específicos na CLI que variam conforme a plataforma. Em roteadores da linha Cisco, o profissional utiliza a sintaxe `show ip arp` para inspecionar os mapeamentos, enquanto em sistemas operacionais Windows o comando `arp -a` é empregado para listar a tabela ativa na máquina.

⚠️ Impacto e Riscos de Segurança   
O tráfego excessivo de broadcasts ARP, comum quando muitas máquinas são ligadas simultaneamente, pode gerar quedas temporárias de desempenho na LAN. Além disso, a falta de autenticação no protocolo abre brechas para o envenenamento ARP, técnica em que um atacante envia respostas falsas fingindo ser o gateway padrão, interceptando o tráfego de dados ao associar seu próprio MAC ao IP da rota de saída.
# Network Addressing and Basic Troubleshooting - Módulo 2   <img src="../0-aux/logo_course.png" alt="sfp_009" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">sfp_009 (Network Addressing and Basic Troubleshooting)   <img src="../0-aux/logo_course.png" alt="sfp_009" width="auto" height="25"></a>
### Module: 2. Camada de Link de Dados

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

### Course Module 2 Structure:
2. <a name="item02">Camada de Link de Dados</a><br>
  2.1 <a href="#item02.01">Introdução</a><br>
  2.2 <a href="#item02.02">Topologias</a><br>
  2.3 <a href="#item02.03">Métodos de Controle de Acesso ao Meio</a><br>
  2.4 <a href="#item02.04">Resumo da Camada de Enlace de dados</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item02.01"><h4>2.1 Introdução</h4></a>[Back to summary](#item02)

🗺️ Topologias e Controle de Acesso na Camada de Enlace   
A organização de uma infraestrutura de comunicação corporativa exige tanto o mapeamento da distribuição geográfica dos equipamentos quanto a compreensão das regras lógicas que governam a transmissão de dados. Na camada de enlace (Camada 2 do modelo OSI), essas definições determinam a forma como as informações são encapsuladas e como os múltiplos dispositivos gerenciam o compartilhamento dos meios de transmissão, evitando colisões de pacotes e assegurando a integridade do fluxo de dados tanto em redes lógicas quanto físicas.

🎯 Objetivo do módulo:   
- Explicar a função dos métodos de controle de acesso ao meio e a importância das representações topológicas no suporte à comunicação em redes locais e de longa distância.

📘 Tópicos do módulo:   
- Topologias: Análise comparativa entre o mapeamento físico (disposição geográfica de hardwares e cabeamentos) e o mapeamento lógico (caminhos de dados e esquemas de endereçamento virtuais).
- Métodos de Controle de Acesso ao Meio Físico: Estudo dos mecanismos e regras que regulam como as interfaces de rede disputam e utilizam o meio físico compartilhado para a transmissão eficiente de quadros.

<a name="item02.02"><h4>2.2 Topologias</h4></a>[Back to summary](#item02)

🏢 Classificação das Topologias de Rede: Física vs. Lógica   
A Camada de Enlace de Dados (Camada 2 do modelo OSI) atua como a interface de preparação dos dados vindos das camadas superiores para o envio rumo ao meio físico. Para desempenhar essa função com eficiência, ela precisa mapear o arranjo e o relacionamento entre os dispositivos da rede, o que constitui a topologia da rede. O mapeamento dessas interconexões em ambientes locais (LAN) ou de longa distância (WAN) subdivide-se em duas categorias de análise:
- Topologia Física: Descreve a disposição real e tangível dos componentes de hardware. Ela mapeia como os cabos e as conexões interligam os dispositivos finais (computadores, servidores) e os ativos intermediários (switches, roteadores, pontos de acesso). Esse mapeamento frequentemente traz dados minuciosos de infraestrutura, como o número de identificação de salas, a numeração de tomadas e a posição ocupada pelo equipamento dentro de um rack metálico.
- Topologia Lógica: Representa o caminho abstrato ou virtual que os quadros de dados percorrem para trafegar de um nó ao próximo. Essa visão foca exclusivamente nas interfaces de rede, conexões virtuais e no esquema de endereçamento IP (Camada 3).

A Camada de Enlace adota a perspectiva da topologia lógica para arbitrar as regras de acesso ao meio e o formato de encapsulamento dos quadros. Isso significa que, mesmo que uma rede possua uma determinada disposição física de cabos, o comportamento dos dados obedece às regras estabelecidas pela sua arquitetura lógica.

🗺️ Modelos de Topologias Físicas em Redes WAN   
As redes de longa distância utilizam arquiteturas de interconexão padronizadas para estruturar os links geográficos entre matrizes, filiais e provedores. Os três modelos fundamentais são:
- Ponto a Ponto: Representa o arranjo mais simples e comum em WANs. Estabelece um link permanente e exclusivo dedicado a interconectar apenas duas extremidades, sem compartilhamento de mídia.
- Hub and Spoke (Estrela em WAN): Arquitetura centralizada onde um site principal (Hub) atua como concentrador e estabelece conexões ponto a ponto exclusivas com as diversas filiais (Spokes). Nesse modelo híbrido, as filiais ficam impedidas de trocar informações diretamente entre si; todo e qualquer tráfego deve obrigatoriamente transitar pelo nó central antes de alcançar outro ponto da periferia.
- Malha (Mesh): Modelo focado em tolerância a falhas e alta disponibilidade, caracterizado pela interconexão direta de cada nó a todos os outros dispositivos da malha. Essa redundância integral neutraliza pontos únicos de falha, embora gere um aumento considerável nos custos de contratação de links e na complexidade de gerência administrativa. Variações parciais desse modelo (Malhas Parciais) interconectam diretamente apenas os pontos críticos da organização para reduzir custos.

🔄 A Conexão Ponto a Ponto e o Fluxo de Dados   
Na arquitetura ponto a ponto clássica, a ligação física direta entre dois nós elimina a necessidade de dividir a mídia de transmissão com outros computadores.

Quando essa topologia opera com protocolos de comunicação serial dedicados, como o PPP (Point-to-Point Protocol), a mecânica da Camada de Enlace torna-se extremamente simplificada. Como os pacotes injetados em uma extremidade do cabo possuem como destino óbvio e único o nó fixado na outra ponta, o dispositivo receptor dispensa o processamento necessário para verificar se o endereço contido no quadro coincide com a sua própria identidade.

É importante ressaltar que a inclusão de conexões físicas intermediárias ou o trânsito por dentro de uma nuvem de operadora não descaracteriza essa topologia. Dois roteadores geograficamente distantes podem estar separados por múltiplos switches e sistemas de transporte físico de terceiros; contudo, do ponto de vista lógico da Camada 2, eles continuam enxergando um canal ponto a ponto direto e transparente entre si.

Por outro lado, se a tecnologia Ethernet for empregada para estabelecer um link ponto a ponto (como no caso de dois roteadores interconectados por um cabo de rede tradicional), as interfaces mantêm as regras nativas do protocolo, exigindo que o dispositivo processador inspecione o cabeçalho do quadro para validar se ele é o destinatário real da informação.

🎛️ Topologias em Redes Locais (LAN) Modernas   
Nas redes locais contemporâneas, o arranjo de múltiplos computadores adota estruturas centralizadas que facilitam a expansão e o isolamento de problemas físicos:
- Estrela: Modelo onde todos os dispositivos terminais convergem suas conexões cabeadas para um único ativo intermediário central, papel desempenhado modernamente por um switch Ethernet (e historicamente por hubs).
- Estrela Estendida: Evolução do modelo básico criada para expandir o alcance da LAN. Consiste na interconexão em cascata de múltiplos switches centrais, onde cada um gerencia seu próprio grupo de dispositivos em estrela. Essa arquitetura entrega alta escalabilidade para inserção ou remoção de hosts e simplifica o processo de identificação de falhas (troubleshooting). Em diagramas técnicos, é comum simplificar a representação de segmentos Ethernet complexos desenhando apenas uma linha reta contínua ligando as estações aos switches.

⏳ Infraestruturas Locais Legadas   
O desenvolvimento histórico das redes locais envolveu duas arquiteturas de cabeamento que caíram em desuso devido a limitações de desempenho, mas que consolidaram os fundamentos de controle de acesso:
- Barramento (Bus): Topologia onde todas as estações de trabalho eram encadeadas linearmente ao longo de um único cabo coaxial compartilhado. As duas extremidades físicas do barramento exigiam a instalação de terminadores resistivos para absorver os sinais e evitar o eco eletromagnético. Dispensava o uso de switches ou concentradores, apresentando baixo custo de implantação inicial, mas sofria com colisões massivas de dados e quedas totais da rede caso o cabo sofresse qualquer interrupção mecânica.
- Anel (Ring): Arquitetura circular onde cada computador conecta-se diretamente aos seus dois vizinhos imediatos, fechando um anel físico que dispensa terminadores. Os dados trafegavam de forma unidirecional, sendo inspecionados e regenerados por cada nó até alcançarem o destinatário. Tecnologias legadas como o Token Ring e redes de alta velocidade de fibra óptica como o FDDI (Fiber Distributed Data Interface) utilizavam essa estrutura para coordenar o tráfego de dados livre de colisões.

<a name="item02.03"><h4>2.3 Métodos de Controle de Acesso ao Meio</h4></a>[Back to summary](#item02)

📡 Modos de Transmissão Duplex e Alinhamento de Interfaces   
A compreensão dos mecanismos de duplexação é um fator crítico na análise de topologias de redes locais, pois esse conceito define a direção e a simultaneidade do fluxo de dados entre dois pontos interconectados. A engenharia de redes adota dois modos operacionais principais:
- Comunicação Half-Duplex (Meio Duplex): Permite que ambos os dispositivos realizem tarefas de transmissão e recepção através do meio físico compartilhado, porém essas ações nunca podem ocorrer ao mesmo tempo. Caso um dispositivo esteja injetando dados na mídia, ele deve concluir o envio antes de conseguir escutar o canal. Esse modelo rege o funcionamento das redes sem fio locais (WLANs) e das antigas topologias em barramento estruturadas com hubs Ethernet. Nessas mídias de acesso compartilhado, apenas uma estação retém o privilégio de transmissão por vez.
- Comunicação Full-Duplex (Duplex Completo): Viabiliza o envio e o recebimento de dados de forma estritamente simultânea na mídia de rede. Sob essa perspectiva, a Camada de Enlace pressupõe que o canal físico encontra-se disponível de forma permanente para ambos os nós realizarem transmissões bidirecionais a qualquer instante. Os switches Ethernet operam de forma nativa e por padrão em modo Full-Duplex. Contudo, suas portas possuem a capacidade de regredir para o modo Half-Duplex caso sejam interconectadas a um ativo legado (como um hub Ethernet).

Para assegurar a estabilidade e a eficiência de um link de comunicação, as duas interfaces diretamente conectadas — como a placa de rede (NIC) de um computador e a respectiva porta do switch — devem ser configuradas para operar sob o mesmo regime duplex. O desalinhamento desses parâmetros gera uma falha conhecida como incompatibilidade de duplex (duplex mismatch), anomalia que provoca colisões tardias, descarte massivo de quadros, perda de vazão e alta latência no canal de comunicação.

🎛️ Estratégias de Controle de Acesso em Redes Multiacesso   
Os ambientes de rede local (LANs e WLANs) são classificados como redes de multiacesso, pois possuem uma arquitetura que permite a dois ou mais dispositivos terminais tentar disputar a utilização da mídia de transmissão de forma simultânea. Para evitar o caos eletromagnético e garantir a integridade dos dados em mídias compartilhadas, criaram-se duas abordagens de mediação:

Acesso Baseado em Contenção (Não Determinístico)   
- Neste modelo, todos os nós da rede operam obrigatoriamente em modo Half-Duplex e competem ativamente pelo direito de transmitir dados no meio físico compartilhado. Como a mídia é única, apenas um dispositivo pode injetar sinais por vez, exigindo regras claras para gerenciar o tráfego e resolver conflitos caso duas ou mais estações transmitam em sincronia. Os dois principais métodos de contenção do mercado são:
  - CSMA/CD (Carrier Sense Multiple Access with Collision Detection): Mecanismo de acesso múltiplo com detecção de colisão empregado nas redes locais Ethernet legadas estruturadas em barramento ou concentradas por hubs.
  - CSMA/CA (Carrier Sense Multiple Access with Collision Avoidance): Mecanismo de acesso múltiplo com prevenção de colisão adotado de forma nativa nas redes sem fio locais (padrão IEEE 802.11).

Acesso Controlado (Determinístico)   
Abordagem onde cada dispositivo possui um intervalo de tempo exclusivo e previamente agendado para realizar suas transmissões na mídia de rede. Trata-se de uma arquitetura legada e altamente ineficiente sob a ótica moderna, visto que um host com dados prontos para envio é forçado a aguardar passivamente a sua vez na rotação do sistema para conseguir acessar o meio de transmissão. As tecnologias Token Ring e ARCNET são os exemplos históricos que utilizavam esse modelo de controle de acesso.

Nota de Evolução Tecnológica: As redes locais Ethernet modernas operam exclusivamente através de conexões ponto a ponto dedicadas fornecidas por switches em modo Full-Duplex. Como os canais de transmissão e recepção são fisicamente isolados em cada porta, o risco de colisões foi integralmente extinto, dispensando o uso de qualquer mecanismo de controle de acesso ao meio na Camada 2.

🏎️ Funcionamento do Protocolo CSMA/CD em Redes Ethernet Legadas   
Os ambientes que operam com hubs ou cabos coaxiais compartilham o mesmo domínio de colisão e operam em Half-Duplex, limitando o canal a uma única transmissão por vez. Quando duas interfaces ignoram essa restrição e injetam sinais de forma simultânea no meio físico, ocorre o fenômeno da colisão, evento que corrompe mutuamente os sinais elétricos de ambos os quadros e exige a retransmissão posterior dos dados.

O fluxo de transmissão de dados em uma rede baseada em CSMA/CD obedece à seguinte sequência operacional:
- Sondagem da Mídia (Carrier Sense): Antes de liberar um quadro Ethernet em direção ao destino, a placa de rede (NIC) do host emissor realiza uma escuta ativa no cabo para verificar a presença de um sinal portador. Se a interface não detectar nenhuma atividade de tensão elétrica, ela assume que o canal está livre e inicia a transmissão do quadro.
- Encaminhamento pelo Hub: O hub Ethernet atua como um repetidor multiporta de Camada 1. Ao receber os bits de dados por uma de suas portas de entrada, o hardware simplesmente regenera o sinal elétrico e o replica de forma idêntica para todas as outras portas ativas do equipamento.
- Filtragem no Destino: Devido à replicação em massa do hub, todas as estações de trabalho conectadas recebem uma cópia do quadro. Contudo, as placas de rede dos computadores inspecionam o endereço de destino contido no cabeçalho de Camada 2. Apenas o host que possui a identidade correspondente ao destino aceita o pacote e copia os dados para as camadas superiores; todas as outras interfaces descartam o quadro silenciosamente.
- Mecanismo de Detecção de Colisão (Collision Detection): Se outra estação disparar dados no mesmo instante, ocorre a colisão. As placas de rede dos emissores detectam o conflito comparando os dados que estão transmitindo com os sinais que retornam pela linha ou percebendo uma elevação incomum na amplitude da tensão elétrica da mídia. Ao constatar o choque de sinais, os dispositivos interrompem a transmissão, acionam um temporizador de espera aleatório e reiniciam o ciclo após a liberação do meio.

📡 Prevenção de Conflitos com o Protocolo CSMA/CA em WLANs   
No ecossistema das redes sem fio (WLANs), a natureza da propagação das ondas de rádio no espaço livre impede que uma interface consiga detectar colisões de forma confiável enquanto realiza uma transmissão. Por essa limitação física, o padrão IEEE 802.11 substitui a detecção pela estratégia de prevenção de colisões (CSMA/CA), agindo proativamente para evitar que os conflitos ocorram.

O protocolo CSMA/CA emprega técnicas adicionais para coordenar o espaço aéreo compartilhado:
- Anúncio de Reserva do Meio: O método de escuta do CSMA/CA monitora se o espectro de rádio está livre de forma semelhante ao sistema cabeado. Contudo, ao iniciar uma transmissão, o dispositivo sem fio inclui no cabeçalho do quadro a informação exata do tempo necessário para concluir o envio daquela mensagem.
- Sincronização de Vizinhança: Todos os outros hosts sem fio situados no raio de cobertura interceptam esse quadro, leem o indicador de duração e passam a saber exatamente por quanto tempo a mídia aérea permanecerá ocupada. Consequentemente, as estações vizinhas adiam suas próprias transmissões, aguardando o término do período de reserva estipulado para evitar interferências.
- Mecanismo de Confirmação (ACK): Diferente da rede Ethernet cabeada, o receptor de um quadro sem fio deve obrigatoriamente devolver um pacote de confirmação (Acknowledgment - ACK) imediato para o emissor após receber os dados com sucesso. Se o remetente original não receber o pacote ACK dentro de uma janela de tempo determinada, ele assume que o quadro sofreu interferência ou foi perdido, iniciando o processo de retransmissão.

É importante frisar que, tanto em LANs Ethernet estruturadas com hubs quanto em redes sem fio locais, os sistemas baseados em contenção sofrem com sérios problemas de escalabilidade. À medida que o volume de tráfego e o número de hosts ativos aumentam no segmento, o índice de colisões e o tempo de espera preventiva crescem exponencialmente, degradando sensivelmente a capacidade útil da rede sob condições de uso intenso.

<a name="item02.04"><h4>2.4 Resumo da Camada de Enlace de dados</h4></a>[Back to summary](#item02)

📐 Topologias Físicas e Lógicas   
A organização de uma rede é classificada sob duas perspectivas distintas: a estrutura física, que mapeia a disposição real dos cabos e equipamentos, e a estrutura lógica, que define o caminho virtual que os dados percorrem. A camada de enlace de dados interpreta a rede através do modelo lógico, e essa percepção dita o formato dos quadros e as regras de controle de acesso ao meio físico.

🌐 Modelos de Topologia em Redes WAN   
As redes de longa distância adotam três arranjos físicos principais para conectar localidades geograficamente separadas:
- Ponto a Ponto: Une diretamente duas extremidades da rede, mantendo essa relação lógica mesmo se houver repetidores físicos no trajeto.
- Hub and Spoke: Centraliza o tráfego em um nó principal que se ramifica para unidades satélites.
- Malha (Mesh): Conecta os locais de forma redundante, oferecendo múltiplos caminhos para os dados.

🏢 Disposição de Redes Locais (LAN)   
No ambiente das redes locais, os dispositivos finais são interconectados por meio de topologias como estrela, estrela estendida, barramento ou anel. Nos modelos em estrela e estrela estendida, que dominam as infraestruturas modernas, todos os computadores convergem para um equipamento intermediário central, como um switch, que gerencia a distribuição das mensagens.

🔄 Modos de Transmissão Duplex   
O fluxo de dados entre duas interfaces pode operar em duas modalidades. No modo half-duplex, a comunicação é bidirecional, mas ocorre em apenas um sentido por vez, exigindo que um dispositivo espere o outro terminar de transmitir. No modo full-duplex, o envio e o recebimento de dados acontecem simultaneamente; ambas as pontas do link devem estar alinhadas no mesmo modo para evitar incompatibilidades que geram lentidão.

📢 Redes de Múltiplo Acesso   
Tecnologias como redes Ethernet cabeadas e conexões Wi-Fi (WLAN) são classificadas como ambientes de múltiplo acesso, pois permitem que vários dispositivos compartilhem a mesma infraestrutura de comunicação simultaneamente. Devido a essa concorrência, o sistema necessita de regras estritas de arbitragem para ditar como e quando cada equipamento pode utilizar o meio físico.

🚦 Controle de Acesso Baseado em Contenção   
Para gerenciar redes compartilhadas, os sistemas dividem-se entre o acesso controlado e o acesso baseado em contenção. No modelo por contenção, os dispositivos operam em half-duplex e competem pelo uso do canal. Para evitar o caos de transmissões simultâneas, utilizam-se protocolos de escuta: o CSMA/CD atua em redes Ethernet antigas de topologia em barramento para detectar colisões, enquanto o CSMA/CA é empregado em redes sem fio para prevenir e evitar que as colisões aconteçam.
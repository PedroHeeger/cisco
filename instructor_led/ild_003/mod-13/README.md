# Fundamentos de Redes - Módulo 13   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_003 (Fundamentos de Redes)   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="25"></a>
### Module: 13. O Processo de ARP

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

### Course Module 13 Structure:
13. <a name="item13">O Processo de ARP</a><br>
  13.1 <a href="#item13.01">Introdução</a><br>
  13.2 <a href="#item13.02">MAC e IP</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;13.2.1 <a href="../../../pkt/files/pkt_??/">Packet Tracer – Identificar endereços MAC e IP</a><br>
  13.3 <a href="#item13.03">Contenção de Broadcast</a><br>
  13.4 <a href="#item13.04">Resumo da O Processo de ARP</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item13.01"><h4>13.1 Introdução</h4></a>[Back to summary](#item13)

🆔 Endereçamento Lógico e Físico: IP e MAC   
A comunicação em redes de computadores depende da interação entre dois níveis distintos de identificação. Enquanto o endereço IP (lógico) é dinâmico e identifica a localização de um dispositivo em uma infraestrutura específica, o endereço MAC (físico) é permanente e identifica o hardware de forma única. A coordenação entre esses dois endereçamentos permite que os dados sejam roteados globalmente e entregues com precisão ao terminal de destino final.

🎯 Objetivo do módulo:   
- Explicar a função do protocolo ARP na viabilização da comunicação dentro de uma infraestrutura de rede.

📘 Tópicos do módulo:   
- MAC e IP: Comparação técnica entre as responsabilidades do endereçamento de Camada 2 (físico) e Camada 3 (lógico) na entrega de dados.
- Contenção de Broadcast: Análise da necessidade de limitar o tráfego de difusão para preservar a largura de banda e a eficiência do processamento nos dispositivos da rede.

<a name="item13.02"><h4>13.2 MAC e IP</h4></a>[Back to summary](#item13)

🧩 A Necessidade da Resolução de Endereços   
A comunicação eficiente em uma rede local depende da coexistência de duas identificações distintas em cada dispositivo. O endereço lógico (IP) atua na camada 3 e é responsável por orientar o pacote desde a sua origem até o destino final, independentemente da distância. Já o endereço físico (MAC) opera na camada 2, sendo o identificador permanente da placa de rede (NIC) utilizado para a entrega de dados entre dispositivos conectados ao mesmo segmento físico.

A resolução de endereços manifesta-se como um processo crítico sempre que um host conhece o IP do destinatário, mas carece do endereço MAC necessário para realizar a transmissão física dos dados através do meio.

🏠 Dinâmica na Rede Local   
Quando a origem e o destino encontram-se na mesma rede IP, o processo de entrega ocorre de forma direta. O pacote IP é encapsulado em um quadro Ethernet, onde os campos de endereçamento de camada 2 são preenchidos com o MAC da placa de rede do emissor e o MAC da placa de rede do receptor. Nesse contexto, o switch utiliza a informação física para encaminhar o sinal elétrico precisamente para a porta onde o host de destino está vinculado, permitindo que a mensagem seja recebida e processada sem a necessidade de intermediários de camada 3.

🗺️ Interação com Redes Remotas   
A lógica de endereçamento sofre uma alteração importante quando o destino final reside em uma rede externa ou na internet. Devido às limitações tecnológicas, um host não possui a capacidade de descobrir endereços físicos de dispositivos situados além das fronteiras de sua própria rede local. Para solucionar este impasse, o pacote é encaminhado ao Gateway Padrão, que representa a interface do roteador local.

Nessa operação, o pacote mantém o endereço IP do destino final original, mas o quadro Ethernet utiliza o endereço MAC do roteador como destino de camada 2. Ao recepcionar o dado, o roteador executa o desencapsulamento do quadro, analisa o endereço IP de destino para determinar a melhor rota e realiza um novo encapsulamento. Esse ciclo de alteração dos endereços MAC de origem e destino repete-se a cada salto (hop) entre roteadores, enquanto o conteúdo do pacote IP permanece inalterado até o alcance da rede de destino.

🔄 Protocolos de Descoberta Automática   
A associação sistemática entre os endereços de camada 3 e camada 2 é gerida por protocolos de controle especializados, que variam conforme a versão do protocolo de internet utilizada:
- ARP (Address Resolution Protocol): Empregado em redes IPv4, este protocolo realiza consultas ao segmento de rede para mapear endereços IP em endereços MAC correspondentes.
- ICMPv6 Neighbor Discovery (ND): Utilizado em redes IPv6, este mecanismo substitui o ARP, integrando funções de descoberta de vizinhos e verificação de acessibilidade de forma otimizada e eficiente.

A manutenção da integridade desse mapeamento garante que, embora o trajeto envolva múltiplos links físicos e diferentes tecnologias de enlace, a mensagem lógica chegue ao destinatário pretendido com precisão.

<a name="item13.03"><h4>13.3 Contenção de Broadcast</h4></a>[Back to summary](#item13)

📡 Domínios de Broadcast e a Dinâmica do ARP   
O funcionamento de uma rede local Ethernet baseia-se na capacidade de propagação de mensagens para todos os integrantes de um mesmo segmento. Quando ocorre o envio de um broadcast, os switches encaminham o quadro para todas as interfaces ativas, definindo o que se conhece tecnicamente como domínio de broadcast. A recepção e o processamento dessas mensagens são realizados por todos os hosts como se a comunicação fosse direcionada individualmente a cada um deles.

📉 Impacto no Desempenho e Segmentação   
A existência de domínios de broadcast excessivamente amplos pode comprometer a estabilidade da rede. O aumento no número de dispositivos conectados eleva proporcionalmente o volume de tráfego de difusão, o que demanda recursos significativos de processamento tanto dos switches quanto dos próprios hosts.

Para mitigar a lentidão e otimizar o tráfego, aplica-se a divisão da rede local em segmentos menores. Nesse contexto, os roteadores desempenham um papel fundamental, pois atuam como fronteiras físicas e lógicas que impedem a propagação de broadcasts entre diferentes redes, isolando o tráfego de difusão em domínios restritos.

🔍 O Desafio da Resolução de Endereços   
Embora os aplicativos utilizem endereços IP lógicos para identificar serviços e clientes, a entrega física de dados na camada de enlace exige o conhecimento do endereço MAC do destinatário. Uma Placa de Interface de Rede (NIC) só processa quadros cujo endereço de destino coincida com o seu próprio endereço físico ou com o endereço de broadcast.

Para solucionar a lacuna entre o endereço IP conhecido e o endereço MAC necessário, utiliza-se o protocolo ARP (Address Resolution Protocol) em redes IPv4. Em infraestruturas IPv6, uma função análoga é desempenhada pelo mecanismo de Descoberta de Vizinhos (Neighbor Discovery).

⚙️ O Ciclo de Operação do ARP   
O processo de descoberta e mapeamento de endereços físicos ocorre de forma metódica em três estágios principais:
- Solicitação de Broadcast: O host emissor gera um quadro destinado ao endereço MAC de broadcast. No conteúdo desta mensagem, insere-se o endereço IPv4 do destinatário que se pretende alcançar.
- Verificação e Resposta: Todos os dispositivos no domínio de broadcast recebem o quadro. Cada host analisa a mensagem e compara o IP solicitado com o seu próprio endereço configurado. Apenas o detentor do IPv4 correspondente envia uma resposta direta ao emissor original, informando o seu endereço MAC.
- Armazenamento em Tabela: Ao recepcionar a resposta, o host de origem registra a associação entre o IPv4 e o MAC em uma estrutura de memória denominada tabela ARP.

Uma vez que a informação encontra-se armazenada na tabela ARP, as comunicações subsequentes entre esses dois hosts ocorrem de forma direta, sem a necessidade de novas consultas de broadcast. A eficácia deste protocolo depende estritamente de que todos os envolvidos habitem o mesmo domínio de broadcast, permitindo a circulação livre das solicitações iniciais de mapeamento.

<a name="item13.04"><h4>13.4 Resumo da O Processo de ARP</h4></a>[Back to summary](#item13)

🔍 Necessidade da Resolução de Endereços   
Para que a comunicação ocorra em uma rede Ethernet, o conhecimento apenas do endereço IP não é suficiente; o hardware precisa identificar o endereço físico (MAC) do destino. Enquanto o endereço IP (lógico) serve para rotear a mensagem globalmente, o endereço MAC (físico) é o que permite a entrega real entre as placas de rede (NICs) dentro de um mesmo segmento físico.

🛣️ Encaminhamento entre Redes   
Quando o destino está em uma rede externa, o host remetente não busca o MAC do destinatário final, mas sim o endereço físico do seu gateway padrão. O roteador, ao receber o quadro, remove a camada de enlace para ler o IP e decidir a melhor rota. A cada "salto" entre roteadores, o pacote é re-encapsulado em um novo quadro com endereços MAC atualizados para aquele link específico, até chegar à rede de destino.

📢 O Papel do MAC de Broadcast   
Existem situações em que um host precisa falar com todos ou descobrir alguém sem saber seu endereço específico. Para isso, utiliza-se o endereço MAC de broadcast, composto por 48 bits em nível lógico alto (representado em hexadecimal como FFFF.FFFF.FFFF). Qualquer dispositivo que receba um quadro com esse destino é obrigado a processar a mensagem, permitindo a disseminação de informações essenciais na rede local.

🏢 Domínios de Broadcast e Performance   
Uma rede composta por um ou mais switches forma o que chamamos de domínio de broadcast, pois o switch replica essas mensagens para todas as suas portas. No entanto, se houver muitos dispositivos gerando transmissões simultâneas, o desempenho pode cair drasticamente. Para solucionar isso, utilizam-se roteadores para segmentar a infraestrutura em domínios menores, filtrando o tráfego e otimizando os recursos dos switches.

⚙️ Funcionamento do Protocolo ARP   
O ARP (Address Resolution Protocol) é o mecanismo que traduz um IPv4 conhecido em um endereço MAC. O processo ocorre em três etapas:
- O emissor envia um quadro de broadcast perguntando "Quem possui este IP?".
- Todos recebem, mas apenas o dono do IP responde enviando seu endereço MAC.
- O emissor armazena essa relação em uma tabela ARP para comunicações futuras, evitando novas consultas. No mundo IPv6, essa função é desempenhada pelo protocolo de Descoberta de Vizinhos (Neighbor Discovery).
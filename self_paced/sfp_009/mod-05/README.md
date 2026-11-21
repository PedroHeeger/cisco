# Network Addressing and Basic Troubleshooting - Módulo 5   <img src="../0-aux/logo_course.png" alt="sfp_009" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">sfp_009 (Network Addressing and Basic Troubleshooting)   <img src="../0-aux/logo_course.png" alt="sfp_009" width="auto" height="25"></a>
### Module: 5. Descoberta de vizinhos IPv6

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

### Course Module 5 Structure:
5. <a name="item05">Descoberta de vizinhos IPv6</a><br>
  5.1 <a href="#item05.01">Introdução</a><br>
  5.2 <a href="#item05.02">Operação de descoberta de vizinho</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;5.2.1 <a href="../../../pkt/files/pkt_025/">Packet Tracer - Descoberta de Vizinhos IPv6</a><br>
  5.3 <a href="#item05.03">Resumo da descoberta de vizinhos IPv6</a><br>
  5.4 Exame de ponto de verificação: Endereçamento IP.<br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item05.01"><h4>5.1 Introdução</h4></a>[Back to summary](#item05)

🔍 Protocolo de Descoberta de Vizinhos no Ecossistema IPv6   
No ambiente IPv6, o gerenciamento de relações locais e a tradução de parâmetros de rede ocorrem por meio de uma arquitetura unificada conhecida como Descoberta de Vizinhos (ND - Neighbor Discovery). Este protocolo elimina o uso de transmissões generalizadas (broadcast), integrando funções que permitem aos dispositivos mapear endereços de hardware, localizar roteadores disponíveis no link local e certificar-se de que não existem identificadores lógicos duplicados operando no mesmo segmento de rede.

🎯 Objetivo do módulo:   
- Explicar os mecanismos e as mensagens do protocolo ND que viabilizam a comunicação e o reconhecimento de dispositivos em redes IPv6.

📘 Tópicos do módulo:   
- Operação de descoberta de vizinho: Estudo das interações baseadas no protocolo ICMPv6, detalhando o funcionamento das mensagens de Solicitação/Anúncio de Vizinho (Neighbor Solicitation/Advertisement).

<a name="item05.02"><h4>5.2 Operação de descoberta de vizinho</h4></a>[Back to summary](#item05)

🤝 O Protocolo de Descoberta de Vizinhos (ND)   
O protocolo de Descoberta de Vizinhos do IPv6, amplamente conhecido como ND ou NDP (Neighbor Discovery Protocol), é a engrenagem baseada em mensagens ICMPv6 que substitui o antigo protocolo ARP do IPv4 e adiciona funções inteligentes de infraestrutura. Normatizado pela especificação RFC 4861 da IETF, o ND fornece serviços essenciais de resolução de endereços físicos, localização de roteadores e otimização de rotas.

Para gerenciar essas interações, o protocolo utiliza uma estrutura baseada em cinco tipos de mensagens ICMPv6:
- Solicitação de Roteador (RS): Enviada por hosts para localizar roteadores ativos no link.
- Anúncio de Roteador (RA): Emitida por roteadores para propagar prefixos e parâmetros de rede.
- Solicitação de Vizinho (NS): Utilizada em comunicações direta entre dispositivos para descobrir endereços MAC ou validar a exclusividade de um IP.
- Anúncio de Vizinho (NA): Funciona como a resposta direta e confirmatória para as mensagens NS.
- Mensagem de Redirecionamento: Disparada por um roteador para informar a um host a existência de um caminho ou próximo salto mais eficiente para alcançar determinado destino.

As mensagens de interação com roteadores (RS e RA) são o pilar para mecanismos de provisionamento dinâmico e autoconfiguração de estações (SLAAC). Já as mensagens de vizinhança (NS e NA) governam as conversas de dispositivo para dispositivo, abrangendo computadores, servidores e as próprias interfaces dos roteadores locais.

🔍 Resolução de Endereços MAC no IPv6   
O processo de mapear um endereço lógico de Camada 3 para um endereço físico de Camada 2 (MAC) é chamado de resolução de endereços. No IPv6, essa tarefa dispensa as transmissões em broadcast e adota um fluxo otimizado de solicitações e anúncios de vizinho.

Para compreender a mecânica de funcionamento desse recurso, analisa-se o seguinte cenário prático:
- O Envio da Solicitação (NS): O computador PC1 (com o IP 2001:db8:acad:1::10) precisa realizar um teste de ping contra o PC2 (IP 2001:db8:acad:1::11). Como o PC1 conhece apenas a identidade lógica do destino, ele cria uma mensagem de Solicitação de Vizinho (NS) equivalente a um questionamento direcionado: "Quem possui o endereço IPv6 2001:db8:acad:1::11? Por favor, envie-me o seu endereço MAC."
- A Otimização de Hardware: Em vez de propagar essa pergunta para todas as máquinas da rede local em broadcast, o PC1 encapsula a mensagem NS utilizando um endereço de rede e um endereço físico Ethernet multicast especial (o nó solicitado). Essa engenharia permite que as placas de rede (NICs) dos demais computadores da LAN interceptem o quadro e identifiquem, diretamente no hardware, se a mensagem é de seu interesse. Se o IP consultado não for o delas, a própria placa descarta o pacote sem interromper o processamento do sistema operacional.
- A Resposta com o Anúncio (NA): Ao receber e processar a solicitação NS, o PC2 reconhece seu próprio endereço IPv6. Ele monta imediatamente uma mensagem de Anúncio de Vizinho (NA) e a envia de volta para o PC1, respondendo de forma direta: "Eu sou o detentor do IP 2001:db8:acad:1::11 e o meu endereço MAC é F8-94-C3-E4-C5-0A."

Ao capturar o anúncio NA, o PC1 registra o endereço físico do parceiro em seu cache local, completa o encapsulamento dos quadros pendentes e estabelece a comunicação direta de Camada 2 através do switch local.

<a name="item05.03"><h4>5.3 Resumo da descoberta de vizinhos IPv6</h4></a>[Back to summary](#item05)

🔄 O Protocolo Neighbour Discovery (ND)   
O ecossistema IPv6 descarta completamente o uso do protocolo ARP. Em seu lugar, adota-se o protocolo ND (Neighbour Discovery), que opera integrado ao ICMPv6 para gerenciar as comunicações locais da Camada 2. Suas funções vão além da simples descoberta de hardware, abrangendo a localização automática de roteadores na rede e o redirecionamento de fluxos de tráfego para caminhos mais eficientes.

💬 As Cinco Mensagens do ND   
Para estruturar todos os seus serviços de infraestrutura sem recorrer a transmissões em broadcast, o protocolo baseia-se em um diálogo composto por cinco tipos de mensagens específicas do ICMPv6:
- Solicitação de Vizinho (NS - Neighbor Solicitation): Mensagem enviada para descobrir o endereço físico de um dispositivo local conhecido.
- Anúncio de Vizinho (NA - Neighbor Advertisement): Resposta contendo o endereço MAC correspondente, enviada pelo dono do IP solicitado.
- Solicitação de Roteador (RS - Router Solicitation): Pedido enviado pelos hosts locais para localizar os roteadores ativos no link.
- Anúncio de Roteador (RA - Router Advertisement): Resposta periódica ou imediata dos roteadores, fornecendo prefixos de IP e gateway padrão.
- Redirecionamento (Redirect): Mensagem usada pelos roteadores para informar a um host que existe uma rota melhor ou um gateway mais próximo para um destino específico.

🎯 Resolução de Endereços Físicos   
Assim como o ARP realiza a tradução no mundo IPv4, os dispositivos com suporte a IPv6 recorrem ao ND para mapear e descobrir o endereço MAC de um computador a partir de seu endereço IPv6. A grande diferença técnica está na eficiência: o ND utiliza o tráfego multicast em vez de inundar a rede local com broadcasts, garantindo que apenas os dispositivos interessados gastem recursos de processamento para ler a mensagem.
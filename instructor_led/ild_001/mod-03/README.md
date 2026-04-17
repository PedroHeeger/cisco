# CCNA: Introduction to Networks - Módulo 3   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_001 (CCNA: Introduction to Networks)   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="25"></a>
### Module: 3. Protocolos e modelos

---

### Theme:
- Network

### Used Tools:
- Operating System (OS): 
  - Windows 11 <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/windows13.png" alt="windows11" width="auto" height="25">
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
3. <a name="item03">Protocolos e modelos</a><br>
  3.1 <a href="#item03.01">Introdução</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.1.1 <a href="../../../labs/files/lab_006/">Atividade em Classe - Projetar um Sistema de Comunicação</a><br>
  3.2 <a href="#item03.02">As regras</a><br>
  3.3 <a href="#item03.03">Protocolos</a><br>
  3.4 <a href="#item03.04">Conjuntos de protocolos</a><br>
  3.5 <a href="#item03.05">Empresas de padrões</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.5.1 <a href="../../../labs/files/lab_007/">Laboratório - Pesquisa dos Padrões de Rede</a><br>
  3.6 <a href="#item03.06">Modelos de Referência</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.6.1 <a href="../../../pkt/files/pkt_013/">Packet Tracer - Investigue os modelos TCP / IP e OSI em ação</a><br>
  3.7 <a href="#item03.07">Encapsulamento de dados</a><br>
  3.8 <a href="#item03.08">Acesso a dados</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.8.1 <a href="../../../labs/files/lab_008/">Laboratório - Instalar o Wireshark</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.8.2 <a href="../../../labs/files/lab_009/">Laboratório - Usar o Wireshark para ver o tráfego na Rede</a><br>
  3.9 <a href="#item03.09">Módulo Prático e Quiz</a><br>
  3.10 Exame de Comunicação e Conectividade de Rede Básica<br>
  
---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item03.01"><h4>3.1 Introdução</h4></a>[Back to summary](#item03)

📘 Introdução
Neste módulo, o foco foi em entender como a comunicação em rede realmente acontece. Para que diferentes dispositivos consigam trocar informações, é necessário seguir conjuntos de regras bem definidos, conhecidos como protocolos. Esses protocolos são organizados em modelos que ajudam a visualizar o caminho que os dados percorrem e a função de cada etapa desse processo. Com essa base, fica mais fácil compreender como redes de qualquer tamanho operam de forma coordenada.

🎯 Objetivo Geral   
Apresentar como os protocolos permitem que dispositivos utilizem recursos tanto locais quanto remotos por meio de regras padronizadas.

✅ Objetivos Específicos   
- Tipos de regras necessárias para que a comunicação funcione de forma consistente.
- Importância dos protocolos na troca de informações entre dispositivos.
- Motivos para seguir um conjunto padronizado de protocolos.
- Papel das organizações de padrões na construção de regras que asseguram interoperabilidade.
- Uso dos modelos TCP/IP e OSI para padronizar o processo de comunicação.
- Funcionamento do encapsulamento como mecanismo para transportar dados pela rede.
- Acesso de hosts a recursos disponíveis localmente.

<a name="item03.02"><h4>3.2 As regras</h4></a>[Back to summary](#item03)

🌐 Diversidade das Redes e a Necessidade de Regras   
Redes podem conectar desde apenas dois dispositivos até milhões espalhados pelo mundo. A simples existência de um cabo ou sinal sem fio não garante comunicação. Para que a troca de informações ocorra, os dispositivos precisam seguir um conjunto definido de regras que orienta como a mensagem deve ser enviada, recebida e interpretada.

💬 Elementos Básicos da Comunicação   
Independentemente de ser uma conversa presencial ou um envio de dados, toda comunicação envolve três componentes:
- Origem: quem gera a mensagem.
- Destino: quem recebe e interpreta.
- Meio: caminho utilizado para transportar a informação.

Esses elementos formam a estrutura mínima para qualquer troca de dados.

📜 Papel dos Protocolos na Comunicação   
A transmissão de uma mensagem — seja uma conversa, uma carta ou um pacote de dados — depende de regras específicas chamadas protocolos. Cada meio de comunicação usa regras próprias, garantindo que emissor e receptor consigam entender a mensagem usando os mesmos critérios de formato, ordem e comportamento.

- Analogia: Para que duas pessoas conversem de forma clara, precisam concordar sobre:
  - qual idioma usar;
  - omo estruturar frases;
  - quando falar e quando ouvir;
  - como confirmar entendimento.
  - Sem essas regras, a comunicação se torna confusa ou impossível.

- Aplicação em Redes de Computadores: Em redes, o conceito é o mesmo. Protocolos definem:
  - como identificar origem e destino;
  - como organizar e transportar a mensagem;
  - como lidar com erros;
  - como controlar a velocidade da transmissão;
  - como solicitar confirmação de entrega.
  - Essas regras tornam a comunicação previsível e confiável.

🔡 Codificação da Mensagem   
Antes de ser transmitida, a informação precisa ser convertida para um formato que o meio físico consiga transportar.

- Analogia: Comunicação Humana: Ao conversar por telefone sobre um pôr do sol, a descrição verbal traduz o pensamento em linguagem falada, que chega ao ouvinte e é interpretada novamente.
- Aplicação em Redes de Computadores: O host converte a mensagem em bits. Esses bits são traduzidos em sinais elétricos, pulsos de luz ou ondas de rádio, dependendo do meio. O dispositivo de destino decodifica os sinais e reconstrói a informação original.

📦 Formatação e Encapsulamento   
Todo envio de mensagem segue um padrão de estrutura.

- Analogia: Uma carta precisa de remetente, destinatário e endereço colocado no local correto do envelope. A carta (conteúdo) é colocada dentro de outro formato (envelope), caracterizando o encapsulamento.
- Aplicação em Redes de Computadores: Pacotes seguem formatos rígidos definidos por protocolos. O IP, por exemplo, adiciona campos que indicam origem e destino. No recebimento, ocorre o desencapsulamento para revelar os dados.

✂️ Tamanho da Mensagem   
Mensagens longas não são transmitidas de uma só vez.

- Analogia: Na comunicação verbal, frases longas são divididas em partes menores para que o ouvinte consiga acompanhar.
- Aplicação em Redes de Computadores: Protocolos exigem que mensagens grandes sejam divididas em quadros ou pacotes menores. Cada parte recebe um cabeçalho com endereços e informações necessárias. No destino, as partes são reorganizadas para restaurar a mensagem completa.

⏱️ Temporização na Comunicação   
A troca de informações depende de sincronização entre as partes. Isso envolve:
- Controle de fluxo: garante que o receptor não receba dados mais rápido do que pode processar.
- Tempo de resposta: define quanto tempo aguardar uma confirmação antes de considerar a transmissão falha.
- Método de acesso: determina quando um dispositivo pode transmitir sem causar colisões no meio.

Esses mecanismos evitam sobrecarga, congestionamento e perda de dados.

📡 Modos de Entrega da Mensagem   
A comunicação em rede pode ocorrer de formas distintas:
- Unicast: envio direcionado a um único destino.
- Multicast: entrega para um grupo específico de destinatários.
- Broadcast: envio para todos os dispositivos de uma rede.

Cada método é escolhido conforme a necessidade e o tipo de aplicação.

🟣 Representação de Dispositivos   
Em diagramas e topologias, dispositivos costumam ser representados como nós, geralmente exibidos como círculos. Essa convenção facilita a visualização das diferentes formas de envio e dos caminhos utilizados pela comunicação.

<a name="item03.03"><h4>3.3 Protocolos</h4></a>[Back to summary](#item03)

📡 Visão geral dos protocolos   
Dispositivos em uma rede só conseguem trocar informações quando seguem o mesmo conjunto de regras. Esses conjuntos são os protocolos, responsáveis por definir formatos, comportamentos e como as mensagens são manipuladas durante a comunicação.

🧩 Função dos protocolos   
Cada protocolo cumpre um papel específico dentro da rede, podendo estar implementado em hardware, software ou ambos. Eles definem como mensagens são criadas, transmitidas e interpretadas.

- Funções exercidas pelos protocolos   
Para que dados circulem entre dispositivos finais, protocolos desempenham funções essenciais:
  - Endereçamento: identifica origem e destino (ex.: Ethernet, IPv4, IPv6).
  - Confiabilidade: garante entrega mesmo com perdas (ex.: TCP).
  - Controle de fluxo: evita sobrecarga entre remetente e receptor (ex.: TCP).
  - Sequenciamento: mantém a ordem correta dos segmentos (ex.: TCP).
  - Detecção de erros: verifica integridade dos dados (ex.: Ethernet, IPv4, TCP).
  - Interface de aplicação: define como aplicações trocam informações (ex.: HTTP/HTTPS).

🗂️ Tipos de protocolos em redes   
Existem diferentes categorias de protocolos, cada uma atendendo a necessidades distintas dentro da comunicação:
- Comunicação: viabilizam trocas de dados através de uma ou mais redes (ex.: IP, TCP, HTTP).
- Segurança: fornecem autenticação, integridade e criptografia (ex.: SSH, SSL, TLS).
- Roteamento: permitem que roteadores troquem rotas e escolham caminhos (ex.: OSPF, BGP).
- Descoberta de serviços: realizam detecção automática de serviços e dispositivos (ex.: DHCP, DNS).

🌐 Protocolos atuando juntos   
Uma comunicação completa normalmente utiliza vários protocolos ao mesmo tempo. Em uma solicitação a um servidor web, por exemplo, diferentes camadas participam:
- HTTP: define como cliente e servidor web estruturam solicitações e respostas.
- TCP: mantém a conversa, controla fluxo e oferece entrega confiável.
- IP: encaminha os pacotes entre redes até o destino final.
- Ethernet: permite a entrega entre dispositivos dentro da mesma rede local.

<a name="item03.04"><h4>3.4 Conjuntos de protocolos</h4></a>[Back to summary](#item03)

🔗 Suítes de protocolos   
Protocolos precisam operar em conjunto para permitir comunicação completa. Uma suíte de protocolos é um conjunto organizado de protocolos inter-relacionados que atuam de forma integrada para executar funções de rede.

🪜 Pilha de protocolos   
A interação entre protocolos é representada como uma pilha em camadas.
- As camadas inferiores lidam com movimentação de dados pela rede.
- As camadas superiores tratam do conteúdo e da lógica de comunicação.

Cada camada depende das funcionalidades fornecidas pelas camadas abaixo.

- Exemplo de camadas na comunicação humana
A comunicação face a face pode ser usada como analogia:
  - Camada física: pessoas falando, som e voz.
  - Camada de regras: língua escolhida e normas de comunicação.
  - Camada de conteúdo: ideia transmitida na conversa.

🧬 Evolução das suítes de protocolos   
Diversas suítes foram criadas desde os anos 1970, algumas abertas e outras proprietárias. Entre elas:
- TCP/IP
- OSI
- AppleTalk
- Novell NetWare

🌍 TCP/IP e outras suítes históricas   
TCP/IP é o conjunto de protocolos mais relevante atualmente, mantido pela IETF. OSI foi uma suíte completa com modelo em sete camadas, hoje usado principalmente como referência teórica. AppleTalk e NetWare/IPX foram suítes proprietárias que acabaram substituídas pelo TCP/IP.

🛰️ Camadas atendidas pelo TCP/IP   
TCP/IP abrange protocolos para:
- Camada de Aplicação
- Camada de Transporte
- Camada de Internet
- A Camada de Acesso à Rede utiliza protocolos LAN, como Ethernet e WLAN.

- Exemplo de uso do TCP/IP
Em uma comunicação entre navegador e servidor web, os protocolos típicos são:
  - Aplicação: HTTP
  - Transporte: TCP
  - Internet: IP
  - Acesso à Rede: Ethernet ou WLAN

📦 Componentes atuais do TCP/IP   
- Camada de Aplicação:
  - DNS: converte nomes de domínio em endereços IP.
  - DHCPv4: atribui endereços IPv4 automaticamente.
  - DHCPv6: atribui endereços IPv6 automaticamente.
  - SLAAC: configura IPv6 sem necessidade de servidor DHCP.
  - SMTP: envia mensagens entre clientes e servidores de e-mail.
  - POP3: baixa mensagens para o dispositivo do usuário.
  - IMAP: acessa mensagens mantendo-as no servidor.
  - FTP: transfere arquivos com confirmação.
  - SFTP: transfere arquivos com segurança via SSH.
  - TFTP: transfere arquivos com baixa sobrecarga e sem confirmação.
  - HTTP: acessa documentos, páginas e conteúdo Web.
  - HTTPS: mesma função do HTTP, porém com criptografia.
  - REST: modelo de APIs baseado em métodos HTTP.
- Camada de Transporte:
  - TCP: comunicação confiável e ordenada.
  - UDP: comunicação sem confiabilidade e sem controle de ordem.
- Camada de Internet:
  - IPv4: endereçamento de 32 bits.
  - IPv6: endereçamento de 128 bits.
  - NAT: traduz endereços privados em endereços públicos.
  - ICMPv4: envia mensagens de erro e diagnóstico.
  - ICMPv6: envia avisos e erros para IPv6.
  - ICMPv6 ND: descobre vizinhos e detecta duplicidade de endereço.
  - OSPF: protocolo de roteamento por estado de enlace.
  - BGP: troca rotas entre grandes redes e provedores.
  - EIGRP: protocolo com métrica composta e rápida convergência.
- Camada de Acesso à Rede:
  - ARP: relaciona endereços IPv4 a endereços MAC.
  - Ethernet: define comunicação em redes cabeadas.
  - WLAN: define comunicação em redes sem fio.

🧭 Características do TCP/IP   
TCP/IP possui duas propriedades fundamentais:
- Padrão aberto: disponível gratuitamente e implementável por qualquer fornecedor.
- Baseado em padrões: garante interoperabilidade entre fabricantes distintos.

<a name="item03.05"><h4>3.5 Empresas de padrões</h4></a>[Back to summary](#item03)

🧩 Importância dos padrões   
A indústria de redes utiliza padrões para garantir que dispositivos de diferentes fabricantes funcionem juntos. Esses padrões asseguram interoperabilidade, concorrência justa e inovação, evitando que qualquer fornecedor monopolize o mercado.

🚗 Analogia com a indústria automotiva   
Assim como diversos fabricantes podem produzir pneus que servem no mesmo carro por seguirem padrões automotivos, diversos fornecedores de equipamentos de rede podem produzir dispositivos compatíveis porque seguem padrões abertos (como IPv4, IPv6, Ethernet e 802.11).

🌍 Padrões abertos   
Padrões abertos permitem:
- Interoperabilidade entre dispositivos e sistemas operacionais diferentes.
- Implementações livres por qualquer fornecedor.
- Manutenção de uma Internet aberta e acessível.

🏛️ Organizações de padronização   
As organizações de padronização são, em geral, entidades sem fins lucrativos dedicadas a desenvolver e manter padrões internacionais.

- Organizações gerais:
  - IEEE: Define padrões como Ethernet (802.3) e WLAN (802.11).
  - IETF: Desenvolve e mantém os protocolos da Internet e TCP/IP por meio dos RFCs.
  - IANA: Gerencia alocação de endereços IP, nomes de domínio e identificadores de protocolos.
  - ICANN: Coordena o sistema global de nomes de domínio e endereços IP.
  - ITU-T: Define padrões de telecomunicações, como IPTV, DSL e compressão de vídeo.
  - EIA: Desenvolve padrões de cabeamento, conectores e racks.
  - TIA: Cria padrões para comunicações VoIP, rádio, satélites e cabos estruturados.

- Organizações focadas em Internet:
  - ISOC (Internet Society): Promove o desenvolvimento aberto da Internet.
  - IAB (Internet Architecture Board): Supervisiona o desenvolvimento dos padrões da Internet.
  - IETF (via IESG): Mantém e atualiza tecnologias TCP/IP e especificações dos RFCs.
  - IRTF (via IRSG): Realiza pesquisas de longo prazo sobre Internet, como criptografia, P2P e antispam.

<a name="item03.06"><h4>3.6 Modelos de Referência</h4></a>[Back to summary](#item03)

🧩 Conceito de modelo   
Modelos em camadas são representações que ajudam a visualizar e compreender o funcionamento de redes. Eles simplificam conceitos complexos dividindo operações em partes menores e gerenciáveis.

🎯 Benefícios do uso de modelos em camadas   
- Auxiliam no projeto de protocolos ao definir funções claras por camada.
- Incentivam concorrência ao permitir interoperabilidade entre fabricantes.
- Evitam que mudanças em uma camada impactem outras.
- Fornecem linguagem comum para descrever funções de rede.

🧭 Principais modelos de referência   
Dois modelos descrevem a operação das redes:
  - Modelo OSI (Open Systems Interconnection)
  - Modelo TCP/IP

🗂️ Modelo OSI (7 Camadas)   
  - Aplicação: Protocolos usados para comunicação entre processos.
  - Apresentação: Fornece representação comum dos dados trocados.
  - Sessão: Gerencia diálogos e organização da troca de dados.
  - Transporte: Segmenta, transfere e remonta dados entre dispositivos finais.
  - Rede: Fornece serviços para encaminhar dados entre dispositivos identificados.
  - Enlace de Dados: Define métodos para troca de quadros em um meio compartilhado.
  - Física: Define aspectos mecânicos, elétricos e de sinalização para transmissão de bits.

🌐 Modelo TCP/IP (4 Camadas)   
- Aplicação: Representa dados ao usuário, incluindo controle de diálogo e codificação.
- Transporte: Oferece comunicação entre dispositivos em redes distintas.
- Internet: Define o melhor caminho para entrega dos pacotes.
- Acesso à Rede: Controla hardware e meio físico utilizados na transmissão.

📦 Suíte de Protocolos TCP/IP por Camada   
- Acesso à Rede (OSI 1–2):
  - Ethernet
  - WLAN
  - SONET
  - SDH
- Internet (OSI 3):
  - IPv4
  - IPv6
  - ICMPv4
  - ICMPv6
- Transporte (OSI 4):
  - TCP
  - UDP
- Aplicação (OSI 5–7):
  - HTTP
  - DNS
  - DHCP
  - FTP

🔍 Relação entre OSI e TCP/IP   
- Mapeamentos diretos:
  - OSI 3 ↔ TCP/IP Internet: Endereçamento e roteamento.
  - OSI 4 ↔ TCP/IP Transporte: Entrega confiável e ordenada.
- Mapeamentos agrupados:
  - OSI 5, 6 e 7 ↔ TCP/IP Aplicação: Protocolos e serviços de aplicação.
  - OSI 1 e 2 ↔ TCP/IP Acesso à Rede: Acesso à mídia e transmissão física.

🏛️ Padrões e RFCs   
- RFCs:
  - Definições dos padrões TCP/IP são discutidas publicamente na IETF.
  - RFCs documentam especificações de protocolos e atualizações.
- Modelo TCP/IP como modelo de protocolo:
  - Criado nos anos 70.
  - Representa a organização real dos protocolos usados na Internet.

<a name="item03.07"><h4>3.7 Encapsulamento de dados</h4></a>[Back to summary](#item03)

✂️ Segmentação de dados   
Grandes fluxos de dados não são enviados como um bloco único; eles são divididos em partes menores chamadas segmentos para evitar atrasos, facilitar o compartilhamento do canal e reduzir impacto em caso de falhas.

- Por que segmentar?
  - Mais velocidade: pacotes menores permitem multiplexação, várias comunicações compartilhando o mesmo link.
  - Mais eficiência: se um pacote falha, apenas ele é retransmitido — não toda a mensagem.

- Caminhos diferentes:
  - Pacotes de uma mesma mensagem podem seguir rotas diferentes até o destino, chegando fora de ordem e exigindo remontagem.

- Complexidade da segmentação:
Cada parte da mensagem precisa de informações adicionais. Isso garante que o destinatário consiga reconstruir tudo corretamente. As principais informações adicionais são:
  - Endereçamento;
  - Número de sequência;
  - Identificação;
  - Controle de ordem.

📥 Encapsulamento   
À medida que os dados descem pela pilha TCP/IP, cada camada adiciona seu próprio cabeçalho. Esse processo é chamado de encapsulamento.

📤 Desencapsulamento   
No host de destino, o processo ocorre ao contrário:
- A camada recebe a PDU;
- Remove seu cabeçalho;
- Entrega os dados à camada superior;
- Até chegar à aplicação.

📚 PDUs em cada camada   
Cada camada nomeia sua PDU de acordo com sua função:
- Dados: Aplicação;
- Segmento: Transporte (TCP);
- Datagrama: Transporte (UDP);
- Pacote: Rede;
- Quadro: Enlace de Dados;
- Bits: Física.

🧪 Observações importantes   
- Terminologia TCP/UDP:
  - Cabeçalho TCP → chama-se segmento;
  - Cabeçalho UDP → chama-se datagrama;
- Camadas e PDUs:
  - Cada camada encapsula a PDU da camada superior dentro do seu próprio cabeçalho (e às vezes trailer).

<a name="item03.08"><h4>3.8 Acesso a dados</h4></a>[Back to summary](#item03)

🧭 Visão Geral dos Endereços em Redes   
As mensagens segmentadas só chegam ao destino quando cada camada trata corretamente seus endereços. As camadas de Rede (Layer 3) e Enlace de Dados (Layer 2) trabalham juntas para entregar dados entre origem e destino.

🌐 Endereços da Camada de Rede   
Os endereços da camada de rede identificam origem lógica e destino final do pacote IP, independente de estarem na mesma ou em redes diferentes.
- Origem (IP): dispositivo que envia o pacote.
- Destino (IP): dispositivo que deve receber o pacote.
- Função: levar o pacote do ponto inicial até o ponto final, passando por qualquer número de roteadores.

🔗 Endereços da Camada de Enlace de Dados   
A camada de enlace entrega quadros de uma NIC para outra dentro da mesma rede física.
- Origem: Endereço físico (MAC) de origem.
- Destino: Endereço físico (MAC) de destino.
- Função: garantir a entrega do quadro dentro do segmento local.

🧱 Funções das Camadas   
- Física: bits, temporização e sincronização.
- Enlace: endereços MAC origem/destino.
- Rede: endereços lógicos IP.
- Transporte: portas dos processos.
- Aplicação: dados da aplicação.

🏷️ Endereço Lógico (Camada 3)   
O endereço IP é o endereço lógico usado para entregar o pacote ao destino final. Cada pacote contém:
- IP de origem: quem envia.
- IP de destino: quem deve receber.

Um endereço IP possui:
- Parte da rede (IPv4) / Prefixo (IPv6): identifica a rede.
- Parte do host (IPv4) / ID da interface (IPv6): identifica o dispositivo na rede.

A máscara (IPv4) ou o comprimento do prefixo (IPv6) define onde a parte da rede termina e onde a parte do host começa.

🖥️ Dispositivos na Mesma Rede   
Quando origem e destino estão na mesma rede IP:
- Origem: 192.168.1.110.
- Destino: 192.168.1.9.
- Parte da rede é igual → está no mesmo segmento.

A camada de rede identifica origem e destino lógicos, mas o envio real ocorre com MACs:
- MAC de origem: da NIC do PC1 (AA-AA-AA-AA-AA-AA).
- MAC de destino: da NIC do servidor FTP (CC-CC-CC-CC-CC-CC).

O quadro é enviado diretamente ao destino.

🛰️ Dispositivos em Redes Diferentes   
Quando origem e destino estão em redes diferentes:
- Origem: 192.168.1.110.
- Destino: 172.16.1.99.
- Partes da rede diferentes → rota através de um gateway.

🚪 Uso do Gateway Padrão (Camada de Enlace)   
Como o host de destino está em outra rede, o remetente envia o quadro para o gateway padrão.
- MAC de origem: NIC do PC1 (AA-AA-AA-AA-AA-AA).
- MAC de destino: NIC do roteador/gateway R1 (11-11-11-11-11-11).

O gateway recebe o quadro, remove a camada 2, e encaminha o pacote IP para o próximo salto. Configurar o gateway padrão é essencial: qualquer pacote para redes remotas é enviado a ele.

🧬 Papel dos Endereços MAC no Caminho   
Em cada salto:
- O pacote IP é encapsulado em um novo quadro.
- Cada quadro usa:
  - MAC de origem: NIC que envia.
  - MAC de destino: NIC que recebe o quadro naquele salto.

A camada 2 sempre opera apenas de NIC para NIC no mesmo segmento.

📦 Encapsulamento ao Longo do Caminho   
Enquanto os roteadores encaminham o pacote IP:
- A camada 2 muda a cada salto.
- A camada 3 permanece a mesma (IP origem/destino fixos).

Cada novo quadro contém:
- Endereço MAC de origem.
- Endereço MAC de destino (próximo salto ou destino final).

<a name="item03.09"><h4>3.9 Módulo Prático e Quiz</h4></a>[Back to summary](#item03)

💬 Elementos da comunicação   
Todo método de comunicação envolve três elementos: remetente, receptor e canal. A troca de mensagens segue regras chamadas protocolos, que definem identificação, linguagem, ritmo, momento e confirmação. Na comunicação de computadores, protocolos incluem codificação, formatação, encapsulamento, tamanho, temporização e opções de entrega (unicast, multicast e broadcast).

🔠 Codificação, formatação e temporização   
A codificação transforma informações em um formato adequado para transmissão; a decodificação reverte esse processo. As mensagens variam em formato conforme o tipo e o canal usado. A temporização envolve controle de fluxo, tempo limite de resposta e método de acesso ao meio.

🔌 Protocolos na operação da rede   
Protocolos podem ser implementados em hardware, software ou ambos. Uma única mensagem normalmente utiliza vários protocolos, cada um responsável por funções específicas.  
- Ethernet/IP/TCP/HTTP: transmissão de dados.
- SSH/SSL/TLS: segurança, integridade e criptografia.
- OSPF/BGP: troca de rotas e seleção de melhores caminhos.
- DHCP/DNS: descoberta automática de serviços e endereços.

Eles garantem endereçamento, confiabilidade, controle de fluxo, sequenciamento, detecção de erros e interface de aplicação.

📚 Suítes e pilhas de protocolos   
Uma suíte de protocolos é um conjunto de protocolos relacionados usados para comunicação. A pilha mostra como eles trabalham juntos. Desde os anos 1970, várias suítes surgiram, mas o TCP/IP prevaleceu por ser aberto e baseado em padrões. Ele opera em: Aplicação, Transporte, Internet e Acesso à Rede. No processo de comunicação, um servidor encapsula dados enviados ao cliente, que os desencapsula para visualização.

🏛️ Organizações de padrões   
Padrões abertos promovem interoperabilidade, concorrência e inovação. Entre as organizações envolvidas na criação e manutenção de padrões estão:  
- ISOC, IAB, IETF, IRTF: padrões para Internet.
- ICANN, IANA: padrões e gestão de TCP/IP.
- IEEE, EIA, TIA, ITU-T: padrões eletrônicos e de telecomunicações.

📦 Modelos OSI e TCP/IP   
Dois modelos descrevem a operação da rede
- **OSI (7 camadas):** Aplicação, Apresentação, Sessão, Transporte, Rede, Enlace, Física.
- **TCP/IP (4 camadas):** Aplicação, Transporte, Internet, Acesso à Rede.

🧩 Segmentação e multiplexação   
As mensagens são divididas em segmentos para permitir que múltiplas conversas compartilhem a rede (multiplexação) e para tornar mais eficiente a retransmissão caso uma parte falhe. O TCP é responsável por ordenar os segmentos.

📘 PDU, encapsulamento e desencapsulamento   
Cada camada opera com uma PDU específica. Durante o envio, o encapsulamento ocorre de cima para baixo. O dispositivo receptor realiza o desencapsulamento, removendo cabeçalhos à medida que os dados sobem na pilha.

🛰️ Endereçamento nas camadas de rede e enlace   
Camadas de rede e enlace entregam os dados da origem ao destino:  
- **Endereços IP (camada de rede):** origem e destino finais, mesmo em redes diferentes.
- **Endereços MAC (camada de enlace):** comunicação entre NICs na mesma rede física.

🌐 Estrutura de endereços IP   
Endereços IP possuem parte de rede/prefixo e parte de host/ID da interface.  
- Mesma rede: envio direto ao dispositivo destino.
- Redes diferentes: o quadro é enviado ao roteador/gateway padrão.
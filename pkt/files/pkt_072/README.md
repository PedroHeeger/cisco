# Packet Tracer - Conectar uma rede com base em um diagrama de rede   <img src="./0-aux/logo_course.png" alt="pkt_072" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../pkt/">pkt</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">pkt_072 (Packet Tracer - Conectar uma rede com base em um diagrama de rede)   <img src="./0-aux/logo_course.png" alt="pkt_072" width="auto" height="25"></a>

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
- Network:
  - Cisco Packet Tracer   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/cisco_packet_tracer.webp" alt="cisco_packet_tracer" width="auto" height="25">

---

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">Parte 1: Revise o Diagrama Lógico de Rede.</a><br>
2. <a href="#item02">Parte 2: Conecte os dispositivos físicos.</a><br>
  2.1 <a href="#item02.01">Etapa 1: Determine o tipo de cabo.</a><br>
  2.2 <a href="#item02.02">Etapa 2: Conecte os dispositivos.</a><br>

---

### Objective:
O objetivo desta atividade foi realizar o cabeamento físico da rede, conectando as interfaces dos dispositivos com os cabos apropriados, de acordo com a topologia especificada.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: Revise o Diagrama Lógico de Rede.</h4></a>[Back to summary](#item00)

A imagem 01 mostra a topologia inicial.

<div align="center"><figure>
    <img src="./0-aux/img01.png" alt="img01"><br>
    <figcaption>Imagem 01.</figcaption>
</figure></div><br>

Revise o diagrama de rede e registre como os dispositivos estão conectados na Tabela de Dispositivos abaixo.

<div align="center">

#### Tabela 1 — Topologia Física dos Dispositivos

| Nome do Dispositivo |   Tipo de Dispositivo   | Interface Local | Dispositivo e Porta Conectados |
|:-------------------:|:-----------------------:|:---------------:|:------------------------------:|
| R1                  | Router / Cisco 4321     | G0/0/0          | Servidor Web Ethernet NIC      |
| R1                  | Router / Cisco 4321     | G0/0/1          | S1 G0/1                        |
| S1                  | Switch / Catalyst 2960  | G0/1            | R1 G0/0/1                      |
| S1                  | Switch / Catalyst 2960  | G0/2            | S2 G0/2                        |
| S1                  | Switch / Catalyst 2960  | F0/1            | PC-A Ethernet NIC              |
| S2                  | Switch / Catalyst 2960  | G0/1            | R2 G0/0/1                      |
| S2                  | Switch / Catalyst 2960  | G0/2            | S1 G0/2                        |
| S2                  | Switch / Catalyst 2960  | F0/1            | PC-B Ethernet NIC              |
| R2                  | Router / Cisco 4321     | G0/0/1          | S2 G0/1                        |
| Servidor Web        | Servidor                | Ethernet        | R1 G0/0/0                      |
| PC-A                | PC                      | Ethernet        | S1 F0/1                        |
| PC-B                | PC                      | Ethernet        | S2 F0/1                        |

</div>

<a name="item02"><h4>2. Parte 2: Conecte os dispositivos físicos.</h4></a>[Back to summary](#item00)

Agora que você determinou como os dispositivos estão interconectados, pode usar as informações do diagrama de rede para conectar os dispositivos no rack dentro do armário de fiação (wiring closet). No Modo Físico no Packet Tracer, você pode praticar a conexão dos dispositivos no rack no armário de fiação.

<a name="item02.01"><h4>2.1 Etapa 1: Determine o tipo de cabo.</h4></a>[Back to summary](#item00)

- a. No diagrama de rede, você determinou que os dispositivos estão conectados via cabos Ethernet do diagrama de rede. Na placa de fixação de cabos no armário de fiação principal, existem alguns tipos diferentes de cabos. Qual é a cor dos cabos diretos Ethernet no Packet Tracer?
  - Os cabos Ethernet diretos (Copper Straight-Through), utilizados para conectar dispositivos de tipos diferentes, são representados pela cor verde. Já os cabos Ethernet cruzados (Copper Cross-Over), utilizados para conectar dispositivos do mesmo tipo, são representados pela cor laranja.

<a name="item02.02"><h4>2.2 Etapa 2: Conecte os dispositivos.</h4></a>[Back to summary](#item00)

Usando os cabos Ethernet, conecte os dispositivos no armário de fiação de acordo com o diagrama de rede.

- a. Para conectar o roteador R1 ao servidor Web, selecione um cabo Ethernet da placa peg. O Web Server é o dispositivo grande na parte inferior do rack de equipamentos.
- b. Clique na porta Web Server FastEthernet0 para conectar o cabo Ethernet.
- c. Clique em GigabitEthernet0/0/1 em R1 para concluir a conexão. Você pode ampliar o dispositivo clicando com o botão direito do mouse no dispositivo > selecione Inspecionar frontal. Clique na lupa para ampliar a frente do dispositivo. Você pode verificar se a conexão está ativa quando as luzes do LED da porta estiverem piscando em verde.
- d. Repita o procedimento para todas as outras conexões para concluir a conexão da rede. Observe que os PCs estão localizados na Mesa.

A imagem 02 evidencia todos os dispositivos devidamente interconectados por meio de seus respectivos cabos de rede.

<div align="center"><figure>
    <img src="./0-aux/img02.png" alt="img02"><br>
    <figcaption>Imagem 02.</figcaption>
</figure></div><br>
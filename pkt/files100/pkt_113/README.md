# Packet Tracer - Configuração do EtherChannel   <img src="./0-aux/logo_course.png" alt="pkt_113" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../pkt/">pkt</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">pkt_113 (Packet Tracer - Configuração do EtherChannel)   <img src="./0-aux/logo_course.png" alt="pkt_113" width="auto" height="25"></a>

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
  - ping   <img src="" alt="iputils" width="auto" height="25">
  - traceroute   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/traceroute.png" alt="traceroute" width="auto" height="25">
  - Trace Route (tracert)   <img src="" alt="tracert" width="auto" height="25">

---

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">Parte 1: Configurar as definições básicas do Switch</a><br>
2. <a href="#item02">Parte 2: Configurar um EtherChannel com Cisco PAgP</a><br>
  2.1 <a href="#item02.01">Etapa 1: Configurar o Port Channel 1.</a><br>
  2.2 <a href="#item02.02">Etapa 2: Verifique o status do Port Channel 1.</a><br>
3. <a href="#item03">Parte 3: Configurar um EtherChannel 802.3ad LACP</a><br>
  3.1 <a href="#item03.01">Etapa 1: Configure o Port Channel 2.</a><br>
  3.2 <a href="#item03.02">Etapa 2: Verifique o status do Port Channel 2.</a><br>
4. <a href="#item04">Parte 4: Configurar um link EtherChannel redundante</a><br>
  4.1 <a href="#item04.01">Etapa 1: Configure o Port Channel 3.</a><br>
  4.2 <a href="#item04.02">Etapa 2: Verifique o status do Port Channel 3.</a><br>
5. <a href="#item05">Diretrizes e restrições de configuração do EtherChannel</a><br>

---

### Objective:
O objetivo desta atividade foi construir uma pequena Rede Local (LAN), conectando os dispositivos finais aos dispositivos de rede, configurando o endereçamento IPv4 e verificando a conectividade por meio de testes de comunicação.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: Configurar as definições básicas do Switch</h4></a>[Back to summary](#item00)

A imagem 01 mostra a topologia inicial.

<div align="center"><figure>
    <img src="./0-aux/img01.png" alt="img01"><br>
    <figcaption>Imagem 01.</figcaption>
</figure></div><br>

- a. Atribuir a cada switch um hostname de acordo com o diagrama de topologia. 
- b. Antes de iniciar a agregação de link entre switches, verifique a configuração existente das portas que conectam os switches para garantir que as portas se juntem com êxito aos EtherChannels. Os comandos que fornecem informações sobre o estado das portas do switch incluem:







A imagem 02 exibe todas as conexões estabelecidas.

<div align="center"><figure>
    <img src="./0-aux/img02.png" alt="img02"><br>
    <figcaption>Imagem 02.</figcaption>
</figure></div><br>

<a name="item02"><h4>2. Parte 2: Configurar um EtherChannel com Cisco PAgP</h4></a>[Back to summary](#item00)

<a name="item02.01"><h4>2.1 Etapa 1: Configurar o Port Channel 1.</h4></a>[Back to summary](#item00)





A imagem 03 comprova que todos dispositivos finais foram corretamente endereçados.

<div align="center"><figure>
    <img src="./0-aux/img03.png" alt="img03"><br>
    <figcaption>Imagem 03.</figcaption>
</figure></div><br>

<a name="item03"><h4>3. Parte 3: Configurar um EtherChannel 802.3ad LACP</h4></a>[Back to summary](#item00)

<a name="item03.01"><h4>3.1 Etapa 1: Configure o Port Channel 2.</h4></a>[Back to summary](#item00)





<a name="item03.02"><h4>3.2 Etapa 2: Verifique o status do Port Channel 2.</h4></a>[Back to summary](#item00)





A imagem 04 mostra o servidor web sendo acessado por meio do endereço IP e o teste de conectividade realizado com êxito entre o Admin PC e a impressora.

<div align="center"><figure>
    <img src="./0-aux/img04.png" alt="img04"><br>
    <figcaption>Imagem 04.</figcaption>
</figure></div><br>

<a name="item04"><h4>4. Parte 4: Configurar um link EtherChannel redundante</h4></a>[Back to summary](#item00)



<a name="item04.01"><h4>4.1 Etapa 1: Configure o Port Channel 3.</h4></a>[Back to summary](#item00)





<a name="item04.02"><h4>4.2 Etapa 2: Verifique o status do Port Channel 3.</h4></a>[Back to summary](#item00)





A imagem 05 exibe o caminho percorrido pelos pacotes até o servidor web, indicando os roteadores atravessados durante o trajeto.

<div align="center"><figure>
    <img src="./0-aux/img05.png" alt="img05"><br>
    <figcaption>Imagem 05.</figcaption>
</figure></div><br>

<a name="item05"><h4>5. Diretrizes e restrições de configuração do EtherChannel</h4></a>[Back to summary](#item00)


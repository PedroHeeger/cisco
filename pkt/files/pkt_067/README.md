# Packet Tracer - Usando o comando ipconfig   <img src="./0-aux/logo_course.png" alt="pkt_067" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../pkt/">pkt</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">pkt_067 (Packet Tracer - Usando o comando ipconfig)   <img src="./0-aux/logo_course.png" alt="pkt_065" width="auto" height="25"></a>

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
  - ipconfig   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/ipconfig.jpeg" alt="ipconfig" width="auto" height="25">

---

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">Parte 1: Verificar configurações</a><br>
2. <a href="#item02">Parte 2: Corrija as configurações incorretas</a><br>

---

### Objective
Esta atividade teve como objetivo utilizar a ferramenta **ipconfig** para verificar as configurações de endereçamento IP dos computadores da rede, identificar o dispositivo com configuração incorreta e corrigir o endereço IP para restabelecer sua conectividade com a rede local.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: Verificar configurações</h4></a>[Back to summary](#item00)

A imagem 01 mostra a topologia inicial.

<div align="center"><figure>
    <img src="./0-aux/img01.png" alt="img01"><br>
    <figcaption>Imagem 01.</figcaption>
</figure></div><br>

- a. Acesse o prompt de comando em cada PC e digite o comando ipconfig /all no prompt.
  - `ipconfig /all`.
- b. Verifique a configuração do endereço IP, da máscara de sub-rede e do gateway padrão para cada PC. Anote essa configuração de IP de cada PC para ajudar a identificar PCs que estão configurados de forma incorreta.

<div align="center">

#### Tabela 1 — Endereçamento IPv4

| Dispositivo | Interface | Endereço IP    | Máscara de Sub-Rede | Gateway Padrão |
|:-----------:|:---------:|:--------------:|:-------------------:|:--------------:|
| PC1         | NIC       | 192.168.1.101  | 255.255.255.0       | 192.168.1.1    |
| PC2         | NIC       | 192.168.10.102 | 255.255.255.0       | 192.168.1.1    |
| PC3         | NIC       | 192.168.1.103  | 255.255.255.0       | 192.168.1.1    |
| PC4         | NIC       | 192.168.1.104  | 255.255.255.0       | 192.168.1.1    |

</div>

A imagem 02 evidencia que o endereço IP configurado no PC2 não pertencia à mesma sub-rede da rede local, impedindo o estabelecimento da comunicação.

<div align="center"><figure>
    <img src="./0-aux/img02.png" alt="img02"><br>
    <figcaption>Imagem 02.</figcaption>
</figure></div><br>

<a name="item02"><h4>2. Parte 2: Corrija as configurações incorretas</h4></a>[Back to summary](#item00)

- a. Selecione o PC que está configurado incorretamente.
- b. Clique na guia Desktop > guia IP Configuration (Configuração de IP) para corrigir a configuração incorreta.

A imagem 03 demonstra que o endereçamento IP do PC2 foi corrigido, passando a ser compatível com a rede configurada.

<div align="center"><figure>
    <img src="./0-aux/img03.png" alt="img03"><br>
    <figcaption>Imagem 03.</figcaption>
</figure></div><br>
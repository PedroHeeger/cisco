# CCNA: SRWE - Módulo 4 - Exam - Q7   <img src="./0-aux/logo_course.png" alt="pkt_106" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../pkt/">pkt</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">pkt_106 (CCNA: SRWE - Módulo 4 - Exam - Q7)   <img src="./0-aux/logo_course.png" alt="pkt_106" width="auto" height="25"></a>

---

### Theme:
- Network

### Used Tools:
- Operating System (OS): 
  - Cisco Internetwork Operating System (Cisco IOS)   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/cisco_ios.jpg" alt="cisco_ios" width="auto" height="25">
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

1. <a href="#item01">CCNA: SRWE - Módulo 4 - Exam - Q7</a><br>

---

### Objective:
O objetivo deste PTSA foi corrigir a configuração do enlace entre o S1 e o roteador, alterando-o do modo de acesso para o modo trunk, a fim de permitir o roteamento entre VLANs e possibilitar o acesso do PC ao site hospedado no servidor.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. CCNA: SRWE - Módulo 4 - Exam - Q7</h4></a>[Back to summary](#item00)

O PC1 está na VLAN 5 e conectado à interface FastEthernet 0/5 do switch SW1. O Server1 está na VLAN 10 e conectado à interface FastEthernet 0/10 do switch SW1. A interface GigabitEthernet 0/0/0 do roteador R1 está conectada à interface GigabitEthernet 0/1 do switch SW1.

- a. Abra o aplicativo Terminal no PC1 para acessar o switch SW1 e examinar a configuração do SW1. Execute o comando de configuração de interface apropriado no switch SW1 para habilitar a comunicação entre o PC1 e o Server1.
  - `show interface trunk`.
  - `enable` -> `configure terminal` -> `interface g0/1` -> `switchport mode trunk` -> `end`.
- a. Qual mensagem é exibida quando 10.10.10.1 é inserido na barra de endereços do navegador da Web do PC1?
  - Ao inserir o endereço `10.10.10.1` na barra de endereços do navegador do PC1, é exibida a mensagem "File Server", conforme apresentado na imagem 01.

<div align="center"><figure>
    <img src="./0-aux/img01.png" alt="img01"><br>
    <figcaption>Imagem 01.</figcaption>
</figure></div><br>
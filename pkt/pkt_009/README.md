# Vídeo Activity - Testar a atribuição de interface   <img src="./0-aux/logo_course.png" alt="pkt_009" width="auto" height="45">

### Cisco: <a href="../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../pkt/">pkt</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">pkt_009 (Vídeo Activity - Testar a atribuição de interface)   <img src="./0-aux/logo_course.png" alt="pkt_009" width="auto" height="25"></a>

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
  - Cisco Internetwork Operating System (Cisco IOS)   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/cisco_ios.jpg" alt="cisco_ios" width="auto" height="25">
  - Cisco Packet Tracer   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/pkt.webp" alt="pkt" width="auto" height="25">

---

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">Vídeo Activity - Testar a atribuição de interface</a><br>

---

### Objective:
O objetivo desta Video Activity foi realizar o acesso via console aos switches para habilitar a interface VLAN e realizar a atribuição de endereçamento IP, garantindo a gestão e a conectividade dos dispositivos na rede.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo desta atividade.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Vídeo Activity - Testar a atribuição de interface</h4></a>[Back to summary](#item00)

A imagem 01 mostra a topologia inicial.

<div align="center"><figure>
    <img src="./0-aux/img01.png" alt="img01"><br>
    <figcaption>Imagem 01.</figcaption>
</figure></div><br>

- PC-A -> Conectar ao switch S1 via cabo console (RS 232 - Console).
- PC-A -> Desktop -> Terminal -> Configurações Padrão (Ok) -> Executar comandos:
  - `enable` -> `show ip interface brief` -> `config terminal` -> `interface vlan 1` -> `no shutdown` -> `Ctrl+C` -> `show ip interface brief`.
- PC-B -> Conectar ao switch S2 via cabo console (RS 232 - Console).
- PC-B -> Desktop -> Terminal -> Configurações Padrão (Ok) -> Executar comandos:
  - `enable` -> `show ip interface brief` -> `config terminal` -> `interface vlan 1` -> `ip address 192.168.1.3 255.255.255.0` -> `no shutdown` -> `Ctrl+C` -> `show ip interface brief`.

A imagem 02 exibe a conclusão da atividade.

<div align="center"><figure>
    <img src="./0-aux/img02.png" alt="img02"><br>
    <figcaption>Imagem 02.</figcaption>
</figure></div><br>
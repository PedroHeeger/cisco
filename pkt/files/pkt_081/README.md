# Networking Essentials (Fundamentos de Redes) - Módulo 29 - Exam - Q15   <img src="./0-aux/logo_course.png" alt="pkt_081" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../pkt/">pkt</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">pkt_081 (Networking Essentials (Fundamentos de Redes) - Módulo 29 - Exam - Q15)   <img src="./0-aux/logo_course.png" alt="pkt_081" width="auto" height="25"></a>

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
  - ipconfig   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/ipconfig.jpeg" alt="ipconfig" width="auto" height="25">
  - Trace Route (tracert)   <img src="" alt="tracert" width="auto" height="25">

---

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">Networking Essentials (Fundamentos de Redes) - Módulo 29 - Exam - Q15</a><br>

---

### Objective:
O objetivo deste PTSA foi identificar os endereços IPv6 dos saltos percorridos na rota entre o PC1 e o PC2.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Networking Essentials (Fundamentos de Redes) - Módulo 29 - Exam - Q15</h4></a>[Back to summary](#item00)

- a. Abra o prompt de comando no PC2 e use o comando ipv6config para anotar o endereço IPv6 do PC2.
  - `ipv6config` -> `2001:DB8:1:4::A`.
- b. Abra o prompt de comando no PC1 e rastreie a rota para o PC2.
  - `tracert 2001:DB8:1:4::A`.
- b. Quais são os três endereços IPv6 exibidos quando a rota de PC1 para PC2 é rastreada? (Escolha três.)
  - `2001:DB8:1:1::1`, `2001:DB8:1:2::1` e `2001:DB8:1:3::2`.
- b. Qual é a mensagem exibida na página da Web?
  - `Trace Completo`.

A imagem 01 mostra o rastreio de rota realizado do PC1 até o PC2, exibindo os três endereços IPv6 correspondentes aos saltos percorridos no caminho.

<div align="center"><figure>
    <img src="./0-aux/img01.png" alt="img01"><br>
    <figcaption>Imagem 01.</figcaption>
</figure></div><br>
# CCNA: ITN - Módulo 7 - Exam - Q30   <img src="./0-aux/logo_course.png" alt="pkt_108" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../pkt/">pkt</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">pkt_108 (CCNA: ITN - Módulo 7 - Exam - Q30)   <img src="./0-aux/logo_course.png" alt="pkt_108" width="auto" height="25"></a>

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
  - ping   <img src="" alt="iputils" width="auto" height="25">

---

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">CCNA: ITN - Módulo 7 - Exam - Q30</a><br>

---

### Objective:
O objetivo deste PTSA foi utilizar a tabela de endereços MAC do switch para identificar a porta física pela qual o quadro é encaminhado ao destino, bem como determinar o endereço MAC correspondente ao dispositivo de destino.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. CCNA: ITN - Módulo 7 - Exam - Q30</h4></a>[Back to summary](#item00)

- a. Abra a área de trabalho PC0. Use a Linha de Comando para determinar o endereço IPv4 e o endereço MAC do PC0. Na linha de comando PC0, execute ping no endereço IPv4 10.1.1.5. Use o aplicativo Terminal no PC0 para acessar o Switch0 e examinar a tabela de endereços MAC.
  - `ipconfig /all` -> `ping 10.1.1.5` -> `show mac-address-table`.
  - O endereço IPv4 do PC0 é 10.1.1.1 e seu endereço MAC é 0060.473E.9176.
- a. Qual porta o Switch0 usa para enviar quadros para o host com o endereço IPv4 10.1.1.5?
  - O Switch0 utiliza a interface Fa0/11 para encaminhar quadros destinados ao host com o endereço IPv4 10.1.1.5, conforme indicado na tabela de endereços MAC.

A imagem 01 apresenta a tabela de endereços MAC, contendo os registros correspondentes ao PC0 e ao host de destino.

<div align="center"><figure>
    <img src="./0-aux/img01.png" alt="img01"><br>
    <figcaption>Imagem 01.</figcaption>
</figure></div><br>
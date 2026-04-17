# Laboratório - Calcular sub-redes IPv4   <img src="./0-aux/logo_course.png" alt="lab_050" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../labs/">labs</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">lab_050 (Laboratório - Calcular sub-redes IPv4)   <img src="./0-aux/logo_course.png" alt="lab_050" width="auto" height="25"></a>

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

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">Parte 1: Determinar/Calcular a Divisão de Endereços IPv4 em Sub-Redes</a><br>
  1.1 <a href="#item01.01">Problema 1</a><br>
  1.2 <a href="#item01.02">Problema 2</a><br>
  1.3 <a href="#item01.03">Problema 3</a><br>
  1.4 <a href="#item01.04">Problema 4</a><br>
  1.5 <a href="#item01.05">Problema 5</a><br>
  1.6 <a href="#item01.06">Problema 6</a><br>
2. <a href="#item02">Perguntas para reflexão</a><br>

---

### Objective:
O objetivo deste laboratório foi calcular e determinar os endereços IPv4 das sub-redes geradas a partir da subdivisão de uma rede maior, aplicando diferentes máscaras de sub-rede e analisando os intervalos de endereços de rede, hosts e broadcast.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: Determinar/Calcular a Divisão de Endereços IPv4 em Sub-Redes</h4></a>[Back to summary](#item00)

<a name="item01.01"><h4>1.1 Problema 1</h4></a>[Back to summary](#item00)

Dados:
  - Endereço IP do Host: 192.168.200.139
  - Máscara de Sub-Rede Original: 255.255.255.0 -> /24
  - Nova Máscara de Sub-Rede: 255.255.255.224 -> 27
Descubra:
  - Número de Bits de Sub-Rede: 27 - 24 = 3
  - Número de Sub-Redes Criadas: 2^3 = 8
  - Número de Bits de Host por Sub-Rede: 32 - 27 = 5
  - Número de Hosts por Sub-Rede: 32 - 30 = 2
  - Endereço de Rede desta Sub-Rede: 192.168.200.128/27 (192.168.200.128-159)
  - Endereço IPv4 do Primeiro Host nesta Sub-Rede: 192.168.200.129
  - Endereço IPv4 do Último Host nesta Sub-Rede: 192.168.200.158
  - Endereço IPv4 de Broadcast nesta Sub-Rede: 192.168.200.159

<a name="item01.02"><h4>1.2 Problema 2</h4></a>[Back to summary](#item00)

Dados:
  - Endereço IP do Host: 10.101.99.228
  - Máscara de Sub-Rede Original: 255.0.0.0 -> /8
  - Nova Máscara de Sub-Rede: 255.255.128.0 -> /17
Descubra:
  - Número de Bits de Sub-Rede: 17 - 8 = 9
  - Número de Sub-Redes Criadas: 2^9 = 512
  - Número de Bits de Host por Sub-Rede: 32 - 17 = 15
  - Número de Hosts por Sub-Rede: 2^15 = 32.768 - 2 = 32.766
  - Endereço de Rede desta Sub-Rede: 10.101.0.0/17
  - Endereço IPv4 do Primeiro Host nesta Sub-Rede: 10.101.0.1
  - Endereço IPv4 do Último Host nesta Sub-Rede: 10.101.127.254
  - Endereço IPv4 de Broadcast nesta Sub-Rede: 10.101.127.255

<a name="item01.03"><h4>1.3 Problema 3</h4></a>[Back to summary](#item00)

Dados:
  - Endereço IP do Host: 172.22.32.12
  - Máscara de Sub-Rede Original: 255.255.0.0 -> /16
  - Nova Máscara de Sub-Rede: 255.255.224.0 -> /19
Descubra:
  - Número de Bits de Sub-Rede: 19 - 16 = 3
  - Número de Sub-Redes Criadas: 2^3 = 8
  - Número de Bits de Host por Sub-Rede: 32 - 19 = 13
  - Número de Hosts por Sub-Rede: 2^13 = 8.192 - 2 = 8.190
  - Endereço de Rede desta Sub-Rede: 172.22.32.0/19
  - Endereço IPv4 do Primeiro Host nesta Sub-Rede: 172.22.32.1
  - Endereço IPv4 do Último Host nesta Sub-Rede: 172.22.63.254
  - Endereço IPv4 de Broadcast nesta Sub-Rede: 172.22.63.255

<a name="item01.04"><h4>1.4 Problema 4</h4></a>[Back to summary](#item00)

Dados:
  - Endereço IP do Host: 192.168.1.245
  - Máscara de Sub-Rede Original: 255.255.255.0 -> 24
  - Nova Máscara de Sub-Rede: 255.255.255.252 -> 30
Descubra:
  - Número de Bits de Sub-Rede: 30 - 24 = 6
  - Número de Sub-Redes Criadas: 2^6 = 64
  - Número de Bits de Host por Sub-Rede: 32 - 30 = 2
  - Número de Hosts por Sub-Rede: 2^2 = 4 - 2 = 2
  - Endereço de Rede desta Sub-Rede: 192.168.1.244/30
  - Endereço IPv4 do Primeiro Host nesta Sub-Rede: 192.168.1.245
  - Endereço IPv4 do Último Host nesta Sub-Rede: 192.168.1.246
  - Endereço IPv4 de Broadcast nesta Sub-Rede: 192.168.1.247

<a name="item01.05"><h4>1.5 Problema 5</h4></a>[Back to summary](#item00)

Dados:
  - Endereço IP do Host: 128.107.0.55
  - Máscara de Sub-Rede Original: 255.255.0.0 -> 16
  - Nova Máscara de Sub-Rede: 255.255.255.0 -> 24
Descubra:
  - Número de Bits de Sub-Rede: 24 - 16 = 8
  - Número de Sub-Redes Criadas: 2^8 = 256
  - Número de Bits de Host por Sub-Rede: 32 - 24 = 8
  - Número de Hosts por Sub-Rede: 2^8 = 256 - 2 = 254
  - Endereço de Rede desta Sub-Rede: 128.107.0.0/24
  - Endereço IPv4 do Primeiro Host nesta Sub-Rede: 128.107.0.1
  - Endereço IPv4 do Último Host nesta Sub-Rede: 128.107.0.254
  - Endereço IPv4 de Broadcast nesta Sub-Rede: 128.107.0.255

<a name="item01.06"><h4>1.6 Problema 6</h4></a>[Back to summary](#item00)

Dados:
  - Endereço IP do Host: 192.135.250.180
  - Máscara de Sub-Rede Original: 255.255.255.0 -> 24
  - Nova Máscara de Sub-Rede: 255.255.255.248 -> 29
Descubra:
  - Número de Bits de Sub-Rede: 29 - 24 = 5
  - Número de Sub-Redes Criadas: 2^5 = 32
  - Número de Bits de Host por Sub-Rede: 32 - 29 = 3
  - Número de Hosts por Sub-Rede: 2^3 = 8 - 2 = 6
  - Endereço de Rede desta Sub-Rede: 192.135.250.176/29
  - Endereço IPv4 do Primeiro Host nesta Sub-Rede: 192.135.250.177
  - Endereço IPv4 do Último Host nesta Sub-Rede: 192.135.250.182
  - Endereço IPv4 de Broadcast nesta Sub-Rede: 192.135.250.183

<a name="item02"><h4>2. Perguntas para reflexão</h4></a>[Back to summary](#item00)

- a. Por que a máscara de sub-rede é tão importante na análise de um endereço IPv4?
  - A máscara de sub-rede é importante porque determina qual parte do endereço IPv4 identifica a rede e qual parte identifica o host dentro dessa rede. Com isso, é possível organizar os dispositivos em diferentes sub-redes, facilitar o roteamento de pacotes entre redes e melhorar o gerenciamento e a eficiência da comunicação na rede.
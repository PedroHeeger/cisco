# Packet Tracer - Configurando Segurança Básica em Redes sem Fios   <img src="./0-aux/logo_course.png" alt="pkt_077" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../pkt/">pkt</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">pkt_077 (Packet Tracer - Configurando Segurança Básica em Redes sem Fios)   <img src="./0-aux/logo_course.png" alt="pkt_077" width="auto" height="25"></a>

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

1. <a href="#item01">Parte 1: Verificar conectividade</a><br>
2. <a href="#item02">Parte 2: Configurar segurança básica sem fio.</a><br>
3. <a href="#item03">Parte 3: Atualizar as configurações sem fio no Laptop.</a><br>
4. <a href="#item04">Parte 4: Verificar conectividade.</a><br>

---

### Objective:
Esta atividade teve como objetivo realizar a configuração básica de autenticação da rede wireless de 2,4 GHz do roteador, utilizando o modo de segurança WPA2-Personal, indicado para redes domésticas, e a criptografia AES, além da definição de uma senha para autenticação dos dispositivos. Em seguida, foi estabelecida a conexão de um dispositivo à rede wireless por meio da senha configurada e realizado o acesso a um servidor web, a fim de comprovar a conectividade com a Internet.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: Verificar conectividade</h4></a>[Back to summary](#item00)

A imagem 01 mostra a topologia inicial.

<div align="center"><figure>
    <img src="./0-aux/img01.png" alt="img01"><br>
    <figcaption>Imagem 01.</figcaption>
</figure></div><br>

- a. Acesse Desktop > Web Browser no laptop.
- b. Digite "www.cisco.pka" na barra de endereço (URL). A página Web deve aparecer.
  - `www.cisco.pka`.

<a name="item02"><h4>2. Parte 2: Configurar segurança básica sem fio.</h4></a>[Back to summary](#item00)

- a. Digite "192.168.1.1" na barra de endereço do navegador para acessar o roteador sem fio. Insira admin como nome de usuário e senha.
  - `192.168.1.1` -> `admin` -> `admin`.
- b. Click no menu "Wireless". Selecione Segurança Wireless no menu.
- c. O modo de segurança está desativado no momento. Para rede de 2,4 GHz, altere o modo de segurança para WPA2 Pessoal. Para as redes de 5 GHz, você pode deixá-las como desativadas.
- d. no campo Passphrase, digite Network123.
  - `Network123`.
- e. Role para baixo até a parte inferior da página e clique em Salvar configurações. Feche o web browser.

<a name="item03"><h4>3. Parte 3: Atualizar as configurações sem fio no Laptop.</h4></a>[Back to summary](#item00)

- a. Clique em PC Wireless na guia Desktop.
- b. Clique na guia conectar. Selecione a Academia e clique em Conectar.
- c. Digite Network123 como a chave pré-compartilhada. Clique Conectar.
  - `Network123`.
- d. Feche a janela PC Wireless.

A imagem 02 exibe o laptop conectado à rede wireless de 2,4 GHz, após a autenticação realizada por meio da senha previamente configurada no roteador.

<div align="center"><figure>
    <img src="./0-aux/img02.png" alt="img02"><br>
    <figcaption>Imagem 02.</figcaption>
</figure></div><br>

<a name="item04"><h4>4. Parte 4: Observe o tráfego entre o cliente e o servidor Web.</h4></a>[Back to summary](#item00)

- a. Acesse o Web Browser.
- b. Digite "www.cisco.pka" na URL. A página Web deve aparecer assim que a configuração básica da rede sem fio for adicionada.
  - `www.cisco.pka`.
c. Se você não conseguir acessar a página da web, verifique as configurações sem fio no roteador sem fio e no laptop. Se não for possível acessar a página Web, verifique as configurações da rede sem fio no roteador sem fio e no laptop.

A imagem 03 demonstra que o acesso ao servidor web foi realizado com sucesso, comprovando que o laptop estava devidamente conectado à rede e possuía acesso à Internet.

<div align="center"><figure>
    <img src="./0-aux/img03.png" alt="img03"><br>
    <figcaption>Imagem 03.</figcaption>
</figure></div><br>
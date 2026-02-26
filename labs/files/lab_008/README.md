# Laboratório - Instalar o Wireshark   <img src="./0-aux/logo_course.png" alt="lab_008" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../labs/">labs</a>
### Software/Subject: wireshark   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/wireshark.png" alt="wireshark" width="auto" height="25"></a>
### Course: <a href="./">lab_008 (Laboratório - Instalar o Wireshark)   <img src="./0-aux/logo_course.png" alt="lab_008" width="auto" height="25"></a>

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
  - Wireshark   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/wireshark.png" alt="wireshark" width="auto" height="25">

---

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">Laboratório - Instalar o Wireshark</a><br>
  1.1 <a href="#item01.01">Etapa 1: Baixar o Wireshark.</a><br>
  1.2 <a href="#item01.02">Etapa 2: Instalar o Wireshark.</a><br>

---

### Objective:
O Wireshark é um software analisador de protocolo, ou aplicação "packet sniffer", usado para solução de problemas de rede, análise, desenvolvimento de software e protocolo, e educação. O objetivo deste laboratório foi baixá-lo e instalá-lo.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Laboratório - Instalar o Wireshark</h4></a>[Back to summary](#item00)

<a name="item01.01"><h4>1.1 Etapa 1: Baixar o Wireshark.</h4></a>[Back to summary](#item00)

- a. O Wireshark pode ser baixado em [www.wireshark.org](www.wireshark.org). 
- b. Escolha a versão do software necessária com base na arquitetura e no sistema operacional do PC. Por exemplo, se você tiver um PC de 64 bits executando o Windows, selecione Windows Installer (64-bit) (Instalador do Windows (64 bits)). Depois de fazer uma seleção, o download será iniciado. O destino do download do arquivo depende do navegador e do sistema operacional usados. Para usuários do Windows, o local padrão é a pasta Downloads. 

<a name="item01.02"><h4>1.2 Parte 2: Rastrear uma rota para um servidor remoto usando o Tracert</h4></a>[Back to summary](#item00)

- a. O arquivo baixado é denominado Wireshark-win64-x.x.x.exe, em que x representa o número da versão se você baixou a versão de 64 bits. Clique duas vezes no arquivo para iniciar o processo de instalação. Responda a todas as mensagens de segurança que aparecerem na tela. Se já tiver uma cópia do Wireshark em seu PC, você deverá desinstalar a versão anterior antes de instalar a nova. Recomenda se que você remova a versão antiga do Wireshark antes de instalar outra versão. Clique em Sim para desinstalar a versão anterior do Wireshark. 
- b. Se esta for a primeira instalação do Wireshark, ou após concluir o processo de desinstalação, você navegará para o assistente de configuração do Wireshark. Clique em Avançar. 
- c. Continue avançando no processo de instalação. Clique em I agree (Eu concordo) quando a janela do contrato de licença for exibida. 
- d. Mantenha as configurações padrão na janela Escolher componentes e clique em Avançar. 
- e. Escolha suas opções de atalho desejadas e clique em Next (Próximo). 
- f. Você pode alterar o local de instalação do Wireshark, porém, a menos que você tenha espaço em disco limitado, recomenda-se manter o local padrão. Clique em Avançar para continuar. 
- g. Para capturar dados de rede ao vivo, o Npcap deve estar instalado no seu PC. Se o Npcap já estiver instalado no seu PC, a caixa de seleção Instalar estará desmarcada. Se a versão instalada do Npcap for anterior à versão que acompanha o Wireshark, é recomendável permitir a instalação da versão mais recente clicando na caixa de seleção Instalar Npcap x.x.x (número da versão). Clique em Avançar para continuar. 
- h. NÃO instale o USBPcap para captura de tráfego normal. NÃO marque a caixa de seleção para instalar o USBPcap. O USBPcap é experimental e pode causar problemas USB no seu PC. Clique em Instalar agora para continuar.
- i. O Wireshark começa a instalar seus arquivos e exibe uma janela separada com o status da instalação.
- j. Em uma janela separada, aceite o contrato de licença no Assistente de configuração Npcap se estiver instalando o Npcap. Clique em Concordo para continuar. Clique em Instalar para instalar o Npcap. Clique em Avançar para concluir a instalação do Npcap e clique em Concluir para sair da instalação do Npcap. 
- k. Clique em Next (Avançar) quando a instalação for concluída.
- l. Clique em Finish (Concluir) para encerrar o processo de instalação do Wireshark. Reinicie o computador, se necessário.
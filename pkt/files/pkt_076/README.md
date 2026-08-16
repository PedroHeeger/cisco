# Packet Tracer - Configure o Controle de Acesso   <img src="./0-aux/logo_course.png" alt="pkt_076" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../pkt/">pkt</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">pkt_076 (Packet Tracer - Configure o Controle de Acesso)   <img src="./0-aux/logo_course.png" alt="pkt_076" width="auto" height="25"></a>

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
  - ping   <img src="" alt="iputils" width="auto" height="25">

---

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">Parte 1: Configurar e usar credenciais de autenticação AAA</a><br>
  1.1 <a href="#item01.01">Etapa 1: Configurar contas de usuário no servidor AAA.</a><br>
  1.2 <a href="#item01.02">Etapa 2: Configure a autenticação wireless no HQ-Laptop-1.</a><br>
  1.3 <a href="#item01.03">Etapa 3: Configure a autenticação wireless no HQ-Laptop-2.</a><br>
2. <a href="#item02">Parte 2: Configurar e Verificar Serviços de E-mail</a><br>
  2.1 <a href="#item02.01">Etapa 1: Ativar os serviços de e-mail e configurar contas de usuário de e-mail.</a><br>
  2.2 <a href="#item02.02">Etapa 2: Configure os clientes de e-mail</a><br>
  2.3 <a href="#item02.03">Etapa 3: Enviar um e-mail como Suk-Yi.</a><br>
3. <a href="#item03">Parte 3: Configurar e usar serviços de FTP</a><br>
  3.1 <a href="#item03.01">Etapa 1: Ative o serviço FTP.</a><br>
  3.2 <a href="#item03.02">Etapa 2: Criar as contas de usuário de FTP.</a><br>
  3.3 <a href="#item03.03">Etapa 3: Transferir arquivos entre o Net-Admin e o servidor FTP.</a><br>
  3.4 <a href="#item03.04">Etapa 4: Verificar se os privilégios de usuário do FTP estão funcionando conforme configurado.</a><br>

---

### Objective:
O objetivo desta atividade foi analisar o funcionamento das transmissões em broadcast em uma rede local e demonstrar como a segmentação da rede em sub-redes melhora sua eficiência, dividindo um único domínio de broadcast em três domínios menores.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: Configurar e usar credenciais de autenticação AAA</h4></a>[Back to summary](#item00)

A imagem 01 mostra a topologia inicial.

<div align="center"><figure>
    <img src="./0-aux/img01.png" alt="img01"><br>
    <figcaption>Imagem 01.</figcaption>
</figure></div><br>



<a name="item01.01"><h4>1.1 Etapa 1: Configurar contas de usuário no servidor AAA.</h4></a>[Back to summary](#item00)

- a. Navegue até a sede e clique no Wiring Closet, que é o gabinete do servidor alto e preto no canto inferior esquerdo.
- b. No lado direito do Rack, clique em AAA-RADIUS server > guia Services e, em seguida, em AAA sob SERVICES.
- c. Ative o serviço AAA.
- d. Em Configuração de Usuário, adicione os seguintes nomes de usuário / senhas.
  - user1 / PASSuser1!
  - user2 / PASSuser2!

<a name="item01.02"><h4>1.2 Etapa 2: Configure a autenticação wireless no HQ-Laptop-1.</h4></a>[Back to summary](#item00)

- a. Navegue de volta para HQ e clique em HQ-Laptop-1. Está localizado a duas salas à direita do Wiring Closet.
- b. Clique na guia Config e, em seguida, em INTERFACE, clique em Wireless0.
- c. Na caixa SSID, digite HQ-INT.
- d. Na área de "Autenticação", clique em WPA2.
- e. Na caixa User ID, digite "user1" e na caixa "Password", digite PASSuser1!.
- f. No espaço "IP Configuration", clique em "DHCP". Aguarde alguns momentos para a oferta do DHCP ser aceita, Verifique se o HQ-Laptop-1 recebeu a configuração de endereço IP e se foi atribuído um endereço na rede 192.168.50.0/24.
- f. Observação: Pode ser necessário alternar entre as opções Static (estático) e "DHCP" para forçar o Packet Tracer a convergir nas suas configurações. Além disso, clique em Check Results para garantir que você configurou corretamente o servidor AAA e as configurações sem fio no laptop. Clicar em "Check Results" também pode forçar o Packet Tracer a convergir. Se tudo estiver configurado corretamente, prossiga para a configuração do "HQ-Laptop-2" e, em seguida, retorne ao "HQ-Laptop-1" para verificar sua configuração de IP. Esse problema normalmente é resolvido.

A imagem 02 exibe a criação da PDU ICMP, bem como, o processo ARP realizado.

<div align="center"><figure>
    <img src="./0-aux/img02.png" alt="img02"><br>
    <figcaption>Imagem 02.</figcaption>
</figure></div><br>

<a name="item01.03"><h4>1.3 Etapa 3: Configure a autenticação wireless no HQ-Laptop-2.</h4></a>[Back to summary](#item00)

- a. Clique em "HQ-Laptop-2", que está localizado no canto superior direito do "HQ".
- b. Repita os passos anteriores para configurar as configurações sem fio para "HQ-Laptop-2", usando as credenciais do "user2".
- c. Verifique se o "HQ-Laptop-2" recebeu uma configuração de endereço IP e foi atribuído um endereço na rede 192.168.50.0/24.

<a name="item02"><h4>2. Parte 2: Configurar e Verificar Serviços de E-mail</h4></a>[Back to summary](#item00)

<a name="item02.01"><h4>2.1 Etapa 1: Ativar os serviços de e-mail e configurar contas de usuário de e-mail.</h4></a>[Back to summary](#item00)

- a. Navegue até o Armário de Cabeamento.
- b. No lado direito do Rack, clique em Mail server > guia Services e depois em EMAIL sob SERVICES.
- c. Ative tanto o serviço SMTP quanto o serviço POP3.
- d. Configure o domínio para mail.cyberhq.com.
- e. Na seção "Configuração de Usuários", digite os seguintes nomes de usuário / senhas. Clique no sinal de adição (+) para adicionar cada par.
  - HQuser1 / Cisco123!
  - HQuser2 / Cisco123~
  - BRuser1 / Cisco123-
  - BRuser2 / Cisco123+

<a name="item02.02"><h4>2.2 Etapa 2: Configure os clientes de e-mail</h4></a>[Back to summary](#item00)

- a. Navegue de volta para "HQ" e clique em "PC 1-1", que está no canto inferior.
- b. Clique na guia Desktop > Email. As configurações de e-mail estão abertas.
- c. Insira as informações a seguir:
  - Seu Nome: Suk-Yi
  - Endereço de e-mail: HQuser1@mail.cyberhq.com
  - Servidor(es) de E-mail de Entrada e Saída: mail.cyberhq.com
  - Nome de Usuário: HQuser1
  - Senha: Cisco123!
- d. Click em Salvar.

A imagem 03 mostra que os dois hosts das novas redes obtiveram seus respectivos endereços IP. A renovação do endereçamento foi realizada de três formas distintas: pela interface de linha de comando (CLI), utilizando o comando `ipconfig /renew`; pela aba IP Configuration; e pela aba Config, alternando a configuração de endereçamento de estático para automático (DHCP).

<div align="center"><figure>
    <img src="./0-aux/img03.png" alt="img03"><br>
    <figcaption>Imagem 03.</figcaption>
</figure></div><br>

<a name="item02.03"><h4>2.3 Etapa 3: Enviar um e-mail como Suk-Yi.</h4></a>[Back to summary](#item00)

- a. No PC 1-1, clique em Compor.
- b. Componha um email para Ajulo em BRuser1@mail.cyberhq.com. Insira um assunto e uma mensagem de e-mail de sua escolha. Clique em Enviar quando terminar.
- b. Observação: O Packet Tracer pode levar alguns segundos para convergir antes de você ver uma mensagem "Envio bem-sucedido" na parte inferior da janela.
- b. Observção: O Packet Tracer não classifica esta etapa. Verifique se você completou corretamente esta etapa recebendo o e-mail enviado por Suk-Yi no PC de Ajulo (PC2-3).
- c. Navegue até o PC2-3 de Ajulo. Se necessário, clique na guia "Desktop" e depois em "Email".
- d. Clique em "Receber" e leia o e-mail de Suk-Yi.

<a name="item03"><h4>3. Parte 3: Configurar e usar serviços de FTP</h4></a>[Back to summary](#item00)

<a name="item03.01"><h4>3.1 Etapa 1: Ative o serviço FTP.</h4></a>[Back to summary](#item00)

- a. Navegue até o Armário de Cabeamento.
- b. No lado direito, clique em "FTP server", em seguida, na guia "Services" e, por fim, em "FTP" na seção "SERVICES".
- c. Ative o serviço de FTP.

<a name="item03.02"><h4>3.2 Etapa 2: Criar as contas de usuário de FTP.</h4></a>[Back to summary](#item00)

- a. Em "Configuração de Usuário", por favor, insira os seguintes nomes de usuário, senhas e privilégios: Clique em Add para adicionar cada usuário. Observação: certifique-se de que o nome de usuário malia não inclua a opção Delete como um dos privilégios de usuário.
- b. Verifique se cada usuário foi criado corretamente e feche o servidor.

<a name="item03.03"><h4>3.3 Etapa 3: Transferir arquivos entre o Net-Admin e o servidor FTP.</h4></a>[Back to summary](#item00)

- a. Clique em Net-Admin PC e então clique em Desktop > Command Prompt.
- b. Digite o comando "ftp 192.168.75.2" para fazer login no servidor FTP e, em seguida, autentique com o nome de usuário "sukyi" e a senha "cisco123".
- c. Insira o comando dir para listar os arquivos no servidor FTP.
- d. Utilize o comando "get" para baixar o arquivo "aMessage.txt".
- e. Saia da sessão de FTP.
- f. Feche o prompt de comando, clique em Text Editor e em File > Open. Abra o arquivo baixado aMessage.txt.
- f. Qual é a mensagem no arquivo?
  - 
- g. Clique File > New. Digite uma mensagem de texto de sua escolha.
- h. Clique em File > Save e salve o novo arquivo como aMessage_new.txt. Feche o Editor de Text.
- i. Clique em Prompt de comando e faça login novamente no servidor FTP como usuário sukyi.
- j. Use o comando put para fazer upload do arquivo aMessage_new.txt.
- k. Saia da sessão de FTP.

<a name="item03.04"><h4>3.4 Etapa 4: Verificar se os privilégios de usuário do FTP estão funcionando conforme configurado.</h4></a>[Back to summary](#item00)

- a. Para retornar ao HQ e clicar em HQ-Laptop-1, vá até a guia "Desktop" e clique em "Command Prompt".
- b. Faça login no servidor FTP em 192.168.75.2 com o nome de usuário malia e a senha cisco123.
- c. Use o comando delete para tentar remover o arquivo recém-carregado aMessage_new.txt.
- c. Você conseguiu excluir o arquivo do servidor FTP? Explique.
  - 
- d. Use o comando rename para tentar alterar o nome do arquivo "aMessage_new.txt para aMessage_rename.txt.
  - ftp> rename aMessage_new.txt aMessage_rename.txt
- d. Você conseguiu renomear o arquivo do servidor FTP?
  - 
- e. Encerre a sessão FTP e feche a janela do HQ-Laptop-1.

A imagem 04 ilustra a solicitação ARP sendo propagada apenas dentro de um domínio de broadcast menor, resultado da segmentação da rede em sub-redes.

<div align="center"><figure>
    <img src="./0-aux/img04.png" alt="img04"><br>
    <figcaption>Imagem 04.</figcaption>
</figure></div><br>
# Laboratório - Exibir informações de NIC com e sem fio   <img src="./0-aux/logo_course.png" alt="lab_013" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../labs/">labs</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">lab_013 (Laboratório - Exibir informações de NIC com e sem fio)   <img src="./0-aux/logo_course.png" alt="lab_013" width="auto" height="25"></a>

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

1. <a href="#item01">Parte 1: Identifique e trabalhe com as placas de rede do PC.</a><br>
  1.1 <a href="#item01.01">Etapa 1: Use a Central de Rede e Compartilhamento.</a><br>
  1.2 <a href="#item01.02">Etapa 2: Trabalhar com placas de rede sem fio.</a><br>
  1.3 <a href="#item01.03">Etapa 3: Trabalhar com placas de rede cabeada.</a><br>
2. <a href="#item02">Parte 2: Identificar e usar os ícones rede da notificação do sistema</a><br>
  2.1 <a href="#item02.01">Etapa 1: Use o ícone de rede.</a><br>
  2.2 <a href="#item02.02">Etapa 2: Identifique o ícone de problemas da rede.</a><br>
3. <a href="#item03">Perguntas para reflexão</a><br>

---

### Objective:
O objetivo deste laboratório foi realizar a inspeção técnica de interfaces de rede (NICs) em um computador, compreendendo como extrair parâmetros de configuração e como gerenciar o estado operacional das placas através de comandos de ativação e desativação.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: Identifique e trabalhe com as placas de rede do PC.</h4></a>[Back to summary](#item00)

Na parte 1, você identificará os tipos de placa de rede no PC que você está utilizando. Você irá explorar formas diferentes de extrair informações sobre essas placas de rede e como ativá-las e desativá-las. Nota: Este laboratório foi realizado usando um PC em execução no sistema operacional Windows 10. Você deve ser capaz de realizar o laboratório com um dos outros sistemas operacionais Windows listados; no entanto, as seleções de menu e as telas podem variar. 

<a name="item01.01"><h4>1.1 Etapa 1: Use a Central de Rede e Compartilhamento.</h4></a>[Back to summary](#item00)

- a. Navegue até o painel de controle. Clique em Exibir status e tarefas da rede em Rede e Internet cabeçalho na Exibição de Categoria. 
- b. No painel esquerdo, clique no link Alterar configurações do adaptador. 
- c. Na janela Conexões de Rede, os resultados fornecem uma lista de NICs disponíveis neste PC. Procure seus adaptadores Wi-Fi. Nota: Os adaptadores de rede virtual privada (VPN) e outros tipos de conexões de rede também podem ser exibidos nesta janela. 

<a name="item01.02"><h4>1.2 Etapa 2: Trabalhar com placas de rede sem fio.</h4></a>[Back to summary](#item00)

- a. Localize a conexão de rede sem fio. Se estiver desativado, clique com o botão direito do mouse e selecione Ativar para ativar a NIC sem fio. 
- b. Se a conexão de rede sem fio não estiver conectada no momento, clique com o botão direito do mouse e selecione Conectar/Desconectar para se conectar a um SSID ao qual você está autorizado a se conectar. 
- c. Clique com o botão direito do mouse em uma conexão de rede sem fio e, em seguida, clique em Status. 
- d. A janela Status da conexão de rede sem fio é exibida onde você pode visualizar informações sobre sua conexão sem fio. O que é o Identificador do Conjunto de Serviços (SSID - Service Set Identifier) para o roteador sem fio de sua conexão? 
  - John_Doe_Wifi
- d. Qual é a velocidade de sua conexão sem fio? 
  - 866,7 Mbps.
- e. Clique em Detalhes para exibir a janela Detalhes da Conexão de Rede. Qual é o endereço MAC de sua placa de rede sem fio? 
  - Oculto.
- e. Você tem vários servidores DNS IPv4 listados? Se sim, por que vários servidores DNS seriam listados? 
  - Sim, vários servidores DNS IPv4 podem estar listados. Isso ocorre para fornecer redundância e alta disponibilidade no processo de resolução de nomes. Caso um servidor DNS não responda, o dispositivo pode consultar outro, garantindo maior confiabilidade e continuidade do acesso à rede. Além disso, múltiplos servidores DNS podem melhorar o desempenho, permitindo que o cliente utilize o servidor mais próximo ou com menor latência.
- f. Abra um prompt de comando do Windows e digite ipconfig /all. Observe que as informações exibidas aqui são as mesmas que foram exibidas na janela Detalhes da conexão de rede na Etapa e. 
- g. Feche a janela de comando e a janela Detalhes da conexão de rede. Isso deve retornar à janela Status do Wi-Fi. Clique em Propriedades sem fio.
- h. Na janela Propriedades da rede sem fio, clique na guia Segurança.
- i. O tipo de segurança implementada pelo roteador sem fio conectado será exibido. Clique na caixa de seleção Mostrar Caracteres para exibir a chave de segurança de rede real, em vez dos caracteres ocultos e, em seguida, clique em OK.
- j. Feche as propriedades de rede sem fio e as janelas de status de Wi-Fi. Selecione e clique com o botão direito do mouse na opção Wi-Fi> Conectar/Desconectar. Uma janela pop-up deve aparecer no canto inferior direito da área de trabalho que exibe sua conexão atual, juntamente com uma lista de SSIDs que estão dentro do alcance da NIC sem fio do seu PC. Se uma barra de rolagem aparecer no lado direito dessa janela, você poderá usá-la para exibir outros SSIDs. 
- k. Para ingressar em um dos outros SSIDs da rede sem fio listados, clique no SSID ao qual deseja ingressar e clique em Conectar. 
- l. Se você selecionou um SSID seguro, você será solicitado a inserir a chave de segurança do SSID. Digite a chave de segurança para esse SSID e clique em OK. Você pode clicar na caixa de seleção Ocultar Caracteres para impedir que as pessoas vejam o que você digita no campo Chave de Segurança. 

<a name="item01.03"><h4>1.3 Etapa 3: Trabalhar com placas de rede cabeada.</h4></a>[Back to summary](#item00)

- a. Na janela Conexões de Rede, selecione e clique com o botão direito do mouse na opção Ethernet para exibir a lista suspensa. Se a NIC estiver desativada, ative-a e clique na opção Status. Nota: Você deve ter um cabo Ethernet conectando a NIC do PC a um comutador ou dispositivo semelhante para ver o status. Muitos roteadores sem fio têm um pequeno switch Ethernet de 4 portas integrado. Você pode se conectar a uma das portas usando um cabo Ethernet reto. 
- b. Na janela Status, os resultados exibem informações sobre sua conexão com fio à LAN.
- c. Clique em Detalhes... para visualizar as informações de endereço da sua conexão LAN.
- d. Abra um prompt da janela de comando e digite ipconfig /all. Encontre as informações do seu adaptador Ethernet e compare-as com as informações exibidas na janela Detalhes da conexão de rede.
- e. Feche todas as janelas no desktop.

<a name="item02"><h4>2. Parte 2: Identificar e usar os ícones rede da notificação do sistema</h4></a>[Back to summary](#item00)

Na parte 2, você usará os ícones de rede na notificação do sistema para determinar e controlar as placas de rede no PC. 

<a name="item02.01"><h4>2.1 Etapa 1: Use o ícone de rede.</h4></a>[Back to summary](#item00)

- a. Clique na bandeja do sistema. Clique no ícone de rede para visualizar a janela pop-up que exibe os SSIDs que estão dentro do alcance da sua NIC sem fio. 
- b. Clique em Rede e Internet.
- c. Nas janelas Configurações, clique em Alterar opções do adaptador no cabeçalho Alterar as configurações de rede. 
- d. Na janela Conexões de rede, clique com o botão direito do mouse em Wi-Fi e selecione Desativar.
- e. Examine a notificação do sistema. Clique no ícone Rede novamente. Com o Wi-Fi desativado, as redes sem fio não estão mais ao alcance e não estão disponíveis para conexões sem fio. 
- f. Você também pode desativar a rede Ethernet desativando os adaptadores Ethernet.

<a name="item02.02"><h4>2.2 Etapa 2: Identifique o ícone de problemas da rede.</h4></a>[Back to summary](#item00)

- a. Na janela Conexões de rede, desative todos os adaptadores Wi-Fi e Ethernet.
- b. A bandeja do sistema agora exibe o ícone Rede Desativada, que indica que a conectividade da rede foi desativada. 
- c. Você pode clicar neste ícone para retornar às configurações de Rede e Internet.
- d. Na janela Configurações de rede e Internet, você pode clicar em Solução de problemas para usar o PC para resolver o problema de rede para você. 
- e. Se a solução de problemas não tiver ativado uma de suas placas de rede, você deverá fazer isso manualmente para restaurar a conectividade de rede do PC. Note: Se um adaptador de rede estiver ativado e a NIC não conseguir estabelecer conectividade de rede, então o ícone Problema de rede aparece na bandeja do sistema. Se este ícone aparecer, você poderá solucionar esse problema como fez na etapa 2c. 

<a name="item03"><h4>3. Perguntas para reflexão</h4></a>[Back to summary](#item00)

- a. Por que você ativaria mais de uma placa de rede em um PC? 
  - Ativar mais de uma placa de rede em um PC permite conectar o dispositivo a diferentes redes simultaneamente ou fornecer redundância de conectividade. Isso pode ser útil para separar tráfego (por exemplo, rede interna e externa), aumentar a disponibilidade em caso de falha de uma interface ou atender a diferentes tipos de conexão, como rede cabeada e sem fio.
# Packet Tracer - Configuração Básica do Switch - Modo Físico   <img src="./0-aux/logo_course.png" alt="pkt_087" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../pkt/">pkt</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">pkt_087 (Packet Tracer - Configuração Básica do Switch - Modo Físico)   <img src="./0-aux/logo_course.png" alt="pkt_087" width="auto" height="25"></a>

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

1. <a href="#item01">Parte 1: Cabear a rede e verificar a configuração padrão do switch</a><br>
  1.1 <a href="#item01.01">Etapa 1: Cabeie a rede conforme mostrado na topologia.</a><br>
  1.2 <a href="#item01.02">Etapa 2: Verifique a configuração de switch padrão.</a><br>
2. <a href="#item02">Parte 2: Definir configurações básicas do dispositivo de rede</a><br>
  2.1 <a href="#item02.01">Etapa 1: Definir as configurações básicas do switch.</a><br>
  2.2 <a href="#item02.02">Etapa 2: Configurar um endereço IP no PC-A.</a><br>
3. <a href="#item03">Parte 3: Verificar e Testar a Conectividade da Rede</a><br>
  3.1 <a href="#item03.01">Etapa 1: Exiba a configuração do switch.</a><br>
  3.2 <a href="#item03.02">Etapa 2: Teste a conectividade de ponta a ponta com ping.</a><br>
  3.3 <a href="#item03.03">Etapa 3: Teste e verifique o gerenciamento remoto de S1.</a><br>
  3.4 <a href="#item03.04">Etapa 4: Implante o switch S1 na rede de produção.</a><br>
4. <a href="#item04">Perguntas para reflexão</a><br>
5. <a href="#item03">Parte 4: Gerenciar a tabela de endereços MAC</a><br>
  5.1 <a href="#item05.01">Etapa 1: Registre o endereço MAC do host.</a><br>
  5.2 <a href="#item05.02">Etapa 2: Determine os endereços MAC que o switch aprendeu.</a><br>
  5.3 <a href="#item05.03">Etapa 3: Liste as opções do show mac address-table.</a><br>
  5.4 <a href="#item05.04">Etapa 4: Configure um endereço MAC estático.</a><br>

---

### Objective:
O objetivo desta atividade foi verificar as configurações padrão do switch, realizar configurações básicas e habilitar uma interface virtual de gerenciamento (SVI) com um endereço IP, permitindo o acesso remoto ao switch via Telnet a partir do PC. Além disso, a atividade permitiu compreender a diferença entre os endereços MAC aprendidos dinamicamente e aqueles configurados estaticamente na tabela de endereços MAC do switch.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: Cabear a rede e verificar a configuração padrão do switch</h4></a>[Back to summary](#item00)

A imagem 01 mostra a topologia inicial.

<div align="center"><figure>
    <img src="./0-aux/img01.png" alt="img01"><br>
    <figcaption>Imagem 01.</figcaption>
</figure></div><br>

Na Parte 1, você configurará a topologia de rede e verificará as configurações padrão do switch.

<a name="item01.01"><h4>1.1 Etapa 1: Cabeie a rede conforme mostrado na topologia.</h4></a>[Back to summary](#item00)

- a. Da prateleira, clique e arraste o interruptor S1 e coloque-o no lado esquerdo da mesa. 
- b. Da prateleira, clique e arraste o dispositivo PC-A e coloque-o no lado direito da mesa. Ligue o PC-A. 
- c. Conecte um cabo de console do dispositivo PC-A para o switch S1, segundo as indicações da topologia. Não conecte ainda o cabo Ethernet do PC-A. 
- d. Na guia Desktop do PC-A, use o Terminal para conectar ao interruptor. Por que você deve usar uma conexão de console para configurar inicialmente o switch? 
  - Porque, por padrão, o switch ainda não possui uma configuração de gerenciamento que permita o acesso remoto. A SVI não possui um endereço IP configurado e pode estar inativa, além de o switch poder não ter um gateway padrão configurado nem as linhas VTY configuradas para permitir acesso por Telnet ou SSH. Por isso, é necessário utilizar uma conexão de console para realizar a configuração inicial do switch.
- Por que não é possível conectar-se ao switch via Telnet ou SSH? 
  - Porque o switch ainda não possui as configurações necessárias para o acesso remoto. A interface SVI não possui um endereço IP configurado, e o acesso Telnet ou SSH também pode não estar configurado nas linhas VTY. Dessa forma, não há uma forma de estabelecer inicialmente uma conexão remota com o switch.

<a name="item01.02"><h4>1.2 Etapa 2: Verifique a configuração de switch padrão.</h4></a>[Back to summary](#item00)

Nesta Etapa, você examinará as configurações de switch padrão, como a configuração em execução no switch, as informações do IOS, as propriedades de interface, as informações de VLAN e a memória flash. 

Você pode acessar todos os comandos IOS do switch no modo EXEC privilegiado. O acesso ao modo EXEC privilegiado deve ser restrito por proteção de senha a fim de evitar a utilização não autorizada, já que fornece acesso direto ao modo de configuração global e aos comandos usados para configurar os parâmetros operacionais. Você definirá senhas posteriormente nesta atividade. 

O conjunto de comandos do modo EXEC privilegiado inclui os comandos contidos no modo EXEC do usuário, assim como o comando configure por meio do qual se obtém acesso aos modos de comando restantes. Use o comando enable para entrar no modo EXEC privilegiado.

- a. Considerando que o switch não tinha um arquivo de configuração armazenado em uma memória de acesso aleatório não volátil (NVRAM), uma conexão de console utilizando o Tera Term ou outro programa emulador de terminal direciona você para o prompt do modo EXEC do usuário no switch com um prompt do Switch>. Use o comando enable para entrar no modo EXEC privilegiado. Observe que o prompt mudou na configuração para refletir o modo EXEC privilegiado.
  - `enable`.
- b. Verifique se há um arquivo de configuração padrão vazio no switch ao emitir o comando show running-config do modo EXEC privilegiado. Se um arquivo de configuração tiver sido salvo anteriormente, ele deverá ser removido. Dependendo do modelo do switch e da versão do IOS, sua configuração pode ser um pouco diferente. No entanto, não deve haver senhas ou endereços IP configurados. Se seu switch não tem uma configuração padrão, apague e recarregue o switch.
  - `show running-config`.
- b. Examine o arquivo de configuração atual em execução. Quantas interfaces GigabitEthernet o switch tem?
  - O switch possui 28 interfaces GigabitEthernet.
- b. Quantas interfaces FastEthernet um switch 2960 tem?
  - O switch não possui interfaces FastEthernet.
- b. Qual é a faixa de valores mostrados nas linhas VTY?
  - A faixa de valor é de 0 a 4, totalizando 5 linhas VTY.
- c. Examine o arquivo de configuração de inicialização na NVRAM. 
  - `show startup-config`.
- c. Por que aparece essa mensagem?
  - Porque não existe um arquivo de configuração de inicialização armazenado no switch.
- d. Examine as características do SVI para a VLAN 1.
  - `show interface vlan1`.
- d. Existe algum endereço IP atribuído à VLAN 1?
  - Não, nenhum endereço IP está atribuído à VLAN 1.
- d. Qual é o endereço MAC do SVI? As respostas variam.
  - O endereço MAC da SVI do switch é 0060.2fde.172d, sendo o BIA (Burned-In Address) também 0060.2fde.172d.
- d. Essa interface está ativa?
  - Não. A interface está administrativamente down na camada física e down na camada de enlace de dados.
- e. Examine as propriedades IP do SVI VLAN 1.
  - `show ip interface vlan1`.
- e. Qual saída você vê?
  - A VLAN 1 está administrativamente desativada (administratively down), o protocolo de linha também está inativo (line protocol is down) e o processamento do protocolo IP está desabilitado (Internet protocol processing disabled).
- f. Conecte um cabo Ethernet do PC-A à GigabitEthernet1/0/6 no switch. Espere até que o switch e o PC negociem os parâmetros duplex e de velocidade. Examine as propriedades IP do SVI VLAN 1. Qual saída você vê?
  - A interface GigabitEthernet1/0/6 passa para o estado up e o protocolo de linha também passa para up, indicando que o switch estabeleceu conexão com o PC-A.
- g. Digite configuração global e habilite a interface SVI VLAN 1. 
  - `configure terminal` -> `interface vlan 1` -> `no shutdown` -> `end`.
- h. Examine as propriedades IP do SVI VLAN 1. Qual saída você vê?
  - Antes, apenas com a conexão na GigabitEthernet1/0/6, a VLAN 1 permanecia no estado administratively down / down. Após ativá-la, a VLAN 1 passou para up / up, enquanto o processamento do protocolo IP continuou desabilitado.
- i. Examine as informações da versão do Cisco IOS do switch. 
  - `show version`.
- i. Qual é a versão do IOS Cisco que o switch está executando?
  - A versão do Cisco IOS em execução no switch é 16.3.2.
- i. Qual é o nome do arquivo de imagem do sistema?
  - O arquivo de imagem do sistema é CAT3K_CAA-UNIVERSALK9.
- i. Qual é o endereço MAC base desse switch?
  - O endereço MAC base do switch é 00:60:2F:DE:17:2D.
- j. Examine as propriedades padrão da interface GigabitEthernet1/0/6 usada pelo PC-A.
  - `show interface gig1/0/6`.
- j. A interface está ativa ou inativa?
  - A interface está ativa (up).
- j. Que evento faria uma interface cair?
  - A desconexão ou falha no cabo, ou a desativação manual da interface (shutdown) em uma das extremidades.
- j. Qual é o endereço MAC da interface?
  - O endereço MAC da interface é 000c.8589.1806, sendo o BIA (Burned-In Address) também 000c.8589.1806.
- j. Qual é a configuração de velocidade e de duplex da interface?
  - A interface está configurada com velocidade de 100 Mb/s e duplex full.
- k. Examine as configurações de VLAN padrão do switch.
  - `show vlan`.
- k. Qual é o nome padrão da VLAN 1?
  - O nome padrão da VLAN 1 é default.
- k. Quais portas estão na VLAN 1?
  - Todas as 28 portas GigabitEthernet estão atribuídas à VLAN 1.
- k. A VLAN 1 está ativa?
  - Sim, a VLAN 1 está ativa.
- k. Qual é o tipo da VLAN default?
  - O tipo da VLAN 1 é enet, que significa Ethernet.
- l. Examine a memória flash. Emita um dos seguintes comandos para examinar o conteúdo do diretório da memória flash.
  - `show flash:` -> `dir flash:`.
- l. Os arquivos têm uma extensão de arquivo, como .bin, no final do nome de arquivo. Os diretórios não têm uma extensão de arquivo. Qual é o nome do arquivo da imagem do IOS Cisco?
  - O nome do arquivo de imagem do Cisco IOS é c2960-lanbase-mz.122-25.FX.bin.

A imagem 02 apresenta os dois dispositivos conectados sobre a mesa, bem como os dois últimos comandos executados no terminal durante essa etapa de verificações.

<div align="center"><figure>
    <img src="./0-aux/img02.png" alt="img02"><br>
    <figcaption>Imagem 02.</figcaption>
</figure></div><br>

<a name="item02"><h4>2. Parte 2: Definir configurações básicas do dispositivo de rede</h4></a>[Back to summary](#item00)

Na Parte 2, você define as configurações básicas para o switch e o computador.

<a name="item02.01"><h4>2.1 Etapa 1: Definir as configurações básicas do switch.</h4></a>[Back to summary](#item00)

- a. Copie a seguinte configuração básica e cole-a no S1 no modo de configuração global.
  - `configure terminal`.
  - `no ip domain-lookup` -> `hostname S1` -> `service password-encryption` -> `enable secret class`.
  - `banner motd #Unauthorized access is strictly prohibited.#`.
- b. Defina o endereço IP SVI do switch. Isso permite o gerenciamento remoto do switch. Antes que você possa gerenciar remotamente o S1 do PC-A, você deve atribuir um endereço IP ao switch. A configuração padrão em um switch tem o gerenciamento do switch controlado por meio da 
VLAN 1. No entanto, uma prática recomendada para a configuração básica do switch consiste em alterar a VLAN de gerenciamento para uma VLAN diferente da VLAN 1. Para fins de gerenciamento, utilize a VLAN 99. A seleção da VLAN 99 é arbitrária e não significa que você deva utilizá-la sempre.
- b. Primeiro, crie a nova VLAN 99 no switch. Em seguida, configure o endereço IP do switch para 192.168.1.2 com uma máscara de sub-rede de 255.255.255.0 na VLAN 99 da interface virtual interna. O endereço IPv6 também pode ser configurado na interface SVI. Use os endereços IPv6 listados na Tabela de Endereçamento. Observe que a interface VLAN 99 está no estado inativo apesar de você ter inserido o comando no shutdown. A interface está atualmente inativa porque nenhuma porta de switch está atribuída à VLAN 99. 
  - `interface vlan 99` -> `ip address 192.168.1.2 255.255.255.0` -> `ipv6 address 2001:db8:acad:1::2/64` -> `ipv6 address fe80::2 link-local` -> `no shutdown` -> `exit`.
- c. Atribua todas as portas do usuário à VLAN 99. Para estabelecer a conectividade entre o host e o switch, as portas usadas pelo host devem estar na mesma VLAN que o switch. Após alguns segundos, a VLAN 99 aparece porque ao menos uma porta ativa (F0/6 com o PC-A conectado) está, agora, atribuída à VLAN 99.
  - `interface range g1/0/1-24, g1/1/1-4` -> `switchport mode access` -> `switchport access vlan 99` -> `end`.
- d. Emita o comando show vlan brief para verificar se todas as portas estão na VLAN 99.
  - `show vlan brief`.
- e. Configure o gateway padrão de S1. Se não houver nenhum gateway padrão configurado, o switch não poderá ser gerenciado de uma rede remota que esteja a uma distância maior do que a de um roteador. Embora esta atividade não inclua um gateway IP externo, considere que você, eventualmente, conectará a LAN a um roteador para acesso externo. Supondo que a interface da LAN no roteador seja 192.168.1.1, configure o gateway padrão para o switch.
  - `configure terminal` -> `ip default-gateway 192.168.1.1`.
- f. O acesso à porta do console também deve ser restrito com uma senha. Use cisco como a senha de login do console nesta atividade. A configuração padrão é permitir todas as conexões de console, sem necessidade de senha. Para evitar que as mensagens do console interrompam os comandos, utilize a opção logging synchronous. 
  - `line console 0` -> `password cisco` -> `login` -> `logging synchronous` -> `exit`.
- g. Configure as linhas virtuais terminais (vty) para que o switch permita o acesso Telnet. Se você não configurar uma senha vty, não poderá  acessar o switch via telnet.
  - `line vty 0 15` -> `password cisco` -> `login` -> `exit`.
- g. Por que o comando login é necessário?
  - O comando login faz com que o switch solicite a senha configurada nas linhas VTY para permitir o acesso via Telnet. Sem ele, a senha definida não será utilizada para autenticação.

<a name="item02.02"><h4>2.2 Etapa 2: Configurar um endereço IP no PC-A.</h4></a>[Back to summary](#item00)

Atribua o endereço IP e a máscara de sub-rede ao PC como mostrado na Tabela de Endereçamento. Uma versão sumarizada de procedimento está descrita aqui. Um gateway padrão não é necessário para esta topologia; no entanto, você pode inserir 192.168.1.1 e fe80::1 para simular um roteador conectado ao S1.

- a. Navegue até a Área de Trabalho. | Navegue até o Painel de Controle. 
- b. Clique em configuração IP. | Na visualização Categoria, selecione Exibir status e tarefas da rede.
- b0. Clique em Alterar configurações do adaptador no painel esquerdo.
- b0. Clique com o botão direito do mouse em uma interface Ethernet e escolha Propriedades.
- c. Verifique se o botão radial Configuração de IP estático está selecionado. | Escolha Internet Protocol Version 4 (TCP / IPv4) e clique em  Propriedades.
- d. Endereço, Máscara de sub-rede e Gateway padrão. | Clique no botão de opção Usar o seguinte endereço IP, digite o endereço IP e a máscara de sub-rede e clique em OK.
  - `192.168.1.10` -> `255.255.255.0` -> `192.168.1.1`.
- e. Verifique se o botão radial Configuração IPv6 estático está selecionado. | Selecione Protocolo de Internet TCP/IP versão 6 (TCP/IPv6) e clique em Propriedades.
- f. Digite o endereço IPv6, o prefixo, e o gateway padrão. | Clique no botão de opção Usar o seguinte endereço IPv6, digite o endereço e o prefixo IPv6 e clique em OK para continuar.
  - `2001:db8:acad:1::10` -> `64` -> `fe80::1`.
- g. Clique no X para fechar a janela configuração IP. | Clique em OK para sair da janela Propriedades.

A imagem 03 mostra as configurações de endereçamento IPv4 e IPv6 realizadas no PC-A.

<div align="center"><figure>
    <img src="./0-aux/img03.png" alt="img03"><br>
    <figcaption>Imagem 03.</figcaption>
</figure></div><br>

<a name="item03"><h4>3. Parte 3: Verificar e Testar a Conectividade da Rede</h4></a>[Back to summary](#item00)

Na Parte 3, você verificará e documentará a configuração do switch, testará a conectividade de ponta a ponta entre o PC-A e o S1 e testará o recurso de gerenciamento remoto do switch.

<a name="item03.01"><h4>3.1 Etapa 1: Exiba a configuração do switch.</h4></a>[Back to summary](#item00)

Use a conexão do console no PC-A para exibir e verificar a configuração do switch. O comando show run exibe a configuração em execução, integralmente, uma página por vez. Use a barra de espaços para percorrer as páginas.

- a. Um exemplo de configuração é apresentado. As configurações que você definiu estão destacadas em amarelo. As outras configuração são padrão do IOS.
  - `show run`.
- b. Verifique as configurações da VLAN 99 de gerenciamento.
  - `show interface vlan 99`.
- b. Qual é a largura de banda nessa interface?
  - A largura de banda da interface VLAN 99 é 100 Mb/s.
- b. Qual é o estado da VLAN 99?
  - O estado da VLAN 99 é ativo (up).
- b. Qual é o estado da linha do protocolo?
  - O estado da linha do protocolo é ativo (up).

<a name="item03.02"><h4>3.2 Etapa 2: Teste a conectividade de ponta a ponta com ping.</h4></a>[Back to summary](#item00)

- a. No prompt de comando do PC-A, primeiro, faça o ping do endereço do PC-A.
  - `ping 192.168.1.10`.
- b. Verifique que o PC-A pode pingar o endereço IPv4 e IPv6 para S1.
  - `ping 192.168.1.2` -> `ping 2001:db8:acad:1::2`.
- a. Como o PC-A precisa solucionar o endereço MAC do S1 por meio do ARP, o tempo do primeiro pacote pode expirar. Se os resultados do ping continuam falhando, identifique e solucione os problemas das configurações básicas do dispositivo. Verifique os cabos e o endereçamento lógico.

<a name="item03.03"><h4>3.3 Etapa 3: Teste e verifique o gerenciamento remoto de S1.</h4></a>[Back to summary](#item00)

Agora você usará o Telnet para acessar remotamente o switch. Neste laboratório, o PC-A e o S1 se encontram lado a lado. Em uma rede de produção, o switch pode estar em um wiring closet no andar superior enquanto o PC de gerenciamento está no andar térreo. Nesta Etapa, você usará o Telnet para acessar remotamente o switch S1 por meio do endereço de gerenciamento do SVI. O Telnet não é um protocolo seguro; entretanto, você o utilizará para testar o acesso remoto. Com o Telnet, todas as informações, inclusive senhas e comandos, são enviadas através da sessão em texto não criptografado. Nos laboratórios subsequentes, você usará o SSH para acessar remotamente os dispositivos de rede.

- a. Abra a guia Área de trabalho no PC-A. 
- b. Role para baixo na lista de aplicativos e clique no cliente Telnet/SSH. 
- c. Ajuste o tipo de conexão como telnet.
  - Connection Type: `Telnet`.
- d. Incorpore o endereço de gerenciamento SVI para conectar ao S1 e o clique conectar.
  - `192.168.1.2`.
- e. Após inserir a senha cisco, você estará no prompt do modo EXEC do usuário. Acesse o modo EXEC privilegiado utilizando o comando enable e fornecendo a senha class.
  - `cisco` -> `enable` -> `class`.
- f. Salvar a configuração.
  - `copy running-config startup-config`.
- g. Digite exit para finalizar a sessão Telnet. Clique em Não para o pop-up.
  - `exit`.

<a name="item03.04"><h4>3.4 Etapa 4: Implante o switch S1 na rede de produção.</h4></a>[Back to summary](#item00)

Agora você instalará o switch S1 na rede de produção e desconectará o cabo do console. Telnet será usado para acessar remotamente o interruptor e concluir toda a configuração e verificação adicionais. Nos laboratórios subsequentes, você usará o SSH para acessar remotamente os dispositivos de rede.

- a. Mova o switch S1 para o Rack.
- b. Clique com o botão direito do mouse no switch S1 e selecione Inspecionar.
- c. Clique e arraste o cabo do console para a placa de peg.

A imagem 04 exibe o acesso remoto à interface de gerenciamento do switch (SVI) realizado pelo PC-A, com acesso ao modo EXEC privilegiado, além da desconexão do cabo de console.

<div align="center"><figure>
    <img src="./0-aux/img04.png" alt="img04"><br>
    <figcaption>Imagem 04.</figcaption>
</figure></div><br>

<a name="item04"><h4>4. Perguntas para reflexão</h4></a>[Back to summary](#item00)

- a. Por que é necessário configurar a senha de vty para o switch?
  - A senha de VTY é necessária para autenticar o acesso remoto ao switch pelas linhas VTY, como ocorre em conexões Telnet ou SSH.
- b. Por que mudar a VLAN 1 padrão para um número de VLAN diferente?
  - Para aumentar a segurança, evitando utilizar a VLAN padrão para o gerenciamento do switch e reduzindo os riscos associados ao uso da VLAN 1.
- c. Como você pode impedir que senhas sejam enviadas em texto simples?
  - Utilizando protocolos que criptografam a comunicação, como o SSH, em vez do Telnet, para o acesso remoto ao switch.

<a name="item05"><h4>5. Parte 4: Gerenciar a tabela de endereços MAC</h4></a>[Back to summary](#item00)

Na Parte 4, você determina o endereço MAC que o switch aprendeu, configura um endereço MAC estático em uma interface do switch e, em seguida, remove o endereço MAC estático daquela interface.

<a name="item05.01"><h4>5.1 Etapa 1: Registre o endereço MAC do host.</h4></a>[Back to summary](#item00)

- a. Abra um prompt de comando em um PC-A e emita o comando ipconfig /all para determinar e gravar os endereços da Camada 2 (física) do NIC.
  - `ipconfig /all`.
  - `000C.854D.C942`.

<a name="item05.02"><h4>5.2 Etapa 2: Determine os endereços MAC que o switch aprendeu.</h4></a>[Back to summary](#item00)

- a. Exiba os endereços MAC, usando o comando show mac address-table. 
  - `show mac address-table`.
- a. Quantos endereços dinâmicos existem? 
  - Existe apenas 1 endereço MAC dinâmico, correspondente ao PC-A.
- a. Quantos endereços MAC existem no total?
  - Existe apenas 1 endereço MAC no total, correspondente ao PC-A.
- a. O endereço MAC dinâmico corresponde ao endereço MAC do PC-A? 
  - Sim, corresponde ao endereço MAC do PC-A.

<a name="item05.03"><h4>5.3 Etapa 3: Liste as opções do show mac address-table.</h4></a>[Back to summary](#item00)

- a. Exiba as opções da tabela de endereços MAC.
  - `show mac address-table ?`.
- a. Quantas opções estão disponíveis para o comando show mac address-table?
  - Existem três opções: dynamic, interface e static.
- b. Emita o comando show mac address-table dynamic para exibir apenas os endereços MAC que foram aprendidos dinamicamente.
  - `show mac address-table dynamic`.
- b. Quantos endereços dinâmicos existem? 
  - Existe apenas 1 endereço MAC dinâmico, correspondente ao PC-A.
- c. Visualize a entrada do endereço MAC do PC-A. A formatação do endereço MAC do comando é xxxx.xxxx.xxxx. 
  - `show mac address-table address 000C.854D.C942`. Esse comando não é suportado pelo modelo de switch utilizado no Packet Tracer.

<a name="item05.04"><h4>5.4 Etapa 4: Configure um endereço MAC estático.</h4></a>[Back to summary](#item00)

- a. Limpe a tabela de endereços MAC. Para remover os endereços MAC atuais, use o comando clear mac address-table dynamic no modo 
EXEC privilegiado. 
  - `clear mac address-table dynamic`.
- b. Verifique se a tabela de endereços MAC foi apagada. 
  - `show mac address-table`
- b. Quantos endereços MAC estáticos existem? 
  - Nenhum endereço MAC estático.
- b. Quantos endereços dinâmicos existem?
  - Existe apenas 1 endereço MAC dinâmico, correspondente ao PC-A.
- c. Examine novamente a tabela MAC. Muito provavelmente, um aplicativo em execução no PC já enviou um quadro através da NIC para o S1. Analise novamente a tabela de endereços MAC no modo EXEC privilegiado para ver se S1 reaprendeu o endereço MAC para o PC-A.
  - `show mac address-table`.
- c. Quantos endereços dinâmicos existem?
  -  Existe apenas 1 endereço MAC dinâmico, correspondente ao PC-A.
- c. Por que isso mudou comparado com a última tela?
  - Nada mudou na tabela de endereços MAC: ela continuou apresentando apenas 1 endereço MAC dinâmico, correspondente ao PC-A.
- d. Configure um endereço MAC estático. Para especificar com quais portas um host pode se conectar, uma opção é criar um mapeamento estático do endereço MAC do host para uma porta. Configure um endereço MAC estático em G1/0/6, usando o endereço que foi registrado para o PC-A na 
Parte 4, Etapa 1. O endereço MAC 0050.56BE.6C89 é usado apenas como um exemplo. Você deve usar o endereço MAC de seu PC-A, que é diferente do dado aqui como exemplo. 
  - `configure terminal` -> `mac address-table static 000C.854D.C942 vlan 99 interface GigabitEthernet 1/0/6` -> `exit`.
- e. Verifique as entradas da tabela de endereços MAC. 
  - `show mac address-table`.
- e. Quantos endereços MAC existem em total? 
  - Continua existindo apenas 1 endereço MAC, correspondente ao PC-A.
- e. Quantos endereços estáticos existem?
  - Agora existe 1 endereço MAC estático, correspondente ao PC-A, que foi configurado manualmente para a interface GigabitEthernet1/0/6.
- f. Remova a entrada MAC estática. Entre no modo de configuração global e remova o comando, incluindo um no na frente da sequência de comando. 
Observação: O endereço MAC 0050.56BE.6C89 é usado apenas no exemplo. Use o endereço MAC de PC-A. 
  - `configure terminal` -> `no mac address-table static 000C.854D.C942 vlan 99 interface GigabitEthernet1/0/6` -> `exit`.
- g. Verifique se o endereço MAC estático foi apagado.
  - `show mac address-table`.
- g. Quantos endereços MAC estáticos totais existem?
  - Nenhum. Nenhum. O endereço MAC do PC-A voltou a ser aprendido dinamicamente pelo switch após a remoção da entrada estática.

A imagem 05 evidencia a alteração do endereço MAC do PC-A de dinâmico para estático e, posteriormente, de estático para dinâmico.

<div align="center"><figure>
    <img src="./0-aux/img05.png" alt="img05"><br>
    <figcaption>Imagem 05.</figcaption>
</figure></div><br>

# Laboratório – Identificando Endereços IPv6   <img src="./0-aux/logo_course.png" alt="lab_051" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../labs/">labs</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">lab_051 (Laboratório – Identificando Endereços IPv6)   <img src="./0-aux/logo_course.png" alt="lab_051" width="auto" height="25"></a>

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
  - ipconfig   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/ipconfig.jpeg" alt="ipconfig" width="auto" height="25">
  
---

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">Parte 1: Prática com diferentes tipos de endereços IPv6</a><br>
  1.1 <a href="#item01.01">Etapa 1: Associe o endereço IPv6 ao seu tipo.</a><br>
  1.2 <a href="#item01.02">Etapa 2: Pratique a compactação e a descompactação de endereços IPv6.</a><br>
2. <a href="#item02">Parte 2: Examinar o Endereço e a Interface de Rede de um Host IPv6</a><br>
  2.1 <a href="#item02.01">Etapa 1: Verifique as configurações do endereço de rede IPv6 do PC.</a><br>
3. <a href="#item03">Perguntas para reflexão</a><br>

---

### Objective:
O objetivo deste laboratório foi analisar as diferentes categorias de endereços IPv6, aplicar as regras de compactação e expansão de quartetos e validar as configurações de rede em ambiente real Windows através do prompt de comando.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: Prática com diferentes tipos de endereços IPv6</h4></a>[Back to summary](#item00)

Nesta parte, você identificará os diferentes tipos de endereços IPv6 e praticará compactação e descompactação de endereços IPv6. 

<a name="item01.01"><h4>1.1 Etapa 1: Associe o endereço IPv6 ao seu tipo.</h4></a>[Back to summary](#item00)

Correlacione os endereços IPv6 ao tipo de endereço correspondente. Observe que os endereços foram compactados na notação abreviada e que o número de prefixo da rede com barra não é exibido. Algumas opções de resposta devem ser usadas mais de uma vez.
- Opções de Resposta:
  - Endereço de loopback
  - Endereço unicast global
  - Endereço de link local
  - Endereço Unique-local
  - Endereço multicast
- Endereço IPv6:
  - 2001:0db8:1:acad::fe55:6789:b210 -> Endereço unicast global
  - ::1 -> Endereço de loopback.
  - fc00:22:a:2::cd4:23e4:76fa -> Endereço Unique-local
  - 2033:db8:1:1:22:a33d:259a:21fe -> Endereço unicast global
  - fe80::3201:cc01:65b1 -> Endereço de link local
  - ff00:: -> Endereço multicast
  - ff00::db7:4322:a231:67c -> Endereço multicast
  - ff02::2 -> Endereço multicast.

<a name="item01.02"><h4>1.2 Etapa 2: Pratique a compactação e a descompactação de endereços IPv6.</h4></a>[Back to summary](#item00)

Usando as regras de abreviação de endereços IPv6, compacte ou descompacte os seguintes endereços: 
- a. 2002:0ec0:0200:0001:0000:04eb:44ce:08a2 -> 2002:ec0:200:1::4eb:44ce:8a2
- b. fe80:0000:0000:0001:0000:60bb:008e:7402 -> fe80::1:0:60bb:8e:7402
- c. fe80::7042:b3d7:3dec:84b8 -> fe80:0000:0000:0000:7042:b3d7:3dec:84b8
- d. ff00:: -> ff00:0000:0000:0000:0000:0000:0000:0000
- e. 2001:0030:0001:acad:0000:330e:10c2:32bf -> 2001:30:1:acad::330e:10c2:32bf

<a name="item02"><h4>2. Parte 2: Examinar o Endereço e a Interface de Rede de um Host IPv6</h4></a>[Back to summary](#item00)

Na Parte 2, você verificará as configurações de rede IPv6 do PC para identificar o endereço IPv6 da interface de rede. 

<a name="item02.01"><h4>2.1 Etapa 1: Verifique as configurações do endereço de rede IPv6 do PC.</h4></a>[Back to summary](#item00)

Confira se o protocolo IPv6 está instalado e ativo em PC-A (verifique as configurações da Conexão local).

- a. Navegue até o Painel de Controle.
- b. Clique no ícone Central de Rede e Compartilhamento. Clique em Exibir status e tarefas da rede.
- c. Na janela Central de Rede e Compartilhamento, você verá suas redes ativas.
- d. No lado esquerdo da janela, clique em Alterar as configurações do adaptador. Agora você verá ícones representando os adaptadores de rede instalados. Clique com o botão direito do mouse na interface de rede ativa (pode ser uma Ethernet ou Wi-Fi) e clique em Propriedades.
- e. Percorra a lista de itens para determinar se o IPv6 está presente, o que indica que está instalado, e também se ele está marcado, o que indica que está ativo.
- f. Selecione Protocolo TCP/IP versão 6 (TCP/IPv6) e clique em Propriedades. Você verá as configurações IPv6 da sua interface de rede. A janela de propriedades IPv6 provavelmente estará definida como Obter um endereço IPv6 automaticamente. Isso não significa que o IPv6 depende do protocolo DHCP. Em vez de usar o DHCP, o IPv6 recorre ao roteador local para obter informações de rede IPv6 e configura automaticamente seus próprios endereços IPv6. Para configurar manualmente o IPv6, você deve fornecer o endereço IPv6, o comprimento do prefixo da sub-rede e o gateway padrão. Clique em Cancelar para fechar a janela de propriedades. Observação: o roteador local pode recorrer a solicitações de host para obter informações IPv6, especialmente informações sobre DNS (Domain Name System), de um servidor DHCPv6 na rede.
- g. Depois de conferir que o IPv6 está instalado e ativo no PC, você deve verificar as informações do endereço IPv6. Abra um prompt de comando, digite ipconfig /all e pressione Enter. A saída deve ser semelhante a: `C:\Users\user> ipconfig /all`.
- h. Você pode ver na saída que o PC cliente tem um endereço de link local IPv6 com uma ID da interface gerada aleatoriamente. O que isso indica sobre a rede em relação ao endereço IPv6 unicast global, o endereço IPv6 unique local ou o endereço IPv6 do gateway?
  - A presença apenas do endereço Link-Local (fe80::) indica que a interface está ativa para IPv6, mas a rede local não possui um roteador configurado para enviar mensagens de Router Advertisement (RA). Sem esses anúncios, o PC não consegue obter um prefixo de roteamento para gerar endereços Unicast Global ou Unique-Local via SLAAC, nem consegue identificar automaticamente o endereço de gateway da rede.
- h. Que tipo de endereços IPv6 você encontrou ao usar ipconfig /all?
  - Foi encontrado dois endereços globais unicast sendo um temporário, o endereço de link-local e o gateway padrão que usa o endereço de link-local (FE80::1).

<a name="item03"><h4>3. Perguntas para reflexão</h4></a>[Back to summary](#item00)

- a. Como você acha que será o suporte ao IPv6 no futuro?
  - O suporte será nativo e predominante, tornando-se o padrão obrigatório para viabilizar a expansão de tecnologias como Internet das Coisas (IoT), redes 5G/6G e cidades inteligentes. A complexidade de configuração diminuirá com a maturidade da autoconfiguração (SLAAC), tornando a gestão de trilhões de dispositivos conectáveis algo invisível para o usuário final.
- b. Você acha que as redes IPv4 continuarão existindo ou todos acabarão migrando para o IPv6? Quanto tempo você acredita que isso levará?
  - As redes IPv4 persistirão por décadas em ambientes legados e redes privadas, mas a internet pública será majoritariamente IPv6. A migração total é um processo lento que deve levar pelo menos mais 15 a 20 anos, dependendo da desativação de infraestruturas antigas e da adoção global de mecanismos de transição como o Dual Stack.
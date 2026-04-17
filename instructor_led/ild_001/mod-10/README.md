# CCNA: Introduction to Networks - Módulo 10   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_001 (CCNA: Introduction to Networks)   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="25"></a>
### Module: 10. Configuração básica do roteador

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

### Course Module 10 Structure:
10. <a name="item10">Configuração básica do roteador</a><br>
  10.1 <a href="#item10.01">Introdução</a><br>
  10.2 <a href="#item10.02">Configurar definições iniciais do roteador</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;10.2.1 <a href="#item10.02.01">Verificador de sintaxe - Executar configurações iniciais do roteador</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;10.2.2 <a href="../../../pkt/files/pkt_026/">Packet Tracer – Configurar definições iniciais do roteador</a><br>
  10.3 <a href="#item10.03">Configurar Interfaces</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;10.3.1 <a href="#item10.03.01">Verificador de sintaxe - Configurar interfaces</a><br>
  10.4 <a href="#item10.04">Configurar o gateway padrão</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;10.4.1 <a href="#item10.04.01">Verificador de Sintaxe - Configurar o Gateway Padrão</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;10.4.2 <a href="../../../pkt/files/pkt_028/">Packet Tracer – Conexão de um Roteador a uma LAN</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;10.4.3 <a href="../../../pkt/files/pkt_029/">Packet Tracer – Solucionar problemas de gateway padrão</a><br>
  10.5 <a href="#item10.05">Módulo Prático e Quiz</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;10.5.1 <a href="../../../pkt/files/pkt_030/">Packet Tracer - Construir uma rede de switch e roteador - Modo Físico</a><br>
  10.6 Exame de comunicação entre redes<br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item10.01"><h4>10.1 Introdução</h4></a>[Back to summary](#item10)

📘 Introdução   
Este módulo aborda os primeiros passos necessários para preparar um roteador para operar em uma rede. Assim como o encaminhamento de pacotes depende de informações corretas sobre o próximo destino, o roteador precisa estar devidamente configurado antes que possa construir suas tabelas de roteamento e participar do transporte de dados entre diferentes redes. A configuração inicial define elementos essenciais, como identificação do dispositivo, parâmetros básicos e ativação das interfaces que permitirão o fluxo de pacotes. Atividades práticas auxiliam no domínio dos comandos fundamentais e no entendimento do comportamento do roteador após cada ajuste realizado.

🎯 Objetivo Geral   
Aplicar as configurações iniciais necessárias para habilitar o funcionamento básico de um roteador e dos dispositivos finais conectados a ele.

✅ Objetivos Específicos   
- Definir os parâmetros iniciais de um roteador Cisco IOS.
- Ativar e configurar interfaces essenciais para o encaminhamento de pacotes.
- Ajustar dispositivos finais para utilizarem o gateway padrão adequado.

<a name="item10.02"><h4>10.2 Configurar definições iniciais do roteador</h4></a>[Back to summary](#item10)

⚙️ Configuração Inicial de um Roteador   
Ao preparar um roteador para uso, existe um conjunto essencial de tarefas que garantem identificação, segurança e preservação das configurações:
- Configurar o nome do dispositivo: define uma identidade clara para o roteador no CLI e em registros.
- Proteger o modo EXEC privilegiado: aplica senha ao nível enable, que permite alterar configurações críticas.
- Proteger o modo EXEC de usuário: adiciona segurança ao acesso inicial, mesmo com permissões limitadas.
- Proteger o acesso remoto (Telnet/SSH): impede que alguém acesse o roteador pela rede sem autorização; o uso de SSH é a prática recomendada.
- Ocultar senhas no arquivo de configuração: evita que senhas apareçam em texto claro no running-config ou startup-config.
- Exibir uma notificação legal (banner): mostra um aviso de acesso restrito antes do login, funcionando como alerta e proteção legal.
- Salvar a configuração: grava todas as alterações para que continuem válidas após reinicialização do equipamento.

<a name="item10.02.01"><h4>10.2.1 Verificador de sintaxe - Executar configurações iniciais do roteador</h4></a>[Back to summary](#item10)

- Entre no modo de configuração global para configurar o nome do roteador como "R1": `enable`; `configure terminal`; `hostname R1`.
- Configure 'class' como a senha secreta: `enable secret class`.
- Configure 'cisco' como a senha da linha do console, exija que os usuários efetuem login e retorne ao modo de configuração global: `line console 0`; `password cisco`; `login`; `exit`.
- Para a linha vty 0 a 4, configure 'cisco' como a senha, exija que os usuários façam login, habilite o acesso SSH e Telnet e retorne ao modo de configuração global: `line vty 0 4`; `password cisco`; `login`; `transport input ssh telnet`; `exit`.
- Criptografe todas as senhas em texto simples: `service password-encryption`.
- Digite o banner "Somente acesso autorizado!" e use # como o caractere delimitante: `banner motd #Authorized Access Only!#`; 

<a name="item10.03"><h4>10.3 Configurar Interfaces</h4></a>[Back to summary](#item10)

🔌 Configuração das Interfaces do Roteador   
Após concluir as configurações básicas, o próximo passo é preparar as interfaces do roteador, pois somente depois disso os dispositivos finais poderão alcançá-lo. Cada modelo Cisco pode oferecer diferentes tipos de interfaces; por exemplo, um ISR 4321 conta com duas portas Gigabit Ethernet identificadas como G0/0/0 e G0/0/1.

A configuração de uma interface segue a mesma lógica usada em um SVI de gerenciamento em switches. O processo envolve entrar no modo da interface e aplicar alguns comandos fundamentais:
- `interface type-and-number`: seleciona a interface a ser configurada.
- `description texto`: registra informações úteis sobre o enlace ou o provedor conectado.
- `ip address endereço máscara`: define o endereço IPv4.
- `ipv6 address endereço/prefixo`: define o endereço IPv6.
- `no shutdown`: ativa a interface.

O comando description não é obrigatório, mas é recomendado, especialmente em redes de produção, pois ajuda a identificar o tipo de conexão, o provedor envolvido e informações de contato. O limite para esse texto é de 240 caracteres. A ativação da interface com `no shutdown` funciona como “ligar” a porta. Para que a camada física fique operacional, a porta deve estar conectada a outro equipamento, como um switch ou outro roteador. Em enlaces diretos entre roteadores, ambas as extremidades precisam ser configuradas e habilitadas.

Após ativar as interfaces, o equipamento normalmente exibe mensagens informando que o link entrou em operação. Para verificar se tudo foi configurado corretamente, alguns comandos de monitoramento são essenciais:
- `show ip interface brief / show ipv6 interface brief`: lista todas as interfaces, endereços configurados e seus estados. Uma interface funcional deve aparecer com Status up e Protocol up.
- `show ip route / show ipv6 route`: apresenta as tabelas de roteamento armazenadas na RAM.
- `show interfaces`: exibe estatísticas detalhadas de cada interface, com foco em informações IPv4.
- `show ip interfaces`: mostra dados específicos de IPv4.
- `show ipv6 interface`: exibe informações específicas de IPv6.

Esses comandos ajudam a confirmar o funcionamento das interfaces e identificar problemas de configuração ou cabeamento.

<a name="item10.03.01"><h4>10.3.1 Verificador de sintaxe - Configurar interfaces</h4></a>[Back to summary](#item10)

- Entre no modo de configuração global: `configure terminal`.
- Configure interface gigabitethernet 0/0/0: `interface gigabitethernet 0/0/0`.
- Descreva o link como 'Link to LAN': `description Link to LAN`.
- Configure a interface com endereço IPv4 192.168.10.1 e máscara de sub-rede 255.255.255.0: `ip address 192.168.10.1 255.255.255.0`.
- Configure a interface com o endereço IPv6 2001:db8:acad:10::1 e o comprimento do prefixo /64: `ipv6 address 2001:db8:acad:10::1/64`.
- Ative a interface e retorne ao modo de configuração global: `no shutdown`; `exit`.

<a name="item10.04"><h4>10.4 Configurar o gateway padrão</h4></a>[Back to summary](#item10)

🌐 Gateway Padrão em Hosts e Switches   
Quando uma rede possui apenas um roteador, ele atua como gateway padrão para todos os dispositivos da LAN. Em redes com vários roteadores, é necessário escolher qual deles assumirá essa função. O gateway padrão é essencial sempre que um host precisa enviar pacotes para dispositivos fora de sua própria rede.

🖥️ Gateway padrão em hosts   
Para que um dispositivo final consiga se comunicar além da sua LAN, ele deve estar configurado com:
- Endereço IP
- Máscara de sub-rede
- Gateway padrão

O gateway padrão normalmente corresponde ao endereço da interface do roteador conectada à rede local. Esse endereço deve pertencer à mesma rede que o IP do host.

Exemplo:
- Roteador com G0/0/0 → 192.168.10.0
- Roteador com G0/0/1 → 192.168.11.0

Se PC1 enviar um pacote para PC2 (mesma LAN), o gateway não é usado; o pacote é encaminhado diretamente pelo switch.
Se PC1 enviar um pacote para PC3 (rede diferente), o pacote é enviado ao gateway padrão (G0/0/0). O roteador consulta sua tabela de roteamento, identifica a interface correta (G0/0/1) e encaminha o pacote para PC3.

O raciocínio é o mesmo em redes IPv6, usando o endereço IPv6 da interface do roteador como gateway padrão.

🔁 Gateway padrão em switches Layer 2   
Switches de Camada 2 não precisam de endereço IP para operar, mas precisam de configuração IP quando vão ser gerenciados remotamente. Para isso, é necessário:
- Configurar um SVI (Switch Virtual Interface) com IP e máscara na LAN local.
- Configurar o gateway padrão, permitindo que o switch responda a administradores que estejam em outra rede.
- Comando para configurar o gateway padrão IPv4 no switch: `ip default-gateway <ip-do-gateway>`.

Esse endereço deve ser o IP da interface do roteador conectada ao switch.

Exemplo de fluxo:
- O administrador envia pacotes de outra rede.
- O switch recebe o pacote e precisa do gateway padrão para devolver a resposta via roteador.
- Sem o gateway configurado, o switch não consegue estabelecer conexões remotas (ex.: SSH).

Observação: Hosts conectados ao switch já devem ter o gateway padrão configurado no próprio sistema operacional.

🧩 Gateway padrão em IPv6   
Um switch também pode ter IPv6 configurado no SVI. Porém, nesse caso, o gateway padrão não precisa ser configurado manualmente. Ele é aprendido automaticamente através das mensagens ICMPv6 Router Advertisement (RA) enviadas pelo roteador.

<a name="item10.04.01"><h4>10.4.1 Verificador de Sintaxe - Configurar o Gateway Padrão</h4></a>[Back to summary](#item10)

- Entre no modo de configuração global: `configure terminal`.
- Configure 192.168.10.1 como o gateway padrão para S1: `ip default-gateway 192.168.10.1`.

<a name="item10.05"><h4>10.5 Módulo Prático e Quiz</h4></a>[Back to summary](#item10)

⚙️ Configuração inicial do roteador   
Ao iniciar um roteador pela primeira vez, é necessário preparar ajustes básicos de segurança e identificação. Isso inclui definir um nome para o equipamento, proteger o modo EXEC privilegiado, bloquear o acesso ao modo EXEC do usuário, configurar a proteção de acesso remoto via Telnet ou SSH, ocultar todas as senhas no arquivo de configuração e exibir um aviso legal para acessos não autorizados. Depois de tudo ajustado, a configuração precisa ser salva para não ser perdida após reinicializações.

🔌 Configuração das interfaces do roteador   
Para que o roteador seja acessível na rede, suas interfaces precisam estar configuradas e ativas. No modelo Cisco ISR 4321, existem as portas G0/0/0 e G0/0/1. Assim como ocorre com um SVI de gerenciamento em um switch, a interface só funciona quando é ativada com `no shutdown` e está fisicamente conectada a outro dispositivo. A verificação pode ser feita com comandos como `show ip interface brief`, `show ipv6 interface brief`, `show ip route`, `show ipv6 route`, além dos comandos detalhados de interface, como `show interfaces`, `show ip interface` e `show ipv6 interface`.

🖧 Configuração de hosts e switches para comunicação   
Um host só consegue participar da rede se tiver um endereço IP configurado, incluindo o gateway padrão — normalmente o IP da interface do roteador conectada à LAN local. O host e o roteador precisam estar na mesma rede. Para que um switch seja administrado pela rede, ele deve possuir um SVI configurado com um IPv4 e máscara da LAN. O switch também precisa de um gateway padrão configurado, permitindo o gerenciamento a partir de outras redes. Isso é feito com o comando global `ip default-gateway endereço_IP`, usando o IP da interface do roteador ligada ao switch.
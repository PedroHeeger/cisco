# CCNA: Introduction to Networks - Módulo 15   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_001 (CCNA: Introduction to Networks)   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="25"></a>
### Module: 15. Camada de aplicação

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

### Course Module 15 Structure:
15. <a name="item15">Camada de aplicação</a><br>
  15.1 <a href="#item15.01">Introdução</a><br>
  15.2 <a href="#item15.02">Aplicação, Apresentação e Sessão</a><br>
  15.3 <a href="#item15.03">Ponto a ponto</a><br>
  15.4 <a href="#item15.04">Protocolos de E-mail e Web</a><br>
  15.5 <a href="#item15.05">Serviços de Endereçamento IP</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;15.5.1 <a href="#item15.05.01">Verificador de Sintaxe - O Comando nslookup</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;15.5.2 <a href="#item15.05.02">Laboratório - Identificando Endereços IPv6</a><br>
  15.6 <a href="#item15.06">Serviços de Compartilhamento de Arquivos</a><br>
  15.7 <a href="#item15.07">Módulo Prático e Quiz</a><br>
  15.8 <a href="#item15.08">Exame de Comunicação de Aplicativos de Rede</a><br>

---

### Objective:
O objetivo deste módulo foi apresentar os fundamentos da governança em segurança digital, destacando políticas, papéis e responsabilidades na administração de dados. Também foram exploradas as principais leis, regulamentações e normas internacionais aplicáveis à proteção da informação. Além disso, foram abordados os princípios éticos na tomada de decisões em ambientes digitais e introduzidos frameworks e controles essenciais, como ISO 27000, NIST, CIS e CSA, para garantir conformidade, proteção de dados e integridade operacional em organizações.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item15.01"><h4>15.1 Introdução</h4></a>[Back to summary](#item15)

🧩 Camada de Aplicação   
A camada de aplicação reúne os serviços e protocolos que preparam os dados para que possam ser utilizados por softwares e sistemas no destino. É nesse nível que as informações ganham formato adequado, permitindo que diferentes aplicações e dispositivos interpretem o conteúdo corretamente. Esse conjunto de funções garante que a comunicação entre sistemas seja compatível, organizada e funcional, servindo como ponte entre as necessidades do usuário e o restante da pilha de rede. Este módulo explora essas funções e apresenta os principais protocolos utilizados no cotidiano das redes modernas.

🎯 Objetivo do módulo   
Explicar a operação de protocolos da camada de aplicação para dar suporte às aplicações do usuário final.

📘 Tópicos do módulo   
- Aplicação, Apresentação e Sessão: Mostrar como essas três camadas trabalham em conjunto para fornecer serviços de comunicação para softwares corporativos e demais aplicações.
- Ponto a ponto: Apresentar o funcionamento de aplicações que trocam dados diretamente entre sistemas, sem depender de um servidor central.
- Protocolos de e-mail e Web: Explicar como protocolos usados na Web e no envio de mensagens eletrônicas operam para disponibilizar conteúdos e entregar mensagens.
- Serviços de endereçamento IP: Descrever o papel de DHCP e DNS na atribuição automática de endereços e na tradução de nomes de domínio.
- Serviços de compartilhamento de arquivos: Abordar como os protocolos de transferência e acesso a arquivos permitem distribuir conteúdos entre diferentes dispositivos.

<a name="item15.02"><h4>15.2 Aplicação, Apresentação e Sessão</h4></a>[Back to summary](#item15)

🌐 Camada de Aplicação nos Modelos OSI e TCP/IP   
Nos modelos de referência OSI e TCP/IP, a Camada de Aplicação atua como a interface direta entre a rede de dados e o software utilizado pelo usuário final. É nesta camada que ocorre a troca de dados entre os programas executados no host de origem e no host de destino. No contexto específico do modelo TCP/IP, a Camada de Aplicação engloba as funcionalidades das três camadas superiores do modelo OSI: Aplicação, Apresentação e Sessão. Para que a comunicação ocorra com êxito, é imprescindível que os protocolos implementados nas extremidades da conexão sejam compatíveis.

🎨 Funções da Camada de Apresentação   
A Camada de Apresentação é responsável por garantir que a informação enviada pela camada de aplicação de um sistema possa ser lida pela camada de aplicação de outro. Suas funções primárias incluem:
- Formatação de Dados: Adaptação dos dados da origem para um formato compreensível pelo destino.
- Compressão: Redução do tamanho dos dados para otimizar a transmissão, permitindo a descompactação no destino.
- Criptografia: Codificação dos dados para segurança durante o transporte e descriptografia no recebimento.

Existem diversos padrões definidos para arquivos nesta camada:
- Vídeo: Matroska Video (MKV), Motion Picture Experts Group (MPG) e QuickTime Video (MOV).
- Imagens: Graphics Interchange Format (GIF), Joint Photographic Experts Group (JPG) e Portable Network Graphics (PNG).

🤝 Funções da Camada de Sessão   
A Camada de Sessão gerencia os diálogos (sessões) entre as aplicações de origem e destino. Cabe a esta camada iniciar a troca de informações, manter a conexão ativa durante a transferência e reiniciar sessões que tenham sido interrompidas ou permanecido ociosas por períodos prolongados.

🏷️ Protocolos de Sistema de Nomes e Configuração de Host   
Estes protocolos são fundamentais para a identificação e endereçamento de dispositivos na rede:
- DNS (Domain Name System): Opera sobre TCP/UDP na porta 53. Sua função é traduzir nomes de domínio legíveis (como cisco.com) em endereços IP numéricos.
- BOOTP (Bootstrap Protocol): Utiliza UDP (Cliente 68, Servidor 67). Permite que estações de trabalho sem disco descubram seu próprio IP e carreguem arquivos de inicialização. Atualmente, está sendo substituído pelo DHCP.
- DHCP (Dynamic Host Configuration Protocol): Utiliza UDP (Cliente 68, Servidor 67). Realiza a atribuição dinâmica de endereços IP, permitindo o reuso de endereços quando estes não são mais necessários pelo host.

📧 Protocolos de Correio Eletrônico (Email)   
O gerenciamento e tráfego de emails dependem de três protocolos principais:
- SMTP (Simple Mail Transfer Protocol): Opera na porta TCP 25. É utilizado para o envio de mensagens de clientes para servidores e para o roteamento de mensagens entre servidores de email.
- POP3 (Post Office Protocol version 3): Opera na porta TCP 110. Permite que o cliente baixe as mensagens do servidor para a aplicação local, removendo-as geralmente do servidor após a transferência.
- IMAP (Internet Message Access Protocol): Opera na porta TCP 143. Permite o acesso e gerenciamento de emails diretamente no servidor, mantendo as mensagens armazenadas remotamente para sincronização entre múltiplos dispositivos.

📂 Protocolos de Transferência de Arquivos   
Para a movimentação de arquivos entre hosts, utilizam-se protocolos com diferentes características de confiabilidade:
- FTP (File Transfer Protocol): Opera nas portas TCP 20 e 21. É um protocolo orientado a conexão e confiável, estabelecendo regras para o acesso e transferência de arquivos com confirmação de entrega.
- TFTP (Trivial File Transfer Protocol): Opera sobre UDP na porta 69. É uma versão simplificada, sem conexão e sem confirmação de entrega (melhor esforço), resultando em menor sobrecarga (overhead) na rede.

🌍 Protocolos de Navegação Web   
A comunicação na World Wide Web baseia-se na troca de hipertexto e multimídia:
- HTTP (Hypertext Transfer Protocol): Opera nas portas TCP 80 ou 8080. Define as regras para a troca de textos, imagens, vídeos e outros arquivos multimídia na web.
- HTTPS (HTTP Secure): Opera nas portas TCP/UDP 443. Adiciona uma camada de segurança ao HTTP através de criptografia, protegendo a integridade dos dados e autenticando o servidor acessado.

<a name="item15.03"><h4>15.3 Ponto a ponto</h4></a>[Back to summary](#item15)

🔄 Modelos de Comunicação: Cliente-Servidor e Peer-to-Peer   
No contexto da camada de aplicação, a comunicação em rede estrutura-se, predominantemente, através de dois modelos distintos: o modelo Cliente-Servidor e o modelo Ponto a Ponto (Peer-to-Peer ou P2P). A escolha do modelo define como os dispositivos interagem, como os recursos são acessados e como os papéis de origem e destino são atribuídos durante a transmissão de dados.

🖥️ O Modelo Cliente-Servidor   
Neste modelo, existe uma distinção clara de funções entre os dispositivos participantes da rede. O cliente é definido como uma combinação de hardware e software utilizada para solicitar informações ou recursos. O servidor é o dispositivo responsável por armazenar recursos e responder a essas solicitações. Os processos de comunicação ocorrem da seguinte forma:
- Requisição e Resposta: O fluxo inicia-se com o cliente enviando uma solicitação de dados. O servidor processa o pedido e retorna uma ou mais sequências de dados.
- Protocolos: Os protocolos da camada de aplicação definem o formato exato das requisições e respostas.
- Autenticação: Além da transferência de dados, pode ser necessário o envio de credenciais para autenticação de usuário e identificação dos arquivos solicitados.
- Upload e Download: A transferência de dados do servidor para o cliente é denominada download, enquanto o envio de dados do cliente para o servidor é chamado de upload.

Um exemplo clássico deste modelo é o serviço de e-mail corporativo ou de um provedor (ISP), onde o cliente de e-mail solicita mensagens não lidas e o servidor as envia.

🔗 Redes Ponto a Ponto (P2P)   
Diferente do modelo anterior, as redes P2P caracterizam-se pela ausência de um servidor dedicado. Dois ou mais computadores conectam-se para compartilhar recursos, como arquivos e impressoras, tratando-se como iguais (peers) dentro da topologia da rede. As principais características das redes P2P incluem:
- Igualdade de Funções: Todo dispositivo final pode atuar tanto como cliente quanto como servidor.
- Dinamicidade: Um computador pode atuar como servidor em uma transação (fornecendo um arquivo) e, simultaneamente, ser cliente em outra (imprimindo um documento em uma impressora compartilhada por outro peer).
- Compartilhamento Direto: Facilita a execução de jogos em rede e compartilhamento de conexões de internet sem intermediários centralizados.

📦 Aplicações P2P e Sistemas Híbridos   
Uma aplicação P2P exige que o dispositivo final possua uma interface de usuário e execute um serviço em segundo plano para gerenciar as comunicações. Embora a transferência de dados seja descentralizada, algumas aplicações utilizam um sistema híbrido. Neste sistema híbrido, o compartilhamento do recurso (arquivo) ocorre diretamente entre os usuários, mas existe um servidor centralizado que armazena índices (diretórios) apontando onde cada recurso está localizado. Assim, o peer consulta o índice central para descobrir onde está o arquivo desejado e, em seguida, conecta-se diretamente ao outro peer para baixá-lo.

🌐 Protocolos e Tecnologias P2P Comuns   
Existem diversos protocolos desenvolvidos para otimizar o compartilhamento de arquivos em redes P2P. Destacam-se duas abordagens principais:
- Protocolo Gnutella:
  - Permite o compartilhamento de arquivos completos.
  - Os usuários conectam-se aos serviços Gnutella para localizar recursos compartilhados por outros usuários.
  - Exemplos de softwares compatíveis: pTorrent, BitComet, DC++, Deluge e eMule.
- Tecnologia BitTorrent:
  - Utiliza uma abordagem de "enxame" (swarming), onde os arquivos são divididos em pequenos trechos ou peças.
  - O cliente utiliza um arquivo .torrent para localizar outros usuários que possuem as peças necessárias e conecta-se a eles simultaneamente.
  - Existem computadores "rastreadores" que monitoram quais usuários possuem quais partes do arquivo.
  - Exemplos de clientes: uTorrent, Deluge e qBittorrent.

⚠️ Considerações sobre Direitos Autorais   
É fundamental notar que a tecnologia P2P é neutra, permitindo o compartilhamento de qualquer tipo de arquivo. No entanto, muitos materiais compartilhados são protegidos por leis de direitos autorais. A distribuição ou o download de arquivos protegidos sem a permissão explícita do detentor dos direitos constitui ilegalidade, sujeitando o infrator a ações civis e criminais.

<a name="item15.04"><h4>15.4 Protocolos de E-mail e Web</h4></a>[Back to summary](#item15)

🌐 Protocolos de Navegação Web (HTTP e HTTPS)   
A interação entre um navegador e um servidor web inicia-se quando um endereço (URL ou URI) é inserido no navegador. O processo de carregamento de uma página segue um fluxo estruturado de etapas:
- Interpretação da URL: O navegador segmenta o endereço em três partes: o protocolo (ex: http), o nome do servidor (ex: www.cisco.com) e o arquivo solicitado (ex: index.html).
- Resolução de Nomes e Conexão: O navegador consulta um servidor DNS para converter o nome do domínio em um endereço IP numérico. Em seguida, inicia uma solicitação HTTP (geralmente do tipo GET) para o servidor, requisitando o arquivo específico.
- Resposta do Servidor: O servidor processa a solicitação e envia o código HTML correspondente ao navegador.
- Renderização: O navegador interpreta o código HTML recebido e formata a visualização da página para o usuário.

📨 Métodos de Requisição HTTP   
O protocolo HTTP define tipos específicos de mensagens para gerenciar a comunicação entre cliente e servidor. Os métodos mais comuns incluem:
- GET: Utilizado para solicitar dados. É o método padrão quando um navegador requisita uma página HTML.
- POST: Utilizado para enviar dados ao servidor, como o preenchimento de formulários ou envio de credenciais.
- PUT: Utilizado para carregar recursos ou conteúdo para o servidor, como o upload de uma imagem.

🔒 Segurança na Web: HTTPS   
O HTTP padrão transmite dados em texto simples, o que permite que informações sejam interceptadas e lidas por terceiros. Para mitigar essa vulnerabilidade, utiliza-se o HTTPS (HTTP Secure). O HTTPS mantém o mesmo processo de requisição e resposta do HTTP, mas adiciona uma camada de criptografia (SSL/TLS). Isso garante que o fluxo de dados seja codificado antes do transporte pela rede, assegurando a confidencialidade e a autenticação do servidor acessado.

📧 Infraestrutura de E-mail   
O serviço de e-mail opera através de um método de "armazenar e encaminhar" (store-and-forward). A comunicação não ocorre diretamente entre dois clientes de e-mail; em vez disso, os clientes dependem de servidores para o transporte das mensagens. O ecossistema de e-mail utiliza três protocolos principais: o SMTP para envio e o POP ou IMAP para recebimento e recuperação de mensagens.

📤 SMTP (Simple Mail Transfer Protocol)   
O SMTP é o protocolo responsável pelo envio de e-mails. Ele opera na porta 25 e gerencia a transferência de mensagens do cliente para o servidor e entre servidores de domínios diferentes.
- Estrutura: As mensagens exigem um cabeçalho (com remetente e destinatário formatados corretamente) e um corpo de texto.
- Processo de Envio: O cliente conecta-se ao servidor SMTP. Se o destinatário for local, a mensagem é entregue na caixa de entrada. Se for externo, o servidor a encaminha.
- Fila de Mensagens: Caso o servidor de destino esteja ocupado ou offline, o SMTP armazena a mensagem e realiza tentativas periódicas de reenvio. Se o tempo limite expirar, a mensagem é devolvida ao remetente como não entregue.

📥 POP (Post Office Protocol)   
O POP (geralmente em sua versão 3, POP3) é utilizado para recuperar mensagens de um servidor. Ele opera na porta TCP 110 e é caracterizado pelo comportamento de download e exclusão.
- Funcionamento: O cliente estabelece conexão com o servidor, baixa as mensagens para o dispositivo local e, por padrão, as remove do servidor.
- Limitação: Como as mensagens não permanecem no servidor, não há backup centralizado. Esse protocolo não é ideal para usuários que precisam acessar seus e-mails em múltiplos dispositivos, pois o histórico fica fragmentado.

☁️ IMAP (Internet Message Access Protocol)   
O IMAP oferece um método mais avançado para recuperação de e-mails, focado na sincronização.
- Sincronização: Ao contrário do POP, o IMAP baixa cópias das mensagens para o cliente, mantendo os originais no servidor até que sejam excluídos manualmente.
- Organização: Permite a criação de hierarquias de pastas e organização de arquivos diretamente no servidor. Qualquer ação realizada no cliente (como ler, mover ou excluir um e-mail) é refletida no servidor e em todos os outros dispositivos conectados à mesma conta.

<a name="item15.05"><h4>15.5 Serviços de Endereçamento IP</h4></a>[Back to summary](#item15)

🌐 Serviços de Endereçamento IP: Visão Geral   
Em redes de grande escala, a configuração manual de endereços IP em cada dispositivo é uma tarefa inviável. Para solucionar isso, existem protocolos na camada de aplicação projetados para automatizar a gestão de endereços e facilitar a navegação. A função primordial desses serviços é traduzir endereços numéricos (essenciais para o roteamento de dados) em nomes amigáveis (fáceis de memorizar por humanos), além de gerenciar a distribuição dinâmica de configurações de rede.

📇 DNS: O Sistema de Nomes de Domínio   
O DNS (Domain Name System) opera como um serviço automatizado que vincula nomes de domínio totalmente qualificados (FQDNs), como www.cisco.com, aos seus respectivos endereços IP numéricos. Essa abstração permite que o endereço IP de um servidor seja alterado sem afetar o acesso do usuário, pois o nome de domínio permanece constante. O processo de resolução de nomes ocorre em etapas sequenciais:
- Solicitação: O usuário insere um FQDN no navegador.
- Consulta: O cliente envia uma consulta ao servidor DNS configurado.
- Correspondência: O servidor DNS busca em seus registros o endereço IP associado ao nome.
- Resposta: O servidor retorna o endereço IP ao cliente.
- Conexão: O dispositivo utiliza o IP recebido para estabelecer a conexão com o servidor de destino.

📝 Estrutura de Registros e Mensagens DNS   
Os servidores DNS armazenam diferentes tipos de registros de recursos para realizar a resolução:
- Registro A: Mapeia um nome de host para um endereço IPv4.
- Registro NS: Identifica um servidor de nomes com autoridade para a zona.
- Registro AAAA: Mapeia um nome de host para um endereço IPv6.
- Registro MX: Identifica servidores de troca de correio (e-mail).

Para otimizar o desempenho, o DNS utiliza um sistema de cache. Servidores armazenam temporariamente endereços resolvidos recentemente. Da mesma forma, sistemas operacionais (como Windows) mantêm um cache local, que pode ser visualizado através do comando `ipconfig /displaydns`.

🌲 Hierarquia e Escalabilidade do DNS   
O protocolo DNS organiza-se em uma estrutura hierárquica e distribuída, dividida em zonas gerenciáveis. Isso garante escalabilidade, pois nenhum servidor único detém todos os registros da internet. A hierarquia compõe-se de:
- Domínios de Nível Superior (TLD): Representam tipos de organização (.com, .org, .net) ou países (.br, .au, .co).
- Domínios de Segundo Nível: Nomes registrados por organizações ou indivíduos (ex: cisco em cisco.com).

Além disso, administradores de rede podem utilizar a ferramenta nslookup para consultar manualmente servidores de nomes, sendo útil para diagnósticos e verificação de configurações.

⚙️ DHCP: Protocolo de Configuração Dinâmica de Host   
O DHCP (Dynamic Host Configuration Protocol) automatiza a atribuição de endereços IPv4, máscaras de sub-rede, gateways e outros parâmetros.
- Endereçamento Dinâmico: Utilizado para dispositivos de usuários finais e redes com alta rotatividade. O servidor DHCP atribui um IP de um "pool" (conjunto) de endereços disponíveis.
- Endereçamento Estático: Reservado para infraestrutura crítica, como roteadores, switches, servidores e impressoras, onde o IP não deve mudar.
- Concessão (Lease): O IP é cedido por um tempo determinado. Ao fim do período ou mediante comando de liberação, o endereço retorna ao pool para ser reutilizado por outro dispositivo.

🔄 O Processo de Operação do DHCPv4   
Quando um dispositivo configurado para DHCP conecta-se à rede, ocorre um processo de negociação conhecido por quatro etapas principais:
- DHCPDISCOVER (Descoberta): O cliente transmite uma mensagem em broadcast para localizar servidores DHCP disponíveis.
- DHCPOFFER (Oferta): Os servidores respondem oferecendo um endereço IP, máscara, gateway e DNS, além do tempo de concessão.
- DHCPREQUEST (Requisição): O cliente escolhe uma das ofertas e solicita formalmente o uso daquele endereço ao servidor específico.
- DHCPACK (Confirmação): O servidor confirma a concessão, finalizando a configuração. Se o IP não estiver mais disponível, o servidor envia um DHCPNAK, forçando o reinício do processo.

🔍 Particularidades do DHCPv6   
O DHCP para IPv6 oferece serviços similares, porém com nomenclaturas de mensagens distintas: SOLICIT, ADVERTISE, INFORMATION REQUEST e REPLY. Uma diferença técnica crucial é que o DHCPv6, por padrão, não fornece o endereço do gateway padrão. Esta informação deve ser obtida pelo cliente dinamicamente através de mensagens de Anúncio do Roteador (Router Advertisement) na rede.

<a name="item15.05.01"><h4>15.5.1 Verificador de Sintaxe - O Comando nslookup</h4></a>[Back to summary](#item15)

- No prompt de comando do Windows, digite o nslookup comando para iniciar uma consulta manual dos servidores de nomes: `nslookup`.
- As saídas listam o nome e o endereço IP do servidor DNS configurado no cliente. Observe que o endereço do servidor DNS pode ser configurado manualmente ou aprendido dinamicamente através do DHCP. Você está agora no modo nslookup. Digite o nome de domínio www.cisco.com: `www.cisco.com`.
- As saídas listam os endereços IP relacionados com www.cisco.com que o servidor 'e2867' tem em seu banco de dados atualmente. Observe que endereços IPv6 também estão listados. Além disso, vários aliases são exibidos e que também serão resolvidos para wwa.cisco.com. Digite o comando exit para sair do modo nslookup e retornar à linha de comando do Windows: `exit`.
- Você pode consultar diretamente os servidores DNS simplesmente adicionando o nome de domínio ao comando nslookup. Entrar nslookup www.googie.com: `nslookup www.googie.com`.
- Você agora está trabalhando no prompt de comando do Linux. O comando nslookup é o mesmo. Insira o comando nslookup para iniciar uma consulta manual dos servidores de nomes: `nslookup`.
- Insira www.cisco.com no prompt: `www.cisco.com`.
- Insira exit para sair do modo nslookup e retornar à linha de comandos do Linux: `exit`.
- Como no Windows, você pode consultar diretamente os servidores DNS simplesmente adicionando o nome de domínio ao comando nslookup. Entrar nslookup www.google.com: `nslookup www.google.com`.

<a name="item15.06"><h4>15.6 Serviços de Compartilhamento de Arquivos</h4></a>[Back to summary](#item15)

📂 Protocolo de Transferência de Arquivos (FTP)   
O FTP é um protocolo da camada de aplicação estruturado para facilitar a transferência de arquivos entre um cliente e um servidor. Sua operação permite o fluxo bidirecional de dados, possibilitando tanto o envio (upload) quanto o recebimento (download) de informações. Para garantir a eficiência e a organização da comunicação, o cliente FTP utiliza duas conexões TCP distintas com o servidor:
- Conexão de Controle (Porta TCP 21): É a primeira conexão estabelecida. Sua função é gerenciar o tráfego de comandos do cliente e as respostas do servidor (autenticação, navegação de diretórios).
- Conexão de Dados (Porta TCP 20): Esta conexão é estabelecida especificamente para o transporte do arquivo propriamente dito. Ela é criada e encerrada conforme a necessidade de transferência de dados surge.

🖨️ Protocolo Server Message Block (SMB)   
O SMB é um protocolo do tipo requisição-resposta desenvolvido para o compartilhamento de recursos de rede, abrangendo arquivos, diretórios, impressoras e portas seriais. As mensagens SMB seguem uma estrutura padronizada, contendo um cabeçalho de tamanho fixo seguido por parâmetros variáveis e o corpo de dados. As funções primárias das mensagens SMB incluem:
- Gestão de Sessão: Iniciar, autenticar e encerrar conexões entre dispositivos.
- Controle de Recursos: Gerenciar o acesso a arquivos e impressoras compartilhados.
- Comunicação entre Aplicações: Permitir o envio e recebimento de mensagens entre softwares em dispositivos diferentes.

💻 Evolução e Integração do SMB   
O protocolo SMB tornou-se a base das redes Microsoft. Uma mudança significativa ocorreu com a introdução do Windows 2000, quando a estrutura passou a utilizar a resolução de nomes via DNS. Isso permitiu que o compartilhamento de recursos SMB fosse suportado diretamente pelos protocolos TCP/IP. Diferentemente do FTP, que foca na transferência pontual, o SMB estabelece uma conexão de longo prazo. Isso permite que, após a conexão, os recursos do servidor (como pastas compartilhadas) sejam acessados e visualizados pelo sistema operacional cliente como se fossem recursos locais. A interoperabilidade do SMB estende-se além do ambiente Windows:
- Linux e UNIX: Utilizam uma implementação do SMB conhecida como SAMBA para compartilhar recursos com redes Microsoft.
- Apple Macintosh: Os sistemas operacionais da Apple também oferecem suporte nativo ao compartilhamento de recursos via SMB.

<a name="item15.07"><h4>15.7 Módulo Prático e Quiz</h4></a>[Back to summary](#item15)

🧩 Camada de Aplicação, Apresentação e Sessão   
Nos modelos OSI e TCP/IP, a camada de aplicação é a mais próxima do usuário e viabiliza a troca de dados entre programas nos hosts. A camada de apresentação prepara os dados para comunicação, cuidando de formatação, compactação e criptografia. Já a camada de sessão estabelece, mantém e retoma diálogos entre aplicações, garantindo continuidade mesmo após interrupções.

🔄 Protocolos da Camada de Aplicação   
Os protocolos da camada de aplicação definem formatos e controles necessários para as comunicações mais comuns da Internet. Eles operam simultaneamente nos dispositivos de origem e destino durante uma sessão, exigindo compatibilidade entre as implementações para que a troca de dados funcione corretamente.

🖥️ Modelo Cliente-Servidor   
No modelo cliente-servidor, um dispositivo atua solicitando dados, enquanto outro responde fornecendo as informações requisitadas. A comunicação sempre começa pelo cliente, que inicia a troca, e o servidor retorna os dados conforme solicitado, caracterizando uma relação bem definida entre quem consome e quem oferece o serviço.

🤝 Modelo P2P   
Em redes ponto a ponto, os dispositivos compartilham recursos diretamente entre si, sem a necessidade de um servidor dedicado. Cada computador pode assumir, ao mesmo tempo, o papel de cliente em uma comunicação e de servidor em outra, tornando a arquitetura mais distribuída.

🔗 Funcionamento das Aplicações P2P   
Aplicações P2P exigem que cada dispositivo tenha interface de usuário e serviços em segundo plano. Algumas utilizam um modelo híbrido, no qual o compartilhamento é descentralizado, mas a localização dos recursos é controlada por servidores centrais. O uso de arquivos torrent permite localizar usuários que possuem partes específicas de arquivos, viabilizando a troca direta entre pares.

🌐 Protocolo HTTP e HTTPS   
Ao acessar um endereço web, o navegador se conecta a um servidor que utiliza HTTP, baseado em um modelo de requisição e resposta. Esse protocolo define os tipos de mensagens usados na comunicação, como GET, POST e PUT. Para conexões seguras, o HTTPS utiliza o mesmo processo, mas com os dados criptografados antes da transmissão.

📧 Protocolos de E-mail   
O funcionamento do e-mail depende de três protocolos distintos. O SMTP é responsável pelo envio das mensagens, enquanto POP e IMAP são usados para a recuperação. As mensagens exigem cabeçalho e corpo bem definidos. No POP, os e-mails são transferidos e removidos do servidor, enquanto no IMAP as mensagens permanecem armazenadas até serem excluídas manualmente.

📛 Sistema de Nomes de Domínio   
O DNS associa nomes de domínio a endereços IP numéricos, permitindo localizar recursos na rede. Ele utiliza um formato padronizado de mensagens para consultas, respostas, erros e transferências entre servidores. A estrutura hierárquica distribui a responsabilidade entre servidores, e ferramentas como o nslookup permitem consultas manuais.

📡 Serviço DHCP   
O DHCP automatiza a configuração de parâmetros de rede em dispositivos IPv4, como endereço IP e gateway. No IPv6, o DHCPv6 oferece funções semelhantes, com diferenças específicas. O processo envolve mensagens trocadas entre cliente e servidor para descoberta, oferta e concessão de configurações, facilitando a integração automática à rede.

📂 Protocolo FTP   
O FTP permite a transferência de arquivos entre cliente e servidor por meio de duas conexões distintas. Uma conexão é usada para controle, estabelecida na porta TCP 21, e outra para a transferência efetiva de dados, utilizando a porta TCP 20. Esse mecanismo possibilita tanto download quanto upload de arquivos.

🗄️ Protocolo SMB   
O SMB oferece recursos para iniciar e encerrar sessões, autenticar usuários e controlar o acesso a arquivos e impressoras. Diferente do FTP, ele mantém conexões de longa duração, permitindo que os recursos remotos sejam acessados como se estivessem localmente disponíveis no dispositivo do cliente.
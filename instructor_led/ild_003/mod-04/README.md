# Fundamentos de Redes - Módulo 4   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_003 (Fundamentos de Redes)   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="25"></a>
### Module: 4. Construindo uma Rede Doméstica

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

### Course Module 4 Structure:
4. <a name="item04">Construindo uma Rede Doméstica</a><br>
  4.1 <a href="#item04.01">Introdução</a><br>
  4.2 <a href="#item04.02">Conceitos básicos da rede doméstica</a><br>
  4.3 <a href="#item04.03">Tecnologias de rede na residência</a><br>
  4.4 <a href="#item04.04">Padrões de Redes Sem Fio</a><br>
  4.5 <a href="#item04.05">Configurar um roteador doméstico</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;4.5.1 <a href="../../../pkt/files/pkt_053/">Packet Tracer - Configurar um Roteador sem fio e um cliente</a><br>
  4.6 <a href="#item04.06">Resumo Construindo uma Rede Doméstica</a><br>
  4.7 Exame de ponto de verificação: Construir uma pequena rede<br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item04.01"><h4>4.1 Introdução</h4></a>[Back to summary](#item04)

🏠 Infraestrutura de Redes Residenciais e Segurança   
A rede doméstica atua como o ponto de convergência para múltiplos dispositivos, utilizando roteadores integrados para intermediar a comunicação entre a rede local e a internet. A correta administração desses equipamentos envolve o conhecimento de suas interfaces físicas e lógicas, além da implementação de protocolos de segurança essenciais para proteger a integridade dos dados e o acesso à infraestrutura sem fio.

🎯 Objetivo do módulo:   
- Configurar um roteador sem fio integrado e terminais clientes para estabelecer uma conectividade segura à rede mundial de computadores.

📘 Tópicos do módulo:   
- Conceitos básicos da rede doméstica: Identificação dos elementos fundamentais para a estruturação de uma rede de dados em ambiente residencial.
- Tecnologias de rede na residência: Diferenciação entre os meios de transmissão cabeados e as tecnologias de propagação de sinal por radiofrequência.
- Padrões de Redes Sem Fio: Especificação técnica dos protocolos Wi-Fi e suas normas de operação no espectro sem fio.
- Configurar um roteador doméstico: Implementação de parâmetros de gestão e medidas de segurança para a proteção das comunicações wireless.

<a name="item04.02"><h4>4.2 Conceitos básicos da rede doméstica</h4></a>[Back to summary](#item04)

🏠 Ecossistema de Conectividade Doméstica   
A infraestrutura de rede residencial evoluiu para suportar uma gama diversificada de dispositivos que transcendem os computadores tradicionais. Nota-se que sistemas de entretenimento, consoles de jogos, televisores inteligentes, periféricos de impressão e digitalização, além de dispositivos de segurança e automação climática, dependem de uma conexão estável para o funcionamento pleno. A tendência tecnológica aponta para uma integração cada vez maior das funções domiciliares ao ambiente de rede, onde o controle centralizado torna-se a norma para a gestão do lar.

📶 Estrutura da Rede Local Sem Fio (WLAN)   
O núcleo de uma rede sem fio doméstica é composto por elementos que permitem a comunicação interna e o acesso externo. O Provedor de Serviços de Internet (ISP) fornece o link de acesso, enquanto o roteador atua como o ponto central de coordenação. Este arranjo permite que smartphones, laptops e outros terminais inteligentes operem de forma integrada sob uma mesma arquitetura de conectividade local.

🔌 Interfaces e Conexões Físicas   
Os roteadores destinados ao uso residencial e em pequenos escritórios possuem interfaces físicas distintas, projetadas para gerenciar o tráfego de dados em diferentes níveis:
- Portas Ethernet (LAN): Estas interfaces estão vinculadas ao switch interno do equipamento. Todos os dispositivos conectados a essas portas integram a mesma rede local, permitindo a troca de informações entre os equipamentos internos de forma direta e protegida.
- Porta de Internet (WAN): Esta conexão é destinada à interligação do roteador com uma rede externa. Geralmente, é utilizada para conectar o equipamento ao modem (DSL ou cabo), estabelecendo a ponte necessária para o acesso à rede mundial. Diferente das portas Ethernet, esta interface opera em um segmento de rede logicamente isolado.

📡 Integração Sem Fio e Lógica de Rede   
A maioria dos roteadores contemporâneos incorpora antenas e pontos de acesso sem fio integrados à sua estrutura. Na configuração padrão de fábrica, nota-se que os terminais conectados via rede sem fio compartilham o mesmo segmento lógico e as mesmas permissões dos dispositivos cabeados nas portas LAN. Dessa forma, em uma configuração típica, a única interface que permanece em uma rede distinta é a porta de Internet, que atua como o gateway para o tráfego externo.

<a name="item04.03"><h4>4.3 Tecnologias de rede na residência</h4></a>[Back to summary](#item04)

📶 Tecnologias Sem Fio e Frequências   
As comunicações sem fio em ambientes residenciais operam predominantemente em faixas de frequências não licenciadas de 2,4 GHz e 5 GHz. O Bluetooth utiliza a banda de 2,4 GHz para estabelecer conexões de curto alcance e baixa velocidade. Nota-se a eficiência desta tecnologia no pareamento simultâneo de múltiplos periféricos, sendo o padrão adotado para a integração de mouses, teclados, impressoras e sistemas de áudio.

🌐 Padrões IEEE 802.11   
As infraestruturas de rede local sem fio operam sob os padrões IEEE 802.11 em faixas de frequência não licenciadas, abrangendo tanto os 2,4 GHz quanto os 5 GHz. Em contraste com protocolos de curto alcance como o Bluetooth, o emprego de potências de transmissão superiores nestas redes garante um alcance geográfico mais vasto e uma capacidade de fluxo de dados (throughput) elevada. Nota-se que a utilização da banda de 5 GHz possibilita atingir taxas de transferência ainda maiores e mitigar interferências eletromagnéticas de outros dispositivos, embora apresente uma redução na eficiência ao transpor barreiras físicas.

🔌 Protocolo Ethernet e Conectividade Cabeada   
O protocolo Ethernet é a tecnologia mais difundida para a implementação de redes locais cabeadas (LAN). Diferente do meio compartilhado das redes sem fio, as conexões cabeadas via switch proporcionam canais dedicados para a troca de informações. A interconexão física entre os dispositivos é realizada majoritariamente através de cabos de par trançado não blindado (UTP) com conectores padronizados RJ-45.

🧶 Tipos de Meios Físicos   
A infraestrutura de cabeamento pode variar de acordo com a necessidade de desempenho e a distância da transmissão:
- Cabo Categoria 5e: Representa o padrão mais comum em redes locais, sendo composto por quatro pares de fios de cobre trançados para minimizar interferências elétricas externas.
- Cabo Coaxial: Formado por um condutor interno central protegido por uma camada isolante e uma blindagem metálica tubular. Este design assegura a integridade do sinal contra ruídos eletromagnéticos.
- Cabo de Fibra Óptica: Constituído por filamentos de vidro ou plástico da espessura de um fio de cabelo. Utiliza pulsos de luz para transportar informações digitais em altíssima velocidade por longas distâncias, oferecendo a maior largura de banda entre os meios físicos disponíveis.

💡 Alternativas de Distribuição   
Em cenários onde o cabeamento UTP não está presente nas paredes, existem tecnologias alternativas para a distribuição do sinal. É possível utilizar a própria fiação da rede elétrica residencial para estender a conectividade cabeada entre diferentes cômodos, garantindo a estabilidade da rede sem a necessidade de reformas estruturais.

<a name="item04.04"><h4>4.4 Padrões de Redes Sem Fio</h4></a>[Back to summary](#item04)

📡 Padrões e Certificações Sem Fio   
A regulamentação técnica para a comunicação entre dispositivos sem fio é estabelecida pelo Instituto de Engenheiros Eletricistas e Eletrônicos (IEEE). O padrão fundamental para redes locais sem fio é o IEEE 802.11, que define o uso do espectro de radiofrequência nas bandas de 2,4 GHz e 5 GHz. O conjunto dessas tecnologias é comercialmente identificado como Wi-Fi.

Para garantir que equipamentos de diferentes fabricantes funcionem de maneira integrada, a organização Wi-Fi Alliance realiza testes de interoperabilidade. A presença do logotipo Wi-Fi em um produto certifica que o dispositivo cumpre os requisitos técnicos necessários para operar com outros equipamentos que adotam o mesmo padrão.

🛠️ Parâmetros de Configuração de WLAN   
O gerenciamento de um roteador sem fio exige o ajuste de variáveis específicas para assegurar a conectividade e o desempenho da rede:
- Modo de Rede: Define os padrões de tecnologia suportados pelo ponto de acesso, podendo ser configurado para versões específicas (como 802.11n ou 802.11ac) ou em Modo Misto (Mixed Mode), que permite a conexão de dispositivos novos e antigos simultaneamente.
- Nome da Rede (SSID): O Identificador de Conjunto de Serviços é o nome alfanumérico que distingue uma rede sem fio de outra. É sensível a letras maiúsculas e minúsculas e possui um limite de 32 caracteres.
- Canal Padrão: Determina a frequência exata da comunicação para evitar interferências. A configuração automática permite que o roteador selecione o canal com menor ruído no ambiente.
- Broadcast de SSID: Refere-se à transmissão pública do nome da rede. Quando ativado, os dispositivos detectam a rede automaticamente; quando desativado, o nome deve ser inserido manualmente em cada estação sem fio.

🚀 Desempenho e Compatibilidade   
A eficiência de uma rede sem fio está diretamente relacionada à uniformidade dos padrões utilizados pelos dispositivos conectados. A velocidade máxima de transmissão é alcançada quando todos os terminais operam sob a mesma versão do protocolo 802.11. Em infraestruturas que utilizam o Modo Misto, a rede garante compatibilidade para equipamentos legados, embora isso possa resultar em uma redução na taxa de transferência global para acomodar tecnologias menos eficientes.

🔐 Identidade e Segurança de Rede   
O SSID atua como um cabeçalho presente em todos os quadros de dados enviados pela rede, informando aos dispositivos a qual estrutura pertencem. Embora a ocultação do SSID (desativação do broadcast) dificulte a identificação imediata da rede por usuários comuns, essa medida não é considerada uma proteção robusta contra acessos não autorizados.

Nota-se que a segurança efetiva de uma rede sem fio depende da implementação de protocolos de criptografia fortes. A restrição de acesso deve ser garantida por métodos de autenticação robustos, independentemente de o nome da rede estar visível ou oculto para os clientes sem fio.

<a name="item04.05"><h4>4.5 Configurar um roteador doméstico</h4></a>[Back to summary](#item04)

⚙️ Configuração Inicial do Roteador   
A realização dos ajustes básicos em um roteador residencial geralmente ocorre por meio de utilitários de configuração automática ou interfaces web. Para esse procedimento, é necessária a conexão física de um computador a uma das portas LAN do equipamento via cabo Ethernet. Deve-se evitar a utilização da porta identificada como "Internet" ou "WAN" para esta finalidade, uma vez que esta interface é destinada exclusivamente à recepção do sinal proveniente do modem DSL ou de cabo.

🌐 Endereçamento e Conectividade Lógica   
Após a interconexão física, o host precisa de um endereçamento IP para estabelecer comunicação com o utilitário de gerenciamento. Na maioria das configurações de fábrica, os roteadores operam com o protocolo DHCP ativo, fornecendo automaticamente o endereço IP, a máscara de sub-rede, o gateway padrão e os dados de DNS ao computador conectado. Caso a atribuição automática não ocorra, torna-se obrigatória a configuração manual desses parâmetros com base nas especificações técnicas do fabricante.

🛡️ Planejamento e Segurança do SSID   
A escolha do nome da rede, ou SSID, é um fator determinante para a segurança da infraestrutura. Recomenda-se que o identificador não contenha informações que revelem a marca ou o modelo do dispositivo, pois tais dados facilitam a busca por vulnerabilidades específicas e pontos fracos conhecidos na internet. Quando o broadcast de SSID está ativo, qualquer terminal sem fio dentro do raio de alcance poderá identificar a presença da rede.

📶 Compatibilidade de Padrões e Modos de Operação   
A eficiência da transmissão de dados depende da compatibilidade entre os rádios dos dispositivos clientes e os padrões suportados pelo roteador (como 802.11b/g/n/ac). Para atingir a performance máxima, é ideal que todos os equipamentos utilizem a mesma norma técnica. No entanto, em ambientes com hardwares heterogêneos, é necessário habilitar o "modo legado" ou "modo misto", garantindo que dispositivos baseados em tecnologias anteriores consigam estabelecer conexão, ainda que isso possa limitar a velocidade global da rede.

👥 Gerenciamento de Acessos e Convidados   
O controle de novos dispositivos pode ser segmentado para proteger a integridade dos dados locais. Muitos roteadores permitem a criação de um acesso para convidados, que consiste em um SSID secundário com acesso restrito apenas à internet. Essa configuração isola o tráfego de visitantes, impedindo a visualização ou interação com os recursos e arquivos da rede doméstica principal.

<a name="item04.06"><h4>4.6 Resumo Construindo uma Rede Doméstica</h4></a>[Back to summary](#item04)

🏠 Estrutura da Rede Doméstica   
Uma rede residencial típica atua como uma ponte entre a infraestrutura pública do provedor e os dispositivos privados do usuário. O roteador centraliza essa comunicação, funcionando como uma pequena LAN (Rede Local) que integra conexões cabeadas e sem fio, permitindo que diversos aparelhos, de consoles de games a sistemas de climatização, troquem informações entre si e acessem a internet de forma simultânea.

📡 Vantagens e Espectro Sem Fio   
A tecnologia Wi-Fi utiliza ondas eletromagnéticas em frequências específicas para transmitir dados sem a necessidade de cabos físicos, oferecendo alta mobilidade e facilidade de instalação. Enquanto algumas partes do espectro são restritas ou licenciadas para rádio e TV, o Wi-Fi opera em faixas livres, como 2,4 GHz e 5 GHz, permitindo que fabricantes criem dispositivos compatíveis globalmente para uso doméstico.

🔌 Conexões Ethernet e Cabeamento   
Apesar da conveniência do sinal sem fio, conexões cabeadas ainda são preferidas para aplicações que exigem estabilidade e alta velocidade. O padrão Ethernet utiliza cabos de par trançado, como o Cat 5e, que possui fios entrelaçados para minimizar interferências elétricas. Em locais onde não há tubulação para cabos, tecnologias como Powerline permitem distribuir o sinal de rede através da própria fiação elétrica da casa.

🌐 Padrões e Certificação Wi-Fi   
O protocolo IEEE 802.11 é o conjunto de regras técnicas que define como as redes locais sem fio devem funcionar. A conformidade com esses padrões é testada pela Wi-Fi Alliance, garantindo que aparelhos de diferentes marcas consigam se comunicar. Dependendo da versão do padrão utilizada, como 802.11n ou 802.11ac, a rede pode oferecer maior alcance ou maior taxa de transferência de dados.

⚙️ Configurações Básicas do Roteador   
Para que uma rede sem fio funcione corretamente, é necessário ajustar parâmetros como o SSID, que é o nome identificador da rede, e o canal de transmissão. O roteador pode operar em modo misto para aceitar dispositivos de tecnologias antigas e novas, ou ser configurado para ocultar o broadcast do SSID, exigindo que o usuário insira o nome da rede manualmente para aumentar a privacidade.

🔑 Identificação e Acesso SSID   
O SSID funciona como a identidade da rede, orientando os dispositivos sobre onde se conectar. Embora a transmissão automática do nome facilite a descoberta da rede, as boas práticas de segurança recomendam evitar nomes que revelem a marca ou modelo do roteador, pois isso pode facilitar a exploração de vulnerabilidades conhecidas por invasores externos.

💻 Conectividade e Endereçamento IP   
Ao conectar um computador ao roteador, seja por cabo ou Wi-Fi, o dispositivo precisa de uma identidade lógica para navegar. Geralmente, os roteadores domésticos possuem um servidor DHCP integrado, que atribui automaticamente um endereço IP ao computador assim que a placa de rede detecta o link ativo, eliminando a necessidade de configuração manual por parte do usuário.

🛡️ Segurança e Controle de Acesso   
Existem métodos para restringir quem pode utilizar a conexão doméstica, como a filtragem de endereços MAC, que autoriza apenas hardwares específicos previamente cadastrados. Outra opção comum é a criação de redes para convidados, que disponibiliza um acesso isolado à internet para visitantes, mantendo os arquivos e dispositivos principais da casa protegidos em uma rede separada.
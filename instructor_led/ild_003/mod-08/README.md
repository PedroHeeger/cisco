# Fundamentos de Redes - Módulo 8   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_003 (Fundamentos de Redes)   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="25"></a>
### Module: 8. Protocolo de Internet (Internet Protocol - IP)

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

### Course Module 8 Structure:
8. <a name="item08">Protocolo de Internet (Internet Protocol - IP)</a><br>
  8.1 <a href="#item08.01">Introdução</a><br>
  8.2 <a href="#item08.02">Finalidade de um endereço IPv4</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;8.2.1 <a href="../../../pkt/files/pkt_???/">Packet Tracer – Conexão com um servidor da Web</a><br>
  8.3 <a href="#item08.03">A estrutura do endereço IPv4</a><br>
  8.4 <a href="#item08.04">Resumo Protocolo IP</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item08.01"><h4>8.1 Introdução</h4></a>[Back to summary](#item08)

🌐 Endereçamento e Protocolo IPv4   
O endereçamento lógico é um componente fundamental para a localização e identificação de dispositivos em uma rede global. Assim como os sistemas postais utilizam códigos específicos para o encaminhamento de correspondências, o protocolo IP (Internet Protocol) atribui identificadores exclusivos aos hosts, permitindo que os roteadores determinem o trajeto de origem e destino dos pacotes de dados. Esse sistema garante que a informação seja entregue com precisão ao destinatário correto dentro de uma infraestrutura complexa.

🎯 Objetivo do módulo:   
- Explicar as características, a função e a organização técnica do endereçamento IPv4 nas comunicações de rede.

📘 Tópicos do módulo: 
- Finalidade de um endereço IPv4: Descrição da importância do identificador lógico para a conectividade global e a entrega de pacotes na Internet.
- A estrutura do endereço IPv4: Análise da composição binária e decimal dos endereços, incluindo a interação entre identificadores de rede e máscaras de sub-rede.

<a name="item08.02"><h4>8.2 Finalidade de um endereço IPv4</h4></a>[Back to summary](#item08)

🌐 Endereçamento IPv4 e Conectividade   
O endereço IPv4 funciona como uma identificação lógica essencial para que um host acesse a rede mundial. Para garantir a troca de informações, essa identificação deve ser configurada de forma exclusiva tanto no âmbito da rede local (LAN) quanto na infraestrutura global. Essa exclusividade permite que um dispositivo localize outros equipamentos e seja localizado por eles na internet.

🔌 Atribuição de Endereços em Interfaces   
A vinculação de um endereço IPv4 ocorre diretamente na interface de rede do equipamento, geralmente por meio de uma placa NIC. Dispositivos finais, incluindo computadores, servidores, impressoras e terminais de voz sobre IP (VoIP), utilizam essas interfaces para a conexão. Nota-se que equipamentos de infraestrutura, como roteadores, e servidores dotados de múltiplas placas de rede, possuem endereçamentos individuais para cada interface ativa.

📦 Fluxo de Dados e Endereçamento de Pacotes   
Cada unidade de informação transmitida pela internet contém obrigatoriamente os endereços IPv4 de origem e de destino. Esses dados são fundamentais para que os ativos de rede encaminhem o pacote corretamente ao receptor e permitam que este envie uma resposta ao remetente original.

🔢 Estrutura Binária e Representação Decimal   
Tecnicamente, um endereço IPv4 é composto por uma sequência de 32 bits. Devido à complexidade de leitura e configuração de longas cadeias binárias, esses bits são segmentados em quatro grupos de 8 bits, denominados octetos.

Para facilitar a manipulação humana, cada octeto é convertido em seu valor correspondente no sistema decimal, resultando no formato conhecido como "notação decimal pontuada". Por exemplo, uma sequência binária extensa é traduzida em quatro números decimais separados por pontos (como 209.165.200.1), tornando a gestão de rede mais eficiente e menos propensa a erros manuais de configuração.

<a name="item08.03"><h4>8.3 A estrutura do endereço IPv4</h4></a>[Back to summary](#item08)

🌐 Estrutura Hierárquica do Endereçamento IPv4   
O endereçamento lógico IPv4 é organizado de forma hierárquica, sendo composto obrigatoriamente por duas divisões fundamentais: a identificação da rede e a identificação do host. Para realizar a distinção entre esses dois segmentos dentro de um endereço, utiliza-se a máscara de sub-rede. Este componente técnico é indispensável para que o sistema reconheça a qual agrupamento de rede um determinado equipamento está vinculado.

📍 Funcionamento da Máscara de Sub-rede   
Ao analisar um endereço como o 192.168.5.11 sob a máscara 255.255.255.0, nota-se que os três primeiros octetos definem a porção de rede, enquanto o último valor identifica o dispositivo específico. Essa organização hierárquica otimiza o tráfego de dados global, uma vez que os roteadores precisam processar apenas as rotas para as redes de destino, sem a necessidade de mapear a localização individual de cada host conectado à internet.

📂 Segmentação Lógica em Infraestrutura Física   
A arquitetura IPv4 permite a coexistência de múltiplas redes lógicas operando sobre uma única plataforma física. Se diferentes grupos de dispositivos possuírem identificadores de rede distintos, a comunicação mútua entre eles é impedida nativamente. Para que a troca de dados ocorra entre esses domínios isolados, torna-se obrigatória a intervenção de um processo de roteamento, mesmo que os aparelhos compartilhem o mesmo meio de conexão cabeada ou sem fio.

📞 Analogia com o Sistema Telefônico   
O conceito de endereçamento hierárquico pode ser comparado à estrutura dos números de telefone. Nesse modelo, os códigos de país e de área, juntamente com o prefixo da central telefônica, desempenham o papel do endereço de rede, encaminhando a chamada para a região correta. Os dígitos finais correspondem ao número do terminal local, servindo como a identificação final do host dentro daquela infraestrutura específica.

<a name="item08.04"><h4>8.4 Resumo Protocolo IP</h4></a>[Back to summary](#item08)

📌 Endereçamento Lógico IPv4   
O endereço IPv4 funciona como uma identidade digital exclusiva que permite localizar um dispositivo dentro de uma rede. Para que a comunicação ocorra sem falhas, essa numeração deve ser única tanto no ambiente local (LAN) quanto no cenário global, garantindo que as informações transitem entre redes distintas e alcancem o destinatário correto em qualquer lugar do mundo.

🔌 Interface de Conexão   
A atribuição de um endereço IP não é feita ao hardware do computador como um todo, mas especificamente à sua interface de comunicação, conhecida como placa de rede (NIC). É através desse ponto de conexão que o dispositivo se torna visível para os demais nós da rede, permitindo o fluxo de entrada e saída de pacotes de dados.

✉️ Fluxo de Origem e Destino   
Todo conjunto de dados que trafega pela rede deve carregar consigo as etiquetas de identificação de quem enviou e de quem deve receber a mensagem. Essa sinalização é indispensável para que os roteadores e switches encaminhem os pacotes pelo caminho correto e para que o dispositivo de destino saiba para onde enviar uma resposta ou confirmação.

🧱 Hierarquia do Endereço   
O IPv4 é composto por 32 bits divididos em duas seções fundamentais: a identificação da rede e a identificação do host. Em um exemplo clássico, os primeiros blocos numéricos definem a "vizinhança" ou sub-rede onde o dispositivo reside, enquanto o segmento final diferencia o aparelho específico dentro desse grupo, facilitando a organização lógica do sistema.

🛣️ Roteamento e Redes Lógicas   
Graças à estrutura hierárquica, os roteadores não precisam memorizar a localização de cada computador individualmente, mas apenas o caminho para as redes principais. Essa característica permite que múltiplas redes lógicas coexistam dentro de uma mesma infraestrutura física, desde que possuam identificadores de rede distintos, otimizando o gerenciamento do tráfego global.
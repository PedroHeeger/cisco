# CCNA: Introduction to Networks - Módulo 7   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_001 (CCNA: Introduction to Networks)   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="25"></a>
### Module: 7. Switching Ethernet

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

### Course Module 7 Structure:
7. <a name="item07">Switching Ethernet</a><br>
  7.1 <a href="#item07.01">Introdução</a><br>
  7.2 <a href="#item07.02">Quadros Ethernet</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;7.2.1 <a href="../../../labs/files/lab_023/">Laboratório - Use o Wireshark para examinar os quadros Ethernet</a><br>
  7.3 <a href="#item07.03">Endereços MAC Ethernet</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;7.3.1 <a href="../../../pkt/files/pkt_021/">Laboratório - Exibir Endereços MAC do dispositivo de rede</a><br>
  7.4 <a href="#item07.04">A Tabela de Endereços MAC</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;7.4.1 <a href="#item07.04.01">Atividade - Encaminhe-o!</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;7.4.2 <a href="../../../pkt/files/pkt_022/">Laboratório - Exibir a tabela de endereços MAC do switch</a><br>
  7.5 <a href="#item07.05">Métodos de encaminhamento e velocidade de switches</a><br>
  7.6 <a href="#item07.06">Módulo Prático e Quiz</a><br>
  7.7 <a href="#item07.07">Exame de Comunicação e Conectividade de Rede Básica</a><br>

---

### Objective:
O objetivo deste módulo foi apresentar os fundamentos da governança em segurança digital, destacando políticas, papéis e responsabilidades na administração de dados. Também foram exploradas as principais leis, regulamentações e normas internacionais aplicáveis à proteção da informação. Além disso, foram abordados os princípios éticos na tomada de decisões em ambientes digitais e introduzidos frameworks e controles essenciais, como ISO 27000, NIST, CIS e CSA, para garantir conformidade, proteção de dados e integridade operacional em organizações.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item07.01"><h4>7.1 Introdução</h4></a>[Back to summary](#item07)

📘 Introdução   
Este módulo aborda os princípios do switching Ethernet, uma das tecnologias de LAN mais amplamente utilizadas no cenário atual. A combinação entre alta capacidade de transmissão e escalabilidade faz da Ethernet a base de grande parte das redes modernas. A análise de quadros, a observação de endereços MAC e o estudo do comportamento dos switches são elementos essenciais para compreender como as informações são encaminhadas dentro de uma rede comutada. Atividades práticas e recursos visuais complementam o conteúdo para facilitar a interpretação das operações realizadas na Camada 2.

🎯 Objetivo Geral   
Apresentar o funcionamento da Ethernet em redes comutadas, destacando como quadros são estruturados, identificados e encaminhados por dispositivos de switching.

✅ Objetivos Específicos   
- Explicar a relação entre as subcamadas da Ethernet e os campos presentes no quadro Ethernet.
- Descrever a função e a estrutura dos endereços MAC.
- Demonstrar como um switch aprende e armazena endereços MAC em sua tabela de encaminhamento.
- Identificar métodos de encaminhamento utilizados por switches e as configurações de porta disponíveis na Camada 2.

<a name="item07.02"><h4>7.2 Quadros Ethernet</h4></a>[Back to summary](#item07)

🧩 Tecnologia Ethernet: Visão Geral   
A Ethernet é uma das bases das redes locais com fio. Ela combina padrões de Camada 1 e Camada 2 para garantir que os dados viajem da NIC de um dispositivo até a NIC de outro dentro da mesma LAN. Assim como as WLANs fazem isso sem fio, a Ethernet faz pela mídia física — cabos, fibras e até coaxial — mantendo funcionamento previsível, rápido e padronizado.

⚙️ Subcamadas da Ethernet   
No padrão IEEE, a Camada de Enlace é dividida em duas partes. Isso permite separar aquilo que lida com o hardware daquilo que conversa com os protocolos superiores.

🧠 LLC (Logical Link Control)   
A subcamada LLC atua como ponte entre as aplicações e os componentes de hardware. Ela identifica qual protocolo da Camada 3 está encapsulado no quadro, permitindo que IPv4, IPv6 e outros coexistam usando a mesma interface física.

🛠️ MAC (Media Access Control)   
Já a subcamada MAC cuida do trabalho físico: encapsular dados, inserir endereços MAC, detectar erros e determinar como os dispositivos acessam a mídia. Tudo isso é implementado diretamente no hardware, como switches e NICs.

📦 Encapsulamento na Ethernet   
A MAC organiza o quadro Ethernet para que ele possa ser transmitido pela mídia física. Três funções se destacam:
- Montagem do quadro: adiciona cabeçalho, dados e trailer.
- Endereçamento: insere MAC de origem e destino.
- Detecção de erros: usa o FCS para verificar se os bits chegaram intactos.

Essa estrutura garante que os dispositivos da LAN reconheçam o quadro e saibam se ele deve ser aceito, descartado ou repassado.

🔗 Acesso ao Meio   
Antigamente, Ethernet funcionava em meio compartilhado e half-duplex, usando o método CSMA/CD, que detectava colisões e definia quando os dispositivos poderiam transmitir. Hoje, com switches operando em full-duplex, não há competição direta pelo meio. Cada porta do switch forma um enlace exclusivo, eliminando colisões e aumentando eficiência.

📏 Tamanho dos Quadros Ethernet   
A Ethernet define limites claros:
- 64 bytes: tamanho mínimo de um quadro.
- 1518 bytes: tamanho máximo padrão.
- Acima de 1500 bytes nos dados: quadros “jumbo”, comuns em redes modernas de alta performance.
- Quadros menores que 64 bytes são inválidos e descartados.

O preâmbulo não entra na contagem do tamanho.

🧱 Estrutura do Quadro Ethernet   
Os campos principais são:
- Preâmbulo + SFD (8 bytes): Serve para sincronizar remetente e receptor. São os “toques na porta” que avisam: prepare-se, quadro chegando.
- Endereço MAC de Destino (6 bytes): Indica o destinatário desejado. Pode ser unicast, multicast ou broadcast.
- Endereço MAC de Origem (6 bytes): Identifica quem enviou o quadro.
- Tipo/Comprimento (2 bytes): Mostra o tipo de protocolo encapsulado. Exemplos (hexadecimal):
  - IPv4: 0x0800;
  - IPv6: 0x86DD;
  - ARP: 0x0806.
- Campo de Dados (46–1500 bytes): Transporta o pacote da Camada 3. Caso o pacote seja pequeno demais, bits de padding completam o tamanho mínimo do quadro.
- FCS – Frame Check Sequence (4 bytes): Responsável por conferir se o quadro chegou íntegro. Ele utiliza CRC:
  - remetente calcula o CRC e coloca no FCS;
  - receptor recalcula;
  - se os valores diferirem, o quadro é descartado.

<a name="item07.03"><h4>7.3 Endereços MAC Ethernet</h4></a>[Back to summary](#item07)

🧮 Sistemas de Numeração e Endereços MAC   
A comunicação em rede depende de diferentes sistemas de numeração. Endereços IPv4 usam decimal e binário, enquanto endereços IPv6 e endereços Ethernet usam hexadecimal. O hexadecimal funciona com 16 símbolos (0–9 e A–F) e é muito eficiente porque cada dígito hex equivale a quatro bits binários. Como um endereço MAC tem 48 bits, ele pode ser representado com apenas 12 dígitos hexadecimais. Por isso, hexadecimal é a forma padrão de escrever endereços de camada 2.

🔢 Hexadecimal, Binário e Conversão   
O byte (8 bits) é o agrupamento fundamental. Binários de 00000000 a 11111111 correspondem ao intervalo hexadecimal 00 a FF. Zeros à esquerda sempre aparecem para completar o byte. Valores hexadecimais podem ser escritos com prefixo 0x (como 0x73) ou com sufixo H (73H). Se for preciso converter entre decimal e hexadecimal, o método ideal é sempre passar pelo binário: converte-se para binário e depois para o formato desejado.

🖧 Função do Endereço MAC na Ethernet   
Em uma LAN Ethernet, todos os dispositivos compartilham o mesmo meio físico. O endereço MAC identifica as NICs de origem e destino na rede local, operando na camada de enlace. Por possuir 48 bits (6 bytes), ele é sempre escrito como 12 dígitos hexadecimais. Esse endereço precisa ser único em cada interface Ethernet.

🏢 OUI e Montagem do Endereço MAC   
Para garantir unicidade, cada fabricante registra um bloco exclusivo de 24 bits no IEEE chamado OUI (Organizationally Unique Identifier). Esse OUI compõe os primeiros 6 dígitos hexadecimais do MAC. Os 6 dígitos finais são atribuídos pelo próprio fabricante. Se a Cisco tem o OUI 00-60-2F, ela pode completar com um identificador próprio, como 3A-07-BC, resultando em um endereço MAC final 00-60-2F-3A-07-BC. Embora o fabricante deva evitar duplicações, colisões de MAC podem ocorrer por erro de produção ou por mudanças de software, especialmente em máquinas virtuais.

🔥 BIA — Burned-In Address   
O endereço MAC tradicionalmente é gravado na ROM da NIC, por isso é chamado de BIA (Burned-In Address). Porém, sistemas modernos permitem alterar esse endereço via software. Isso pode ser útil para contornar filtros de rede baseados em MAC, razão pela qual esse tipo de filtragem hoje é considerado pouco seguro.

📤 Uso do MAC no Encaminhamento de Quadros   
Quando o computador inicializa, a NIC copia o endereço MAC da ROM para a RAM. Ao enviar um quadro Ethernet, o dispositivo insere o seu próprio MAC como origem e o MAC da NIC remota como destino. Quando um quadro chega a uma NIC, ela verifica se o endereço MAC de destino coincide com o seu próprio. Se não coincidir, descarta. Se for unicast destinado a ela, aceita e entrega às camadas superiores. As NICs também aceitam quadros broadcast e multicast quando fazem parte desses grupos.

🎯 Quadro Unicast   
Um endereço MAC unicast identifica um único receptor. Para enviar dados a um host específico, o endereço IP unicast e o endereço MAC unicast precisam aparecer nos respectivos cabeçalhos. Para IPv4, o host descobre o MAC do destinatário usando ARP; para IPv6, usa ND (Neighbour Discovery). Vale lembrar que o MAC de origem é sempre unicast, pois representa um único remetente.

📡 Quadro Broadcast   
O broadcast Ethernet possui endereço de destino FF-FF-FF-FF-FF-FF, que representa 48 bits em 1. Ele é enviado para todas as portas do switch, exceto a de origem, e não atravessa roteadores. Se o pacote encapsulado também for broadcast IPv4, o endereço IP destino terá todos os bits de host em 1, como 192.168.1.255. Protocolos como DHCP e ARP utilizam quadros broadcast na LAN.

👥 Quadros Multicast   
Um quadro multicast é recebido apenas por dispositivos que participam de um grupo de multicast. Para isso, a Ethernet usa endereços MAC especiais: Para IPv4, os endereços começam por 01-00-5E; para IPv6, por 33-33. Assim como no broadcast, o switch inunda as portas — a menos que esteja configurado com técnicas como IGMP Snooping (espionagem multicast). Roteadores só encaminham multicast se estiverem configurados para isso. O endereço IP multicast é sempre destino, nunca origem. O intervalo IPv4 é 224.0.0.0 a 239.255.255.255; para IPv6, começa com ff00::/8. Para entregar quadros na LAN, o endereço IP multicast precisa ser traduzido para o MAC multicast correspondente.

<a name="item07.04"><h4>7.4 A Tabela de Endereços MAC</h4></a>[Back to summary](#item07)

🖧 Encaminhamento de Quadros por Switches Ethernet   
Depois de entender os endereços MAC, é hora de ver como um switch Ethernet usa essas informações para enviar quadros entre dispositivos em uma rede. Se um switch apenas repetisse cada quadro para todas as portas, a rede ficaria congestionada e poderia até parar. Por isso, os switches tomam decisões inteligentes de encaminhamento com base nos endereços MAC da camada 2.

🎯 Função do Switch   
Um switch de camada 2 não examina os dados do quadro, como pacotes IPv4, mensagens ARP ou pacotes ND IPv6. Ele decide para onde enviar cada quadro usando apenas os endereços MAC de origem e destino. Diferente de hubs herdados, que replicam os bits para todas as portas exceto a de entrada, o switch consulta sua tabela de endereços MAC antes de encaminhar qualquer quadro. A tabela de endereços MAC também é conhecida como tabela CAM (Content Addressable Memory).

📝 Aprendizado de Endereços MAC   
O switch aprende dinamicamente os endereços MAC observando os quadros que chegam:
- Cada quadro recebido é verificado quanto ao endereço MAC de origem.
- Se o MAC de origem ainda não estiver na tabela, o switch adiciona o endereço junto com o número da porta em que o quadro entrou.
- Se o MAC já existir, o switch apenas atualiza o cronômetro de validade dessa entrada (geralmente 5 minutos por padrão).

Isso permite que o switch construa sua tabela de endereços MAC automaticamente e mantenha informações atualizadas conforme os dispositivos enviam tráfego. Exemplo: PC-A envia um quadro para PC-D. O switch adiciona o MAC de PC-A à tabela, associando-o à porta de entrada.

🚦 Encaminhamento de Quadros   
Depois de aprender os endereços, o switch procura o MAC de destino para decidir para qual porta enviar o quadro:
- Unicast conhecido: Se o MAC de destino estiver na tabela, o quadro é enviado somente pela porta correspondente.
- Unicast desconhecido: Se o MAC de destino não estiver na tabela, o switch envia o quadro para todas as portas, exceto a porta de entrada (inundação).
- Broadcast ou Multicast: O quadro também é enviado para todas as portas, exceto a de entrada.

Com o tempo, à medida que mais quadros chegam, o switch consegue filtrar e encaminhar quadros para portas específicas, evitando inundação desnecessária.

🔄 Ciclo de Comunicação Entre Hosts   
- PC-D responde ao PC-A: O quadro de entrada do PC-D faz com que o switch registre o MAC de PC-D na tabela, associando-o à porta correta.
- PC-A recebe a resposta: Como o switch já conhece o MAC de destino (PC-A), envia o quadro somente pela porta correspondente.
- PC-A envia outro quadro para PC-D: O MAC de origem (PC-A) já está na tabela, então o cronômetro é reiniciado. O MAC de destino (PC-D) também está na tabela, então o quadro é enviado diretamente para a porta do PC-D.

Dessa forma, o switch mantém uma rede eficiente e organizada, encaminhando quadros apenas para as portas necessárias, sem sobrecarregar a rede.

<a name="item07.04.01"><h4>7.4.1 Atividade - Encaminhe-o!</h4></a>[Back to summary](#item07)

Nesta atividade, o objetivo foi determinar como o switch encaminhava um quadro com base no endereço MAC de origem, no endereço MAC de destino e nas informações na tabela MAC do switch. Com isso as seguintes perguntas foram respondidas:
- Pergunta 1: Para onde o switch encaminhará o quadro? Saindo de Fa1 (0A) para Fa3 (0B).
  - Fa2, Fa3, Fa4, Fa5, Fa6, Fa7, Fa8, Fa9, Fa10, Fa11, Fa12.
- Pergunta 2: Quando o switch encaminha o quadro, quais afirmações são verdadeiras?
  - O switch adiciona o endereço MAC de origem que atualmente não está na tabela de endereços MAC. (F)
  - O quadro é um quadro broadcast e será encaminhado para todas as portas. (F)
  - O quadro é um quadro unicast e será enviado somente para a porta específica. (F)
  - O quadro é um quadro unicast e será inundado em todas as portas. (V)
  - O quadro é um quadro unicast, mas será descartado no switch. (F)

<a name="item07.05"><h4>7.5 Métodos de encaminhamento e velocidade de switches</h4></a>[Back to summary](#item07)

⚡ Encaminhamento de Quadros em Switches Cisco   
Switches Ethernet da Cisco utilizam endereços MAC para determinar a porta de encaminhamento de cada quadro. Diferente de hubs, que replicam todos os sinais para todas as portas, o switch direciona o tráfego de maneira eficiente para reduzir congestionamento.

🗂️ Métodos de Encaminhamento   
Dois métodos principais são utilizados para encaminhamento de quadros:

1️⃣ Switching Store-and-Forward:
- O quadro é recebido por completo antes de qualquer encaminhamento.
- É calculado um CRC para verificar a integridade do quadro.
- Se o quadro estiver correto, a tabela de MAC é consultada para determinar a porta de destino e o quadro é encaminhado.
- Permite descartar quadros com erro, reduzindo o consumo de largura de banda.
- Necessário em redes que aplicam qualidade de serviço (QoS), onde alguns fluxos de dados (como VoIP) possuem prioridade.

2️⃣ Switching Cut-Through:
- O quadro é encaminhado antes de ser totalmente recebido, assim que o endereço MAC de destino é lido.
- Não realiza verificação de erros, proporcionando menor latência.
- Possui duas variações:
  - Fast-Forward: encaminha imediatamente após ler o MAC de destino. Possui latência mínima, mas alguns quadros com erro podem ser transmitidos.
  - Fragment-Free: armazena os primeiros 64 bytes do quadro antes de encaminhar, evitando a maioria das colisões e erros iniciais. Representa um equilíbrio entre alta integridade e baixa latência.

Alguns switches alternam automaticamente entre cut-through e store-and-forward dependendo da taxa de erro da porta.

🧩 Buffer de Memória em Switches   
Switches podem armazenar quadros em buffers antes de enviá-los, principalmente quando a porta de destino está ocupada:
- Memória por porta: cada porta possui sua própria fila; um quadro pode atrasar todos os quadros da fila se a porta estiver ocupada.
- Memória compartilhada: todos os quadros são armazenados em um buffer comum, alocando dinamicamente memória para cada porta. Permite maior eficiência e reduz descartes, especialmente em links com velocidades diferentes (comutação assimétrica).

⚡ Configurações de Velocidade e Duplex   
- Full-duplex: ambas as extremidades podem transmitir e receber simultaneamente.
- Half-duplex: apenas uma extremidade transmite por vez.
- Negociação automática: dispositivos definem automaticamente a melhor velocidade e duplex compatível. Full-duplex é selecionado quando ambos suportam.

Incompatibilidade de duplex ocorre quando uma extremidade opera em full-duplex e a outra em half-duplex, podendo gerar problemas de desempenho.

🔌 Tipo de Cabo e Auto-MDIX   
Conexões entre dispositivos podem exigir cabos diretos ou cruzados, dependendo do tipo de equipamento conectado. O recurso Auto-MDIX detecta automaticamente o tipo de cabo e ajusta a interface da porta. É ativado por padrão em switches modernos, mas o uso do cabo correto continua sendo recomendado.

<a name="item07.06"><h4>7.6 Módulo Prático e Quiz</h4></a>[Back to summary](#item07)

⚡ Ethernet e Camadas   
Ethernet opera nas camadas de enlace de dados e física. Seus padrões definem protocolos da camada 2 e tecnologias da camada 1, usando as subcamadas LLC e MAC para encapsular dados. O quadro Ethernet inclui preâmbulo, delimitador de quadro, endereços MAC de destino e origem, EtherType, dados e FCS. LANs Ethernet geralmente usam switches em full-duplex.

🔢 Endereçamento MAC   
O endereçamento MAC identifica dispositivos físicos (NICs) na rede local. Cada endereço MAC tem 48 bits, representados por 12 dígitos hexadecimais, divididos em código OUI do fornecedor e valor atribuído. Endereços MAC suportam comunicação unicast, broadcast e multicast, sendo incluídos no cabeçalho do quadro Ethernet para indicar origem e destino.

🖧 Encaminhamento em switches   
Switches Ethernet de camada 2 tomam decisões baseadas apenas nos endereços MAC. Eles constroem dinamicamente uma tabela de endereços MAC examinando os endereços de origem dos quadros recebidos e encaminham quadros filtrando a porta de destino correta.

🔀 Métodos de comutação   
Os switches usam comutação de armazenamento e encaminhamento (store-and-forward) ou cut-through, que pode ser fast-forward ou fragment-free. O armazenamento em buffer pode ser baseado em porta ou memória compartilhada.

🔄 Duplex e negociação automática   
Existem comunicações full-duplex e half-duplex em redes Ethernet. A negociação automática permite que dispositivos selecionem a melhor velocidade e duplex disponíveis. Recursos como Auto-MDIX detectam automaticamente o tipo de cabo e configuram a interface de acordo.
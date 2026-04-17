# CCNA: Introduction to Networks - Módulo 6   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_001 (CCNA: Introduction to Networks)   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="25"></a>
### Module: 6. Camada de Enlace de dados

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

### Course Module 6 Structure:
6. <a name="item06">Camada de Enlace de dados</a><br>
  6.1 <a href="#item06.01">Introdução</a><br>
  6.2 <a href="#item06.02">Finalidade da Camada de Enlance de Dados</a><br>
  6.3 <a href="#item06.03">Topologias</a><br>
  6.4 <a href="#item06.04">Quadro de Enlance de Dados</a><br>
  6.5 <a href="#item06.05">Módulo Prático e Quiz</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item06.01"><h4>6.1 Introdução</h4></a>[Back to summary](#item06)

📘 Introdução   
Este módulo apresenta o papel da camada de enlace de dados no funcionamento das redes. Diferentes tipos de mídia — como cabos, fibras e sinais sem fio — exigem formas específicas de preparar e organizar as informações para que elas possam ser transportadas de maneira eficiente. A camada de enlace de dados é responsável por adaptar os dados a cada meio físico, considerando características como tipo de rede, topologia e métodos de acesso ao canal. Ao compreender como essas adaptações ocorrem, torna-se possível entender o caminho inicial percorrido pelas informações antes de seguirem pelas demais camadas.

🎯 Objetivo Geral   
Explicar como os mecanismos de acesso ao meio, definidos na camada de enlace de dados, permitem a comunicação entre redes utilizando diferentes tipos de mídia.

✅ Objetivos Específicos   
- Descrever a função da camada de enlace de dados na preparação das informações para transmissão em mídias específicas.
- Comparar os métodos de controle de acesso ao meio utilizados em topologias de LAN e WAN.
- Identificar as características e funções do quadro de enlace de dados.

<a name="item06.02"><h4>6.2 Finalidade da Camada de Enlance de Dados</h4></a>[Back to summary](#item06)

🔗 Função Geral da Camada de Enlace de Dados   
A Camada 2 do modelo OSI atua como ponte entre o funcionamento lógico da rede e a transmissão física dos dados. Ela prepara os pacotes vindos da Camada 3 para que possam ser transportados pela mídia física e também realiza o processo inverso quando os dados chegam ao destino. É nessa camada que ocorre o encapsulamento em quadros, a identificação de origem e destino no âmbito local e a verificação básica de integridade.

📤 Operações Essenciais da Camada 2   
A camada de enlace organiza diversas etapas necessárias para que a comunicação local funcione adequadamente. Entre as principais operações realizadas estão:
- Receber pacotes da Camada 3 e encapsular em quadros próprios da Camada 2.
- Controlar como esses quadros são enviados e recebidos na mídia física.
- Trocar quadros entre dispositivos que dividem o mesmo meio de acesso.
- Verificar erros simples e descartar quadros corrompidos.
- Entregar o conteúdo ao protocolo correto da camada superior quando o quadro chega ao destino.

Essa camada permite que tecnologias de rede diferentes coexistam sem exigir que protocolos como IP precisem ser adaptados para cada tipo específico de meio físico.

🖧 Nós na Rede e a Importância da Camada 2   
Um nó pode ser qualquer dispositivo capaz de enviar, receber ou encaminhar dados — desde laptops e smartphones até switches e roteadores. A camada de enlace de dados garante que esses nós possam se comunicar independentemente do tipo de mídia utilizada no caminho. Sem ela, cada tecnologia física exigiria adaptações diretas do protocolo de rede, o que tornaria a comunicação extremamente complexa e pouco padronizada.

🏷️ Encapsulamento no Envio e no Recebimento   
Quando um pacote está prestes a ser transmitido, a Camada 2 adiciona informações como endereço físico de destino e de origem. Depois, converte esse quadro para um formato que a camada física consiga transportar. Quando o quadro chega a outro dispositivo, o processo é invertido: o quadro é lido, verificado e o pacote é entregue para a camada superior. Esse ciclo ocorre a cada salto feito na rede.

🧬 Subcamadas IEEE 802: LLC e MAC   
As tecnologias LAN e MAN seguem a família de padrões IEEE 802, que divide a Camada 2 em duas subcamadas:
- LLC (Logical Link Control):
  - Atua entre o software das camadas superiores e o hardware das camadas inferiores.
  - Indica qual protocolo de rede (como IPv4 ou IPv6) está sendo transportado.
  - Permite que diferentes protocolos da Camada 3 compartilhem a mesma interface e a mesma mídia.
- MAC (Media Access Control):
  - Implementada diretamente no hardware, como a interface de rede.
  - Responsável por encapsular os dados, aplicar endereços físicos e controlar o acesso ao meio.
  - Integra-se com a tecnologia da Camada 1 utilizada: Ethernet, redes sem fio, WPAN, etc.

⚙️ Funções do Encapsulamento MAC   
A subcamada MAC organiza o quadro e controla o acesso à mídia. Entre suas funções:
- Delimitação de quadros: define os limites e campos internos para garantir que os dispositivos interpretem o quadro corretamente.
- Endereçamento físico: adiciona endereços de origem e destino usados localmente.
- Detecção de erros: inclui campos que permitem identificar se houve corrupção durante a transmissão.
- Controle de acesso: administra como vários dispositivos compartilham a mesma mídia (quando o link é half-duplex).

Em links que conectam apenas dois dispositivos, como conexões seriais entre roteadores, o controle de acesso pode ser desnecessário.

🔄 Processo de Encapsulamento em Cada Salto   
Roteadores lidam com vários tipos de redes no caminho até o destino. A cada vez que um pacote chega a um roteador, ocorre:
- Recebimento do quadro pelo meio físico.
- Remoção do encapsulamento da Camada 2.
- Decisão de roteamento na Camada 3.
- Criação de um novo quadro adequado ao próximo tipo de mídia.
- Envio para o próximo segmento da rede.

Esse processo se repete até que o pacote alcance o dispositivo final.

🏛️ Organizações que Padronizam a Camada de Enlace   
Diferente das camadas superiores dos protocolos TCP/IP — definidas principalmente pela IETF — a padronização da Camada 2 e da Camada 1 é realizada por outras entidades técnicas. Entre as principais estão:
- IEEE;
- ITU;
- ISO;
- ANSI;

Essas organizações estabelecem normas para métodos de acesso, quadros, sinais e outros aspectos essenciais para interoperabilidade.

<a name="item06.03"><h4>6.3 Topologias</h4></a>[Back to summary](#item06)

🧭 Topologia física vs. topologia lógica   
A camada de enlace de dados precisa entender como a rede é organizada para decidir como enviar quadros entre dispositivos. A topologia física descreve as conexões reais — cabos, portas, equipamentos e onde ficam no espaço. Já a topologia lógica descreve o caminho que os quadros seguem “virtualmente”, ou seja, como os nós conversam entre si segundo o endereçamento e o formato dos quadros. A camada de enlace opera sempre sobre essa topologia lógica, pois é ela que define como o acesso ao meio e o enquadramento serão feitos.

🛠️ Topologias físicas e lógicas na prática   
A topologia física mostra como os dispositivos estão ligados de verdade, geralmente em ponto a ponto ou estrela.
A topologia lógica mostra como os quadros são encaminhados entre os nós, independentemente da fiação física.

Uma rede pode ter vários saltos e cabos diferentes fisicamente, mas continuar sendo logicamente ponto a ponto, pois a ligação percebida entre origem e destino não muda.

🌍 Topologias WAN mais comuns   
As WANs geralmente são desenhadas usando três modelos principais:
- Ponto a ponto: ligação permanente entre dois pontos. É a forma mais simples de conexão WAN.
- Estrela: um site central conecta filiais usando vários enlaces ponto a ponto. Nenhuma filial se comunica diretamente com outra.
- Malha: todos os nós são conectados entre si. Traz alta disponibilidade, mas é cara e complexa.

Existe também a topologia híbrida, como a malha parcial, onde apenas alguns dispositivos possuem conexões múltiplas.

🔌 Ponto a ponto — funcionamento real   
Em um enlace físico ponto a ponto, só dois nós dividem o meio. Isso permite protocolos simples, como PPP, pois não existe dúvida sobre quem deve receber cada quadro. Os quadros colocados no meio por um lado são retirados apenas pelo outro extremo. Quando o enlace ponto a ponto é via Ethernet, o dispositivo precisa verificar se o quadro recebido realmente é para ele, já que Ethernet trabalha com endereços MAC.

🔁 Topologia lógica independente da física   
Mesmo que vários roteadores ou dispositivos intermediários existam no caminho físico, a visão lógica pode continuar a mesma. Adicionar cabos ou saltos intermediários não muda o fato de que, logicamente, a comunicação é “A ↔ B”.

🖧 LANs com múltiplos dispositivos   
Redes LAN modernas usam principalmente estrela ou estrela estendida:
- No modelo estrela, todos os dispositivos finais se conectam a um switch central.
- Na estrela estendida, vários switches são interligados, ampliando a rede.

Essas topologias são fáceis de instalar, escalar e manter. Antigamente, hubs eram usados no lugar dos switches. 

Também pode existir uma conexão Ethernet com apenas dois dispositivos diretos, como dois roteadores conectados entre si — isso cria uma topologia ponto a ponto dentro da LAN.

🕰️ Topologias legadas   
Tecnologias mais antigas usavam modelos diferentes dos atuais:
- Barramento: todos os dispositivos ligados no mesmo cabo coaxial, com terminações nas extremidades. Simples e barato, muito comum no início do Ethernet.
- Anel: cada nó conectado ao próximo formando um circuito fechado. Usado em Token Ring e FDDI, e não requer terminação.

Nos diagramas de rede, costuma-se representar a LAN inteira como uma única linha “reta”, mesmo quando internamente ela usa estrela ou estrela estendida.

🔄 Comunicação Half-Duplex e Full-Duplex   
A comunicação duplex define como dois dispositivos trocam dados na rede. Ela determina se ambos podem enviar/receber ao mesmo tempo ou não, algo essencial para entender o funcionamento das LANs.

⚪ Half-Duplex   
No half-duplex, os dois dispositivos podem transmitir e receber, porém não ao mesmo tempo. Um fala, o outro espera. Depois invertem. Esse modo cria uma mídia compartilhada, onde todos competem pelo uso do meio. Por isso, ele aparece em tecnologias mais antigas ou específicas, como:
- Hubs Ethernet (redes legadas)
- WLANs (porque o meio é compartilhado por natureza)

Quando vários dispositivos tentam transmitir juntos, ocorre colisão — e isso exige métodos de acesso para lidar com conflitos.

🔵 Full-Duplex   
No full-duplex, ambos os dispositivos enviam e recebem simultaneamente, sem disputar o meio. É a forma usada pelos switches Ethernet modernos, que operam em full-duplex por padrão. Esse modo elimina colisões e aumenta a eficiência.

Atenção: Duas interfaces conectadas precisam usar o mesmo modo duplex. Se uma estiver em half e a outra em full, ocorre duplex mismatch, causando lentidão e perda de pacotes.

🌐 Redes Multiacesso   
LANs Ethernet e WLANs são redes onde vários dispositivos podem tentar enviar dados ao mesmo tempo. Por isso, algumas topologias precisam definir como os dispositivos disputam ou recebem permissão para usar o meio. Existem dois métodos: Acesso Baseado em Contenção e Acesso Controlado.

⚔️ Acesso Baseado em Contenção   
Aqui, todos competem pelo meio. Funciona em half-duplex, pois apenas um pode transmitir por vez. Dois protocolos clássicos:
- CSMA/CD → usado em LANs Ethernet antigas com hubs
- CSMA/CA → usado em WLANs (Wi-Fi)

Se dois dispositivos transmitirem ao mesmo tempo, no caso do CSMA/CD, ocorre colisão, e os dados precisam ser reenviados. No Wi-Fi (CSMA/CA), o dispositivo tenta evitar colisões, porque nem sempre consegue detectá-las. Ele espera um tempo antes de enviar e informa quanto tempo ficará usando a mídia, ajudando os outros dispositivos a evitar conflitos.

🎛️ Acesso Controlado   
Cada nó recebe sua vez para transmitir, de forma ordenada e determinística. É eficiente em evitar conflitos, mas ineficiente em redes modernas, pois todos precisam esperar sua vez. Exemplos legados:
- Token Ring
- ARCNET

Hoje praticamente não se usa mais.

💥 Colisões em Redes Half-Duplex (CSMA/CD)   
Quando dois dispositivos transmitem ao mesmo tempo em uma rede com hub, ocorre uma colisão. O processo funciona assim:
- O dispositivo verifica se o meio está livre.
- Se estiver, ele envia.
- O hub repete o sinal para todas as portas.
- Se outro dispositivo transmitir ao mesmo tempo, ambos detectam a colisão.
- Os dados são descartados e reenviados.

Esse mecanismo não é mais usado em redes com switches, porque o full-duplex elimina colisões.

📡 CSMA/CA em WLANs   
Por ser rede sem fio, o dispositivo nem sempre consegue ouvir todos os outros. Por isso, o Wi-Fi usa CSMA/CA:
- Verifica se o meio parece livre.
- Espera um tempo aleatório antes de transmitir.
- Inclui no quadro quanto tempo vai ocupar o meio.
- Outros dispositivos sabem que devem aguardar.
- O destinatário envia uma confirmação (ACK).

Esse método evita colisões, mas não escala bem com muito tráfego.

🟢 Conclusão   
- Half-duplex: disputa, colisões, um transmite por vez.
- Full-duplex: envio e recepção simultâneos, sem colisões.
- CSMA/CD: usado no passado em redes Ethernet com hubs.
- CSMA/CA: usado no Wi-Fi.
- Acesso controlado: legado e pouco eficiente hoje.
- Switches modernos operam em full-duplex, eliminando a necessidade de métodos de contenção.

<a name="item06.04"><h4>6.4 Quadro de Enlance de Dados</h4></a>[Back to summary](#item06)

🧱 Estrutura Geral do Quadro na Camada de Enlace   
A camada de enlace de dados prepara o pacote da Camada 3 (IPv4 ou IPv6) para circular na mídia física. Isso é feito por meio do encapsulamento, onde o pacote recebe um cabeçalho, um campo de dados e um trailer, formando o quadro. Cada protocolo de enlace (Ethernet, Wi-Fi, PPP, etc.) define o seu próprio formato. Não existe um único tipo de quadro que sirva para todos os ambientes, porque cada mídia e cada topologia exige controles diferentes. Em redes mais frágeis ou sujeitas a interferências, é necessário incluir mais informações de controle, o que aumenta o tamanho do quadro e reduz a taxa de transmissão.

📦 Componentes do Enquadramento   
O enquadramento converte o fluxo de bits em blocos compreensíveis, com sinais, limites e indicadores que permitem ao destino reconstruir o pacote corretamente.

Elementos essenciais:
- Cabeçalho: Contém informações como endereços de origem e destino, tipo de protocolo e possíveis controles de QoS.
- Dados: Onde está o pacote IP encapsulado, contendo cabeçalho de transporte e dados da aplicação.
- Trailer: Usado principalmente para detecção de erros.

Cada protocolo decide quais campos realmente usa. Mas os propósitos são sempre os mesmos: delimitar, identificar, endereçar e garantir que o quadro chegue íntegro.

🧪 Detecção de Erros (FCS e CRC)   
No trailer, a camada de enlace coloca um mecanismo de verificação chamado FCS (Frame Check Sequence). Ele carrega um valor matemático criado a partir dos bits do quadro, conhecido como CRC (Cyclic Redundancy Check). O funcionamento acontece da seguinte forma:
- O transmissor calcula o CRC e o coloca no trailer.
- O receptor recalcula o CRC ao receber o quadro.
- Se os valores forem diferentes, o quadro foi corrompido.

Esse mecanismo é necessário porque o sinal sofre interferências, ruídos e distorções na mídia física.

🆔 Endereçamento na Camada 2 (Endereço Físico)   
A camada de enlace usa endereços físicos, usualmente chamados de endereços MAC. Esses endereços:
- Identificam o dispositivo dentro da rede local.
- Não são hierárquicos como endereços IP.
- Não mudam quando o dispositivo troca de rede.

A NIC verifica o campo de destino logo no início do quadro, decidindo rapidamente se deve aceitar ou descartar o restante do conteúdo. Enquanto o IP viaja pela rede inteira, o endereço de Camada 2 vale apenas até o próximo salto físico.

🔁 Endereços de Camada 2 ao Longo do Caminho   
A cada salto, o pacote IP permanece igual, mas o quadro é trocado. Assim, o endereço MAC muda a cada segmento:
- Host → Roteador: MAC origem = do host / MAC destino = do roteador.
- Roteador → Roteador: MAC origem = R1 / MAC destino = R2.
- Roteador → Host final: MAC origem = R2 / MAC destino = servidor.

Isso ocorre porque cada segmento físico é independente. O roteador remove o quadro (desencapsula), lê o IP, decide o caminho e cria um novo quadro.

🌍 Protocolos de Camada 2   
O protocolo usado depende da topologia e da mídia. LANs e WANs, por terem exigências diferentes, tradicionalmente usaram protocolos diferentes.

- Exemplos comuns de protocolos da Camada 2:
  - Ethernet;
  - Wi-Fi (IEEE 802.11);
  - PPP;
  - HDLC;
  - Frame Relay.

Esses protocolos controlam como os dispositivos acessam a mídia e definem o formato do quadro. Hoje, até WANs estão migrando para Ethernet, eliminando protocolos antigos.

🏙️ Diferenças entre LAN e WAN na Camada 2   
Uma LAN geralmente cobre pequenos espaços físicos e suporta muitos hosts, usando tecnologias de alta largura de banda a um custo razoável. Já uma WAN cobre distâncias grandes e utiliza tecnologias mais caras, com menor largura de banda. Por isso, LANs e WANs historicamente adotaram protocolos diferentes. A escolha do protocolo envolve:
- Escopo geográfico;
- Número de dispositivos;
- Tipo de mídia;
- Custos de implantação.

🖧 Dispositivos que Operam na Camada 2
Vários dispositivos podem participar do processo de enquadramento e entrega local:
- NICs dos hosts;
- Interfaces de roteadores;
- Interfaces de switches camada 2;

Cada uma implementa o protocolo específico da rede em que está operando.

<a name="item06.05"><h4>6.5 Módulo Prático e Quiz</h4></a>[Back to summary](#item06)

🔗 Camada de enlace de dados   
A camada de enlace prepara os dados da camada de rede para o envio pelo meio físico e garante a comunicação entre NICs. Sem ela, protocolos como o IP precisariam lidar diretamente com cada tipo de mídia existente. No padrão IEEE 802, essa camada é dividida em LLC e MAC. A MAC faz o encapsulamento, adiciona endereçamento físico, delimita quadros e detecta erros. O acesso ao meio depende do tipo de link, e organizações como IEEE, ITU, ISO e ANSI definem os padrões usados nela.

📡 Topologias e modos de comunicação   
As redes utilizam topologias físicas e lógicas. A camada de enlace trabalha com a topologia lógica, que define como o meio é acessado e como o enquadramento funciona. Em WANs, é comum o uso de ponto a ponto, hub and spoke e malha. Em LANs, predominam estrela, estrela estendida, barramento e anel. A comunicação pode ocorrer em half-duplex ou full-duplex; ambos os lados precisam usar o mesmo modo para evitar latência e colisões lógicas.

🌐 Redes multiacesso e controle de acesso   
Ethernet e WLAN são redes multiacesso, nas quais vários dispositivos podem transmitir ao mesmo tempo. Para isso, existem dois métodos de controle: acesso baseado em contenção (como CSMA/CD e CSMA/CA) ou acesso controlado. No acesso por contenção, todos operam em half-duplex, e existe um processo para lidar com colisões.

📦 Estrutura do quadro   
A camada de enlace encapsula o pacote IPv4 ou IPv6 com um cabeçalho e um trailer, formando o quadro. Os quadros podem incluir campos como início e fim, endereços físicos, tipo, controle, dados e detecção de erros. O endereçamento dessa camada é físico e serve apenas para entrega local dentro da mesma rede.

🛠️ Protocolos de enlace   
Embora todos os protocolos de camada 2 trabalhem com o IP na camada 3, o protocolo usado depende da topologia lógica e da tecnologia física. Entre os principais protocolos de enlace estão Ethernet, 802.11 Wireless, PPP, HDLC e Frame Relay.
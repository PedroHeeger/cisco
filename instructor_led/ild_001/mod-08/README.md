# CCNA: Introduction to Networks - Módulo 8   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_001 (CCNA: Introduction to Networks)   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="25"></a>
### Module: 8. Camada de rede

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
8. <a name="item08">Camada de rede</a><br>
  8.1 <a href="#item08.01">Introdução</a><br>
  8.2 <a href="#item08.02">Características de camada de rede</a><br>
  8.3 <a href="#item08.03">Pacote IPv4</a><br>
  8.4 <a href="#item08.04">Pacote IPv6</a><br>
  8.5 <a href="#item08.05">Como um Host Roteia</a><br>
  8.6 <a href="#item08.06">Introdução ao Roteamento</a><br>
  8.7 <a href="#item08.07">Módulo Prático e Quiz</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item08.01"><h4>8.1 Introdução</h4></a>[Back to summary](#item08)

📘 Introdução   
Este módulo avança para a camada de rede do modelo OSI, responsável por permitir que informações ultrapassem os limites de uma única rede local. Enquanto a comutação atua apenas dentro do mesmo segmento, a entrega de dados entre redes diferentes depende de protocolos de roteamento e do uso de dispositivos capazes de direcionar pacotes ao destino correto. Essa camada define como pacotes são estruturados, encaminhados e identificados ao longo de diversos saltos até alcançarem a rede final. Atividades práticas auxiliam na visualização desse processo, destacando o papel essencial dos roteadores na comunicação de ponta a ponta.

🎯 Objetivo Geral   
Explicar como os roteadores utilizam protocolos e serviços da camada de rede para possibilitar a entrega de pacotes entre redes distintas.

✅ Objetivos Específicos   
- Descrever como a camada de rede utiliza o protocolo IP para garantir o encaminhamento das informações.
- Identificar a função dos principais campos do cabeçalho em pacotes IPv4.
- Identificar a função dos principais campos do cabeçalho em pacotes IPv6.
- Explicar como dispositivos determinam o caminho de um pacote por meio de tabelas de roteamento.
- Descrever a finalidade dos campos presentes nas tabelas de roteamento mantidas por roteadores.

<a name="item08.02"><h4>8.2 Características de camada de rede</h4></a>[Back to summary](#item08)

🌐 Visão Geral da Camada de Rede (Camada 3)   
A Camada de Rede do modelo OSI é responsável por permitir que dispositivos troquem dados entre diferentes redes. É nela que atuam protocolos como IPv4 e IPv6, além de protocolos de suporte como OSPF (roteamento) e ICMP (mensagens de controle). Essa camada viabiliza a comunicação fim a fim executando processos fundamentais: endereçamento, encapsulamento, roteamento e desencapsulamento.

📌 Endereçamento de Host   
Cada dispositivo precisa ter um endereço IP único, que permita identificá-lo entre diversas redes. O IP é esse identificador universal usado pelos roteadores para encontrar o destino correto.

📦 Encapsulamento de Dados   
Antes de enviar informações pela rede, a Camada 3 coloca o conteúdo recebido da Camada 4 dentro de um pacote IP, acrescentando um cabeçalho. Nesse cabeçalho ficam elementos essenciais, como:
- endereço IP de origem;
- endereço IP de destino;
- informações para roteamento.

O encapsulamento sempre é feito no dispositivo que gera o pacote.

🚏 Roteamento Entre Redes   
Para que um pacote viaje de uma rede para outra, ele precisa passar por roteadores. Esses dispositivos analisam o endereço de destino no cabeçalho IP e escolhem o melhor caminho disponível. Cada roteador atravessado pelo pacote é considerado um salto. Dependendo da topologia, um pacote pode atravessar vários saltos até chegar ao destino final.

🔎 Desencapsulamento no Destino   
Quando o pacote alcança o dispositivo de destino, a Camada 3 verifica se o endereço IP no cabeçalho corresponde ao dispositivo. Se corresponder:
- o cabeçalho IP é removido;
- o conteúdo interno (PDU da Camada 4) é encaminhado à camada superior.

Esse processo só ocorre no host que realmente recebe o pacote.

🧱 Estrutura do Pacote e Independência das Camadas   
A Camada de Rede trabalha sem se preocupar com os dados transportados. Independente de ser um segmento TCP, UDP ou outro tipo de PDU, o IP apenas encapsula, endereça e encaminha. Essa separação entre camadas permite que:
- novos protocolos sejam criados sem alterar IPv4/IPv6;
- diferentes meios físicos transportem pacotes da mesma forma;
- o roteamento funcione mesmo sem conhecer o conteúdo transportado.

O cabeçalho IP é analisado em todos os dispositivos de Camada 3 pelos quais o pacote passa. As únicas exceções ocorrem quando há NAT, que altera endereços IP por razões de tradução.

🛰️ Funções e Características do IP   
O protocolo IP mantém um conjunto de características que o tornam simples e eficiente:
- Sem Conexão: O envio de pacotes ocorre sem estabelecer previamente uma sessão entre origem e destino. É semelhante ao envio de uma carta: o remetente entrega e não sabe antecipadamente se o destinatário está disponível. Esse modelo reduz sobrecarga e permite que a transmissão comece imediatamente.
- Entrega de “Melhor Esforço”: IP não garante entrega, ordem ou integridade. Pacotes podem: chegar fora de ordem; ser descartados; sofrer corrupção; nunca alcançar o destino. A camada de rede não tenta reparar esses problemas. Se alguma correção for necessária, ela é feita por protocolos da Camada 4, especialmente o TCP.
- Independência de Mídia: Os pacotes IP podem trafegar por qualquer meio físico: cobre; fibra óptica; rádio (Wi-Fi, celular, etc.). A Camada de Enlace de Dados é quem adapta o pacote ao tipo de transmissão, garantindo que o IP funcione de forma uniforme independentemente do meio.

📏 MTU e Fragmentação   
Cada tecnologia física tem um tamanho máximo de quadro chamado MTU. A Camada de Enlace informa esse limite à Camada de Rede, que decide o tamanho máximo permitido para os pacotes. Quando um roteador precisa enviar um pacote IPv4 por um meio com MTU menor, ele pode fragmentar o pacote. Fragmentação aumenta a latência e reduz eficiência, mas é necessária em alguns cenários. No caso do IPv6, os roteadores não fragmentam pacotes. Se o pacote for grande demais, ele é descartado e o remetente é informado para reduzir o tamanho.

<a name="item08.03"><h4>8.3 Pacote IPv4</h4></a>[Back to summary](#item08)

📦 Estrutura do Cabeçalho IPv4   
O IPv4 é um dos principais protocolos de camada de rede, e seu cabeçalho contém informações essenciais para que cada pacote avance corretamente até o destino final. Cada campo do cabeçalho traz valores binários analisados pela Camada 3 sempre que o pacote passa por um roteador. Os diagramas de cabeçalho seguem um padrão de leitura: da esquerda para a direita e de cima para baixo, facilitando a identificação de cada campo.

Os principais campos do cabeçalho IPv4 incluem:

🧩 Versão   
Indica qual versão do protocolo IP está sendo usada. Para pacotes IPv4, o valor armazenado é 0100 (4 bits).

🎛️ Campo DS (DiffServ)   
Esse campo possui 8 bits e define o comportamento do pacote em relação a prioridade e controle de congestionamento.
- DSCP (6 bits): determina o nível de prioridade do tráfego.
- ECN (2 bits): usado para notificação explícita de congestionamento.

Esse conjunto substituiu o antigo campo ToS.

⏱️ Tempo de Vida (TTL)   
Armazena um valor de 8 bits que limita a permanência do pacote na rede. O TTL é definido pelo dispositivo de origem e reduzido em 1 a cada roteador atravessado. Quando o valor chega a zero:
- o pacote é descartado;
- uma mensagem ICMP Time Exceeded é enviada ao endereço de origem.

Como o valor muda a cada salto, o roteador precisa recalcular a soma de verificação do cabeçalho.

📑 Protocolo   
Indica que tipo de dado está encapsulado dentro do pacote. É um valor de 8 bits que permite à Camada 3 entregar a PDU ao protocolo correto da camada superior. Exemplos comuns:
- ICMP → 1.
- TCP → 6.
- UDP → 17.

✔️ Checksum do Cabeçalho   
Usado para verificar se houve corrupção no cabeçalho IPv4 durante o tráfego. Se o cálculo indicar inconsistência, o pacote é descartado.

🏠 Endereço IPv4 de Origem   
Campo de 32 bits que registra o endereço do dispositivo que enviou o pacote. Esse endereço sempre é unicast.

🎯 Endereço IPv4 de Destino   
Campo de 32 bits que especifica o endereço final pretendido. Pode ser: unicast, multicast, broadcast. Em condições normais, os endereços de origem e destino não mudam durante o trajeto, exceto em situações que envolvem NAT. Esses dois campos são os mais consultados no processo de encaminhamento.

🧱 Campos de Identificação e Fragmentação   
Quando um pacote precisa ser dividido para atravessar um meio com MTU menor, são usados três campos específicos:
- Identificação;
- Flags;
- Deslocamento do Fragmento.

Com esses valores, o destino consegue remontar o pacote original mesmo que tenha chegado em partes.

🧪 Campos de Controle e Validação   
Alguns campos garantem consistência estrutural do pacote:
- IHL (Internet Header Length): informa o tamanho do cabeçalho.
- Tamanho Total: indica o tamanho completo do pacote IP.
- Checksum do Cabeçalho: valida integridade da parte do cabeçalho.

🗂️ Opções e Preenchimento   
Esses campos existem para funcionalidades específicas e raramente aparecem em uso comum. Por estarem fora do escopo prático do módulo, não foram explorados com profundidade.

<a name="item08.04"><h4>8.4 A Pacote IPv6</h4></a>[Back to summary](#item08)

🌐 Por que o IPv6 Foi Criado   
O IPv4 permanece amplamente utilizado, porém apresenta limitações que motivaram o desenvolvimento do IPv6. As principais dificuldades enfrentadas pelo IPv4 são:
- Escassez de endereços públicos:
  - O espaço de 32 bits oferece cerca de 4,3 bilhões de endereços.
  - O crescimento de dispositivos conectados, serviços permanentes e expansão global tornou esse número insuficiente.
- Ausência de conectividade direta (ponto a ponto):
  - A adoção de NAT permitiu que vários dispositivos compartilhassem um único endereço público.
  - Entretanto, essa técnica oculta os endereços internos e dificulta aplicações que dependem de comunicação direta entre dispositivos.
- Aumento da complexidade das redes:
  - O NAT foi criado como solução temporária para a transição ao IPv6, mas trouxe latência adicional, regras complexas e dificuldades de diagnóstico.

🚀 Surgimento do IPv6   
Diante desses desafios, a IETF iniciou na década de 1990 o desenvolvimento de uma nova versão do protocolo IP. O IPv6 foi projetado para lidar com as demandas modernas da Internet, oferecendo:
- Espaço de endereçamento muito maior:
  - Utiliza 128 bits, permitindo cerca de 340 undecilhões de endereços — número comparável à quantidade de grãos de areia do planeta.
- Processamento de pacotes mais eficiente:
  - O cabeçalho IPv6 possui menos campos e tamanho fixo, simplificando o trabalho dos roteadores.
- Conectividade de ponta a ponta restabelecida:
  - O enorme volume de endereços elimina a necessidade de NAT em redes IPv6.

🧩 Estrutura do Cabeçalho IPv6   
O IPv4 utiliza um cabeçalho variável de 20 a 60 bytes, com vários campos opcionais. O IPv6 adota um cabeçalho fixo de 40 bytes, mais simples e mais rápido de processar.

Principais campos do cabeçalho IPv6:
- Versão (4 bits): Identifica o pacote como IPv6 (valor binário 0110).
- Classe de Tráfego (8 bits): Equivalente ao DifServ/DSCP do IPv4; usada para prioridade e qualidade de serviço.
- Etiqueta de Fluxo (20 bits): Identifica pacotes que pertencem ao mesmo fluxo, permitindo tratamento consistente pelos roteadores.
- Comprimento da Carga Útil (16 bits): Indica o tamanho da parte de dados (não inclui os 40 bytes do cabeçalho).
- Próximo Cabeçalho (8 bits): Indica qual protocolo ou cabeçalho adicional vem a seguir; é o equivalente ao campo "Protocolo" do IPv4.
- Limite de Salto (8 bits): Substitui o TTL. Cada roteador reduz esse valor em 1. Ao chegar a zero, o pacote é descartado e uma mensagem ICMPv6 é enviada de volta ao remetente.
- Endereço IPv6 de Origem (128 bits)
- Endereço IPv6 de Destino (128 bits)

Observação: O IPv6 não possui soma de verificação do cabeçalho. Essa validação é responsabilidade das camadas superiores e inferiores, reduzindo a carga de processamento nos roteadores.

🧱 Cabeçalhos de Extensão (Extension Headers – EH)   
Um pacote IPv6 pode incluir cabeçalhos adicionais entre o cabeçalho principal e a carga útil. Esses cabeçalhos opcionais são usados para:
- Fragmentação;
- Segurança e autenticação;
- Mobilidade;
- Controle avançado de roteamento.

Diferentemente do IPv4, os roteadores não fragmentam pacotes IPv6. Se um pacote for grande demais, cabe ao host de origem ajustá-lo antes do envio.

<a name="item08.05"><h4>8.5 Como um Host Roteia</h4></a>[Back to summary](#item08)

🌐 Criação de Pacotes e Tabelas de Roteamento em Hosts   
A geração de pacotes IPv4 e IPv6 sempre ocorre no host de origem. Para que esses pacotes encontrem o destino correto, cada dispositivo final mantém sua própria tabela de roteamento. Esse conjunto de rotas define como o host encaminha pacotes para si mesmo, para destinos locais ou para redes remotas.

Tipos de Destino que um Host Pode Alcançar:

🌀 1. Loopback (o próprio host)   
Um host pode testar a própria pilha TCP/IP utilizando endereços reservados:
  - IPv4: 127.0.0.1
  - IPv6: ::1

O envio de pacotes para a interface de loopback confirma que os protocolos internos do sistema estão funcionando.

🏡 2. Host Local   
É o dispositivo que está na mesma rede que o host de origem. Ambos compartilham a mesma identificação de rede. Pacotes destinados a hosts locais são enviados apenas para fora da interface do host e passam diretamente pelo switch ou WAP que conecta os dispositivos da rede interna.

🌍 3. Host Remoto   
É o destino fora da rede local. Nesse caso, origem e destino pertencem a redes diferentes, exigindo a atuação de um roteador. A comunicação depende de roteamento, ou seja, da escolha do caminho mais adequado até a rede remota.

🧭 Como o Host Decide se o Destino é Local ou Remoto   
A determinação é feita pelo próprio dispositivo final e depende da versão do IP:
- Em IPv4 a análise usa:
  - endereço IPv4 do host;
  - máscara de sub-rede do host;
  - endereço IPv4 do destino.
  - Com essas informações, o host compara sua rede com a rede do destino.
- Em IPv6: O roteador anuncia automaticamente o prefixo da rede local para todos os hosts. Com o prefixo recebido, o host identifica se o destino pertence à mesma rede ou se está em outra.

📡 Redes Domésticas e Corporativas   
Em redes comuns, vários dispositivos — cabeados ou sem fio — conectam-se por meio de equipamentos intermediários como: switches LAN e pontos de acesso sem fio (WAP). Esses equipamentos apenas interligam dispositivos dentro da mesma rede local. Enquanto todos estiverem no mesmo segmento de rede, a comunicação ocorre diretamente, sem roteadores.

🚪 A Função do Gateway Padrão   
Quando o destino está fora da rede local, o pacote precisa sair do segmento. O dispositivo responsável por essa tarefa é o gateway padrão (default gateway). Ele funciona como a “porta” da rede. Para alcançar outra rede, o host precisa enviar o pacote ao gateway.

- Características do gateway padrão:
  - possui um endereço IP dentro da mesma rede local dos hosts;
  - recebe pacotes vindos da LAN e encaminha para redes externas;
  - sabe como rotear tráfego para outros destinos.
  - Sem o gateway padrão ou com ele inativo, nenhum pacote pode sair da rede local.

📍 Rota Padrão na Tabela de Roteamento   
Ao configurar o endereço do gateway padrão, o host cria automaticamente uma rota padrão. A rota padrão é o caminho usado para alcançar qualquer rede que não esteja diretamente conectada.
- Em IPv4: o endereço do gateway é obtido via DHCP ou configurado manualmente.
- Em IPv6: o roteador envia anúncios de gateway ou o endereço é configurado manualmente.

Assim, todo tráfego destinado a redes remotas é enviado ao gateway padrão.

🗺️ Como Visualizar a Tabela de Roteamento no Windows   
Os comandos `netstat -r` e `route print` exibem a tabela de roteamento do host. Ambos produzem a mesma saída, que é organizada em três partes principais:
- Lista de Interfaces:
  - Mostra o endereço MAC de cada interface;
  - Apresenta o número de identificação atribuído a cada interface;
  - Exibe todos os adaptadores com capacidade de rede (Ethernet, Wi-Fi, Bluetooth, etc.).
- Tabela de Rotas IPv4:
  - Lista as rotas diretamente conectadas ao host;
  - Exibe a rota da rede local;
  - Indica a rota padrão utilizada para alcançar redes remotas.
- Tabela de Rotas IPv6:
  - Segue a mesma organização da tabela IPv4, mas listando todas as rotas IPv6 conhecidas pelo host.

<a name="item08.06"><h4>8.6 Introdução ao Roteamento</h4></a>[Back to summary](#item08)

📘 Operações de Roteadores na Camada de Rede   
Roteadores são dispositivos intermediários que recebem, analisam e encaminham pacotes entre redes. Assim como os hosts possuem suas próprias tabelas de roteamento, os roteadores também mantêm tabelas que listam todos os destinos conhecidos e o próximo salto necessário para alcançá-los.

🛰️ Encaminhamento de Pacotes pelo Roteador   
Quando um pacote chega a uma interface do roteador, ocorre o seguinte processo:
- Desencapsulamento da Camada 2: O roteador remove o cabeçalho e o trailer Ethernet recebidos na interface (por exemplo, GigabitEthernet0/0/0).
- Leitura do Endereço de Destino IPv4: O endereço IP de destino é analisado.
- Busca na Tabela de Roteamento: A tabela contém todas as rotas conhecidas (prefixos). Cada entrada indica para onde o pacote deve ser encaminhado. O roteador seleciona a melhor correspondência, conhecida como Longest Prefix Match.
- Reencapsulamento: Depois de decidir o próximo salto, o roteador encapsula o pacote em um novo quadro Ethernet.
- Encaminhamento: O pacote é enviado pela interface de saída em direção ao próximo roteador no caminho.

Exemplo: No roteador R1, o pacote chega pela interface G0/0/0. A tabela de roteamento indica que o próximo salto é o roteador R2. R1 remove o quadro original, cria um novo quadro e envia o pacote para R2.

📚 Estrutura da Tabela de Roteamento   
A tabela de roteamento armazena três tipos principais de entradas:
- Redes Conectadas Diretamente:
  - Surgem automaticamente quando uma interface é configurada com um endereço IP e está ativa.
  - Cada interface conecta o roteador a um segmento de rede distinto.
- Redes Remotas:
  - São redes que não estão diretamente conectadas ao roteador.
  - Podem ser aprendidas de duas formas:
    - Manual: configuradas com rotas estáticas.
    - Dinâmica: aprendidas por protocolos de roteamento.
- Rota Padrão (Gateway de Último Recurso):
  - Utilizada quando nenhuma outra rota corresponde ao destino.
  - Representada por:
    - Prefixo IPv4: 0.0.0.0/0
    - Código na tabela: S*

🧭 Rotas Estáticas   
Rotas estáticas são inseridas manualmente pelo administrador.

Características:
- Dependem de configuração manual.
- Não se ajustam automaticamente a mudanças de topologia.
- Adequadas para redes pequenas ou segmentos com poucos caminhos redundantes.
- Comumente utilizadas para configurar a rota padrão.

Exemplo: R1 possui uma rota estática para a rede 10.1.1.0/24 via R2. Se o caminho via R2 falhar, uma nova rota deve ser manualmente configurada para R3.

🔄 Protocolos de Roteamento Dinâmico   
Protocolos de roteamento dinâmico permitem que os roteadores troquem automaticamente informações sobre redes remotas.

Vantagens:
- Descobrem redes remotas.
- Escolhem automaticamente o melhor caminho.
- Reagem a falhas e mudanças na topologia.
- Atualizam a tabela de roteamento sem intervenção manual.

Principais protocolos:
- OSPF (Open Shortest Path First)
- EIGRP (Enhanced Interior Gateway Routing Protocol)

Exemplo: R1 informa R2 sobre a rede 192.168.10.0/24 via OSPF. R2 informa R1 sobre 10.1.1.0/24. Se houver mudança de topologia, os dois roteadores ajustam a rota automaticamente.

É comum que redes utilizem uma combinação de rotas estáticas + roteamento dinâmico.

🖥️ Exibindo a Tabela de Roteamento no Cisco IOS   
O comando `show ip route` exibe a tabela de roteamento IPv4 no Cisco IOS. A saída exibe:
- Todos os destinos IPv4 conhecidos.
- O código de origem da rota. Principais códigos:
  - L: endereço local
  - C: rede conectada
  - S: rota estática
  - O: rota aprendida via OSPF
  - D: rota aprendida via EIGRP
  - S*: rota estática padrão

<a name="item08.07"><h4>8.7 Módulo Prático e Quiz</h4></a>[Back to summary](#item08)

🌐 Camada de rede (Camada 3)   
A camada de rede fornece serviços que permitem a troca de dados entre redes. Seus principais protocolos são IPv4 e IPv6; também inclui protocolos de roteamento (ex.: OSPF) e de mensagens (ex.: ICMP). As quatro operações básicas dessa camada são: endereçamento de dispositivos finais, encapsulamento do segmento da camada de transporte em um pacote, roteamento desse pacote entre redes e desencapsulamento no destino.

📦 Características do IP   
O IP encapsula o segmento de transporte adicionando um cabeçalho que roteadores examinam enquanto o pacote percorre a rede. O protocolo IP é sem conexão (não estabelece sessão ponta a ponta), de melhor esforço (não garante entrega) e independente do tipo de mídia subjacente.

🔢 Cabeçalho IPv4   
O cabeçalho IPv4 contém campos binários que controlam o processamento do pacote, incluindo: versão, DS (Differentiated Services), soma de verificação do cabeçalho, TTL (Time To Live), protocolo (campo que indica TCP/UDP, etc.) e os endereços IPv4 de origem e destino.

🌍 IPv6 e vantagens   
IPv6 foi criado para resolver limitações do IPv4 — esgotamento de endereços, complexidade e falta de conectividade ponto a ponto. Ele amplia o espaço de endereçamento, melhora o tratamento de pacotes e elimina a necessidade de NAT. O cabeçalho IPv6 inclui: versão, classe de tráfego, rótulo de fluxo, comprimento da carga útil, próximo cabeçalho, limite de salto e endereços IPv6 de origem e destino.

🔎 Determinação de rede local vs remota   
Um host decide se o destino está na mesma rede usando, no IPv4, sua máscara de sub-rede junto ao seu endereço e ao endereço destino. No IPv6, o roteador anuncia o prefixo local para os hosts. Se o destino estiver fora da rede local, o pacote é enviado ao gateway padrão (roteador local) para encaminhamento.

🛣️ Gateway padrão e tabela de roteamento   
O gateway padrão é o roteador que aceita tráfego da rede local e o encaminha para outras redes. Hosts mantêm uma tabela de roteamento (muitas vezes com uma rota padrão). Em IPv4 essa configuração pode vir via DHCP ou ser manual; em IPv6, roteadores podem anunciar o gateway/prefixo. Em sistemas Windows, comandos como `route print` ou `netstat -r` mostram a tabela de roteamento.

📚 Funcionamento do roteador e tabela de roteamento   
Ao receber um pacote, o roteador lê o endereço IP de destino, consulta sua tabela de roteamento (lista de prefixos e destinos) e escolhe a melhor rota — normalmente a entrada de correspondência mais longa (longest-prefix match). A tabela armazena redes conectadas diretamente, redes remotas (aprendidas dinamicamente) e uma rota padrão. Rotas podem ser estáticas (configuradas manualmente) ou aprendidas por protocolos dinâmicos como OSPF e EIGRP.

🔠 Códigos de origem de rota   
Em tabelas de roteamento IPv4 de roteadores Cisco, há códigos que indicam a origem da rota, por exemplo: L = endereço local da interface, C = conectado diretamente, S = estática, O = OSPF, D = EIGRP. O comando `show ip route` exibe essas rotas no modo EXEC privilegiado.
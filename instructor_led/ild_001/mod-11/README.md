# CCNA: Introduction to Networks - Módulo 11   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_001 (CCNA: Introduction to Networks)   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="25"></a>
### Module: 11. Camada de rede

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

### Course Module 11 Structure:
11. <a name="item11">Endereçamento IPv4</a><br>
  11.1 <a href="#item11.01">Introdução</a><br>
  11.2 <a href="#item11.02">Estrutura do Endereço IPv4</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;11.2.1 <a href="#item11.02.01">Atividade - ANDing to Determine the Network Address</a><br>
  11.3 <a href="#item11.03">Unicast, broadcast e multicast IPv4</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;11.3.1 <a href="#item11.03.01">Atividade - Unicast, Broadcast, or Multicast</a><br>
  11.4 <a href="#item11.04">Tipos de endereços IPv4</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;11.4.1 <a href="#item11.04.01">Atividade - Passar ou bloquear endereços IPv4</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;11.4.2 <a href="#item11.04.02">Atividade - Endereço IPv4 Privado ou Público</a><br>
  11.5 <a href="#item11.05">Segmentação de rede</a><br>
  11.6 <a href="#item11.06">Sub-rede de uma rede IPv4</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;11.6.1 <a href="../../../pkt/files/pkt_031/">Packet Tracer - Sub-rede uma rede IPv4</a><br>
  11.7 <a href="#item11.07">Sub-rede uma barra 16 e um prefixo de barra 8</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;11.7.1 <a href="#item11.07.01">Atividade - Cálculo da Máscara de Sub-Rede</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;11.7.2 <a href="../../../labs/files/lab_050/">Laboratório - Calcular sub-redes IPv4</a><br>
  11.8 <a href="#item11.08">Divisão em sub-redes para atender a requisitos</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;11.8.1 <a href="#item11.08.01">Atividade - Determinando o Número de Bits para Pegar Emprestado</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;11.8.2 <a href="../../../pkt/files/pkt_032/">Packet Tracer - Criação de sub-redes no cenário</a><br>
  11.9 <a href="#item11.09">VLSM</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;11.9.1 <a href="#item11.09.01">Atividade - Prática VLSM</a><br>
  11.10 <a href="#item11.10">Projeto estruturado</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;11.10.1 <a href="../../../pkt/files/pkt_033/">Packet Tracer - Prática de projeto e implementação do VLSM</a><br>
  11.11 <a href="#item11.11">Módulo Prático e Quiz</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;11.11.1 <a href="../../../pkt/files/pkt_034/">Packet Tracer - Projete e implemente um esquema de endereçamento VLSM</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;11.11.2 <a href="../../../pkt/files/pkt_035/">Packet Tracer - Projetar e Implementar um Esquema de Endereçamento VLSM - Modo Físico</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item11.01"><h4>11.1 Introdução</h4></a>[Back to summary](#item11)

📘 Introdução   
IPv4 continua amplamente presente nas redes atuais, mesmo com a adoção gradual do IPv6. Por esse motivo, compreender com precisão como esse sistema de endereçamento funciona permanece essencial. Este módulo apresenta os princípios fundamentais do IPv4, como a estrutura do endereço, o uso de máscaras e a divisão de uma rede em partes menores por meio de sub-redes. A prática de subnetting exige atenção, mas torna-se natural à medida que os métodos são aplicados repetidamente. Atividades guiadas, exemplos e exercícios interativos auxiliam no desenvolvimento dessas habilidades, permitindo criar planos de endereçamento adequados para diferentes cenários.

🎯 Objetivo Geral   
Construir esquemas de sub-redes IPv4 capazes de segmentar redes de forma eficiente e organizada.

✅ Objetivos Específicos   
- Identificar os elementos que compõem um endereço IPv4: parte de rede, parte de host e máscara.
- Diferenciar endereços unicast, broadcast e multicast no contexto do IPv4.
- Reconhecer endereços públicos, privados e faixas reservadas.
- Compreender o papel da sub-rede na organização da comunicação dentro de uma rede.
- Realizar cálculos de subnetting para prefixos /24, /16 e /8.
- Criar sub-redes adequadas a requisitos específicos de um projeto.
- Desenvolver planos de endereçamento flexíveis usando VLSM.
- Construir esquemas estruturados de endereçamento baseados em VLSM.

<a name="item11.02"><h4>11.2 Estrutura do Endereço IPv4</h4></a>[Back to summary](#item11)

🌐 Endereço IPv4   
Um endereço IPv4 é um código de 32 bits usado para identificar dispositivos em uma rede. Ele é hierárquico, ou seja, dividido em duas partes:
- Parte de rede: identifica a rede à qual o dispositivo pertence. Todos os dispositivos na mesma rede compartilham esses bits.
- Parte de host: identifica cada dispositivo individualmente dentro da rede. Cada host tem bits exclusivos nesta parte.

🔑 Máscara de Sub-rede   
A máscara de sub-rede indica quais bits de um endereço IPv4 representam a rede e quais representam o host. Ela permite que os dispositivos determinem se outro dispositivo está na mesma rede ou em uma rede remota. Para que um host funcione corretamente, além do endereço IPv4 e máscara de sub-rede, ele também precisa de:
- Gateway padrão: para acessar redes externas.
- Endereço de servidor DNS: para traduzir nomes de domínio em endereços IPv4.

📊 Estrutura da Máscara de Sub-rede   
A máscara de sub-rede é formada por uma sequência de bits “1” seguida por bits “0”:
- 1: corresponde à parte da rede.
- 0: corresponde à parte do host.

A comparação entre o endereço IPv4 e a máscara de sub-rede é feita bit a bit, usando a operação lógica AND, para determinar o endereço de rede.

📏 Comprimento do Prefixo   
Em vez de escrever a máscara em formato decimal, podemos usar o comprimento do prefixo. Ele é o número de bits “1” na máscara de sub-rede e é escrito em notação de barra, por exemplo: /24 significa que os primeiros 24 bits são da rede. Exemplo: 192.168.10.10/24 indica que os primeiros 24 bits representam a rede e os 8 restantes representam o host.

🔬 Operação AND Lógica   
A operação AND compara dois bits e retorna:
- 1 AND 1 = 1
- 0 AND 1 = 0
- 1 AND 0 = 0
- 0 AND 0 = 0

Para descobrir o endereço de rede de um host, deve ser feito um AND bit a bit entre o endereço IPv4 e a máscara de sub-rede. Exemplo:
- Endereço do host: 192.168.10.10
- Máscara: 255.255.255.0 (/24)
- Resultado (endereço de rede): 192.168.10.0

🏠 Tipos de Endereços em uma Rede   
Dentro de cada rede existem três tipos de endereços:
- Endereço de rede: representa a rede inteira.
  - Possui todos os bits de host como 0.
  - Não pode ser atribuído a um dispositivo.
- Endereços de host: identificam dispositivos individuais na rede.
  - Podem ter qualquer combinação de bits na parte do host, exceto todos 0 (endereço de rede) ou todos 1 (endereço de difusão).
  - Todos os hosts na rede compartilham os mesmos bits de rede.
- Endereço de difusão (broadcast): usado para enviar pacotes a todos os dispositivos da rede.
  - Possui todos os bits de host como 1.
  - Também não pode ser atribuído a um host.

📌 Primeiro e Último Endereço de Host   
- Primeiro host: todos os bits de host são 0, exceto o último bit que é 1.
- Último host: todos os bits de host são 1, exceto o último bit que é 0.

No exemplo 192.168.10.0/24:
- Primeiro host: 192.168.10.1
- Último host: 192.168.10.254

Endereços entre esses valores podem ser atribuídos a dispositivos.

<a name="item11.02.01"><h4>11.2.1 Atividade - ANDing to Determine the Network Address</h4></a>[Back to summary](#item11)

Nesta atividade foi utilizada a operação AND para determinar o endereço de rede em formatos binário e decimal pontilhado:
- Host Address: 10.3.33.55
- Subnet Mask: 255.255.255.192
- Host Address in binary: 00001010 00000011 00100001 00110111
- Subnet Mask in binary: 11111111 11111111 11111111 11000000
- Network Address in binary: 00001010 00000011 00100001 00000000
- Network Address in decimal: 10.3.33.0/24

<a name="item11.03"><h4>11.3 Unicast, broadcast e multicast IPv4</h4></a>[Back to summary](#item11)

📬 Transmissão Unicast   
A transmissão unicast ocorre quando um dispositivo envia dados para um único destinatário. O pacote contém um endereço de destino unicast, identificando apenas o host que deve receber a mensagem. O endereço de origem também é sempre unicast, já que o pacote parte de um único dispositivo. No IPv4, os endereços unicast de host estão no intervalo de 1.1.1.1 a 223.255.255.255, embora muitos desses endereços sejam reservados para usos especiais. 

🌐 Transmissão Broadcast   
O broadcast permite que um dispositivo envie uma mensagem para todos os dispositivos de uma rede. Um pacote de broadcast possui todos os bits da parte do host definidos como 1, e deve ser processado por todos os hosts no mesmo domínio de difusão, ou seja, no mesmo segmento de rede. Existem diferentes tipos de broadcast: um broadcast limitado, enviado para 255.255.255.255, alcança todos os hosts na rede local; já o broadcast direcionado é enviado para o endereço de broadcast específico de cada rede, que é o endereço mais alto da rede, onde todos os bits de host são 1. Por exemplo, na rede 192.168.1.0/24, o broadcast direcionado é 192.168.1.255.

💡 Observações sobre Broadcast   
Roteadores normalmente não encaminham broadcasts, evitando que o tráfego se propague indefinidamente. Pacotes de broadcast consomem recursos de todos os dispositivos da rede, por isso o tráfego deve ser limitado para não prejudicar o desempenho. Dividir a rede em sub-redes menores ajuda a reduzir o excesso de broadcast. Em dispositivos Cisco, transmissões direcionadas podem ser desativadas por padrão, utilizando o comando `ip directed-broadcasts`, principalmente por questões de segurança.

🔄 Transmissão Multicast   
A transmissão multicast permite que um pacote seja enviado para um grupo específico de dispositivos, economizando recursos em relação ao broadcast. Endereços multicast IPv4 estão reservados no intervalo de 224.0.0.0 a 239.255.255.255. Os dispositivos que recebem pacotes multicast são chamados de clientes multicast, e cada grupo multicast é representado por um único endereço IPv4. Um host que se inscreve em um grupo multicast processa tanto os pacotes endereçados ao seu próprio endereço unicast quanto os pacotes enviados ao endereço multicast do grupo.

Protocolos de roteamento, como OSPF, utilizam multicast para comunicação entre roteadores. Por exemplo, os roteadores habilitados com OSPF enviam pacotes para o endereço multicast 224.0.0.5, e somente os dispositivos que participam do protocolo processam esses pacotes; todos os demais os ignoram. Esse método permite reduzir o tráfego, já que um único pacote pode atingir apenas os dispositivos interessados.

<a name="item11.03.01"><h4>11.3.1 Atividade - Unicast, Broadcast, or Multicast</h4></a>[Back to summary](#item11)

Nesta atividade o objetivo consistiu em selecionar os hosts que receberia um pacote com base no tipo de endereço (unicast, broadcast, multicast).
- Endereço IP Destino: 225.5.77.126 (Multicast)
- 192.168.100.1/24 225.5.77.126 agrupar: Recebe.
- 192.168.100.5/24 225.5.77.126 agrupar: Recebe.
- 192.168.100.2/24 237.192.126.17 agrupar: Não Recebe.
- 192.168.100.4/24 237.192.126.17 agrupar: Não Recebe.
- 192.168.100.3/24: Não Recebe.

- Endereço IP Destino: 192.168.100.2 (Unicast)
- 192.168.100.1/24 225.5.77.126 agrupar: Não Recebe.
- 192.168.100.5/24 225.5.77.126 agrupar: Não Recebe.
- 192.168.100.2/24 237.192.126.17 agrupar: Recebe.
- 192.168.100.4/24 237.192.126.17 agrupar: Não Recebe.
- 192.168.100.3/24: Não Recebe.

- Endereço IP Destino: 192.168.100.255 (Broadcast)
- 192.168.100.1/24 225.5.77.126 agrupar: Recebe.
- 192.168.100.5/24 225.5.77.126 agrupar: Recebe.
- 192.168.100.2/24 237.192.126.17 agrupar: Recebe.
- 192.168.100.4/24 237.192.126.17 agrupar: Recebe.
- 192.168.100.3/24: Recebe.

<a name="item11.04"><h4>11.4 Tipos de endereços IPv4</h4></a>[Back to summary](#item11)

🌐 Tipos de endereços IPv4   
Assim como existem várias maneiras de encaminhar pacotes IPv4, também há diferentes categorias de endereços IPv4. Alguns podem sair para a Internet, outros ficam restritos à rede interna, alguns servem para testes e outros são gerados automaticamente. Com o tempo, quem trabalha com redes aprende quando cada tipo deve ser usado.

🌍 Endereços IPv4 públicos e privados   
Endereços públicos circulam livremente entre os roteadores dos provedores de Internet. Mas nem todo endereço do IPv4 pode ser usado na Internet. Parte do espaço foi reservada para endereçamento privado, usado dentro de redes internas de empresas, provedores e residências. Quando a Internet cresceu nos anos 90, a quantidade de endereços começou a ficar insuficiente. Para evitar o colapso, foram criados intervalos privados que poderiam ser reutilizados por qualquer organização. Entretanto, a solução real e definitiva para o esgotamento é o IPv6.

🔒 Blocos de endereços privados (RFC 1918)   
Esses são os blocos padronizados:
- 10.0.0.0/8 → 10.0.0.0 a 10.255.255.255
- 172.16.0.0/12 → 172.16.0.0 a 172.31.255.255
- 192.168.0.0/16 → 192.168.0.0 a 192.168.255.255

Esses intervalos atendem redes internas de todos os portes. Eles não são roteáveis na Internet.

🔁 Como o NAT entra na história   
Quando um dispositivo interno precisa acessar a Internet, o roteador deve converter o endereço privado em um endereço público antes de enviar o pacote para o ISP. Essa conversão é feita pelo NAT (Network Address Translation). Isso permite que muitos dispositivos internos compartilhem poucos endereços públicos. Apesar de ser comum pensar que NAT aumenta a segurança, o IETF não considera isso uma medida de proteção.

🛡️ DMZ e publicação de serviços   
Empresas que disponibilizam serviços públicos — como sites ou APIs — mantêm servidores com endereços públicos em uma área separada da rede, chamada DMZ. O roteador geralmente faz roteamento, NAT e funções de firewall ao mesmo tempo. Para estudos, é mais comum usar endereços privados, evitando usar endereços reais da Internet.

⚠️ Endereços IPv4 especiais   
Alguns endereços não servem para hosts comuns (como rede e broadcast) e outros têm funções específicas. Entre eles:
- Loopback: O bloco 127.0.0.0/8, especialmente 127.0.0.1, é utilizado por um host para enviar tráfego para si mesmo. Serve para testar a pilha TCP/IP local. Qualquer endereço dentro do intervalo retorna para o próprio host.
- Link-local (APIPA): O intervalo 169.254.0.0/16 é usado quando uma máquina, normalmente com DHCP habilitado, não consegue contato com o servidor DHCP. Nesse caso, ela se autoconfigura com um endereço provisório. É possível usar esse intervalo em ligações ponto a ponto, mas não é comum.
- Endereçamento clássico (Classful): Em 1981, o IPv4 era distribuído com base em classes, definidas pela RFC 790. Três delas eram destinadas a unicast. Esse modelo funcionou enquanto a Internet era pequena. Mas as classes A e B desperdiçavam um volume enorme de endereços, acelerando o esgotamento do IPv4.
  - Classe A — 0.0.0.0/8 a 127.0.0.0/8: Redes muito grandes; mais de 16 milhões de hosts.
  - Classe B — 128.0.0.0/16 a 191.255.0.0/16: Redes médias ou grandes; cerca de 65 mil hosts.
  - Classe C — 192.0.0.0/24 a 223.255.255.0/24: Redes pequenas; até 254 hosts.
  - Outras classes:
    - Classe D: multicast (224.0.0.0 a 239.0.0.0)
    - Classe E: experimental (240.0.0.0 a 255.255.255.255)

🧩 CIDR — Endereçamento sem classes   
Na metade dos anos 1990, o sistema baseado em classes foi substituído pelo CIDR, que permite criar redes com tamanhos variados usando prefixos flexíveis (como /20, /27 etc.).
Esse método é o usado até hoje e tornou a distribuição de endereços muito mais eficiente.

🏛️ Atribuição de endereços públicos   
Endereços IPv4 públicos precisam ser globais e exclusivos. Eles são controlados pela IANA, que delega grandes blocos para os RIRs (Registros Regionais da Internet). Esses RIRs repassam endereços para ISPs e organizações.

🌎 RIRs (Regional Internet Registries):
- AfriNIC: África
- APNIC: Ásia e Pacífico
- ARIN: América do Norte
- LACNIC: América Latina e parte do Caribe
- RIPE NCC: Europa, Oriente Médio e Ásia Central

Empresas podem solicitar blocos diretamente a um RIR, desde que cumpram as regras de cada região.

<a name="item11.04.01"><h4>11.4.1 Atividade - Passar ou bloquear endereços IPv4</h4></a>[Back to summary](#item11)

Nesta atividade o objetivo foi decidir se cada endereço de IP deveria passar ou ser bloqueado, dependendo se ele era um endereço público ou privado.
- 192.168.103.4: Bloquear
- 192.168.223.6: Bloquear
- 213.83.41.203: Passar
- 192.168.241.27: Bloquear
- 182.178.152.97: Passar
- 100.122.73.132: Passar
- 192.168.115.117: Bloquear
- 10.213.196.194: Bloquear
- 66.125.216.182: Passar
- 10.126.130.80: Bloquear

<a name="item11.04.02"><h4>11.4.2 Atividade - Atividade - Endereço IPv4 Privado ou Público</h4></a>[Back to summary](#item11)

Nesta atividade a proposta foi definir o tipo de rede correta entre Pública e Privada com base no endereço de IP.
- 172.16.35.2: Privada
- 192.168.3.5: Privada
- 192.0.3.15: Pública
- 64.104.0.22: Pública
- 209.165.201.30: Pública
- 192.168.11.5: Privada
- 172.16.30.30: Privada
- 10.55.3.168: Privada

<a name="item11.05"><h4>11.5 Segmentação de rede</h4></a>[Back to summary](#item11)

📢 O que é Broadcast na Rede   
Uma transmissão é uma mensagem enviada para todos os dispositivos de um segmento de rede — pense naquele e-mail enviado para toda a empresa. Em LANs Ethernet, serviços essenciais como ARP e DHCP usam broadcasts para descobrir endereços MAC ou localizar um servidor que forneça configuração IP. Assim, broadcasts são uma ferramenta necessária, mas também têm custo: todos os equipamentos do mesmo segmento precisam receber e processar cada pacote de difusão.

🔎 ARP e DHCP como Exemplos de Broadcast   
Quando um host precisa saber o MAC correspondente a um IPv4 conhecido, ele emite uma requisição ARP em broadcast. Da mesma forma, clientes DHCP enviam broadcasts para descobrir um servidor que entregue suas configurações (endereço, máscara, gateway, DNS). Esses protocolos funcionam porque alcançam todos os nós daquele mesmo domínio de difusão.

🔀 Como Switches e Roteadores Tratam Broadcasts   
Switches reproduzem broadcasts em todas as portas, exceto por aquela onde o frame foi recebido, garantindo que todos os dispositivos do mesmo segmento recebam a mensagem. Roteadores, por outro lado, não encaminham broadcasts entre interfaces: cada interface de roteador define um domínio de broadcast isolado. Por isso, uma difusão em uma LAN não alcança redes conectadas por roteadores, salvo configurações específicas.

⚠️ Problemas em Domínios de Broadcast Grandes   
Domínios de broadcast grandes (muitos hosts na mesma rede) tendem a sofrer com excesso de tráfego de difusão. Cada broadcast consome CPU e tempo de processamento dos dispositivos; quando muitos hosts geram broadcasts, a rede fica mais lenta e os dispositivos podem ter desempenho degradado. Além disso, um problema local (configuração errada, falha ou ataque) pode afetar uma parcela maior da infraestrutura.

🧩 Sub-redes como Solução   
A forma prática de mitigar isso é dividir a rede em sub-redes menores — o chamado subnetting. Ao transformar uma rede grande em várias sub-redes, cada uma vira seu próprio domínio de broadcast, e difusões são confinadas localmente. Por exemplo, transformar uma rede 172.16.0.0/16 em duas sub-redes /24 (172.16.0.0/24 e 172.16.1.0/24) reduz o alcance das difusões: um broadcast em uma sub-rede não alcançará a outra.

📈 Benefícios Extras do Subnetting   
Além de reduzir tráfego, sub-redes permitem aplicar políticas de segurança mais granulares (quem pode se comunicar com quem), isolar problemas e organizar melhor recursos por localização, função ou tipo de dispositivo. Essas divisões também tornam a rede mais escalável e resiliente contra falhas localizadas.

🧭 Como Organizar Sub-redes   
Administradores podem criar sub-redes com base no que fizer mais sentido: por prédio, por departamento, por função (servidores, estações, IoT) ou por tipo de equipamento. O importante é manter consistência e documentar o plano de endereçamento para facilitar roteamento, políticas e troubleshooting.

🛠️ Prática e Compreensão   
Entender como e por que dividir redes em sub-redes é essencial. No começo pode parecer confuso, mas com prática os conceitos de domínio de broadcast, máscara/prefixo e alocação de sub-redes ficam naturais — e se tornam ferramentas poderosas para projetar redes eficientes.

<a name="item11.06"><h4>11.6 Sub-rede de uma rede IPv4</h4></a>[Back to summary](#item11)

🧩 Por que Criar Sub-redes   
À medida que a rede cresce, dividir o espaço de endereçamento se torna indispensável. Essa divisão recebe o nome de sub-rede, e é uma das habilidades mais importantes ao trabalhar com IPv4. No início pode parecer pesado, mas com o tempo a lógica de máscaras e prefixos se torna intuitiva.

🧱 Como Sub-redes São Formadas   
Para construir sub-redes, parte dos bits destinados aos hosts é reaproveitada para representar a porção de rede. Isso acontece ao ampliar a máscara de sub-rede, o que “toma emprestado” bits da área do host.
- Mais bits para rede: mais sub-redes disponíveis.
- Mais bits para rede: menos hosts possíveis em cada sub-rede.

Esse equilíbrio é o centro de todo o subnetting.

📏 Trabalhando nos Limites dos Octetos   
Uma forma simples de criar sub-redes é usar os limites naturais dos octetos: /8, /16 e /24. Eles são fáceis de visualizar porque cada um coincide com um octeto inteiro da máscara.
- /8 (255.0.0.0): redes gigantes.
- /16 (255.255.0.0): redes muito grandes.
- /24 (255.255.255.0): redes comuns, adequadas para a maioria das LANs.

Quanto maior o prefixo, menor o número de hosts em cada sub-rede.

🏢 Exemplo: Rede 10.0.0.0/8   
Considere que uma empresa utilize o bloco privado 10.0.0.0/8. Ele permite milhões de hosts em um único domínio de broadcast — algo totalmente impraticável. A solução é quebrar esse bloco em sub-redes menores:
- Transformar em /16: Gera 256 sub-redes (10.0.0.0/16 até 10.255.0.0/16), cada uma com mais de 65 mil hosts.
- Transformar em /24: Gera 65.536 sub-redes, com 254 hosts cada. O prefixo /24 é extremamente usado porque organiza bem e facilita o planejamento.

🎯 Indo Além dos Limites Fixos   
Embora /8, /16 e /24 sejam populares, nada impede que se emprestem bits de outras posições. É muito comum pegar um bloco /24 e continuar dividindo dentro dele, ajustando o tamanho da sub-rede conforme a necessidade real de dispositivos. Essa liberdade permite criar redes bem pequenas e extremamente específicas.

🔢 Exemplo: Dividindo um /24 em Redes Menores   
Quando os bits emprestados vêm do quarto octeto, o efeito é imediato: o número de sub-redes dobra a cada bit extra, e a quantidade de hosts cai pela metade. Alguns cenários típicos:
- /25: 2 sub-redes, 126 hosts cada;
- /26: 4 sub-redes, 62 hosts cada;
- /27: 8 sub-redes, 30 hosts cada;
- /28: 16 sub-redes, 14 hosts cada;
- /29: 32 sub-redes, 6 hosts cada;
- /30: 64 sub-redes, 2 hosts cada.

Essa progressão é o que torna o subnetting tão flexível.

<a name="item11.07"><h4>11.7 Sub-rede uma barra 16 e um prefixo de barra 8</h4></a>[Back to summary](#item11)

🧩 Sub-redes com Quantidade Igual de Hosts   
Nem todas as sub-redes têm a mesma complexidade para planejar. Quando o objetivo é criar várias sub-redes idênticas — todas com a mesma quantidade de endereços disponíveis — o processo se torna mais direto: basta decidir quantos bits da parte de host serão convertidos em bits de rede.

No caso de um endereço como 172.16.0.0/16, existem 16 bits de host livres para “emprestar”. Esses bits podem ser usados para formar o número de sub-redes desejadas, sem alterar a lógica de que todas terão o mesmo tamanho. É por isso que as possibilidades de subnetting de um /16 são numerosas: há muitos bits disponíveis para manipular.

🧮 Quando a Empresa Precisa de Muitas Sub-redes   
Imagine uma organização grande, que precisa criar pelo menos 100 sub-redes a partir do endereço 172.16.0.0/16. O processo é simples:
- Começa-se a pegar bits do terceiro octeto, da esquerda para a direita.
- Empresta-se um bit por vez, até alcançar o total necessário.
- Para atingir a marca de 100 sub-redes, é preciso emprestar 7 bits, pois: 2^7 = 128 sub-redes. Isso já cobre o requisito com folga.
- Máscara Gerada ao Emprestar 7 Bits: Se a rede original é /16, e mais 7 bits são adicionados à parte de rede, o novo prefixo torna-se: 16 + 7 = /23. A máscara correspondente fica: 255.255.254.0. Terceiro octeto: 11111110 (254) e Quarto octeto: 00000000 (0).
- As sub-redes resultantes avançam de 2 em 2 no terceiro octeto: 172.16.0.0/23, 172.16.2.0/23, 172.16.4.0/23, ..., 172.16.254.0/23.
- Hosts Restantes em Cada Sub-rede /23: Depois de emprestar 7 bits, sobra 1 bit no terceiro octeto e 8 bits no quarto octeto. Total de bits de host: 1 + 8 = 9 bits. Hosts por sub-rede: 2^9 − 2 = 510 hosts. O intervalo de hosts da primeira sub-rede fica: 172.16.0.1 à 172.16.1.254.

🛰️ Quando São Necessárias Centenas ou Milhares de Sub-redes   
Agora considere um caso ainda mais extremo: Um ISP pequeno precisa criar 1000 sub-redes, e cada cliente ainda deve ter um número considerável de endereços disponíveis para usar internamente. O provedor possui o bloco 10.0.0.0/8, que oferece 24 bits de host disponíveis para empréstimo. Para descobrir o total de bits necessários: 2^10 = 1024 sub-redes Portanto, é preciso emprestar 10 bits.
- Resultado do Empréstimo de 10 Bits: Prefixo final: 8 + 10 = /18. Máscara: 255.255.192.0. Isso acontece porque:
  - Segundo octeto: todos os 8 bits emprestados.
  - Terceiro octeto: 2 bits emprestados → 11000000 (192).
- As sub-redes avançam em blocos de 64 no terceiro octeto: 10.0.0.0/18, 10.0.64.0/18, 10.0.128.0/18, 10.0.192.0/18, ..., 10.255.192.0/18.
- Capacidade de Hosts em Cada Sub-rede /18: Depois de emprestar 10 bits, sobram 14 bits de host e hosts por sub-rede: 2^14 - 2 = 16.384 hosts. Essa quantidade já é suficiente para que cada cliente desse provedor possa criar suas próprias sub-redes internas.

<a name="item11.07.01"><h4>11.7.1 Atividade - Passar ou bloquear endereços IPv4</h4></a>[Back to summary](#item11)

Nesta atividade, foi fornecido uma máscara de sub-rede em formato decimal e solicitada a representação binária dela, assim como o formato de notação de prefixo.
- Máscara de Sub-Rede: 255.255.240.0
- Máscara de Sub-Rede em Binário: 11111111 11111111 11110000 00000000
- Notação de Prefixo: /20

- Máscara de Sub-Rede: 255.255.255.192
- Máscara de Sub-Rede em Binário: 11111111 11111111 11111111 11000000
- Notação de Prefixo: /26

- Máscara de Sub-Rede: 255.255.255.252
- Máscara de Sub-Rede em Binário: 11111111 11111111 11111111 11111100
- Notação de Prefixo: /30

<a name="item11.08"><h4>11.8 Divisão em sub-redes para atender a requisitos</h4></a>[Back to summary](#item11)

🧩 Visão geral sobre subnetting com endereços públicos e privados   
Ao dividir uma rede em sub-redes, o tipo de endereço utilizado — público ou privado — influencia como o processo deve ser planejado. Em uma empresa típica, existe a parte interna da rede (intranet) e a DMZ, cada uma com necessidades diferentes.

🏢 Intranet: uso de endereços privados   
A intranet utiliza endereços IPv4 privados. Esses endereços são abundantes e não precisam ser roteados pela internet. Por isso, a empresa pode usar redes grandes, como 10.0.0.0/8, que possui muitos bits de host e facilita a criação de sub-redes de diversos tamanhos. Com um bloco como 10.0.0.0/8, é possível transformar esse espaço em várias sub-redes. Por exemplo:
- Usar uma máscara /16 gera 256 redes, cada uma com mais de 65 mil endereços disponíveis.
- Usar uma máscara /24 gera mais de 65 mil sub-redes, cada uma com 254 endereços.

O administrador pode escolher qualquer outro tamanho de prefixo — /12, /18, /20, etc. — conforme a necessidade, já que o espaço privado é amplo e flexível.

🛡️ DMZ: uso de endereços públicos   
Na DMZ ficam os recursos que precisam ser acessíveis pela internet. Como esses dispositivos precisam de endereços públicos, surge o principal problema: o IPv4 público acabou. A IANA e quase todos os RIRs já não têm mais blocos disponíveis, então cada organização normalmente possui poucos endereços públicos. Por causa dessa escassez, é obrigatório evitar desperdício. A forma de fazer isso é usar VLSM (máscaras de tamanhos diferentes), criando cada sub-rede exatamente do tamanho que precisa, sem sobrar muitos endereços.

🔧 Planejamento: quantidade de hosts × quantidade de sub-redes   
O planejamento de sub-redes envolve duas decisões:
- Quantos hosts cada sub-rede precisa suportar.
- Quantas sub-redes totais precisam existir.

Há uma relação inversa: quanto mais sub-redes são criadas, menos hosts cabem em cada uma; quanto mais hosts forem necessários, menos sub-redes poderão existir. É necessário reservar bits suficientes para atender a maior sub-rede, e os bits restantes podem ser usados para multiplicar o número total de redes. O número de hosts utilizáveis é sempre calculado como 2ⁿ − 2, porque dois endereços são reservados (rede e broadcast).

🏛️ Exemplo prático com um bloco público /22   
A empresa recebeu do provedor o bloco 172.16.0.0/22. Esse bloco tem 10 bits de host, o que permite 1022 endereços utilizáveis. A topologia tem cinco locais: a sede e quatro filiais. Cada local precisa de acesso à internet, e isso gera a necessidade de dez sub-redes (cada local precisa de sub-redes separadas para conectividade interna e para a conexão com o ISP).

A maior sub-rede precisa acomodar 40 hosts. Para comportar 40 endereços utilizáveis, são necessários 6 bits de host, porque 2⁶ − 2 = 62 hosts válidos. Como o bloco possui 10 bits de host no total, sobram 4 bits que podem ser usados para criar sub-redes. Com 4 bits disponíveis para subnetting, é possível formar 16 sub-redes, o suficiente para as 10 necessárias, ainda deixando margem para crescimento.

📌 Resultado final do planejamento   
Ao emprestar 4 bits do espaço de host do bloco 172.16.0.0/22, o prefixo passa a ser /26. A máscara correspondente é 255.255.255.192. Com isso, cada sub-rede possui 62 endereços utilizáveis, e o total de sub-redes geradas é 16. Essas sub-redes podem então ser distribuídas entre a sede, a DMZ e as quatro filiais, incluindo as redes usadas para conexão com o provedor.

<a name="item11.08.01"><h4>11.8.1 Atividade - Determinando o Número de Bits para Pegar Emprestado</h4></a>[Back to summary](#item11)

Nesta atividade o objetivo foi determinar a máscara de sub-rede (em binário, decimal e notação de prefixo) que suportaria o número de hosts determinado.
- Número de Hosts Necessários: 25
- Máscara de Sub-Rede (Binário): 11111111.11111111.11111111.11100000 
- Máscara de Sub-Rede (Decimal): 255.255.255.224
- Notação de Prefixo: /27

- Número de Hosts Necessários: 1000
- Máscara de Sub-Rede (Binário): 11111111.11111111.11111100.00000000 
- Máscara de Sub-Rede (Decimal): 255.255.252.0
- Notação de Prefixo: /22

- Número de Hosts Necessários: 75
- Máscara de Sub-Rede (Binário): 11111111.11111111.11111111.10000000 
- Máscara de Sub-Rede (Decimal): 255.255.255.128
- Notação de Prefixo: /25

- Número de Hosts Necessários: 10
- Máscara de Sub-Rede (Binário): 11111111.11111111.11111111.11110000 
- Máscara de Sub-Rede (Decimal): 255.255.255.240
- Notação de Prefixo: /28

- Número de Hosts Necessários: 500
- Máscara de Sub-Rede (Binário): 11111111.11111111.111111110.00000000 
- Máscara de Sub-Rede (Decimal): 255.255.254.0
- Notação de Prefixo: /23

<a name="item11.09"><h4>11.9 VLSM</h4></a>[Back to summary](#item11)

🧩 Por que o VLSM existe   
Quando uma rede é dividida usando apenas uma máscara fixa — por exemplo, um /16 ou um /24 — todas as sub-redes geradas têm exatamente o mesmo tamanho. Isso até funciona, mas cria um problema clássico: nem todas as partes da rede precisam de tantos endereços. Algumas sub-redes vão ficar lotadas, enquanto outras terão dezenas de endereços sobrando que nunca serão usados. No caso de endereços públicos IPv4, desperdiçar endereços é algo totalmente inviável, já que esse espaço acabou há anos. Por isso surgiu o VLSM (Variable Length Subnet Mask), que permite criar sub-redes de tamanhos diferentes dentro do mesmo bloco.

🧱 Limitações do modelo de sub-rede fixa   
No método tradicional, escolhe-se uma máscara única para toda a rede. Se a máscara for /27, por exemplo, todas as sub-redes terão 30 endereços utilizáveis. Se uma determinada parte da rede precisa de 40 hosts, a máscara terá que ser mudada para atender essa necessidade — e assim todas as sub-redes aumentam também, mesmo que nenhuma das outras precise de tantos hosts. O resultado é que se perde flexibilidade: todas as sub-redes ficam grandes demais ou pequenas demais dependendo da necessidade da maior LAN. Em ambientes com recursos públicos escassos, isso é um desperdício enorme.

🌐 Por que o IPv6 não sofre com isso   
O IPv6 tem um espaço absurdamente maior de endereços. Isso significa que economizar endereços não é uma preocupação. Exatamente por isso a transição para IPv6 é tão importante — muitos problemas clássicos de planejamento simplesmente deixam de existir. Mas, enquanto o IPv4 existir, especialmente redes públicas, o desperdício precisa ser evitado.

🛠️ Quando o problema aparece na prática   
Imagine que uma rede precise de sete sub-redes: quatro LANs e três links entre roteadores. O administrador recebe o bloco 192.168.20.0/24. Se usar o método tradicional, é possível pegar 3 bits da parte de host e gerar oito sub-redes. Cada uma dessas sub-redes terá 30 endereços utilizáveis.

Funciona? Funciona. Mas cria outro problema: os links entre roteadores só precisam de dois endereços — um para cada ponta do link. Criar sub-redes de 30 endereços para algo que só precisa de dois resulta em sobra enorme. Cada um dos três links desperdiça 28 endereços, acumulando mais de 80 endereços desperdiçados. É uma estratégia funcional, mas muito ineficiente. Além disso, como todos os bits já foram usados, não há mais espaço para gerar sub-redes menores depois. Isso limita o crescimento da topologia.

🔧 Onde entra o VLSM   
O VLSM permite subdividir uma sub-rede já existente em partes menores. Isso significa que você pode usar uma máscara maior (por exemplo, /27) para LANs que precisam de mais hosts e depois "quebrar" uma dessas sub-redes /27 em blocos menores, como /30, para atender os links dos roteadores. É exatamente isso que resolve o desperdício.

🧭 Como funciona o processo   
Pegue a rede 192.168.20.0/24. Primeiro, ela é dividida em oito sub-redes /27, suficientes para as quatro LANs e para separar as áreas da rede inicial. Até aqui, tudo segue o mesmo modelo tradicional. Agora vem a diferença: em vez de usar uma sub-rede /27 inteira para cada link de roteador, uma dessas sub-redes é subdividida novamente. A última sub-rede — que começa em 192.168.20.224/27 — é escolhida para isso.

Essa sub-rede /27 ainda possui 5 bits de host. Se forem emprestados mais 3 bits, restam 2 bits para hosts. Dois bits permitem 4 endereços, sendo 2 utilizáveis, que é exatamente o necessário para um link ponto a ponto. O resultado é um conjunto de sub-redes /30, perfeitas para enlaces entre roteadores. Com isso, três sub-redes /30 são usadas nos links e várias outras ficam disponíveis para crescimento.

📌 Estratégia recomendada ao aplicar VLSM   
Quando o VLSM é usado, existe uma regra prática fundamental: sempre começar criando a sub-rede que tem a maior necessidade de hosts. Depois disso, o bloco restante pode ser subdividido progressivamente até chegar às menores sub-redes, que normalmente são as redes de enlaces entre roteadores. Esse processo garante que nenhuma sub-rede grande fique sem espaço e permite que os blocos menores se encaixem de forma eficiente sem gerar desperdícios.

🔗 Resultado final   
Com o VLSM aplicado:
- As LANs recebem sub-redes maiores, adequadas ao número de hosts que realmente precisam.
- Os links entre roteadores usam sub-redes mínimas, sem desperdício.
- O bloco original passa a ser utilizado de forma eficiente.
- Sub-redes que antes estariam “presas” a um tamanho fixo agora podem ser adaptadas conforme a necessidade.

Além disso, a distribuição dos endereços fica padronizada: geralmente o primeiro endereço de host de cada sub-rede é atribuído à interface LAN do roteador, e os hosts usam esse endereço como gateway padrão.

<a name="item11.09.01"><h4>11.9.1 Atividade - Prática VLSM</h4></a>[Back to summary](#item11)

Nesta atividade o objetivo foi identificar e selecionar em duas tabelas os seguintes itens:
- Máscara de Sub-Rede (Decimal);
- Primeira Notação de Prefixo;
- Primeiro Intervalo de Sub-Rede Completa;
- Segundo Intervalo de Sub-Rede Completa;
- Último Intervalo de Sub-Rede Completa.

<a name="item11.10"><h4>11.10 Projeto estruturado</h4></a>[Back to summary](#item11)

🧭 A importância de planejar o endereçamento IPv4   
Antes de começar a dividir uma rede em sub-redes, é essencial montar um plano completo de endereçamento. Isso envolve entender quantas sub-redes existirão, quantos hosts cada uma deve suportar, quais dispositivos estarão conectados, onde serão usados endereços privados e onde entrarão os endereços públicos. Esse estudo inicial é o que garante que a rede possa crescer sem desorganização e é também um indicador de maturidade do administrador que está conduzindo o projeto.

🧱 Como iniciar o planejamento   
O primeiro passo é analisar toda a estrutura da rede da empresa — a intranet, a DMZ e qualquer segmento adicional. O objetivo é entender como essas áreas serão separadas em sub-redes e quais precisam de restrições mais rígidas no uso de endereços. Normalmente, a DMZ é a região onde o uso de endereços deve ser tratado com mais cuidado, já que nela costuma existir necessidade de utilizar endereços IPv4 públicos. Isso faz com que técnicas como VLSM entrem em cena para evitar desperdício.

Dentro da intranet, o cenário costuma ser mais flexível. Como a maioria das empresas utiliza faixas privadas — como o bloco 10.0.0.0/8 — existe uma quantidade enorme de endereços disponíveis. Para muitas redes, esse espaço é mais do que suficiente. Porém, empresas muito grandes e provedores de acesso podem ultrapassar até mesmo essa capacidade, o que reforça por que tantas organizações estão migrando gradualmente para o IPv6.

🧩 Combinando intranet e DMZ no plano de endereçamento   
Se a intranet usa endereços privados e a DMZ usa endereços públicos, o planejamento precisa ser detalhado. Cada parte da rede tem características específicas e exige tamanhos de sub-rede diferentes. É necessário definir claramente quantos hosts existirão em cada sub-rede e como esses endereços serão distribuídos. Além disso, o plano deve antecipar como cada endereço será utilizado: quais equipamentos exigem endereços fixos e quais podem funcionar com endereços dinâmicos entregues por DHCP. Essa organização evita conflitos, facilita auditorias, melhora o monitoramento e aumenta a segurança.

🛠️ Distribuição de endereços conforme o tipo de dispositivo   
Dentro de uma rede, cada tipo de equipamento tem características próprias de endereçamento:
- Clientes finais: Os dispositivos dos usuários geralmente recebem IP automaticamente via DHCP. Isso reduz erros e diminui a carga operacional da equipe de suporte. Como os endereços são alugados por tempo limitado, eles retornam ao pool após o vencimento, o que é essencial em ambientes com muitos dispositivos móveis e usuários temporários. Em ambientes IPv6, esse processo pode ser feito via DHCPv6 ou SLAAC.
- Servidores e periféricos críticos: Servidores internos, impressoras, equipamentos de automação e outros dispositivos que precisam ser encontrados sempre no mesmo IP devem utilizar endereços estáticos. Manter um padrão de numeração para esses equipamentos facilita muito o gerenciamento.
- Servidores expostos à Internet: Servidores que precisam ser acessados publicamente devem receber endereços IPv4 públicos. Normalmente, isso ocorre por meio de NAT, que direciona tráfego externo para o servidor interno. Já servidores que não devem ficar expostos podem ser acessados remotamente por VPN, simulando o acesso como se o usuário estivesse dentro da intranet.
- Equipamentos intermediários: Switches gerenciáveis, pontos de acesso, controladoras, firewalls e outros dispositivos de infraestrutura precisam de IPs estáticos e previsíveis, pois são essenciais para monitoramento e gerenciamento da rede.
- Gateways: Roteadores e firewalls recebem um endereço IP em cada interface, servindo como porta de saída para os hosts daquela sub-rede. Por padrão, o gateway costuma utilizar o primeiro ou o último endereço da sub-rede.

🗺️ Criando um padrão de endereçamento   
Ao desenhar o esquema final, é recomendado seguir uma lógica consistente na forma como os endereços são alocados. Separar faixas específicas para servidores, para hosts dinâmicos, para impressoras, para dispositivos de rede e para a DMZ ajuda a manter a rede organizada e simplifica atividades futuras. Quando há um padrão claro, adicionar ou remover equipamentos se torna mais rápido, filtros baseados em IP ficam mais compreensíveis e a documentação se mantém coerente com o ambiente real. Isso evita confusão, reduz erros e mantém a operação da rede mais segura e estruturada.

<a name="item11.11"><h4>11.11 Módulo Prático e Quiz</h4></a>[Back to summary](#item11)

🌐 Endereços IPv4: estrutura e partes   
Um endereço IPv4 possui 32 bits organizados de forma hierárquica: parte destinada à identificação da rede e parte reservada aos hosts. Todos os dispositivos pertencentes à mesma rede compartilham os mesmos bits da porção de rede, enquanto cada host deve ter um conjunto exclusivo de bits na parte de host. Para que um dispositivo funcione corretamente, precisa de um endereço IPv4 válido e de uma máscara de sub-rede que mostre onde termina a porção de rede e onde começa a porção de host. Essa máscara também pode ser representada pela notação de prefixo, como /24, indicando quantos bits estão definidos como 1 no início da máscara. A divisão entre rede e host é determinada pelo processo de AND lógico, onde somente 1 AND 1 resulta em 1. Em cada rede existem três tipos básicos de endereços: o endereço de rede, o conjunto de endereços usados por hosts e o endereço de broadcast.

📡 Unicast, broadcast e multicast   
Um envio unicast ocorre quando um host direciona um pacote diretamente a outro dispositivo específico. Já o broadcast é um envio de um para todos dentro da mesma rede, utilizando um endereço cujo campo de host é composto apenas por bits 1. O multicast ocupa um espaço intermediário: permite que o host envie um pacote a um grupo selecionado de dispositivos. Para isso, existe um intervalo específico de endereços IPv4 — de 224.0.0.0 até 239.255.255.255 — reservado exclusivamente para essa finalidade.

🌍 Endereços públicos, privados e especiais   
Os endereços públicos são roteáveis globalmente pela Internet, enquanto os endereços privados são usados internamente pelas organizações e não podem trafegar pela Internet sem NAT. Existem também endereços especiais, como os de loopback, que permitem que o dispositivo envie tráfego para si mesmo, e os endereços de link-local, atribuídos automaticamente por falta de DHCP. Antes da adoção de máscaras variáveis, o endereçamento IPv4 usava as classes A, B e C. A distribuição global de endereços — tanto IPv4 quanto IPv6 — é realizada pela IANA, que repassa blocos aos RIRs.

🔁 Broadcast em LANs e necessidade de sub-redes   
Em redes Ethernet, dispositivos utilizam ARP para encontrar outros hosts ou gateways. Como switches propagam broadcast por todas as portas (exceto a de entrada), um único domínio de broadcast pode crescer demais e prejudicar o desempenho da rede com tráfego desnecessário. Roteadores não encaminham esse tipo de pacote, limitando a área de impacto. Para evitar sobrecarga, divide-se a rede em domínios menores, criando sub-redes. Assim, o tráfego se mantém mais organizado e o desempenho melhora.

🧮 Criando sub-redes com máscaras estendidas   
Sub-redes IPv4 são formadas “pegando emprestado” bits da porção de host e convertendo-os em bits de rede. Quanto mais bits forem usados para criar novas sub-redes, mais sub-redes estarão disponíveis — porém com um número menor de hosts em cada uma. Sub-redes são mais simples de calcular quando se trabalha com divisões inteiras de octetos, como /8, /16 ou /24, mas também podem ser criadas utilizando qualquer quantidade de bits necessária. Em redes maiores, como uma /16, normalmente os bits começam a ser emprestados a partir do terceiro octeto.

🏛️ Intranet, DMZ e endereços públicos/privados   
Ambientes corporativos geralmente utilizam endereços privados na intranet e endereços públicos na DMZ. A intranet costuma usar blocos amplos como 10.0.0.0/8, que podem ser subdivididos com diversos comprimentos de prefixo. Na DMZ, onde ficam sistemas acessíveis via Internet, usa-se espaço público — um recurso limitado e caro — e por isso é comum aplicar VLSM para criar sub-redes menores e evitar desperdício de endereços, adequando cada sub-rede exatamente ao número de hosts necessários. Isso garante uso eficiente do bloco público disponível e mantém a organização da rede.
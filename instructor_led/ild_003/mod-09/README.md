# Fundamentos de Redes - Módulo 9   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_003 (Fundamentos de Redes)   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="25"></a>
### Module: 9. IPv4 e segmentação de rede

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

### Course Module 9 Structure:
9. <a name="item09">IPv4 e segmentação de rede</a><br>
  9.1 <a href="#item09.01">Introdução</a><br>
  9.2 <a href="#item09.02">Unicast, broadcast e multicast IPv4</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;9.2.1 <a href="#item09.02.01">Atividade - Unicast, Broadcast ou Multicast</a><br>
  9.3 <a href="#item09.03">Tipos de endereços IPv4</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;9.3.1 <a href="#item09.03.01">Atividade - Passar ou bloquear endereços IPv4</a><br>
  9.4 <a href="#item09.04">Segmentação de rede</a><br>
  9.5 <a href="#item09.05">Resumo - IPv4 e segmentação de rede</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item09.01"><h4>9.1 Introdução</h4></a>[Back to summary](#item09)

📡 Segmentação e Tipos de Endereçamento IPv4   
A eficiência na entrega de dados em uma rede depende da forma como os pacotes são direcionados aos destinatários. O protocolo IPv4 utiliza diferentes métodos de transmissão para otimizar o fluxo de informações, permitindo desde comunicações individuais até o envio de dados para grupos específicos ou para todos os dispositivos de um segmento. Além disso, a organização do espaço de endereçamento entre redes públicas e privadas é essencial para a conservação de recursos e para a segurança da infraestrutura.

🎯 Objetivo do módulo:   
- Explicar a utilização dos endereços IPv4 nos processos de comunicação e na segmentação de redes.

📘 Tópicos do módulo:   
- Unicast, broadcast e multicast IPv4: Comparação técnica entre as modalidades de transmissão direcionada, ampla e para grupos selecionados.
- Tipos de endereços IPv4: Diferenciação entre endereçamentos públicos para internet, faixas privadas para redes locais e intervalos reservados para fins técnicos.
- Segmentação de Rede: Análise do processo de sub-rede (subnetting) como estratégia para organizar o tráfego e melhorar a administração dos domínios de rede.

<a name="item09.02"><h4>9.2 Unicast, broadcast e multicast IPv4</h4></a>[Back to summary](#item09)

👤 Transmissão Unicast   
A transmissão unicast caracteriza-se pelo envio de informações de um único emissor para um único receptor específico, configurando uma comunicação um-para-um. O endereço IP de destino aponta para um dispositivo exclusivo, e o endereço de origem deve ser obrigatoriamente unicast, independentemente do tipo de comunicação realizada.

Os endereços unicast IPv4 estão compreendidos no intervalo de 1.1.1.1 a 223.255.255.255, ressalvadas as faixas reservadas para usos específicos. Nota-se que a representação de máscaras de sub-rede pode utilizar a notação CIDR, como o "/24", que equivale ao valor decimal 255.255.255.0, indicando a presença de 24 bits ativos na porção de rede.

📢 Transmissão Broadcast   
O modelo broadcast consiste na propagação de uma mensagem de um ponto para todos os demais hosts integrantes de uma rede local, definindo uma comunicação de um-para-todos. O endereço de destino para este tipo de pacote é composto por bits ativos (valor 1) em toda a sua porção de host. Diferente do IPv4, o protocolo IPv6 não utiliza este método de transmissão.

A recepção e o processamento de um pacote broadcast ocorrem obrigatoriamente em todos os dispositivos contidos no mesmo domínio de broadcast, que abrange todos os hosts em um segmento de rede. Existem duas categorias principais:
- Broadcast Limitado: Enviado ao endereço 255.255.255.255, alcançando todos os dispositivos na rede local atual.
- Broadcast Direcionado: Encaminhado a todos os hosts pertencentes a uma rede ou sub-rede específica.

Como o tráfego de broadcast consome recursos de processamento em todos os receptores e utiliza largura de banda, sua ocorrência deve ser controlada para evitar a degradação do desempenho. Roteadores atuam como fronteiras para esses domínios, não encaminhando essas transmissões por padrão, o que permite subdividir redes para isolar e reduzir o tráfego desnecessário.

👥 Transmissão Multicast   
A transmissão multicast permite que um host envie uma única mensagem para um conjunto específico de destinatários interessados, reduzindo o volume de tráfego global. Os hosts que recebem essas informações são denominados clientes multicast e utilizam serviços de software para se inscreverem em um grupo de interesse.

O intervalo reservado para o endereçamento multicast no IPv4 abrange de 224.0.0.0 a 239.255.255.255. Um dispositivo que participa de um grupo multicast processará dados enviados tanto para o seu endereço unicast individual quanto para o endereço representativo do grupo.

Esta técnica é amplamente empregada por protocolos de infraestrutura. Nota-se a aplicação no protocolo de roteamento OSPF, onde os roteadores se comunicam através do endereço multicast reservado 224.0.0.5. Equipamentos que não executam o OSPF ignoram automaticamente esses pacotes, preservando seus recursos de processamento.

<a name="item09.02.01"><h4>9.2.1 Atividade - Unicast, Broadcast ou Multicast</h4></a>[Back to summary](#item09)

- Instruções: Clique em Iniciar para visualizar o endereço de IP de destino. Em seguida, clique no host ou hosts que receberão um pacote com base no tipo de endereço (unicast, broadcast ou multicast). Clique Verificar para verificar sua resposta. Clique Novo Problemar novamente para obter um novo problema.
- 192.168.100.2 -> 192.168.100.2/24
- 192.168.100.5 -> 192.168.100.5/24
- 225.5.77.126 -> 192.168.100.1/24 e 192.168.100.5/24
- 192.168.100.255 -> Todos.

<a name="item09.03"><h4>9.3 Tipos de endereços IPv4</h4></a>[Back to summary](#item09)

🌐 Tipos de Endereçamento IPv4   
O endereçamento IPv4 é segmentado em categorias distintas conforme a finalidade de uso e o alcance na infraestrutura de rede. Enquanto alguns endereços são destinados exclusivamente à comunicação global na internet, outros são reservados para funções internas ou diagnósticos de conectividade. Nota-se que o gerenciamento adequado dessas faixas é uma responsabilidade fundamental para garantir a integridade da comunicação local e remota.

🏢 Endereços Privados e RFC 1918   
Devido à escassez de endereços IPv4 disponíveis na rede mundial, surgida com a expansão da World Wide Web (WWW), foram estabelecidos blocos de endereçamento privado para uso em redes locais (intranets). Estes intervalos, definidos pela norma RFC 1918, não possuem exclusividade global e podem ser reutilizados em diferentes organizações de forma independente. As faixas reservadas para uso privado compreendem:
- 10.0.0.0/8: Abrange o intervalo de 10.0.0.0 até 10.255.255.255.
- 172.16.0.0/12: Abrange o intervalo de 172.16.0.0 até 172.31.255.255.
- 192.168.0.0/16: Abrange o intervalo de 192.168.0.0 até 192.168.255.255.

Embora o IPv6 tenha sido desenvolvido como a solução definitiva para o esgotamento do espaço de endereçamento, o uso de IPs privados permanece como o padrão na maioria das redes corporativas e residenciais atuais.

🔄 Tradução de Endereços de Rede (NAT)   
Endereços privados não são roteáveis na internet global. Para que um host em uma intranet consiga se comunicar com um destino externo, torna-se necessário o emprego da Tradução de Endereços de Rede (NAT). Este processo é realizado, na maioria das vezes, pelo roteador de borda que conecta a rede local ao Provedor de Serviços de Internet (ISP).

O mecanismo de NAT realiza a conversão sistemática dos endereços IPv4 privados de origem em um endereço IPv4 público válido antes do encaminhamento do pacote para a internet. Pacotes que contenham endereços privados e alcancem a rede externa sem essa tradução são automaticamente descartados pelos roteadores dos ISPs, uma vez que não possuem uma identificação globalmente reconhecida para o retorno da informação.

🛑 Endereçamentos Especiais e Restritos   
Dentro do protocolo IPv4, existem identificadores que não podem ser atribuídos a hosts individuais, como os endereços de rede e de broadcast. Adicionalmente, certas faixas são reservadas para funções operacionais específicas:
- Endereços de Loopback (127.0.0.0/8): Utilizados para que um host direcione tráfego para si mesmo. O endereço 127.0.0.1 é frequentemente empregado para validar se a pilha de protocolos IP do próprio dispositivo está configurada e operando corretamente através do comando ping.
- Endereços de Link-Local ou APIPA (169.254.0.0/16): Atuam como um mecanismo de autoconfiguração. Em sistemas operacionais como o Windows, o host assume um endereço desta faixa caso não consiga obter um endereçamento via DHCP ou outro método de atribuição automática.

🏷️ Sistema de Endereçamento Classful (Legado)   
No início da estruturação da rede, a alocação de endereços era baseada em classes rígidas, definidas pelo prefixo do primeiro octeto. Essa metodologia visava organizar a distribuição conforme o porte das organizações:
- Classe A: Utilizava o prefixo /8, destinando o primeiro octeto à rede e os demais aos hosts. Com suporte a mais de 16 milhões de dispositivos por rede, esse bloco ocupava metade do espaço IPv4 disponível.
- Classe B: Operava com o prefixo /16, dividindo os bits igualmente entre rede e hosts. Suportava aproximadamente 65.000 identificadores por rede.
- Classe C: Empregava o prefixo /24, reservando apenas o último octeto para hosts, o que limitava a capacidade a 254 dispositivos por rede.
- Existem ainda as faixas de Classe D, voltada para tráfego multicast, e a Classe E, reservada exclusivamente para fins experimentais e de pesquisa.

🗺️ Evolução para o Endereçamento Sem Classe   
O sistema baseado em classes tornou-se obsoleto com a expansão da internet devido à sua ineficiência, pois gerava um desperdício massivo de endereços não utilizados em redes de grande escala. Atualmente, utiliza-se o endereçamento sem classe, que ignora as divisões fixas e aloca blocos de acordo com a necessidade real justificada pelas instituições. Essa abordagem permite uma gestão mais racional e granular dos recursos IPv4 remanescentes.

🌍 Gestão e Distribuição Global de IPs   
A coordenação mundial dos endereços IP é de responsabilidade da IANA (Internet Assigned Numbers Authority). Esta entidade distribui grandes blocos de endereçamento para cinco Registros Regionais de Internet (RIRs), que gerenciam a alocação para provedores de serviços (ISPs) e organizações em áreas geográficas específicas:
- AfriNIC: Atende a região do continente africano.
- APNIC: Responsável pela região da Ásia e do Pacífico.
- ARIN: Gerencia o endereçamento na América do Norte.
- LACNIC: Coordena a alocação na América Latina e em partes do Caribe.
- RIPE NCC: Responsável pela Europa, Oriente Médio e Ásia Central.

Os ISPs recebem seus blocos de endereçamento dos RIRs e os subdividem para fornecer conectividade aos usuários finais e empresas menores, garantindo a exclusividade e o roteamento dos endereços públicos em toda a internet.

<a name="item09.03.01"><h4>9.3.1 Atividade - Passar ou bloquear endereços IPv4</h4></a>[Back to summary](#item09)

- Instruções: Decida passar ou bloquear cada endereço IP, dependendo de ser público (a Internet) ou privado (pequena rede local). Clique em Iniciar para começar e clique em Passar ou Bloquear.
- 192.168.190.253 -> Bloquear
- 10.168.58.176 -> Bloquear
- 123.79.191.206 -> Passar
- 130.87.118.155 -> Passar
- 141.129.210.112 -> Passar
- 200.132.234.14 -> Passar
- 67.108.240.194 -> Passar
- 138.182.209.224 -> Passar

<a name="item09.04"><h4>9.4 Segmentação de rede</h4></a>[Back to summary](#item09)

📣 Domínios de Broadcast e Segmentação de Rede   
Nas redes locais do tipo Ethernet, os dispositivos utilizam mensagens de difusão (broadcast) para funções essenciais de conectividade. O Protocolo de Resolução de Endereços (ARP) emprega esse método para associar um endereço IPv4 conhecido ao respectivo endereço MAC. De forma análoga, o protocolo DHCP utiliza transmissões de broadcast para localizar servidores e obter configurações automáticas de endereçamento.

A propagação dessas mensagens varia conforme o equipamento de rede utilizado. Os switches encaminham os broadcasts por todas as suas portas ativas, exceto por aquela onde o sinal foi recebido. Em contrapartida, os roteadores estabelecem o limite físico dessas transmissões; uma mensagem de broadcast recebida em uma interface de roteador não é replicada para as demais interfaces, definindo assim o perímetro de um domínio de broadcast.

📉 Impactos de Domínios de Broadcast Extensos   
A existência de redes com um número excessivo de hosts interconectados em um único domínio de broadcast pode acarretar degradação no desempenho. Esse cenário exige que cada dispositivo conectado aceite e processe todos os pacotes de difusão circulantes, o que consome recursos de processamento e largura de banda desnecessários, resultando em lentidão nas operações de rede.

✂️ Sub-redes e Divisão Lógica   
A solução para mitigar o tráfego excessivo consiste na fragmentação de um domínio de broadcast grande em segmentos menores, processo tecnicamente denominado subdivisão em sub-redes. Através da manipulação dos bits destinados aos hosts no endereço IP — como a transição de um prefixo de rede mais amplo para um mais específico — criam-se redes lógicas independentes que restringem a propagação das mensagens de broadcast aos seus próprios limites.

🛡️ Vantagens e Critérios de Organização   
A implementação de sub-redes oferece benefícios que transcendem a melhoria de performance:
- Políticas de Segurança: Permite ao administrador estabelecer regras de acesso específicas, determinando quais segmentos podem trocar informações entre si.
- Isolamento de Falhas: Reduz o impacto de problemas de hardware, configurações equivocadas ou atividades maliciosas, limitando os efeitos ao segmento afetado.
- Organização Estruturada: Facilita o gerenciamento através de agrupamentos lógicos baseados em localização geográfica, função departamental ou categoria de dispositivo, como servidores, impressoras e estações de trabalho.

A compreensão detalhada do processo de divisão em sub-redes é uma competência fundamental para a administração eficiente de infraestruturas de rede, permitindo o escalonamento e o controle rigoroso do tráfego de dados.

<a name="item09.05"><h4>9.5 Resumo - IPv4 e segmentação de rede</h4></a>[Back to summary](#item09)

👤 Comunicação Unicast   
A transmissão unicast é o modelo de comunicação direta entre um único remetente e um único destinatário. Nesse formato, o pacote carrega um endereço IP específico que identifica apenas um host na rede. É importante notar que, embora o destino possa variar em outros modos, o endereço de origem é sempre unicast, representando o ponto único de onde a informação partiu.

📢 Transmissão em Broadcast   
O broadcast permite que um dispositivo envie uma informação simultaneamente para todos os outros integrantes de um mesmo domínio de rede. Existem variantes limitadas, voltadas para a rede local imediata, e direcionadas a segmentos específicos. Como o tráfego de "um para todos" exige que todos os hosts processem a mensagem, os roteadores geralmente bloqueiam esse sinal para evitar congestionamentos globais.

👥 Tecnologia Multicast   
Diferente do broadcast, o multicast envia pacotes apenas para um grupo selecionado de dispositivos que manifestaram interesse em receber determinado conteúdo. Esse método economiza recursos de rede significativos, pois o host envia apenas um pacote, e a infraestrutura se encarrega de replicá-lo apenas para os membros do grupo, que monitoram um endereço IP específico reservado para essa função.

🛡️ Endereços Públicos vs Privados   
A internet utiliza endereços públicos que são visíveis e roteáveis mundialmente, mas, devido à escassez, a maioria das redes internas utiliza blocos de endereços privados. Esses IPs "internos" não funcionam diretamente na rede externa; por isso, o roteador utiliza a técnica de NAT para converter o endereço privado em um público, permitindo que dispositivos domésticos ou corporativos naveguem na web com segurança.

⚙️ IPs de Loopback e APIPA   
Existem faixas de endereços destinadas a funções de diagnóstico e emergência. O endereço de loopback permite que um computador envie dados para si mesmo, testando sua própria pilha de protocolos. Já o endereço APIPA é atribuído automaticamente pelo sistema operacional quando um servidor DHCP não é encontrado, permitindo que os dispositivos de uma rede local se comuniquem mesmo sem uma configuração centralizada.

📂 Sistema de Classes de Endereço   
Historicamente, os endereços IPv4 eram divididos em classes (A, B e C) para atender diferentes tamanhos de organizações, desde corporações globais com milhões de hosts até pequenas redes locais. Embora o modelo tenha evoluído, essa divisão original definiu como os blocos de IPs são distribuídos e gerenciados por entidades globais como a IANA e seus registros regionais.

🔍 Descoberta e Protocolo ARP   
Em redes locais, os dispositivos precisam descobrir o endereço físico (MAC) uns dos outros para entregar os quadros de dados. Esse processo utiliza o protocolo ARP, que envia uma pergunta em broadcast para a rede. Da mesma forma, serviços essenciais como o DHCP dependem dessas transmissões abertas para que um novo computador consiga localizar automaticamente o servidor que lhe fornecerá um IP.

✂️ Sub-redes e Domínios de Broadcast   
Quando uma rede possui muitos dispositivos, o excesso de tráfego de broadcast pode degradar o desempenho e criar riscos de segurança. A solução é a divisão em sub-redes, um processo que segmenta uma rede grande em grupos menores e mais gerenciáveis. Isso não apenas organiza o tráfego, mas também permite que administradores apliquem regras de segurança específicas para cada departamento ou setor.
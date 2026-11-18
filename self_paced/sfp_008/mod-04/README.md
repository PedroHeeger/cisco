# Networking Devices and Initial Configuration - Módulo 4   <img src="../0-aux/logo_course.png" alt="sfp_008" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">sfp_008 (Networking Devices and Initial Configuration)   <img src="../0-aux/logo_course.png" alt="sfp_008" width="auto" height="25"></a>
### Module: 4. Comutação Ethernet

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
4. <a name="item04">Comutação Ethernet</a><br>
  4.1 <a href="#item04.01">Introdução</a><br>
  4.2 <a href="#item04.02">Ethernet</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;4.2.1 <a href="../../../labs/files/lab_057/">Laboratório – Como determinar o endereço MAC de um host</a><br>
  4.3 <a href="#item04.03">Quadros Ethernet</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;4.3.1 <a href="../../../labs/files/lab_058/">Laboratório - Observar o tráfego capturado pelo Wireshark</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;4.3.2 <a href="../../../labs/files/lab_059/">Laboratório - Use o Wireshark para examinar quadros Ethernet</a><br>
  4.4 <a href="#item04.04">Endereços MAC Ethernet</a><br>
  4.5 <a href="#item04.05">A tabela de endereços MAC</a><br>
  4.6 <a href="#item04.06">Resumo do Ethernet Switching</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item04.01"><h4>4.1 Introdução</h4></a>[Back to summary](#item04)

🔌 Protocolos e Operação de Redes Comutadas Ethernet   
O padrão Ethernet constitui a base tecnológica para a maioria das redes locais cabeadas, regulando o fluxo de dados por meio de diretrizes estabelecidas nas camadas física e de enlace de dados do modelo de referência. A correta operação dessa arquitetura envolve a estruturação de unidades de transmissão de dados e o mapeamento de identificadores de hardware por dispositivos de comutação, garantindo que o tráfego seja encaminhado de maneira eficiente e direcionada dentro do segmento de rede.

🎯 Objetivo do módulo:   
- Explicar os princípios de funcionamento, encapsulamento e encaminhamento de dados em uma infraestrutura baseada no padrão Ethernet.

📘 Tópicos do módulo:   
- Ethernet: Análise das atribuições e responsabilidades operacionais das Camadas 1 e 2 do modelo OSI no ambiente de redes locais.
- Quadros Ethernet: Estudo da organização interna das subcamadas de enlace e sua correlação direta com os campos estruturais do quadro de dados.
- Endereços MAC Ethernet: Classificação e diferenciação técnica entre as modalidades de endereçamento físico utilizadas na identificação de interfaces.
- A tabela de endereços MAC: Funcionamento dos switches no processo de aprendizagem dinâmica, mapeamento de portas e comutação de quadros na rede.

<a name="item04.02"><h4>4.2 Ethernet</h4></a>[Back to summary](#item04)

🌐 Padronização de Redes e a Evolução da Tecnologia Ethernet   
No início da era das redes de computadores, a interconexão de dispositivos sofria com a fragmentação de mercado, pois cada fabricante desenvolvia métodos e protocolos proprietários de forma isolada. A ausência de compatibilidade impedia a comunicação entre hardwares de marcas distintas, gerando dependência tecnológica exclusiva de um único fornecedor e limitando a expansão das infraestruturas.

📈 Vantagens da Normatização Técnica   
O estabelecimento de padrões internacionais estabeleceu regras universais para o funcionamento dos ativos de rede, trazendo benefícios fundamentais para o setor de tecnologia:
- Simplificação de Projetos: Facilita o planejamento de arquiteturas de rede complexas por meio de estruturas previsíveis.
- Desenvolvimento Acelerado: Agiliza a criação de novos produtos compatíveis pela indústria de hardware e software.
- Estímulo à Concorrência: Abre o mercado para diversos fabricantes, ampliando as opções de aquisição e reduzindo custos.
- Conexões Consistentes: Assegura a integridade e a estabilidade das interconexões em ambientes multiplataforma.
- Facilidade de Capacitação: Simplifica o treinamento de profissionais da área técnica através de conceitos unificados.

🔌 A Consolidação da Tecnologia Ethernet   
Diante da necessidade de convergência, a tecnologia Ethernet estabeleceu-se como o padrão dominante para redes locais com fio (LAN). Suas especificações normativas operam de forma estrita nas Camadas 1 (Física) e 2 (Enlace) do modelo OSI, determinando as regras para a formatação e a transmissão dos dados pelo cabeamento estruturado.

🏢 O Instituto IEEE e o Comitê 802.3   
O IEEE (Instituto de Engenheiros Elétricos e Eletrônicos) é a entidade global encarregada de regulamentar, aprovar e manter as normas de conectividade industrial e sem fio. Dentro da organização, os grupos de trabalho dividem-se por numeração técnica, sendo o comitê 802.3 o responsável exclusivo pelas diretrizes da tecnologia Ethernet.

A nomenclatura adotada para diferenciar as variantes tecnológicas segue uma codificação posicional rígida. O padrão 100BASE-T, por exemplo, subdivide-se nos seguintes parâmetros:
- 100: Indica a taxa de transferência máxima nominal da interface, mensurada em Megabits por segundo (Mbps).
- BASE: Sinaliza o método de transmissão em banda base (baseband).
- T: Especifica o tipo de meio físico empregado para o transporte dos sinais, representando o cabo de par trançado (twisted pair).

⏳ Linha do Tempo e Incremento de Performance   
Desde a concepção inicial em 1973, a tecnologia Ethernet demonstrou alta capacidade de adaptação e escalabilidade. As primeiras versões comerciais operavam em taxas de 10 Mbps. O aprimoramento contínuo das especificações físicas e lógicas permitiu o alcance de velocidades de 10 Gbps ou superiores nas infraestruturas modernas, mantendo a relevância da tecnologia perante o aumento exponencial da demanda por largura de banda global.

<a name="item04.03"><h4>4.3 Quadros Ethernet</h4></a>[Back to summary](#item04)

🌐 A Tecnologia Ethernet no Modelo OSI   
A Ethernet consolidou-se como a principal tecnologia para redes locais com fio (LAN), coexistindo com as redes sem fio (WLAN). Essa arquitetura baseia-se em meios físicos variados, como cabos de par trançado, links de fibra óptica e cabos coaxiais.

No modelo de referência OSI, a operação da Ethernet abrange de forma estrita a Camada 1 (Física) e a Camada 2 (Enlace de Dados). Suas diretrizes técnicas são regulamentadas pelas especificações IEEE 802.2 e 802.3, suportando taxas de transmissão nominais que evoluíram de 10 Mbps até patamares de 100 Gbps ou superiores.

🔀 Divisão Funcional: As Subcamadas LLC e MAC   
Para otimizar o processamento dos dados antes do envio ao meio físico, a Camada de Enlace é subdividida em duas camadas lógicas independentes:
- Subcamada LLC (Logical Link Control - IEEE 802.2): 
  - Atua como a interface de comunicação entre o software da rede (camadas superiores) e o hardware de conectividade (camadas inferiores).
  - Função: Inserir marcações no quadro para identificar qual protocolo da Camada de Rede (como IPv4 ou IPv6) originou o tráfego. Essa sinalização permite que múltiplos protocolos de Camada 3 utilizem simultaneamente a mesma interface de rede física.
- Subcamada MAC (Media Access Control - IEEE 802.3): 
  - Implementada diretamente nos componentes de hardware da placa de rede (NIC).
  - Função: Responsável pelo encapsulamento dos dados, provimento do endereçamento físico e controle de acesso ao meio físico de transmissão, integrando-se diretamente com as tecnologias da Camada 1.

🚦 Métodos de Acesso ao Meio Físico   
O comportamento da subcamada MAC varia de acordo com a topologia e o tipo de hardware empregado na infraestrutura:
- Redes Legadas (Half-Duplex): Em estruturas antigas baseadas em barramentos ou concentradores (hubs), o meio físico é compartilhado. Para evitar transmissões simultâneas, utiliza-se o mecanismo CSMA/CD (Acesso Múltiplo com Detecção de Portadora e Detecção de Colisão). Esse algoritmo gerencia as disputas pelo canal, identifica colisões de sinal e dita um tempo de espera (back-off) aleatório antes da retransmissão dos dados.
- Redes Modernas (Full-Duplex): As infraestruturas atuais operam por meio de switches em modo bidirecional simultâneo (full-duplex). Como cada dispositivo possui um canal de comunicação exclusivo com a porta do switch, o risco de colisões é eliminado, dispensando o uso do algoritmo CSMA/CD.

📏 Dimensionamento e Limites do Quadro Ethernet   
O tamanho estrutural de um quadro Ethernet padrão possui limites rígidos para garantir a estabilidade do tráfego. A medição padrão considera o intervalo que vai do endereço MAC de destino até o campo de checagem de erros (FCS), desconsiderando os bytes iniciais de sincronização.
- Tamanho Mínimo (64 bytes): Qualquer quadro capturado com dimensão inferior a este limite é classificado como um fragmento de colisão (runt frame) e sofre descarte automático pela interface receptora.
- Tamanho Máximo Padrão (1518 bytes): Define o teto esperado para transmissões convencionais. Caso o quadro transporte marcações específicas de rede (como tags de VLAN), este valor pode sofrer pequenas variações.
- Anomalias e Exceções: Quadros que excedem o limite do payload de 1500 bytes são denominados jumbo frames ou baby giants. Se um dispositivo receber um quadro fora dos limites operacionais permitidos pela sua configuração, o pacote é descartado e categorizado como inválido devido a prováveis distorções de sinal ou colisões no percurso.

🗟 Estrutura de Campos do Quadro Ethernet   
O encapsulamento de dados na subcamada MAC organiza os bits em uma ordem sequencial específica:
- Preâmbulo e Delimitador de Início de Quadro (SFD): Compostos por um bloco inicial de 8 bytes (7 bytes de preâmbulo e 1 byte de SFD). Esses bits servem exclusivamente para sincronizar o relógio (clock) entre os dispositivos emissores e receptores, alertando a interface de destino sobre a chegada iminente de um novo quadro.
- Endereço MAC de Destino (6 bytes): Contém o identificador físico do dispositivo receptor. A placa de rede analisa este campo para determinar se o quadro deve ser processado ou descartado. Pode representar um destino individual (unicast), um grupo (multicast) ou a totalidade da rede (broadcast).
- Endereço MAC de Origem (6 bytes): Registra a identidade física da interface de rede que gerou a transmissão.
- Tipo / Comprimento (2 bytes): Também conhecido como EtherType, este campo aponta qual protocolo da camada superior está encapsulado no campo de dados. Padrões comuns em formato hexadecimal incluem 0x800 para pacotes IPv4, 0x86DD para IPv6 e 0x806 para requisições ARP.
- Dados (46 a 1500 bytes): Aloja a unidade de dados (PDU) recebida da Camada 3. Caso o pacote original seja menor do que o mínimo exigido pela arquitetura (46 bytes de payload), ocorre o preenchimento artificial do campo com bits nulos (padding) para alcançar o tamanho mínimo de 64 bytes totais do quadro.
- Sequência de Verificação de Quadro (FCS - 4 bytes): Destinado à detecção de falhas de transmissão por meio do mecanismo de Verificação de Redundância Cíclica (CRC). O emissor calcula os dados e insere o resultado neste campo; o receptor refaz a operação matemática ao coletar o quadro. Caso os valores sejam divergentes, o que sinaliza corrupção de bits por interferência elétrica ou ruído, o quadro é imediatamente eliminado.

<a name="item04.04"><h4>4.4 Endereços MAC Ethernet</h4></a>[Back to summary](#item04)

🔢 O Sistema Numérico Hexadecimal na Infraestrutura de Rede   
Enquanto o protocolo IPv4 emprega os sistemas decimal e binário para o gerenciamento de rotas, as arquiteturas de endereçamento IPv6 e os padrões Ethernet utilizam o sistema hexadecimal (base 16). A composição desta base compreende os algarismos de 0 a 9 e as letras de A a F.

A adoção do modelo hexadecimal simplifica a visualização de dados binários extensos:
- Compactação de Bits: Um único caractere hexadecimal é capaz de consolidar exatamente quatro bits binários.
- Representação de Endereços MAC: Um endereço físico Ethernet possui uma extensão de 48 bits. Através da conversão posicional, essa cadeia complexa de bits é reduzida a uma sequência legível de apenas 12 caracteres hexadecimais.
- Agrupamento por Bytes: Um conjunto de 8 bits (1 byte), que varia do binário 00000000 ao 11111111, encontra equivalência direta no intervalo hexadecimal de 00 a FF.

Na documentação técnica e em sistemas operacionais, a identificação de valores hexadecimais ocorre por meio de sintaxes específicas para evitar confusão com números decimais. Utiliza-se habitualmente o prefixo 0x (como em 0x73), o sufixo H (73H) ou a indicação por índice subscrito (73₁₆). Nos blocos de dados, a manutenção de zeros à esquerda é mandatória para preservar a integridade estrutural do alinhamento de bits (como a indicação 0A). Para fins práticos de conversão entre decimal e hexadecimal, adota-se o sistema binário como etapa intermediária do cálculo.

🚪 Categorias de Endereçamento MAC na Camada 2   
O encaminhamento de quadros dentro de uma rede local (LAN) segmenta-se em três metodologias de comunicação distintas baseadas no destino pretendido para a informação.

🎯 1. Endereçamento Unicast   
O fluxo unicast destina-se à comunicação direta e exclusiva de um único dispositivo de origem para um único dispositivo de destino.
- Mecanismo de Entrega: A transmissão exige a associação explícita entre os cabeçalhos das Camadas 2 e 3. O pacote IP deve registrar o endereço lógico do destinatário, enquanto o quadro Ethernet deve conter o endereço MAC físico correspondente àquela interface específica.
- Protocolos de Resolução: Para mapear e associar o IP ao MAC de destino correto, o host emissor recorre ao ARP (Address Resolution Protocol) em redes IPv4, ou ao mecanismo de ND (Neighbor Discovery) em infraestruturas IPv6.
- Regra de Origem: O endereço MAC que identifica o transmissor do quadro deve ser, em todos os cenários, um endereço do tipo unicast.

📢 2. Endereçamento Broadcast (Difusão)   
O método de broadcast espalha o sinal para que o pacote seja recebido e processado por todas as estações presentes no mesmo segmento físico de rede.
- Identificação de Hardware: O quadro Ethernet de difusão utiliza como destino o endereço MAC fixo FF-FF-FF-FF-FF-FF.
- Comportamento dos Ativos: Os switches replicam o quadro por todas as suas portas ativas, exceto pela interface física por onde o tráfego ingressou. Os roteadores barram esse tipo de dado, impedindo que o broadcast ultrapasse as fronteiras da rede local.
- Identificação Lógica (IPv4): No pacote de Camada 3, a porção destinada aos hosts dentro do IP de destino deve conter apenas bits em nível lógico alto (1), resultando em endereços como 192.168.1.255.
- Casos de Uso: Essencial para a operação inicial de requisições de configuração dinâmica de IP (DHCP) e mensagens de busca do protocolo ARP.

👥 3. Endereçamento Multicast (Multidifusão)   
A engenharia de multicast permite o envio de pacotes para um grupo delimitado de dispositivos que compartilham o interesse por um determinado serviço ou fluxo de dados.
- Prefixos de Hardware:
  - Para tráfego contendo pacotes IPv4 Multicast, o endereço MAC de destino adota o prefixo inicial 01-00-5E.
  - Para tráfego baseado em IPv6 Multicast, a identificação do MAC de destino inicia-se com o prefixo 33-33.
  - Protocolos de controle de infraestrutura que não operam sobre o protocolo IP (como STP e LLDP) possuem faixas de MAC multicast exclusivas e reservadas.
- Comportamento dos Ativos: O tráfego sofre inundação nas portas do switch de forma semelhante ao broadcast, a menos que o equipamento possua recursos de filtragem lógica ativos, como a espionagem multicast (multicast snooping). Dispositivos de roteamento bloqueiam esses pacotes por padrão, exigindo configuração explícita de protocolos de roteamento multicast para permitir sua passagem.
- Escopo de IPs: O direcionamento lógico utiliza a Classe D no IPv4 (intervalo de 224.0.0.0 a 239.255.255.255) e o prefixo ff00::/8 no ambiente IPv6.

⚠️ Restrição Operacional   
Endereços do tipo broadcast e multicast são estruturados para atuar unicamente como parâmetros de destino de pacotes. A identificação de origem de uma transmissão deve permanecer sempre associada a uma identidade unicast individual.

<a name="item04.05"><h4>4.5 A tabela de endereços MAC</h4></a>[Back to summary](#item04)

🔄 Operação de Switches de Camada 2 e a Tabela de Endereços MAC   
Os comutadores (switches) de Camada 2 utilizam os endereços físicos para gerenciar o direcionamento do tráfego dentro de uma rede local. Diferente dos antigos concentradores (hubs), que replicavam os sinais elétricos por todas as interfaces indiscriminadamente, o switch toma decisões de encaminhamento inteligentes, o que evita o congestionamento e o colapso da largura de banda.

A operação deste ativo ocorre de forma isolada em relação aos dados ou protocolos encapsulados no payload do quadro. O dispositivo realiza a comutação sem analisar pacotes IPv4, mensagens ARP ou estruturas IPv6, baseando-se unicamente nas informações de cabeçalho da Camada 2 do modelo OSI.

📊 A Tabela de Endereços MAC (Tabela CAM)   
Para determinar o destino dos quadros, o switch consulta uma estrutura dinâmica interna conhecida como tabela de endereços MAC ou tabela CAM (Content Addressable Memory). Essa tabela correlaciona cada endereço físico detectado na rede à respectiva porta física do switch onde o dispositivo está conectado.

⚙️ O Mecanismo de Aprendizado (Análise da Origem)   
A construção e a manutenção da tabela CAM ocorrem de forma automatizada através da inspeção contínua de todo o tráfego que ingressa no equipamento. O processo segue duas diretrizes fixas:
- Mapeamento de Nova Identidade: Sempre que um quadro entra por uma porta, o switch examina o endereço MAC de origem. Caso esse endereço não conste na tabela, uma nova entrada é gerada, vinculando o MAC consultado ao número da porta de entrada correspondente.
- Atualização de Registros Existentes: Se o MAC de origem já estiver registrado na tabela associado àquela mesma porta, o switch reinicia o temporizador de inatividade (aging timer), cujo padrão na maioria dos hardwares é de 5 minutos. Caso o dispositivo mude de porta física, a tabela substitui imediatamente o registro antigo pelo número da interface mais atual.

🚦 O Mecanismo de Encaminhamento e Filtragem (Análise do Destino)   
Após processar a origem, o switch avalia o endereço MAC de destino indicado no quadro para definir a ação de saída:
- Unicast Conhecido (Filtragem): Se o MAC de destino estiver mapeado na tabela CAM, o switch direciona o quadro exclusivamente pela porta associada àquele endereço, bloqueando o envio pelas demais interfaces.
- Unicast Desconhecido (Inundação): Caso o endereço de destino não seja encontrado na tabela, o switch realiza a inundação (flooding), replicando o quadro por todas as portas ativas, exceto por aquela onde o tráfego foi recebido originalmente.
- Broadcast ou Multicast: Quadros direcionados a múltiplos destinos ou difusões gerais recebem o mesmo tratamento de inundação, sendo propagados por todas as portas operacionais do equipamento (com exceção da porta de origem).

🔄 Ciclo Operacional Prático: Cenário de Comunicação   
O comportamento dinâmico da tabela CAM pode ser observado no fluxo de comunicação entre dois hosts genéricos (Host A e Host D) conectados a um switch recém-inicializado:
- Fase 1: Envio Inicial do Host A para o Host D
  - O Host A transmite um quadro para a porta 1 do switch.
  - O switch intercepta o tráfego, analisa o MAC de origem e insere a identidade do Host A associada à porta 1 na tabela CAM.
  - O switch analisa o MAC de destino (Host D). Como a tabela está vazia para este endereço, o quadro é inundado por todas as outras interfaces do equipamento.
- Fase 2: Resposta do Host D para o Host A
  - O Host D processa o pacote recebido e envia uma resposta, que ingressa na porta 4 do switch.
  - O switch analisa a origem do novo quadro e registra o MAC do Host D vinculado à porta 4.
  - O switch consulta o destino (Host A) na tabela CAM. Como o registro do Host A foi armazenado na Fase 1, o switch realiza a filtragem e encaminha o tráfego exclusivamente através da porta 1.
- Fase 3: Próximas Transmissões
  - Em um envio subsequente do Host A para o Host D, o tráfego entra pela porta 1.
  - O switch valida a origem e renova o temporizador de 5 minutos para o Host A na porta 1.
  - Ao checar o destino, o MAC do Host D já consta associado à porta 4. O switch entrega o quadro diretamente pela porta 4, sem necessidade de inundar a rede.

<a name="item04.06"><h4>4.6 Resumo do Ethernet Switching</h4></a>[Back to summary](#item04)

⚡ Domínio da Tecnologia Ethernet   
A Ethernet consolidou-se como o padrão universal para conexões de redes locais cabeadas. Suas diretrizes técnicas abrangem tanto a infraestrutura de cabos e sinais elétricos quanto as regras de formatação de mensagens, operando de forma integrada nas duas primeiras camadas do modelo de referência OSI.

🏢 Padronização pelo IEEE   
O órgão encarregado de regulamentar e atualizar as evoluções da Ethernet é o IEEE, especificamente através do comitê 802.3. Ao longo dos anos, esse grupo técnico aprimorou o protocolo para suportar velocidades que variam de conexões iniciais de 10 Mbps até transmissões modernas que alcançam a faixa de 100 Gbps.

🔌 Filtre de Quadros na Placa de Rede   
Quando uma mensagem trafega pela rede, a placa de interface (NIC) de cada dispositivo realiza a checagem do endereço físico contido no pacote. Se o identificador de destino não corresponder ao endereço gravado no próprio hardware, o dispositivo descarta o restante da informação imediatamente, poupando os recursos de processamento do computador.

📚 Divisão da Camada de Enlace   
Para garantir flexibilidade e conversar tanto com o software quanto com o hardware, a camada de enlace divide-se em duas partes operacionais: a subcamada LLC (802.2), que identifica qual protocolo de rede (como IPv4 ou IPv6) está envelopado na mensagem, e a subcamada MAC, que cuida do acesso físico ao meio de transmissão e da montagem final do quadro.

📐 Anatomia do Quadro Ethernet   
Operando em modo full-duplex — que permite enviar e receber dados simultaneamente eliminando a ocorrência de colisões —, os quadros possuem tamanhos estritos entre 64 e 1518 bytes. Sua estrutura interna organiza-se em campos sequenciais que incluem sinais de sincronismo, endereços de origem e destino, tipo do protocolo, carga útil e o código FCS para detecção de erros.

🔢 Natureza do Endereço MAC   
O endereço físico é composto por uma sequência binária de 48 bits, mas, para simplificar a escrita e a leitura, é representado em formato hexadecimal com 12 caracteres. Para correspondências individuais, o emissor utiliza técnicas como o ARP no mundo IPv4 ou a Descoberta de Vizinhos (ND) no ecossistema IPv6 para descobrir o endereço físico do destinatário.

📢 Comportamento do Broadcast Ethernet   
Uma mensagem de broadcast carrega o endereço físico universal estruturado em FFFF.FFFF.FFFF. Ao receber esse tipo de pacote, o switch propaga o sinal por todas as interfaces ativas, exceto por aquela onde a mensagem entrou, e o tráfego permanece contido na rede local, sendo barrado por qualquer roteador no caminho.

👥 Particularidades do Multicast   
O tráfego destinado a grupos específicos utiliza prefixos de endereçamento reservados, começando com 01-00-5E para pacotes originados em IPv4 e 33-33 para IPv6, além de códigos específicos para protocolos de controle como o STP. O switch encaminha esses pacotes para todos os lados, a menos que possua recursos avançados de filtragem como o IGMP Snooping.

🧠 Aprendizado e a Tabela CAM   
Os switches operam na Camada 2 e guiam o tráfego consultando uma base de dados interna conhecida como tabela de endereços MAC ou tabela CAM. O equipamento ignora o conteúdo lógico da mensagem, focando exclusivamente em mapear quais dispositivos físicos pertencem a quais portas para otimizar o direcionamento dos dados.

🔄 Atualização e Inundação Dinâmica   
O mapeamento das portas ocorre de forma automatizada: o switch analisa o endereço MAC de origem de todo quadro que chega e registra a interface correspondente. Se o destino de um quadro for conhecido, ele cria um canal direto para a porta correta; caso contrário, realiza a inundação enviando o pacote para todas as saídas até que o alvo responda e revele sua localização.

🔀 Múltiplas Identidades e Saída da Rede   
Uma única interface física de um switch pode registrar diversos endereços MAC em sua tabela, cenário comum quando há outro switch interconectado na mesma porta. Por fim, quando o dispositivo de destino reside em um segmento de rede externo, o quadro é direcionado localmente para o endereço físico do roteador, que atua como o gateway da infraestrutura.
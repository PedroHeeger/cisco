# CyberOps Associate - Módulo 8   <img src="../0-aux/logo_course.png" alt="ild_002" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="../">ild_002 (CyberOps Associate)   <img src="../0-aux/logo_course.png" alt="ild_002" width="auto" height="25"></a>
### Module: 8. Protocolo de Resolução de Endereços

---

### Theme:
- Cybersecurity

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

8. <a name="item08">Protocolo de Resolução de Endereços</a><br>
  8.1 <a href="#item08.01">Introdução</a><br>
  8.2 <a href="#item08.02">MAC e IP</a><br>
  8.3 <a href="#item08.03">ARP</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;8.3.1 <a href="../../../labs/lab_043/">Laboratório - Usando Wireshark para Examinar Quadros Ethernet</a><br>
  8.4 <a href="#item08.04">Problemas do ARP</a><br>
  8.5 <a href="#item08.05">Resumo do protocolo de resolução de endereço</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item08.01"><h4>8.1 Introdução</h4></a>[Back to summary](#item08)

🔹 Resolução de Endereços em Camadas de Rede   
A entrega precisa de dados entre dispositivos exige a cooperação entre diferentes sistemas de identificação. Este módulo detalha a interação entre as camadas de enlace e de rede, demonstrando como as máquinas utilizam o protocolo de resolução de endereços para vincular identidades lógicas a identificadores físicos permanentes. Compreender essa dinâmica é essencial para garantir que o tráfego alcance o destino correto dentro de um segmento de rede e para identificar vulnerabilidades inerentes a esse processo de mapeamento.

🎯 Objetivo Geral   
- Avaliar a estrutura e o funcionamento das unidades de dados do protocolo de resolução de endereços em ambientes locais.

✅ Objetivos Específicos   
- MAC e IP: Diferenciar as responsabilidades e o escopo de atuação dos endereços físicos em relação aos endereços lógicos na comunicação de dados.
- ARP: Investigar a mecânica de funcionamento do protocolo por meio da análise detalhada dos quadros que circulam na rede.
- Problemas do ARP: Examinar o impacto das requisições constantes na eficiência do tráfego e identificar as ameaças de segurança associadas a falhas ou manipulações desse protocolo.

<a name="item08.02"><h4>8.2 MAC e IP</h4></a>[Back to summary](#item08)

🏷️ Endereçamento Físico e Lógico em Redes Ethernet   
Em uma rede LAN, a comunicação entre dispositivos depende da combinação de dois tipos de identificadores: o endereço físico (MAC) e o endereço lógico (IP). Cada um desempenha uma função distinta conforme o pacote atravessa a infraestrutura.
- Endereço MAC (Camada 2): Utilizado para a entrega de quadros entre placas de rede (NICs) dentro do mesmo segmento de rede.
- Endereço IP (Camada 3): Responsável pela identificação da origem original e do destino final, independentemente de estarem na mesma rede ou em continentes diferentes.

🏠 Comunicação na Mesma Rede Local   
Quando o dispositivo de destino reside no mesmo segmento IP da origem, o processo de entrega é direto. O quadro Ethernet contém o endereço MAC da placa de rede do destinatário final.
- Camada 2 (Quadro): O endereço MAC de destino é o do próprio servidor ou host alvo.
- Camada 3 (Pacote): O endereço IP de destino aponta para o dispositivo final na LAN.

🌐 Comunicação em Redes Remotas e o Gateway   
Caso o destino final esteja em uma rede externa, o pacote exige a intermediação de um roteador. Nesse cenário, ocorre uma distinção importante no endereçamento de Camada 2:
- MAC de Destino: O endereço físico utilizado no quadro será o da interface do Gateway Padrão (roteador local), e não o do destino final.
- IP de Destino: Permanece sendo o endereço do dispositivo remoto final.
- Analogia Postal: O envio de uma carta para outra cidade exige apenas a entrega ao balcão dos correios local. O remetente não precisa saber o caminho exato; cabe à agência (roteador) processar o endereço do destinatário (IP) e encaminhar a correspondência pelo melhor trajeto.

🔄 O Processo de Encapsulamento nos Roteadores   
Roteadores atuam como pontos de decisão baseados no endereço IP de destino. Ao receber um quadro, o roteador realiza as seguintes etapas:
- Desencapsulamento: Remove as informações da Camada 2 (MAC de origem e destino anteriores).
- Análise de Rota: Examina o endereço IP de destino para determinar o próximo salto (next hop).
- Reencapsulamento: Cria um novo quadro de enlace de dados com novos endereços MAC (ou outra tecnologia de camada 2) específicos para o próximo link.

Esse ciclo se repete em cada roteador ao longo do caminho. Enquanto os endereços IP geralmente permanecem constantes, os endereços MAC são alterados a cada salto para refletir o transporte físico entre os dispositivos intermediários.

🔗 A Conexão entre IP e MAC: Protocolo ARP   
A associação entre um endereço lógico (IPv4) e um endereço físico (MAC) em cada segmento de rede é realizada pelo ARP (Address Resolution Protocol). Sem esse mapeamento, o host de origem não conseguiria descobrir qual endereço físico deve inserir no cabeçalho do quadro Ethernet para que os dados cheguem à interface correta.

<a name="item08.03"><h4>8.3 ARP</h4></a>[Back to summary](#item08)

🛠️ Protocolo de Resolução de Endereços (ARP)   
O ARP é o protocolo responsável por realizar o mapeamento entre endereços lógicos (IPv4) e endereços físicos (MAC) em redes Ethernet. Para que um quadro de Camada 2 seja transmitido, a placa de rede de origem necessita obrigatoriamente do endereço MAC de destino. Enquanto o endereço IP é obtido via nome de domínio ou configuração, o endereço MAC correspondente deve ser descoberto dinamicamente através do ARP.

📋 Tabela ARP (Cache)   
Os mapeamentos descobertos são armazenados temporariamente na memória RAM do dispositivo em uma estrutura denominada Tabela ARP ou Cache ARP.
- Busca Local: Se o destino reside na mesma sub-rede, o host pesquisa o IP do alvo na tabela.
- Busca Remota: Se o destino pertence a uma rede externa, o host pesquisa o IP do Gateway Padrão na tabela para obter o endereço físico do roteador.
- Uso do Mapeamento: Caso a entrada exista, o MAC é inserido no quadro Ethernet e o envio ocorre imediatamente. Na ausência da entrada, inicia-se o processo de descoberta.

🔄 Mecanismo de Funcionamento: Requisição e Resposta   
Quando o mapeamento necessário não consta na cache, o protocolo executa duas etapas principais:
- Requisição ARP (Broadcast): O host envia um quadro especial para todos os dispositivos do segmento local.
  - MAC de Destino: FF-FF-FF-FF-FF-FF (Broadcast).
  - Tipo de Quadro: 0x806 (Sinaliza que os dados pertencem ao processo ARP).
  - Processamento: Todos os dispositivos da LAN recebem o quadro, mas apenas aquele que possui o endereço IPv4 solicitado processará a mensagem.
- Resposta ARP (Unicast): O dispositivo alvo responde diretamente ao solicitante original.
  - Conteúdo: Inclui o endereço MAC físico correspondente ao IP solicitado.
  - Atualização: O solicitante recebe a resposta, armazena o novo mapeamento na Tabela ARP e finaliza o encapsulamento dos pacotes pendentes.

⏳ Manutenção e Expiração   
As entradas na tabela ARP possuem características de gerenciamento temporal:
- Carimbo de Data/Hora (Timestamp): Cada registro possui um tempo de vida limitado. A ausência de tráfego para um dispositivo específico resulta na remoção automática da entrada após a expiração do tempo.
- Entradas Estáticas: Mapeamentos inseridos manualmente não expiram, exigindo remoção manual, embora o uso em redes dinâmicas seja raro.
- Descarte de Pacotes: A ausência de resposta ARP impossibilita a criação do quadro Ethernet, resultando no descarte do pacote IP original.

🌐 Evolução para IPv6   
No protocolo IPv6, a funcionalidade de resolução de endereços foi integrada ao Neighbor Discovery Protocol (NDP) através do ICMPv6. Mensagens de Solicitação de Vizinho (Neighbor Solicitation) e Anúncio de Vizinho (Neighbor Advertisement) substituem o mecanismo de broadcast do ARP, proporcionando maior eficiência na rede.

🌐 ARP e o Gateway Padrão   
Sempre que o endereço IPv4 de destino pertence a uma rede externa, o dispositivo de origem deve encaminhar o quadro para o Gateway Padrão (interface do roteador local). O processo de decisão baseia-se na comparação entre o IP de origem e o de destino através da máscara de sub-rede.
- Identificação de Rede Remota: Constatada a diferença entre as redes de Camada 3, o host não busca o endereço MAC do destino final, mas sim o endereço MAC do roteador.
- Resolução via ARP: O host consulta a tabela ARP em busca do IP do gateway. Caso o mapeamento não esteja presente, uma requisição ARP é disparada especificamente para o endereço IP do roteador local.
- Encapsulamento: O pacote IP original é encapsulado em um quadro Ethernet onde o MAC de Destino é o da interface do gateway.

⏳ Gerenciamento e Temporização do Cache ARP   
Para manter a eficiência e a precisão dos mapeamentos, as tabelas ARP são dinâmicas e gerenciadas por temporizadores internos que variam conforme o sistema operacional:
- Remoção Automática: Entradas que permanecem inativas por um período determinado são descartadas da memória RAM. Em sistemas Windows, este intervalo geralmente oscila entre 15 e 45 segundos.
- Limpeza Manual: É possível forçar a exclusão de entradas específicas ou de toda a tabela através de comandos de terminal. Após a remoção, o dispositivo deverá realizar um novo ciclo de requisição/resposta ARP para restabelecer a comunicação com os vizinhos.

🖥️ Comandos para Visualização da Tabela ARP   
A inspeção dos mapeamentos armazenados em cache é fundamental para a resolução de problemas de conectividade. Os comandos variam conforme a plataforma utilizada:
- Cisco IOS (Roteador): `show ip arp` - Exibe a lista completa de mapeamentos IP-MAC conhecidos pelo roteador.
- Windows (PC): `arp -a` - Lista todas as entradas dinâmicas e estáticas presentes no cache do host.

<a name="item08.04"><h4>8.4 Problemas do ARP</h4></a>[Back to summary](#item08)

⚠️ Desafios e Vulnerabilidades do Protocolo ARP   
O funcionamento do protocolo ARP, embora essencial para a conectividade em redes IPv4, apresenta limitações operacionais e riscos de segurança significativos devido à sua dependência de mensagens de broadcast e à falta de mecanismos nativos de autenticação.

📡 Impacto das Transmissões em Larga Escala   
Como as requisições ARP são enviadas via broadcast, todos os dispositivos do segmento de rede local são obrigados a processar esses quadros. Em condições normais, o tráfego gerado é mínimo. No entanto, cenários de "tempestade de broadcast" podem ocorrer quando centenas de dispositivos são ligados simultaneamente, gerando uma redução temporária no desempenho da rede até que os mapeamentos sejam estabelecidos. Após o preenchimento das tabelas ARP nos hosts, o volume de broadcasts diminui, minimizando o impacto nos recursos da rede.

🛡️ Falsificação e Envenenamento por ARP (ARP Spoofing)   
A ausência de validação nas respostas ARP permite a exploração por agentes maliciosos através da técnica de ARP Poisoning (Envenenamento de ARP).
- O Mecanismo do Ataque: Um invasor envia respostas ARP falsas para a rede, alegando possuir um endereço IPv4 que pertence a outro dispositivo (geralmente o Gateway Padrão).
- Consequência: O dispositivo vítima atualiza a tabela ARP com o endereço MAC do invasor. A partir desse momento, todo o tráfego destinado à internet ou a outras redes é encaminhado para o agente de ameaça, permitindo a interceptação ou manipulação dos dados.

🔒 Mitigação em Redes Corporativas   
Para proteger a infraestrutura contra esses vetores de ataque, switches de nível empresarial implementam recursos avançados de segurança:
- DAI (Dynamic ARP Inspection): Esta técnica inspeciona todas as mensagens ARP que transitam pelo switch, descartando respostas inválidas ou suspeitas que não correspondam aos mapeamentos legítimos da rede.

Embora o protocolo ARP seja inerentemente inseguro, a aplicação de controles em Camada 2 é a defesa primária utilizada por analistas de segurança para garantir a integridade do tráfego local.

<a name="item08.05"><h4>8.5 Resumo do protocolo de resolução de endereço</h4></a>[Back to summary](#item08)

🏷️ Identificação de Dispositivos   
Cada equipamento em uma rede local possui duas identidades fundamentais: o endereço IP, que funciona como uma etiqueta lógica para localizar a origem e o destino final da mensagem, e o endereço MAC, um registro físico fixado na placa de rede. Enquanto o IP pode representar destinos em qualquer lugar do mundo, o endereço físico serve exclusivamente para transportar a informação de uma interface para outra dentro da mesma vizinhança digital.

🤝 Mapeamento com ARP   
Para que um pacote IP seja entregue via cabo ou Wi-Fi, o sistema precisa descobrir o endereço físico do destinatário através do protocolo ARP. Se o destino estiver na mesma rede, o emissor pergunta abertamente a todos os dispositivos quem possui aquele IP específico; o dono legítimo responde informando seu endereço MAC, permitindo que a mensagem seja devidamente envelopada e enviada.

🗂️ Tabela de Endereços   
Os computadores mantêm uma lista temporária para agilizar a comunicação, evitando a necessidade de perguntar o endereço físico a cada nova mensagem. Antes de iniciar um envio, o sistema consulta essa tabela interna; caso a informação não esteja presente, ele inicia o processo de busca para associar o IP ao MAC correspondente e atualizar seus registros para usos futuros.

✉️ Formato da Resposta   
Diferente da busca inicial que é aberta a todos, a resposta é direcionada especificamente para quem fez o pedido, contendo os dados físicos do respondente. Essas mensagens são identificadas por um código técnico específico no cabeçalho, garantindo que o sistema operacional saiba tratar aquela informação como um dado de mapeamento de endereços.

🚪 Saída para Outras Redes   
Quando o destino final não está na mesma rede local, o processo de descoberta física foca no gateway padrão, que é a porta de saída da rede. No ambiente IPv6, essa tarefa de localizar vizinhos e roteadores é realizada de forma moderna pelo protocolo Neighbor Discovery (ND), que utiliza mensagens de solicitação e anúncio de forma similar ao método usado no IPv4.

⚡ Impacto no Desempenho   
Por envolver mensagens que atingem todos os dispositivos da rede, o processo de descoberta pode causar pequenos picos de tráfego, especialmente quando muitos aparelhos são ligados simultaneamente. No entanto, em redes corporativas saudáveis, esse impacto é passageiro e se estabiliza assim que as tabelas de endereços dos dispositivos são preenchidas.

⚠️ Riscos de Segurança   
A confiança cega no processo de resposta abre brechas para que criminosos realizem ataques de envenenamento ou falsificação de endereços. Ao responder a um pedido de mapeamento que não era para ele, um invasor pode enganar os outros computadores, fazendo com que todo o tráfego da rede passe por sua máquina antes de chegar ao destino real ou ao gateway.
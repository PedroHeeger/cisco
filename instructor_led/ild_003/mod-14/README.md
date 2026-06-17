# Fundamentos de Redes - Módulo 14   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_003 (Fundamentos de Redes)   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="25"></a>
### Module: 14. Roteamento entre redes

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

### Course Module 14 Structure:
14. <a name="item14">Roteamento entre redes</a><br>
  14.1 <a href="#item14.01">Introdução</a><br>
  14.2 <a href="#item14.02">A necessidade do Roteamento</a><br>
  14.3 <a href="#item14.03">A tabela de roteamento</a><br>
  14.4 <a href="#item14.04">Criando uma LAN</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;14.4.1 <a href="../../../pkt/files/pkt_??/">Packet Tracer - Observar o fluxo de tráfego em uma rede roteada</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;14.4.2 <a href="../../../pkt/files/pkt_??/">Packet Tracer - Criar uma LAN</a><br>
  14.5 <a href="#item14.05">Resumo de Roteamento entre Redes</a><br>
  14.6 Exame de ponto de verificação: comunicação entre redes<br>


---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item14.01"><h4>14.1 Introdução</h4></a>[Back to summary](#item14)

🛣️ Roteamento e Eficiência de Fluxo em LANs   
A gestão do tráfego em redes de dados assemelha-se ao controle de fluxos viários, onde o excesso de pacotes pode resultar em latência e degradação do desempenho. Para mitigar o congestionamento, os roteadores atuam como sistemas inteligentes de direcionamento, selecionando as trajetórias mais eficientes para a transmissão da informação. Esse processo garante que os dados alcancem o destino final através de caminhos otimizados, mantendo a estabilidade e a velocidade da comunicação entre diferentes redes locais.

🎯 Objetivo do módulo:   
- Desenvolver uma rede de área local (LAN) com conectividade integral entre todos os seus nós.

📘 Tópicos do módulo:   
- A necessidade do roteamento: Explicação sobre a importância do direcionamento de tráfego para evitar saturação e garantir a entrega de pacotes.
- A tabela de roteamento: Análise técnica de como os dispositivos de camada 3 processam informações de endereçamento para selecionar o melhor caminho.
- Criando uma LAN: Procedimentos para a implementação de uma infraestrutura de rede local totalmente funcional e interconectada.

<a name="item14.02"><h4>14.2 A necessidade do Roteamento</h4></a>[Back to summary](#item14)

🌐 Conectividade e o Conceito de Hosts Remotos   
A necessidade de comunicação em redes modernas frequentemente transcende os limites do segmento local, buscando a interação com outras residências, corporações e a rede mundial. Dispositivos situados fora da infraestrutura local são classificados como hosts remotos. Para que um pacote alcance um destinatário nessas condições, torna-se indispensável a atuação de roteadores por meio do processo de roteamento, que consiste na identificação e seleção da trajetória mais eficiente para o tráfego de dados.

🚦 O Papel do Roteador na Camada 3   
Diferente dos switches, que operam na camada de enlace e baseiam suas decisões em endereços físicos (MAC), o roteador é um dispositivo de Camada 3 (Rede) responsável por interconectar múltiplas redes IP. Localizados estrategicamente na camada de distribuição, os roteadores possuem a capacidade de decodificar e processar o cabeçalho das mensagens para fundamentar o encaminhamento no endereço IP.

O formato de um pacote IP inclui os endereços lógicos de origem e de destino, além dos dados da mensagem. O roteador analisa especificamente a porção de rede do endereço IP de destino para determinar qual das interfaces conectadas representa o melhor caminho para que a informação prossiga em direção ao seu destino final.

🔄 Dinâmica de Encaminhamento e Reencapsulamento   
A intervenção de um roteador é obrigatória sempre que a porção de rede do emissor e do receptor não coincidem. Em uma situação onde um host na rede 1.1.1.0 necessita enviar dados para a rede 5.5.5.0, a mensagem é inicialmente encaminhada ao gateway local (roteador).

Ao recepcionar o sinal, o roteador executa o desencapsulamento do quadro Ethernet para inspecionar o pacote IP interno. Após verificar o endereço de destino e identificar a interface de saída adequada, o dispositivo realiza o reencapsulamento do pacote original em um novo quadro de camada de enlace, compatível com a tecnologia do próximo segmento, antes de dar continuidade à transmissão. Esse ciclo garante que a identidade lógica da mensagem permaneça intacta enquanto a estrutura física de transporte se adapta a cada salto da jornada.

<a name="item14.03"><h4>14.3 A tabela de roteamento</h4></a>[Back to summary](#item14)

🗺️ A Inteligência do Roteamento e as Tabelas de Redes   
Os roteadores atuam como os arquitetos do tráfego de dados, gerenciando o fluxo de informações entre redes locais e remotas. Para desempenhar essa função, esses dispositivos utilizam tabelas de roteamento, que funcionam como mapas estratégicos. Diferente de um registro de hosts individuais, essas tabelas armazenam os endereços das redes e os melhores caminhos para alcançá-las.

A alimentação desses dados ocorre de duas formas principais:
- Dinamicamente: Através da troca constante de informações entre roteadores vizinhos sobre as condições da rede.
- Manualmente: Por meio da inserção estática de rotas realizada por um administrador de rede.

🛡️ Rota Padrão: A Rede de Segurança dos Dados   
A ausência de uma rede de destino na tabela de roteamento resulta, invariavelmente, no descarte do pacote pelo roteador. Para evitar a perda de informações em casos de destinos desconhecidos, configura-se uma rota padrão. Essa rota funciona como um "caminho de última instância", direcionando qualquer tráfego com destino ignorado para uma interface específica, que geralmente conecta a outro roteador com maior conhecimento da topologia global da internet.

🔄 Comunicação Local vs. Comunicação Remota   
O processo de envio de mensagens sofre uma alteração lógica profunda dependendo da localização do destinatário:
- Segmento Local: Quando a origem e o destino residem na mesma rede, a comunicação é direta. O host utiliza o protocolo ARP para descobrir o endereço físico (MAC) do destinatário, encapsula o pacote IPv4 no quadro Ethernet e realiza a entrega imediata.
- Segmento Remoto: Quando o destino pertence a outra rede, o host obrigatoriamente recorre ao roteador. Embora o endereço IP de destino no pacote seja o do host remoto, o endereço MAC de destino no quadro deve ser o da interface do roteador local.

🚪 O Gateway Padrão e a Resolução de Camada 2   
A identificação do roteador pelo host de origem ocorre através da configuração do Gateway Padrão nos parâmetros de TCP/IP. Este endereço representa a "porta de saída" da rede local. Ao identificar que o IP de destino é remoto, o host utiliza o gateway padrão para:
- Realizar uma consulta ARP e obter o endereço MAC da interface do roteador.
- Encapsular os dados de forma que o roteador aceite o quadro na camada de enlace.

A precisão na configuração do gateway padrão em cada dispositivo é vital. A ausência ou incorreção desse parâmetro impossibilita completamente a entrega de mensagens para redes externas, isolando o host dentro do seu próprio domínio local.

<a name="item14.04"><h4>14.4 Criando uma LAN</h4></a>[Back to summary](#item14)

🏗️ Definição e Evolução das LANs   
O conceito de Rede de Área Local (LAN) abrange tanto uma rede individual quanto um conjunto de redes interconectadas que operam sob uma gestão administrativa única. Historicamente, as LANs eram restritas a perímetros físicos reduzidos, como uma sala ou residência. No entanto, a infraestrutura moderna expandiu essa definição para abranger centenas de dispositivos distribuídos em múltiplos edifícios e localidades, desde que mantida a centralização do controle.

As características fundamentais dessas redes incluem a utilização predominante de tecnologias Ethernet ou Wireless e a capacidade de sustentar elevadas taxas de transferência de dados. Quando uma LAN é configurada para uso exclusivo de uma organização, permitindo o acesso apenas a membros autorizados, utiliza-se o termo Intranet.

📍 Segmento Local Único   
Em projetos de rede simplificados, é comum posicionar todos os dispositivos em um único segmento. Nessa configuração, a visibilidade entre os hosts é total, uma vez que compartilham o mesmo domínio de broadcast e utilizam o protocolo ARP para identificação mútua.

Vantagens do segmento único:
- Baixa Complexidade: Implementação facilitada e custos reduzidos de infraestrutura.
- Acessibilidade: Facilidade para que os dispositivos localizem uns aos outros.
- Velocidade Direta: Comunicação imediata entre máquinas sem intermediários de camada 3.

Desvantagens do segmento único:
- Excesso de Tráfego: O domínio de broadcast unificado pode sobrecarregar a largura de banda à medida que novos hosts são adicionados.
- Fragilidade na Segurança: Dificuldade em isolar tráfego sensível ou aplicar restrições de acesso granulares.
- Limitações de QoS: Implementação complexa de políticas de Qualidade de Serviço para priorização de tráfego.

🗺️ Segmentos Remotos e Roteamento   
Para redes que apresentam crescimento constante, a estratégia recomendada é a divisão dos hosts em segmentos remotos. Esse processo exige a utilização de roteadores para interconectar as diferentes sub-redes, criando uma hierarquia na camada de distribuição.

Vantagens da segmentação remota:
- Escalabilidade: Estrutura ideal para redes amplas e geograficamente dispersas.
- Controle de Broadcast: Redução drástica do tráfego desnecessário ao fragmentar os domínios de transmissão.
- Segurança Avançada: Capacidade de tornar máquinas invisíveis para outros departamentos e aplicar filtros de segurança rigorosos.
- Organização Lógica: Facilita a gestão de recursos por função, grupo ou localização.

Desvantagens da segmentação remota:
- Complexidade Técnica: Exige conhecimentos avançados de roteamento e configuração de interfaces.
- Custo Elevado: Necessidade de aquisição de equipamentos de camada 3 (roteadores ou switches Layer 3).
- Latência Adicional: O processamento realizado pelo roteador pode introduzir pequenos atrasos no tráfego entre segmentos.

A escolha entre manter uma rede plana ou segmentada deve basear-se no equilíbrio entre a simplicidade desejada e a necessidade de performance e proteção dos dados corporativos.

<a name="item14.05"><h4>14.5 Resumo de Roteamento entre Redes</h4></a>[Back to summary](#item14)

✂️ Necessidade de Segmentação   
Conforme uma infraestrutura cresce, manter todos os dispositivos em um único grupo torna-se inviável. A divisão da rede em segmentos menores é essencial para limitar o alcance de mensagens indesejadas, proteger setores com dados sensíveis, organizar usuários por departamentos ou conectar escritórios que estão em cidades diferentes, garantindo que a rede permaneça organizada e eficiente.

🏢 Papel da Camada de Distribuição   
Esta camada funciona como o centro de inteligência que interliga as diversas redes locais da organização. Ela é responsável por gerenciar a comunicação entre esses grupos distintos, garantindo que o tráfego interno de um departamento não sobrecarregue os outros e aplicando regras de controle para que os dados sigam apenas para onde são realmente necessários.

🚦 Inteligência do Roteador   
Diferente dos switches, que olham para o endereço físico dos aparelhos, os roteadores operam na Camada 3 e tomam decisões baseadas no endereço IP. Eles funcionam como guias que analisam o destino final da mensagem para determinar se ela deve permanecer na rede atual ou ser enviada para fora, sendo peças fundamentais sempre que a rede de origem e destino são diferentes.

🗺️ Tabela de Roteamento e Interfaces   
Cada entrada física de um roteador representa o acesso a uma rede local distinta. Para se organizar, o aparelho mantém uma tabela interna que lista todos os caminhos conhecidos; ao receber um dado, ele consulta esse mapa para encontrar a interface de saída correta, realizando o processo de roteamento ao encaminhar a informação para o próximo salto no caminho do destino.

📦 Processo de Encaminhamento   
Quando um pacote chega ao roteador, ele é aberto para que o endereço IP de destino seja verificado. Após encontrar a rota ideal, o roteador "reempacota" a informação em um novo quadro Ethernet, inserindo o endereço MAC do próximo roteador ou do host final. Esse ciclo de abrir, conferir e fechar o pacote se repete em cada nó da rede até a entrega ser concluída.

🚪 Ponto de Saída e Gateway   
Para um computador conseguir enviar dados para fora de sua vizinhança imediata, ele precisa conhecer o endereço de seu gateway padrão. Esse endereço nada mais é do que o IP da porta do roteador que está fisicamente ligada àquela rede local, servindo como a única porta de saída para qualquer comunicação que não seja destinada a um colega da mesma rede.

🔄 Atualização das Rotas   
As tabelas que guiam o tráfego podem ser preenchidas de duas formas: manualmente, por um administrador que insere os caminhos um a um, ou de forma dinâmica. No modo dinâmico, os roteadores conversam entre si, trocando informações sobre novas redes e falhas em links, permitindo que a infraestrutura se adapte automaticamente a mudanças e encontre sempre o melhor trajeto.

🌐 Características de uma LAN   
Uma rede local ou LAN é definida por estar sob uma única gestão administrativa, utilizando geralmente tecnologias como Wi-Fi e Ethernet para oferecer altas velocidades. Embora todos os hosts possam ser colocados juntos para facilitar a descoberta via ARP, dividi-los através de roteadores na camada de distribuição aumenta a segurança e a performance, apesar de exigir uma configuração mais técnica e detalhada.
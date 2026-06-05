# Fundamentos de Redes - Módulo 2   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_003 (Fundamentos de Redes)   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="25"></a>
### Module: 2. Componentes, tipos e conexões de rede

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

### Course Module 2 Structure:
2. <a name="item02">Componentes, tipos e conexões de rede</a><br>
  2.1 <a href="#item02.01">Introdução</a><br>
  2.2 <a href="#item02.02">Clientes e Servidores</a><br>
  2.3 <a href="#item02.03">Componentes de rede</a><br>
  2.4 <a href="#item02.04">Opções de conectividade com o ISP</a><br>
  2.5 <a href="#item02.05">Resumo de componentes de rede, tipos e conexões</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item02.01"><h4>2.1 Introdução</h4></a>[Back to summary](#item02)

💻 Componentes e Conectividade de Rede   
A infraestrutura de rede é composta por elementos distintos que desempenham papéis específicos na transmissão e no processamento de dados. A organização desses componentes, que incluem terminais de usuário e equipamentos de interconexão, permite que a informação trafegue de forma estruturada entre diferentes sistemas, garantindo a interoperabilidade em ambientes corporativos e domésticos.

🎯 Objetivo do módulo:   
- Explicar as tipologias de rede, as funções de seus componentes fundamentais e os métodos de conexão estabelecidos.

📘 Tópicos do módulo:   
- Clientes e Servidores: Definição dos papéis operacionais de dispositivos que solicitam e fornecem recursos dentro de uma arquitetura de rede.
- Componentes de Rede: Análise das funções desempenhadas por dispositivos finais, equipamentos intermediários e meios de transmissão física ou sem fio.
- Opções de conectividade com o ISP: Descrição técnica das modalidades de acesso oferecidas pelos provedores de serviços de internet para viabilizar a comunicação externa.

<a name="item02.02"><h4>2.2 Clientes e Servidores</h4></a>[Back to summary](#item02)

🖥️ Definição e Papéis dos Hosts   
Dispositivos conectados que participam ativamente da comunicação em uma estrutura de rede são denominados hosts. Estes equipamentos possuem a capacidade de originar e receber dados. A função específica de um host — seja como provedor de recursos ou como consumidor — é determinada pelo software instalado no sistema.

📁 Modelos de Serviços em Rede   
O modelo de interação em rede baseia-se na distinção entre provedores e solicitantes de informações:
- Servidores: São hosts configurados com softwares específicos que permitem a disponibilização de serviços, como páginas web, bancos de dados ou correio eletrônico, para outros dispositivos da rede. Cada serviço exige uma aplicação dedicada para operar corretamente.
- Clientes: Constituem os hosts que utilizam aplicações para realizar requisições e processar os dados obtidos dos servidores. Navegadores e gerenciadores de e-mail são exemplos clássicos de ferramentas instaladas no lado do cliente.
- Exemplos de Interação: No serviço de correio eletrônico, o servidor gerencia o tráfego e armazenamento das mensagens, enquanto o cliente utiliza interfaces para o acesso. Na navegação web, o servidor hospeda os arquivos que são requisitados e renderizados pelo navegador no host cliente.

🤝 Arquitetura Ponto a Ponto (P2P)   
Em cenários de pequena escala, como residências ou pequenos escritórios, é comum que um host desempenhe simultaneamente os papéis de cliente e servidor. Esta configuração caracteriza a rede ponto a ponto (P2P). 

Uma rede P2P simplificada pode ser estabelecida por meio da conexão direta entre dois dispositivos. Para expansões desse modelo, utiliza-se um equipamento de interconexão, como um switch, permitindo que múltiplos computadores troquem serviços e arquivos entre si sem a necessidade de um servidor centralizado.

⚖️ Análise de Vantagens e Limitações   
A implementação de modelos P2P apresenta características distintas que devem ser avaliadas conforme a necessidade da infraestrutura:
- Vantagens: Apresenta baixa complexidade técnica e facilidade de montagem. O custo é reduzido devido à dispensa de hardware dedicado e servidores de alto desempenho, sendo ideal para tarefas elementares como o compartilhamento de impressoras.
- Desvantagens: A ausência de uma gestão centralizada dificulta o controle da rede. Observa-se uma segurança fragilizada e falta de escalabilidade para grandes operações. Além disso, o acúmulo de funções de cliente e servidor em um único host pode acarretar lentidão e perda de performance.

🔄 Multitarefa e Sistemas Híbridos   
Hosts modernos possuem a capacidade de executar múltiplos softwares de servidor de forma simultânea, permitindo que um único equipamento atue, por exemplo, como servidor de arquivos e de web ao mesmo tempo. Da mesma forma, um host cliente pode manter conexões ativas com diversos servidores distintos para realizar tarefas variadas paralelamente.

Existem sistemas denominados híbridos, onde a localização dos recursos é mantida em um índice centralizado, enquanto o compartilhamento dos arquivos em si ocorre de forma descentralizada entre os participantes da rede. Nesse formato, os dispositivos consultam o diretório central para identificar onde o dado pretendido está armazenado.

<a name="item02.03"><h4>2.3 Componentes de rede</h4></a>[Back to summary](#item02)

🏗️ Infraestrutura e Base da Comunicação   
O alicerce que sustenta as comunicações digitais é denominado infraestrutura de rede. Este sistema atua como uma plataforma estável e confiável, permitindo que a informação transite entre pontos de origem e destinos, independentemente de a conexão ser um enlace simples entre dois equipamentos ou um sistema complexo de alcance global.

🛠️ Categorias de Componentes de Rede   
A composição física e lógica de uma rede é segmentada em três classes fundamentais de elementos:
- Dispositivos Finais: Equipamentos que servem como o ponto de partida ou o encerramento de um fluxo de dados.
- Dispositivos Intermediários: Hardwares responsáveis por conectar os dispositivos finais e gerenciar o tráfego de dados através da rede.
- Meios de Rede: Canais de comunicação que fornecem o caminho físico ou invisível para a propagação dos sinais.

🖥️ Dispositivos Finais e Endereçamento   
Os dispositivos finais, tecnicamente chamados de hosts, operam como a interface primária entre as pessoas e a infraestrutura de comunicação. Exemplos integrados a essa categoria abrangem estações de trabalho, servidores (web e de arquivos), impressoras de rede, sistemas de videoconferência, smartphones e terminais de pagamento.

Para que a troca de mensagens ocorra de forma organizada, cada host possui um endereçamento único. No início de uma transmissão, o dispositivo de origem utiliza o endereço específico do destino para garantir que os dados sejam entregues corretamente ao receptor pretendido.

🔌 Meios de Transmissão e Hardware   
O hardware da rede compreende todos os componentes físicos visíveis, como computadores, roteadores, switches e pontos de acesso sem fio. No entanto, a infraestrutura também integra elementos menos perceptíveis. Enquanto redes cabeadas utilizam mídias de cobre ou fibra óptica, as comunicações sem fio utilizam o espectro de radiofrequência ou ondas infravermelhas para transportar informações pelo ar.

Em ambientes residenciais, a infraestrutura típica engloba dispositivos finais conectados a pontos de acesso ou roteadores domésticos, utilizando tanto o cabeamento interno quanto sinais de rádio para estabelecer o acesso à rede externa.

📡 Dispositivos Intermediários e Conectividade   
O tráfego de informações é viabilizado por dispositivos intermediários, que incluem roteadores, switches LAN, switches multicamada e firewalls. Estes componentes garantem que os dados fluam de maneira eficiente pelos diversos meios de rede, que podem ser classificados em mídias de rede local (LAN), rede de longa distância (WAN) ou conexões sem fio.

<a name="item02.04"><h4>2.4 Opções de conectividade com o ISP</h4></a>[Back to summary](#item02)

🌐 Provedores de Serviços de Internet (ISP)   
Os Provedores de Serviços de Internet, conhecidos pela sigla ISP, atuam como o elo fundamental de ligação entre as redes locais (residenciais ou comerciais) e o ecossistema global da internet. Essas entidades podem ser originárias de empresas de telefonia fixa, operadoras de TV a cabo ou redes de telefonia celular. Além da conectividade básica, os ISPs frequentemente disponibilizam serviços agregados, como contas de correio eletrônico, hospedagem de páginas web, armazenamento em nuvem e sistemas de backup automatizado.

🛣️ O Backbone da Internet   
A estrutura da internet é formada por uma hierarquia de ISPs interconectados, garantindo que o tráfego de dados percorra os trajetos mais eficientes entre a origem e o destino. O núcleo dessa comunicação é o backbone (espinha dorsal) da internet, uma infraestrutura de alta performance composta majoritariamente por cabos de fibra óptica. Esses cabos são instalados de forma subterrânea para ligar cidades e de forma submarina para interconectar continentes, suportando o fluxo massivo de informações globais através de roteadores e switches de alta capacidade.

🛡️ Estrutura de Conexão Residencial   
Para o estabelecimento de uma conexão em ambientes domésticos, a configuração técnica influencia diretamente a segurança dos dados. O uso isolado de um modem para conectar um computador diretamente ao ISP é considerado uma prática insegura, pois expõe o host a ameaças externas.

A arquitetura mais comum e recomendada envolve a utilização de um roteador integrado. Este dispositivo desempenha múltiplas funções: atua como um switch para conexões cabeadas, fornece um ponto de acesso (AP) para dispositivos sem fio e gerencia o endereçamento IP interno da rede. Além da conectividade, o roteador provê uma camada essencial de proteção para os hosts internos.

📡 Tecnologias de Acesso à Rede   
A disponibilidade de métodos de conexão varia conforme a localização geográfica e a infraestrutura das operadoras. As principais modalidades de acesso para usuários finais incluem:
- Cabo: Utiliza a infraestrutura de televisão por assinatura (cabo coaxial). Oferece alta largura de banda e uma conexão permanentemente ativa, separando os dados de internet dos sinais de vídeo por meio de um modem específico.
- DSL (Linha Digital de Assinante): Opera sobre linhas telefônicas convencionais. A tecnologia segmenta a linha em três canais: um para chamadas de voz, um para recebimento de dados (download) e outro para envio (upload). A eficiência deste serviço é afetada pela qualidade da fiação e pela distância física entre a residência e a central da operadora.
- Celular: Utiliza ondas de rádio e a rede de torres de telefonia móvel. É uma alternativa viável para usuários em deslocamento ou em áreas sem infraestrutura cabeada, embora possa estar sujeita a limites de consumo de dados conforme o plano contratado.
- Satélite: Recomendada para regiões remotas ou rurais onde o cabo e o DSL são inexistentes. Requer uma antena parabólica com linha de visada desobstruída para o satélite. Embora ofereça conectividade em locais isolados, os custos de instalação e equipamentos tendem a ser mais elevados.
- Conexão Discada (Dial-up): Método legado que utiliza um modem e a linha telefônica para realizar uma chamada para o ISP. Apresenta largura de banda extremamente limitada, sendo considerada apenas em situações de emergência ou quando não há outras tecnologias disponíveis.
- Fibra Óptica: Em áreas metropolitanas densas, a fibra é levada diretamente até os imóveis. Essa tecnologia suporta as maiores taxas de transferência e permite a convergência de serviços de internet, telefonia e televisão em uma única conexão de alta velocidade.

<a name="item02.05"><h4>2.5 Resumo de componentes de rede, tipos e conexões</h4></a>[Back to summary](#item02)

🖥️ Funções dos Hosts   
Em um ecossistema de rede, qualquer computador que participa ativamente das comunicações é definido como um host. A função específica que ele desempenha, seja solicitando serviços como cliente ou fornecendo recursos como servidor, é ditada exclusivamente pelo software instalado, permitindo uma versatilidade onde um único hardware pode assumir ambos os papéis simultaneamente.

🤝 Redes Ponto a Ponto   
Ambientes domésticos ou pequenos escritórios frequentemente utilizam o modelo P2P, onde os dispositivos compartilham recursos entre si sem a necessidade de um servidor central. Embora essa arquitetura seja econômica e simples de implementar para tarefas básicas, ela carece de gerenciamento centralizado, o que compromete a segurança e a escalabilidade em comparação a redes corporativas robustas.

🏗️ Infraestrutura de Rede   
A base que sustenta toda a comunicação digital é composta por uma combinação de elementos físicos e lógicos categorizados em dispositivos finais, intermediários e meios de transmissão. Essa infraestrutura funciona como uma plataforma invisível mas essencial, garantindo que o fluxo de dados tenha um caminho estável e confiável para trafegar entre os diferentes pontos da rede.

📱 Dispositivos Finais   
Estes componentes atuam como o ponto de contato direto entre o usuário humano e a rede, servindo de interface para o envio e recebimento de dados. O grupo de dispositivos finais é vasto e inclui desde computadores e impressoras de rede até sistemas de monitoramento e terminais de pagamento móveis, todos funcionando como origem ou destino final de uma mensagem.

🏢 Papel dos Provedores ISP   
O acesso à rede mundial é viabilizado por empresas que oferecem o link de comunicação entre a estrutura privada do usuário e a espinha dorsal da internet. Esses provedores se conectam entre si em uma estrutura hierárquica organizada, garantindo que o tráfego de dados percorra o trajeto mais eficiente e curto possível para alcançar qualquer lugar do planeta.

🌍 Backbone da Internet   
A estrutura principal que mantém a internet funcionando consiste em uma malha global de alta tecnologia, composta majoritariamente por cabos de fibra ótica de alta capacidade. Equipamentos de roteamento avançados gerenciam o tráfego nessa rede central, direcionando volumes massivos de informações entre continentes com precisão e velocidade extrema.

🛰️ Opções de Conectividade   
O usuário final geralmente acessa a rede através de um roteador doméstico que centraliza funções de switch, ponto de acesso sem fio e segurança. Dependendo da localidade e da infraestrutura disponível, essa conexão pode ser estabelecida via cabo, linhas digitais DSL, redes de telefonia móvel ou até mesmo links de satélite para áreas mais remotas. Atualmente, a tecnologia mais utilizadas para redes doméstica é a fibra óptica.
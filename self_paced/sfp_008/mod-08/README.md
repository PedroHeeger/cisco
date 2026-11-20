# Networking Devices and Initial Configuration - Módulo 8   <img src="../0-aux/logo_course.png" alt="sfp_008" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">sfp_008 (Networking Devices and Initial Configuration)   <img src="../0-aux/logo_course.png" alt="sfp_008" width="auto" height="25"></a>
### Module: 8. Serviços de endereçamento IP

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
8. <a name="item08">Serviços de endereçamento IP</a><br>
  8.1 <a href="#item08.01">Introdução</a><br>
  8.2 <a href="#item08.02">Serviços DNS</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;8.2.1 <a href="../../../labs/files/lab_061/">Laboratório - Observe a resolução do DNS</a><br>
  8.3 <a href="#item08.03">Serviços DHCP</a><br>
  8.4 <a href="#item08.04">Resumo dos serviços de endereçamento IP</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item08.01"><h4>8.1 Introdução</h4></a>[Back to summary](#item08)

⚙️ Operação de Serviços de Rede: DNS e DHCP   
A automação e a simplificação do acesso aos recursos de rede baseiam-se no funcionamento coordenado de serviços essenciais da camada de aplicação. Em vez de exigir que os utilizadores memorizem sequências numéricas complexas para aceder a servidores ou que os administradores configurem manualmente cada terminal, a infraestrutura utiliza protocolos específicos para traduzir identificadores textuais em endereços lógicos e para gerir a distribuição dinâmica de parâmetros de rede, garantindo a eficiência e a escalabilidade do ambiente operacional.

🎯 Objetivo do módulo:   
- Explicar os mecanismos de operação e as interações dos serviços DNS e DHCP na infraestrutura de redes.

📘 Tópicos do módulo:   
- Serviços DNS: Explicação sobre o funcionamento do Domain Name System no processo de resolução e mapeamento de nomes de domínios em endereços IP correspondentes.
- Serviços DHCP: Descrição dos estágios de comunicação e troca de mensagens envolvidos na atribuição automatizada de parâmetros lógicos de rede aos dispositivos clientes.

<a name="item08.02"><h4>8.2 Serviços DNS</h4></a>[Back to summary](#item08)

🌐 Serviços de Endereçamento e Resolução na Camada de Aplicação   
O funcionamento prático de redes de médio e grande porte depende de serviços automatizados que operam na Camada de Aplicação (Camada 7 OSI). Memorizar sequências numéricas de endereços IP para cada recurso ou configurar manualmente os parâmetros de rede de centenas de estações de trabalho geraria uma sobrecarga de gerenciamento inviável. É nesse cenário que protocolos como o DNS e o DHCP tornam-se indispensáveis para a usabilidade e a administração da infraestrutura.

🧭 O Protocolo DNS (Domain Name System)   
Os computadores utilizam identificadores numéricos estruturados para o encaminhamento de pacotes, mas os seres humanos assimilam com maior facilidade cadeias de caracteres textuais. O DNS é o serviço responsável por realizar a tradução automatizada entre esses dois mundos, mapeando Nomes de Domínio Totalmente Qualificados (FQDNs) em seus respectivos endereços lógicos.

Essa abstração confere flexibilidade à infraestrutura. Caso o servidor de uma empresa mude de provedor ou de endereço IP, a alteração é mapeada no sistema DNS e permanece completamente transparente para o usuário final, que continua acessando o recurso pelo mesmo nome de domínio.

🔄 O Fluxo de Resolução DNS   
A obtenção de um endereço IP a partir de um nome de domínio segue cinco etapas sequenciais:
- Requisição do Usuário: O operador insere um FQDN (como www.cisco.com) no campo de endereços de um navegador web.
- Envio da Consulta: O sistema operacional cliente gera um pacote de consulta DNS e o direciona ao servidor DNS configurado em sua interface de rede.
- Processamento e Tradução: O servidor DNS recebe a mensagem e busca a correspondência do FQDN em seu banco de dados local.
- Resposta ao Cliente: O servidor local retorna uma mensagem contendo o endereço IP associado àquele nome.
- Conectividade: O host cliente armazena o IP e inicia o processo de encapsulamento para abrir a conexão direta de dados com o servidor de destino.

🗂️ Tipos de Registros de Recursos (Resource Records)   
Para organizar as diferentes funções de mapeamento, o banco de dados de um servidor DNS armazena registros categorizados por tipos específicos de uso:
- Registro A: Vincula um nome de host a um endereço lógico IPv4.
- Registro AAAA (Quad-A): Vincula um nome de host a um endereço lógico IPv6.
- Registro NS (Name Server): Aponta quais são os servidores de nomes autoritativos responsáveis por gerenciar aquela zona específica.
- Registro MX (Mail Exchanger): Identifica e direciona o tráfego para os servidores de correio eletrônico encarregados de processar e-mails daquele domínio.

Se o servidor DNS local não possuir um registro em seu banco de dados, ele consulta outros servidores da hierarquia global de forma recursiva. Assim que a resposta é obtida, o servidor local armazena o resultado temporariamente em sua memória cache para otimizar requisições idênticas futuras. Os sistemas operacionais dos clientes também realizam esse armazenamento local. No Windows, o estado dessa memória pode ser inspecionado por meio do utilitário de linha de comando `ipconfig /displaydns`.

🧱 Estrutura de Mensagem e Hierarquia Distribuída   
O protocolo DNS emprega um formato de mensagem único e padronizado para todas as operações (consultas, respostas, sinalizações de erro e transferências de dados entre servidores). A estrutura básica dessa mensagem subdivide-se em quatro seções principais de dados:
- Pergunta: Contém o nome do recurso e o tipo de consulta que o servidor precisa resolver.
- Resposta: Aloja os registros de recursos que trazem a solução da pergunta feita.
- Autoridade: Apresenta os registros que apontam para os servidores oficiais de controle da zona.
- Informações Adicionais: Contém dados complementares que auxiliam no processo de comunicação.

O sistema opera de forma descentralizada por meio de uma estrutura hierárquica, onde o banco de dados global é fragmentado em pequenas zonas gerenciáveis. Cada servidor DNS responde por uma porção delimitada dessa árvore de nomes, o que garante a escalabilidade do sistema.

No topo da topologia, encontram-se os Domínios de Nível Superior (TLDs), organizados para representar o propósito institucional ou o país de origem do registro:
- .com: Setor corporativo, comercial ou industrial.
- .org: Entidades e organizações sem fins lucrativos.
- .au / .co: Identificadores de base geográfica (Austrália e Colômbia, respectivamente).

🛠️ Diagnóstico de DNS via CLI: O Utilitário nslookup   
Durante a parametrização de rede de um dispositivo, os endereços dos servidores DNS são fornecidos manualmente ou via DHCP, sendo comumente herdados dos servidores do Provedor de Serviços de Internet (ISP).

Para testar a integridade e auditar as respostas desses servidores, administradores utilizam a ferramenta de linha de comando nslookup. Ao executar o comando isoladamente, o prompt exibe o nome e o IP do servidor DNS padrão do host. A partir desse terminal interativo, o profissional pode digitar qualquer FQDN para testar a resposta do servidor, alterar os tipos de registros consultados e isolar falhas de resolução lógica na infraestrutura.

<a name="item08.03"><h4>8.3 Serviços DHCP</h4></a>[Back to summary](#item08)

📡 O Protocolo DHCP e a Automação do Endereçamento Lógico   
O protocolo DHCP (Dynamic Host Configuration Protocol) gerencia a distribuição automatizada de parâmetros essenciais de rede, como endereços IP, máscaras de sub-rede, gateways padrão e servidores DNS. Esse método de atribuição automatizada é denominado endereçamento dinâmico.

A abordagem contrária é o endereçamento estático, configuração manual em que o administrador insere os dados diretamente no sistema operacional de cada host. Em ambientes corporativos de médio a grande porte, ou em redes onde o fluxo de usuários é rotineiro, o endereçamento dinâmico torna-se obrigatório para evitar o consumo excessivo de tempo técnico e falhas operacionais, como a duplicação de IPs.

⏳ O Mecanismo de Concessão e Pools de Endereços   
O servidor DHCP opera com base em um banco de dados de endereços IPs válidos conhecido como pool. Quando um cliente conecta-se ao meio físico, o servidor seleciona um endereço disponível nesse pool e o entrega ao host por um intervalo de tempo predefinido, denominado período de concessão (lease time).
- Liberação de Recursos: O endereço IP retorna automaticamente ao pool e fica disponível para reutilização assim que o tempo de concessão expira ou quando o host envia uma mensagem de liberação explícita (DHCPRELEASE).
- Flexibilidade: Esse ciclo permite a mobilidade dos usuários, que podem transitar entre diferentes redes locais obtendo conectividade imediata sem necessidade de reconfiguração de software.

Vários ativos de rede podem atuar como servidores DHCP. Em redes residenciais, essa função é executada diretamente pelo roteador de borda fornecido pelo Provedor de Serviços de Internet (ISP). Em redes corporativas, utiliza-se comumente um servidor dedicado.

Muitas redes combinam as duas abordagens de configuração: o DHCP atende aos dispositivos de usuário final (PCs, laptops e smartphones), enquanto o endereçamento estático é reservado para ativos de infraestrutura fixa, como servidores, switches, impressoras de rede e interfaces de roteadores.

🚦 O Processo de Alocação DHCPv4 (Transações DORA)   
A obtenção de um endereço dinâmico em redes IPv4 baseia-se em uma troca sequencial de quatro mensagens padronizadas, conhecida pela sigla DORA:
- Descoberta (DHCPDISCOVER): Ao inicializar ou se acoplar à mídia, o host cliente envia uma mensagem em broadcast para localizar qualquer servidor DHCP ativo no segmento local.
- Oferta (DHCPOFFER): Os servidores DHCP disponíveis respondem enviando uma proposta de concessão. Essa mensagem já inclui um endereço IP disponível, a máscara correspondente, o gateway, o servidor DNS e a duração estipulada para a locação.
- Requisição (DHCPREQUEST): Como o cliente pode receber múltiplas propostas se houver mais de um servidor na rede, ele seleciona uma delas e envia uma requisição em broadcast. Essa mensagem sinaliza qual servidor foi escolhido e avisa aos demais que suas ofertas foram recusadas. Este pacote também serve para requisitar a renovação de um IP previamente utilizado.
- Confirmação (DHCPACK): O servidor escolhido valida a requisição e finaliza o processo enviando um pacote de confirmação, oficializando a locação. Se a oferta perder a validade antes da conclusão do processo, o servidor envia uma confirmação negativa (DHCPNAK), forçando o cliente a reiniciar o fluxo a partir do envio de um novo pacote DHCPDISCOVER. Para manter o mesmo IP, o host precisa enviar uma mensagem de renovação (DHCPREQUEST) antes do vencimento do temporizador de concessão.

🌐 Particularidades do DHCP para IPv6 (DHCPv6)   
O ecossistema IPv6 introduz mudanças estruturais significativas nessa dinâmica de provisionamento. A principal divergência em relação ao modelo anterior reside no fato de que o DHCPv6 não fornece o endereço do gateway padrão. Na arquitetura IPv6, a rota de saída da rede é obtida obrigatoriamente de forma dinâmica por meio das mensagens de Anúncio de Roteador (RA - Router Advertisement) trocadas diretamente na Camada 3.

Além disso, o DHCPv6 substitui as nomenclaturas das mensagens clássicas do DHCPv4 por novos termos correspondentes para a execução das etapas de autoconfiguração:
- Localizar o Servidor na Rede: O cliente inicia o processo enviando uma mensagem do tipo SOLICIT, que substitui o pacote DHCPDISCOVER do IPv4.
- Propor Parâmetros de Concessão: O servidor responde com uma mensagem de sinalização chamada ADVERTISE, exercendo a função que antes cabia ao pacote DHCPOFFER.
- Requisitar a Alocação Formal: O host valida as informações e encaminha uma mensagem de INFORMATION REQUEST, equivalente estrutural do pacote DHCPREQUEST.
- Confirmar a Configuração Final: O servidor encerra o ciclo de provisionamento devolvendo um pacote do tipo REPLY, assumindo o papel que pertencia à mensagem DHCPACK no IPv4.

<a name="item08.04"><h4>8.4 Resumo dos serviços de endereçamento IP</h4></a>[Back to summary](#item08)

🌐 O Propósito do Sistema DNS   
O DNS foi desenvolvido para solucionar a incompatibilidade entre a forma como os humanos e as máquinas se comunicam, traduzindo nomes de domínios fáceis de memorizar em endereços IP estruturados. Todas as transações desse protocolo, sejam elas perguntas de clientes, respostas de servidores ou notificações de erro, utilizam uma estrutura de mensagem padronizada e universal para garantir a interoperabilidade.

🗂️ Registros e Blocos de Mensagem   
Para processar os pedidos de conversão, os servidores mantêm bancos de dados populados com registros de recursos que vinculam nomes, IPs e o tipo de entrada técnica correspondente. O cabeçalho e o corpo de cada mensagem trafegada mantêm um formato fixo dividido em seções para especificar a pergunta realizada, a resposta obtida, os dados de autoridade da zona e informações adicionais úteis.

🏗️ Escalabilidade e Zonas Hierárquicas   
A resiliência e o crescimento contínuo do DNS são garantidos por sua arquitetura descentralizada, distribuída em uma árvore hierárquica dividida em zonas de controle. Cada servidor assume a responsabilidade exclusiva por um pequeno pedaço desse mapa global; quando recebe uma requisição fora de seu escopo, ele a encaminha para a autoridade competente, evitando sobrecarga em um único ponto central.

💻 Testes e Consultas com Nslookup   
Os administradores e analistas de suporte utilizam a ferramenta CLI de diagnóstico nslookup para testar e validar o status do sistema de resolução de nomes. Ao abrir o utilitário, o sistema identifica imediatamente o servidor DNS padrão da máquina e abre um prompt interativo onde o usuário pode digitar domínios para checar respostas em tempo real, isolando problemas de configuração.

⏱️ O Conceito de Concessão DHCP   
Diferente da atribuição fixa, o protocolo DHCP gerencia recursos lógicos de forma temporária através de contratos chamados tempos de concessão. Quando o prazo expira ou o dispositivo notifica sua saída enviando um aviso de liberação, o identificador IP correspondente retorna para o pool comum do servidor, permitindo que novos usuários acessem o ambiente dinamicamente.

🚦 Peculiaridades do DHCPv6   
Embora o DHCPv6 exerça um papel automatizado semelhante para redes de nova geração, ele possui regras de funcionamento distintas em relação ao seu antecessor. A principal diferença reside no fato de que o servidor DHCPv6 não repassa a rota de saída da rede; a identidade do gateway padrão deve ser adquirida de forma independente através de anúncios periódicos enviados pelos roteadores locais.

🔄 O Diálogo DHCPv4 (DORA)   
O processo de autoconfiguração IPv4 baseia-se em um fluxo estruturado de quatro mensagens fundamentais:
- O cliente inicializa o processo espalhando uma mensagem de descoberta para localizar servidores.
- Os servidores disponíveis respondem enviando uma oferta com termos de aluguel.
- O cliente devolve uma requisição formalizando qual proposta escolheu.
- O servidor selecionado encerra o ciclo enviando uma confirmação de sucesso para validar o uso do IP.

⚠️ Tratamento de Falhas na Reserva   
Caso o IP sugerido na oferta se torne indisponível antes do encerramento do contrato, o servidor rejeita o pedido final emitindo uma mensagem de negação (DHCPNAK). Essa resposta força o cliente a descartar o processo atual e reiniciar o ciclo inteiro desde o primeiro estágio de descoberta para garantir que nenhum IP duplicado entre em operação.

🔀 Equivalência de Mensagens no IPv6   
Para realizar a mesma dinâmica de configuração de rede sem a necessidade de broadcasts, o protocolo DHCPv6 utiliza um mapeamento de mensagens correspondente estruturado em quatro etapas próprias. O fluxo inicializa-se com o envio de uma solicitação (SOLICIT), recebe anúncios de servidores (ADVERTISE), formula pedidos de dados (INFORMATION REQUEST) e encerra-se com a resposta final (REPLY).
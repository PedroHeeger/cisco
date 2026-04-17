# CCNA: Introduction to Networks - Módulo 16   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_001 (CCNA: Introduction to Networks)   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="25"></a>
### Module: 16. Fundamentos de segurança de rede

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

### Course Module 16 Structure:
16. <a name="item16">Fundamentos de segurança de rede</a><br>
  16.1 <a href="#item16.01">Introdução</a><br>
  16.2 <a href="#item16.02">Ameaças à Segurança e Vulnerabilidades</a><br>
  16.3 <a href="#item16.03">Ataques à Rede</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;16.3.1 <a href="../../../labs/files/lab_053/">Laboratório - Pesquisa de Ameaças à segurança da rede</a><br>
  16.4 <a href="#item16.04">Mitigações de ataque à rede</a><br>
  16.5 <a href="#item16.05">Segurança de dispositivos</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;16.5.1 <a href="../../../pkt/files/pkt_045/">Packet Tracer - Configurar Senhas Seguras e SSH</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;16.5.2 <a href="../../../pkt/files/pkt_055/">Packet Tracer - Configurar dispositivos de rede com SSH</a><br>
  16.6 <a href="#item16.06">Módulo Prático e Quiz</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;16.6.1 <a href="../../../pkt/files/pkt_046/">Packet Tracer - Dispositivos de Rede Segura</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;16.6.2 <a href="../../../pkt/files/pkt_056/">Packet Tracer - Dispositivos de rede seguros</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item16.01"><h4>16.1 Introdução</h4></a>[Back to summary](#item16)

🔐 Fundamentos de Segurança de Rede   
A segurança de rede é um elemento essencial no funcionamento de qualquer infraestrutura conectada. Além da configuração básica de dispositivos, é necessário aplicar mecanismos que reduzam riscos e dificultem acessos não autorizados. Este módulo apresenta uma visão geral das principais ameaças existentes em redes, os tipos de ataques mais comuns e as práticas iniciais utilizadas para proteger switches e roteadores. O foco está na compreensão dos riscos e na aplicação de medidas preventivas para aumentar a confiabilidade do ambiente de rede.

🎯 Objetivo do módulo   
Configurar switches e roteadores com recursos de proteção de dispositivo para aumentar a segurança.

📘 Tópicos do módulo   
- Ameaças à segurança e vulnerabilidades: Explicar a necessidade da aplicação de medidas básicas de segurança em dispositivos de rede para reduzir pontos de exposição.
- Ataques à rede: Identificar tipos comuns de ataques e as vulnerabilidades exploradas em ambientes mal protegidos.
- Mitigação de ataques à rede: Apresentar técnicas gerais utilizadas para minimizar impactos e reduzir a probabilidade de ataques bem-sucedidos.
- Segurança de dispositivos: Descrever como configurar recursos de proteção em dispositivos de rede para atenuar ameaças e fortalecer a infraestrutura.

<a name="item16.02"><h4>16.2 Ameaças à Segurança e Vulnerabilidades</h4></a>[Back to summary](#item16)

🌐 O Impacto das Ameaças em Redes de Computadores   
A dependência atual em redes de computadores, tanto em âmbito corporativo quanto operacional, torna a segurança da infraestrutura uma prioridade crítica. Invasões realizadas por indivíduos não autorizados podem resultar em paralisações dispendiosas, perda de trabalhos e danos financeiros significativos. Os indivíduos que exploram vulnerabilidades de software, realizam ataques em hardware ou descobrem credenciais de acesso para invadir sistemas são classificados tecnicamente como agentes de ameaças.

⚠️ Classificação das Ameaças de Rede   
Após o agente da ameaça obter acesso indevido à infraestrutura, o sistema fica suscetível a quatro categorias principais de ataques diretos:
- Roubo de Informações: Consiste na invasão do sistema com o objetivo de extrair dados confidenciais, como pesquisas proprietárias e segredos industriais, os quais podem ser comercializados ou utilizados indevidamente.
- Perda e Manipulação de Dados: Caracteriza-se pela invasão com o intuito de destruir ou alterar registros do sistema. Exemplifica-se pelo envio de códigos maliciosos que formatam discos rígidos ou pela alteração não autorizada de informações em bancos de dados, como o preço de produtos.
- Roubo de Identidade: É uma ramificação do roubo de informações focada na captura de dados pessoais. O objetivo é assumir a identidade do usuário para solicitar créditos, forjar documentos e realizar transações financeiras fraudulentas, gerando perdas globais bilionárias.
- Interrupção de Serviço (DoS): Refere-se a ataques que impedem o acesso de usuários legítimos aos serviços de rede. É comumente executado mediante a sobrecarga intencional de servidores, equipamentos de tráfego ou links de comunicação.

🕳️ Conceito de Vulnerabilidade   
A vulnerabilidade define o nível de fraqueza presente em uma topologia de rede ou em seus equipamentos. Dispositivos de infraestrutura, como roteadores e firewalls, assim como endpoints (servidores e desktops), possuem graus variados de vulnerabilidades inerentes. Essas fraquezas são categorizadas em três pilares principais, que funcionam como portas de entrada para invasões.

💻 Vulnerabilidades Tecnológicas   
Essas fraquezas originam-se na arquitetura de protocolos, sistemas e hardwares utilizados na rede:
- Falhas em Protocolos TCP/IP: Protocolos fundamentais como HTTP, FTP e ICMP são estruturalmente inseguros. Serviços de gerenciamento (SNMP) e de correio eletrônico (SMTP) também herdam deficiências de segurança oriundas da concepção inicial do TCP.
- Vulnerabilidades de Sistemas Operacionais: Todas as plataformas (Windows, macOS, Linux e UNIX) apresentam brechas de segurança nativas. Tais falhas exigem atualizações constantes e são monitoradas por organizações de resposta a incidentes (como o CERT).
- Deficiências em Equipamentos de Rede: Roteadores e firewalls estão sujeitos a falhas em algoritmos de roteamento, proteção fraca por senha e vulnerabilidades nos mecanismos de autenticação.

⚙️ Vulnerabilidades de Configuração   
Estes problemas surgem da parametrização inadequada de sistemas e serviços implementados:
- Contas Desprotegidas: O uso de senhas de baixa complexidade ou a transmissão de credenciais sem criptografia facilita a interceptação por agentes maliciosos.
- Serviços de Internet Mal Ajustados: A ativação irrestrita de scripts (como JavaScript) em navegadores ou a má configuração de servidores Web (IIS, Apache) e serviços FTP expõem o ambiente a acessos indevidos.
- Configurações Padrão Inseguras: Inúmeros dispositivos e softwares entram em operação mantendo os padrões de fábrica, os quais frequentemente habilitam brechas graves de segurança.
- Equipamentos Mal Parametrizados: Erros na definição de listas de controle de acesso (ACLs) ou nas credenciais de protocolos de gerência abrem portas diretas para o controle da rede por terceiros.

📜 Vulnerabilidades de Política de Segurança   
A falta de diretrizes operacionais compromete toda a defesa sistêmica da organização:
- Ausência de Documentação: A falta de uma política de segurança escrita impossibilita a aplicação padronizada de regras de proteção.
- Conflitos Políticos Internos: Divergências entre departamentos e problemas de gestão dificultam a implementação e manutenção de diretrizes seguras.
- Falhas de Autenticação e Controle Lógico: A inexistência de auditorias e o uso continuado de senhas fracas permitem acessos sistêmicos duradouros e silenciosos, o que pode acarretar penalidades legais à gestão de TI.
- Implementações Não Homologadas: A alteração da topologia física ou a instalação de softwares que desviam das regras corporativas introduzem novos vetores de ataque.
- Inexistência de Plano de Recuperação: A ausência de um plano formal de resposta a desastres gera inoperância prolongada e falhas de comunicação em caso de ataques severos.

🏢 Ameaças Físicas a Equipamentos   
A proteção lógica de uma rede é ineficaz se o acesso físico aos dispositivos for comprometido. Um invasor com acesso local pode causar danos irreparáveis ou assumir o controle direto dos recursos. Estas ameaças dividem-se em:
- Ameaças de Hardware: Compreendem danos físicos, vandalismo ou sabotagem diretamente aplicados a servidores, estações de trabalho e cabeamentos estruturados.
- Ameaças Ambientais: Ocorrem devido à falta de climatização adequada no datacenter, expondo equipamentos a limites críticos de temperatura e umidade (excesso de condensação ou ar excessivamente seco).
- Ameaças Elétricas: Incluem oscilações e anomalias no fornecimento de energia, como picos de tensão, ruídos na linha elétrica ou blecautes completos.
- Ameaças de Manutenção: Derivam de erros operacionais, como cabeamento desorganizado, ausência de peças de reposição e danos causados por descarga eletrostática (ESD) durante o manuseio.

🛡️ Estruturação do Plano de Segurança Física   
Para neutralizar ameaças locais, é necessário elaborar e aplicar medidas restritivas de acesso às instalações:
- Bloqueio Estrutural: Trancar fisicamente as salas de telecomunicações e bloquear possíveis rotas de acesso secundárias, como tetos removíveis, pisos elevados, janelas e dutos de ventilação.
- Controle Eletrônico: Implementar sistemas de catracas, biometria ou crachás para restringir e registrar em logs todas as entradas e saídas de indivíduos nas áreas sensíveis.
- Monitoramento Visual: Empregar um circuito fechado de câmeras de segurança para garantir a vigilância contínua das áreas que abrigam os ativos da rede.

<a name="item16.03"><h4>16.3 Ataques à Rede</h4></a>[Back to summary](#item16)

🦠 Ameaças de Código Malicioso (Malware)   
Malware é a terminologia técnica para malicious software (software malicioso). Refere-se a qualquer código desenvolvido intencionalmente para causar danos, interromper operações, roubar dados ou executar ações não autorizadas em hosts e redes. As três tipologias primárias de malware são:
- Vírus: Código malicioso que se anexa a um arquivo executável ou programa legítimo (o "hospedeiro"). O vírus permanece inativo até que o usuário execute o arquivo infectado. Ao ser ativado, o vírus se propaga infectando outros programas e pode causar desde lentidão até a destruição de dados (sobrescrevendo o código hospedeiro). A disseminação depende da transferência do arquivo infectado (via rede, pendrives ou e-mail).
- Worms: Diferente do vírus, o worm é um programa autônomo. Ele não precisa se anexar a um arquivo hospedeiro nem da interação do usuário para ser executado. Os worms exploram vulnerabilidades sistêmicas para se autorreplicar e viajar de forma independente pela rede, consumindo largura de banda e recursos de processamento no processo.
- Cavalos de Troia (Trojans): Software que se disfarça de um programa legítimo e inofensivo para enganar o usuário e induzi-lo à instalação. O Trojan não se autorreplica nem infecta outros arquivos. Após ser ativado intencionalmente pelo usuário, ele executa ações danosas em segundo plano, como corromper arquivos ou criar "backdoors" (portas dos fundos), permitindo que agentes maliciosos acessem o sistema remotamente.

🎯 Categorias de Ataques à Rede   
Além da contaminação por malware, a infraestrutura de rede está sujeita a ataques diretos, que são classificados em três grandes grupos baseados em seus objetivos:
- Ataques de Reconhecimento: Focados no mapeamento da rede para descobrir sistemas ativos, serviços em execução e vulnerabilidades exploráveis.
- Ataques de Acesso: Focados em burlar mecanismos de segurança para obter privilégios não autorizados ou manipular dados restritos.
- Ataques de Negação de Serviço (DoS): Focados em sobrecarregar ou corromper sistemas para indisponibilizar a rede ou seus serviços para usuários legítimos.

🔎 Dinâmica dos Ataques de Reconhecimento   
Estes ataques funcionam como uma fase de coleta de inteligência. Os agentes de ameaça utilizam uma sequência de técnicas e ferramentas para mapear o alvo:
- Consultas na Internet: Utilização de ferramentas públicas (como whois ou motores de busca) para identificar o bloco de endereços IP atribuído à organização e coletar informações corporativas.
- Varredura de Ping (Ping Sweep): Utilização de ferramentas (como fping ou gping) para enviar requisições ICMP a um intervalo inteiro de endereços IP. O objetivo é identificar quais hosts estão ativos na rede, similar a ligar para todos os números de uma lista telefônica para ver quais atendem.
- Verificação de Portas (Port Scanning): Após identificar os IPs ativos, o atacante varre esses hosts para descobrir quais portas TCP/UDP estão abertas e, consequentemente, quais serviços estão em execução e passíveis de exploração.

🔓 Tipologia dos Ataques de Acesso   
Os ataques de acesso exploram as informações obtidas no reconhecimento para invadir serviços web, FTP e bancos de dados. Eles dividem-se em quatro métodos principais:
- Ataques de Senha: Tentativas de descobrir credenciais por meio de força bruta (testando combinações exaustivamente), captura de tráfego na rede (packet sniffing) ou uso de Cavalos de Troia do tipo keylogger.
- Exploração de Confiança: O atacante compromete um host com privilégios menores e utiliza as permissões ou a relação de confiança desse host para acessar partes mais seguras e críticas da rede.
- Redirecionamento de Porta: O agente malicioso compromete um dispositivo intermediário e o utiliza como plataforma (pivô) para lançar ataques contra o alvo final, mascarando a origem real do ataque. Exemplo: Acessar o Host A via SSH e usar o Host A para acessar o Host B via Telnet.
- Homem no Meio (Man-in-the-Middle): O atacante intercepta a comunicação entre duas entidades legítimas. O tráfego passa pelo equipamento do atacante, permitindo a leitura e até a modificação (adulteração) dos pacotes de dados antes de encaminhá-los ao destino correto.

🚧 Negação de Serviço (DoS e DDoS)   
Ataques de Negação de Serviço visam exaurir os recursos de um sistema (como processamento, memória ou banda de rede) para torná-lo inacessível. A prevenção primária envolve a aplicação de patches e atualizações de segurança.
- DoS (Denial of Service): O ataque é originado de uma única fonte (um único atacante ou dispositivo). É simples de ser executado, mas altamente disruptivo.
- DDoS (Distributed Denial of Service): O ataque é originado de múltiplas fontes simultaneamente, amplificando o volume do tráfego malicioso. Geralmente, o atacante controla uma rede de computadores previamente infectados (botnet) através de um servidor de Comando e Controle (C&C). Quando acionados, todos os hosts "zumbis" direcionam tráfego para o alvo simultaneamente.

<a name="item16.04"><h4>16.4 Mitigações de ataque à rede</h4></a>[Back to summary](#item16)

🛡️ Defesa em Profundidade na Rede   
Para mitigar ataques e proteger a infraestrutura, adota-se a abordagem de defesa em profundidade, também conhecida como segurança em camadas. Esta estratégia exige o funcionamento conjunto de diversos serviços e equipamentos para proteger roteadores, switches, servidores e hosts, garantindo que o acesso a esses dispositivos seja rigidamente controlado e monitorado. 

Dentre as principais soluções implementadas em uma topologia de rede segura, destacam-se:
- VPN (Rede Privada Virtual): Utilizada em roteadores para estabelecer túneis criptografados, garantindo acesso remoto seguro aos recursos corporativos.
- Firewall ASA: Equipamento dedicado que realiza a inspeção de estado, permitindo que o tráfego de saída retorne com segurança, mas bloqueando conexões externas não solicitadas.
- IPS (Sistema de Prevenção contra Intrusões): Inspeciona ativamente o tráfego em busca de assinaturas de ataques ou malwares, interrompendo a ameaça imediatamente ao detectá-la.
- ESA e WSA: O dispositivo de segurança de e-mail (ESA) filtra mensagens indesejadas e perigosas, enquanto o equipamento de segurança web (WSA) bloqueia o acesso a sites maliciosos.
- Servidor AAA: Mantém um banco de dados centralizado que determina quem possui autorização para acessar e administrar os ativos da rede.

💾 Gestão de Backups e Recuperação   
A realização de cópias de segurança é um procedimento primordial para a proteção contra a perda definitiva de dados decorrente de falhas de hardware ou ataques cibernéticos. O procedimento adequado exige o armazenamento de imagens de sistemas e configurações de ativos de rede em servidores dedicados, além da utilização de mídias externas ou armazenamento em nuvem para arquivos de usuários.

Uma política de backup corporativa deve observar as seguintes características operacionais:
- Frequência: Execução de rotinas periódicas (diárias, semanais ou mensais), combinando cópias completas espaçadas com cópias parciais frequentes dos arquivos recém-modificados.
- Armazenamento: Movimentação das cópias para um ambiente físico ou lógico externo (offsite), garantindo a preservação dos dados caso ocorra um desastre na instalação principal.
- Segurança: Proteção rigorosa dos arquivos de backup através do uso de criptografia e senhas de alta complexidade.
- Validação: Realização constante de testes nas mídias e nos procedimentos de restauração para comprovar a integridade das informações salvas.

🔄 Atualizações e Gerenciamento de Patches   
A principal defesa sistêmica contra a proliferação de worms e exploração de vulnerabilidades é a manutenção contínua de sistemas operacionais e softwares de proteção. A aplicação de pacotes de correção (patches) elimina brechas técnicas documentadas.

Em arquiteturas de rede extensas, a estratégia mais eficaz consiste em configurar mecanismos de atualização automática nos dispositivos finais. Isso garante que os pacotes de segurança sejam baixados e implementados sem a necessidade de intervenção humana, mantendo o ecossistema tecnológico padronizado e protegido contra ameaças emergentes.

🔑 Controle de Acesso e Estrutura AAA   
A proteção dos dispositivos de rede requer a limitação de acesso estrita a indivíduos devidamente credenciados. Este controle é estruturado pelo modelo de segurança AAA, que estabelece os seguintes parâmetros operacionais:
- Autenticação: O processo de verificação da identidade do indivíduo ou dispositivo que solicita acesso à rede.
- Autorização: A definição dos níveis de privilégio, determinando quais ações e comandos o usuário autenticado pode executar.
- Auditoria (Accounting): O registro cronológico e detalhado de todas as atividades realizadas pelo usuário durante a sua sessão no ambiente.

🧱 Arquitetura e Filtros de Firewall   
Posicionados estrategicamente na fronteira entre redes distintas, os firewalls controlam o fluxo de dados e impedem o acesso externo indesejado. Para serviços que precisam permanecer públicos (como servidores web), utiliza-se a arquitetura de Zona Desmilitarizada (DMZ). A DMZ funciona como um segmento de rede isolado onde regras permissivas específicas são aplicadas, sem comprometer a segurança da rede interna principal.

As tecnologias de firewall operam fundamentadas em diferentes mecanismos de filtragem:
- Filtragem de Pacotes: Baseia a liberação ou o bloqueio exclusivamente em endereços IP de origem/destino e endereços físicos (MAC).
- Filtragem de Aplicações: Restringe o tráfego analisando os números das portas lógicas utilizadas por softwares e serviços específicos.
- Filtragem de URL: Interrompe ou autoriza o acesso a páginas web baseando-se em endereços específicos ou palavras-chave detectadas.
- Inspeção de Estado (SPI): Avalia o contexto da comunicação. Garante que os pacotes recebidos pela rede sejam obrigatoriamente respostas a requisições originadas internamente, descartando fluxos não solicitados e mitigando ataques de negação de serviço.

💻 Segurança de Endpoints   
A proteção de terminais (laptops, desktops, smartphones e servidores) constitui um desafio administrativo complexo, pois depende diretamente da interação humana. O estabelecimento da segurança nesta camada exige a elaboração de políticas corporativas claras e o treinamento contínuo das equipes operacionais. Tecnicamente, a defesa dos endpoints é complementada pelo uso de softwares antivírus, sistemas de controle de acesso à rede (NAC) e mecanismos de prevenção de intrusões locais.

<a name="item16.05"><h4>16.5 Segurança de dispositivos</h4></a>[Back to summary](#item16)

🔒 Segurança de Dispositivos de Rede   
A proteção dos dispositivos de infraestrutura é um pilar fundamental para a segurança da rede. Quando um sistema operacional é recém-instalado, as configurações padrão geralmente oferecem um nível inadequado de proteção. Em equipamentos Cisco, ferramentas nativas como o recurso Cisco AutoSecure podem ser utilizadas para automatizar e auxiliar no fortalecimento inicial do sistema.

Alem disso, práticas universais de segurança devem ser aplicadas de forma rigorosa antes da implementação de qualquer equipamento em produção:
- Alteração imediata de todos os nomes de usuário e senhas padrão de fábrica.
- Restrição do acesso aos recursos do sistema apenas a indivíduos estritamente autorizados.
- Desativação e desinstalação de todos os serviços e aplicações desnecessários.
- Instalação de atualizações de software e patches de segurança, mitigando o fato de que equipamentos armazenados fisicamente por longos períodos possuem versões de sistema obsoletas e vulneráveis.

🔑 Diretrizes para Senhas Fortes   
A implementação de senhas robustas é a defesa primária contra o acesso não autorizado a dispositivos de rede. A elaboração de credenciais seguras baseia-se em critérios técnicos específicos:
- Comprimento mínimo de oito caracteres, recomendando-se dez ou mais caracteres para elevar o nível de segurança.
- Complexidade estrutural, exigindo a combinação de letras maiúsculas e minúsculas, números, símbolos e, quando suportado, espaços.
- Rejeição de padrões previsíveis, como o uso de palavras comuns de dicionário, sequências lógicas numéricas ou alfabéticas, nomes de fabricantes (ex: toyota), dados biográficos (datas de nascimento, nomes de parentes) ou o próprio nome de usuário.
- Aplicação de erros ortográficos intencionais em palavras comuns para dificultar ataques baseados em dicionários.
- Rotação e alteração periódica das senhas, limitando a janela de tempo na qual uma credencial eventualmente comprometida possa ser explorada por agentes maliciosos.
- Proibição absoluta da anotação de senhas em locais físicos ou visíveis.

Nota-se uma grande diferença técnica entre credenciais. Senhas curtas, baseadas em palavras de dicionário ou dados do usuário (ex: "secret", "bob1967") são consideradas altamente vulneráveis. Em contrapartida, credenciais que mesclam caracteres alfanuméricos e símbolos sem formar palavras reconhecíveis (ex: "b67n42d39c", "12^hu4@1p7") fornecem segurança adequada. Nos sistemas Cisco, uma técnica recomendada é a criação de frases secretas (passphrases). Como o sistema ignora espaços à esquerda, mas reconhece espaços inseridos no meio do texto, é possível construir frases longas. Estas frases oferecem maior entropia e são mais complexas de serem quebradas, ao mesmo tempo em que são mais fáceis de memoriza

🛡️ Proteção de Credenciais no Cisco IOS   
Para garantir que as senhas permaneçam confidenciais na configuração de roteadores e switches Cisco, configurações complementares são indispensáveis:
- Criptografia Geral: A aplicação do comando de configuração global `service password-encryption` impede a visualização de senhas em texto claro dentro do arquivo de configuração, aplicando criptografia automática a todas as credenciais.
- Comprimento Mínimo: A utilização do comando `security passwords min-length [min-length]` força a exigência de um tamanho mínimo para a criação de novas senhas, rejeitando credenciais curtas.
- Mitigação de Força Bruta: O comando `login block-for [segundos] attempts [tentativas] within [segundos]` protege o equipamento contra softwares de quebra de senha. Ele bloqueia tentativas de acesso por um tempo determinado após o registro de sucessivas falhas de login.
- Desconexão por Inatividade: A aplicação do comando `exec-timeout [minutos] [segundos]` nas linhas de acesso garante que sessões privilegiadas inativas sejam encerradas automaticamente. O padrão do sistema é de 10 minutos, mas recomenda-se reduzir esse tempo para evitar que terminais abandonados sejam manipulados.

🔐 Acesso Remoto Seguro com SSH   
O uso do protocolo Telnet para acesso remoto transmite dados em pacotes sem criptografia, tornando a infraestrutura insegura. É imprescindível ativar o protocolo Secure Shell (SSH) para garantir a criptografia de todo o tráfego de gerenciamento. A habilitação do SSH em um equipamento Cisco exige seis etapas técnicas:
- Etapa 1: Configuração de um nome de host (hostname) exclusivo, substituindo o nome padrão do equipamento.
- Etapa 2: Definição do domínio da rede utilizando o comando global `ip domain-name`.
- Etapa 3: Geração das chaves de criptografia RSA utilizando o comando `crypto key generate rsa`. O tamanho da chave (módulo) determina o nível de segurança, sendo 1024 bits o valor mínimo recomendado. Valores maiores (até 2048 bits) são mais seguros, porém demandam maior capacidade de processamento para criptografar os dados.
- Etapa 4: Criação de um banco de dados local contendo usuários e credenciais, por meio do comando `username`. O parâmetro `secret` deve ser utilizado para armazenar a senha de forma criptografada no sistema.
- Etapa 5: Configuração das linhas virtuais (vty) com o comando `login local`, obrigando o dispositivo a autenticar os acessos com base no banco de dados local recém-criado.
- Etapa 6: Restrição do acesso remoto exigindo o SSH. O comando `transport input ssh` aplicado nas linhas vty bloqueia ativamente as conexões via Telnet.

⚙️ Desativação de Serviços Não Utilizados   
Os equipamentos Cisco inicializam com uma lista de serviços ativos cujo uso depende da arquitetura de cada rede. A desativação compulsória de todos os serviços inativos é uma medida de segurança que bloqueia vetores de ataque em potencial e poupa o processamento (CPU) e a memória (RAM) do roteador. Os serviços habilitados por padrão variam conforme a versão do sistema operacional. Para identificar portas lógicas em estado de escuta, utiliza-se o comando `show ip ports all` nas versões modernas (IOS-XE) ou o comando `show control-plane host open-ports` em versões legadas do IOS.

Caso serviços inseguros sejam identificados nos relatórios, eles devem ser paralisados. Exemplifica-se essa ação desativando o servidor HTTP não seguro por meio do comando global `no ip http server` e garantindo que o Telnet não esteja operante nas interfaces de gerenciamento.

<a name="item16.06"><h4>16.6 Módulo Prático e Quiz</h4></a>[Back to summary](#item16)

🛡️ Ameaças e Vulnerabilidades de Rede   
Ataques a redes podem causar prejuízos financeiros e operacionais ao comprometer informações e recursos importantes. Quando invasores exploram falhas de software ou configurações, surgem riscos como roubo de dados, alteração de informações, fraude de identidade e indisponibilidade de serviços. Essas ameaças costumam explorar fraquezas ligadas a tecnologia, configuração e políticas de segurança, além de riscos físicos envolvendo hardware, energia, ambiente e manutenção.

🦠 Malware e Tipos de Ataque   
Malware reúne códigos criados para causar danos, interromper serviços ou furtar dados, incluindo vírus, worms e cavalos de Troia. Os ataques em rede geralmente se dividem em reconhecimento, acesso indevido e negação de serviço. O reconhecimento busca mapear alvos por consultas, ping e portas; o acesso envolve técnicas como quebra de senha, exploração de confiança e interceptação; já a indisponibilidade ocorre por ataques DoS e DDoS.

🏰 Defesa em Profundidade   
A mitigação começa pela proteção de roteadores, switches, servidores e hosts, adotando uma estratégia em camadas. Essa defesa combina diferentes dispositivos e serviços de segurança, como VPN, firewall, sistemas de prevenção de intrusão, filtros de e-mail e web, além de servidores AAA. A ideia é criar múltiplas barreiras para proteger usuários, dados e infraestrutura contra ameaças diversas.

💾 Backup, Atualizações e Controle de Acesso   
Manter cópias de segurança das configurações e imagens do sistema em servidores apropriados permite rápida restauração após falhas. Atualizações e correções de segurança reduzem significativamente a ação de worms e outras explorações conhecidas. O AAA complementa a proteção ao validar quem acessa, definir permissões e registrar as ações realizadas dentro da rede.

🔥 Firewalls, DMZ e Segurança de Endpoints   
Firewalls controlam o tráfego entre redes e bloqueiam acessos não autorizados por diferentes métodos de filtragem e inspeção. Serviços expostos a usuários externos costumam ser isolados em uma DMZ para reduzir riscos ao ambiente interno. A segurança também depende da proteção dos dispositivos finais, com políticas claras, antivírus, prevenção contra intrusão e mecanismos de controle de acesso à rede.

🔐 Endurecimento de Dispositivos   
As configurações padrão de sistemas e equipamentos normalmente não oferecem proteção suficiente, exigindo ajustes imediatos. Alterar credenciais padrão, remover serviços desnecessários, restringir acessos e adotar ferramentas automáticas de reforço aumentam a segurança. O uso de senhas fortes ou frases secretas, criptografia de credenciais, limites mínimos de complexidade, bloqueio contra tentativas de força bruta e acesso via SSH fortalecem ainda mais a proteção dos dispositivos.
# Laboratório - Pesquisa sobre Rede Baseada em Intenção (IBN)   <img src="./0-aux/logo_course.png" alt="lab_018" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../labs/">labs</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">lab_018 (Laboratório - Pesquisa sobre Rede Baseada em Intenção (IBN))   <img src="./0-aux/logo_course.png" alt="lab_018" width="auto" height="25"></a>

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

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">Parte 1: Explorar o site do IBN (Cisco Intent-Based Networking, Rede baseada em intenção)</a><br>
2. <a href="#item02">Parte 2: Introdução à rede baseada em intenção (IBN) com Cisco DevNet</a><br>
3. <a href="#item03">Parte 3: Explorar as solicitações da comunidade de IBN e compartilhar suas próprias solicitações</a><br>
4. <a href="#item04">Reflexão</a><br>

---

### Objective:
Explorar a arquitetura Cisco Intent-Based Network (IBN) via plataforma DevNet, visando compreender como a captura da intenção de negócio permite a automação e a proteção contínua de redes ponta a ponta.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: Explorar o site do IBN (Cisco Intent-Based Networking, Rede baseada em intenção)</h4></a>[Back to summary](#item00)

Nesta parte, você terá uma visão geral e vários casos de uso de rede baseada em intenção (IBN) com a Cisco. Ao ler este site e assistir aos vídeos incorporados, você aprenderá como a intenção humana está sendo transformada em implementação de políticas de máquina. Acesse o [link](https://www.cisco.com/c/en/us/solutions/intent-based-networking.html?dtid=osscdc000283) para acessar o site da solução Cisco IBN. Leia o site Cisco Solutions acima e responda às seguintes perguntas:

- a. O que é rede baseada em intenção (IBN, Intent-Based Networking)
  - Rede baseada em intenção (IBN) é um modelo de gerenciamento de redes no qual o administrador define o que a rede deve fazer, com base em objetivos de negócio ou políticas de alto nível, em vez de configurar manualmente dispositivos e regras técnicas. A rede utiliza automação, análise de dados e inteligência artificial para interpretar essa intenção, implementar as configurações necessárias, monitorar o ambiente continuamente e se ajustar automaticamente para garantir que a intenção definida seja mantida.
- b. Liste pelo menos dois motivos para usar IBN.
  - Automação e redução de erros humanos: A IBN automatiza a configuração e o gerenciamento da rede, diminuindo a complexidade operacional e reduzindo falhas causadas por configurações manuais.
  - Maior agilidade e alinhamento com o negócio: Permite que mudanças na rede sejam feitas de forma rápida e consistente, alinhando o comportamento da infraestrutura aos objetivos do negócio.
  - Monitoramento contínuo e autocorreção: A rede monitora seu próprio estado e pode se ajustar automaticamente quando detecta desvios em relação à intenção definida.
  - Melhoria na segurança e conformidade: Políticas de segurança são aplicadas de forma consistente em toda a rede, facilitando auditorias e o cumprimento de normas.

<a name="item02"><h4>2. Parte 2: Introdução à rede baseada em intenção (IBN) com Cisco DevNet</h4></a>[Back to summary](#item00)

Nesta parte, você será apresentado ao IBN com Cisco DevNet. Ao ler este blog, você aprenderá sobre as redes serem programáveis e como o IBN pode ser integrado via código. Clique no [link](https://blogs.cisco.com/enterprise/building-Intent-Based-network-with-devnet?ccid=cc000006&dtid=esoxsp000263&oid=psten009481) para acessar o blog da Cisco. Leia o blog usando o link acima e responda às perguntas a seguir:

- a. Qual é a primeira etapa para iniciar e praticar a codificação?
  - A primeira etapa é definir claramente o problema ou objetivo que se deseja resolver, entendendo os requisitos e o resultado esperado antes de escrever qualquer código. Isso inclui analisar o cenário, planejar a lógica e, quando necessário, representá-la por meio de fluxogramas ou pseudocódigo.
- b. Com IBN em uso, o que deve acontecer se uma empresa especificar uma intenção à rede?
  - A rede deve interpretar automaticamente a intenção definida, traduzi-la em configurações técnicas, implementar essas configurações de forma automatizada e, em seguida, monitorar continuamente o ambiente para garantir que a intenção esteja sendo cumprida, realizando ajustes ou correções automaticamente sempre que necessário.

<a name="item03"><h4>3. Parte 3: Explorar as solicitações da comunidade de IBN e compartilhar suas próprias solicitações</h4></a>[Back to summary](#item00)

Nesta parte, você verá as solicitações de código IBN de outros membros da comunidade e compartilhará sua ideia de intenção comercial com a comunidade. Os desenvolvedores na comunidade podem transformar sua ideia em código. Clique no [link](https://developer.cisco.com/codeintent/) para acessar a Comunidade Cisco DevNet para IBN e criar uma nova conta. Leia algumas das intenções desenvolvidas pela comunidade.

- a. Depois de ler algumas das intenções criadas pelos membros da comunidade, escolha duas intenções de seu interesse e liste-as abaixo.
  - Garantir prioridade de tráfego para aplicações críticas: Intenção voltada para assegurar que aplicações essenciais ao negócio (como sistemas financeiros ou de videoconferência) tenham prioridade de banda e baixa latência, independentemente do volume de tráfego na rede.
  - Aplicar políticas de segurança baseadas em perfis de usuários: Intenção que define automaticamente diferentes níveis de acesso à rede com base no perfil do usuário (funcionários, convidados ou parceiros), garantindo segurança e conformidade sem configurações manuais em cada dispositivo.
- b. Crie seu próprio Intent Wish (pedido de intenção) no site Cisco DevNet e publique abaixo:
  - Cargo: Analista de Redes / Arquiteto de Soluções de TI
  - Informações do evento: Criar uma intenção de rede que permita configurar automaticamente políticas de qualidade de serviço (QoS) e segurança para ambientes corporativos híbridos, garantindo desempenho adequado para aplicações críticas, isolamento de tráfego sensível e adaptação dinâmica da rede conforme mudanças de carga, usuários e localização.

<a name="item04"><h4>4. Reflexão</h4></a>[Back to summary](#item00)

- a. Você consegue pensar em outros casos de uso para IBN além dos que encontrou nos três sites?
  - Gerenciamento automático de redes para ambientes IoT: Aplicar políticas de conectividade, segurança e segmentação automaticamente para milhares de dispositivos IoT com requisitos diferentes.
  - Otimização dinâmica de desempenho de aplicações: Ajustar rotas, largura de banda e priorização de tráfego em tempo real conforme o comportamento das aplicações.
  - Automação de resposta a incidentes: Detectar anomalias na rede e aplicar correções automáticas, como isolamento de dispositivos comprometidos.
  - Gerenciamento de redes em ambientes multicloud e híbridos: Garantir políticas consistentes de conectividade e segurança entre data centers locais e provedores de nuvem.
  - Suporte a trabalho remoto e mobilidade: Adaptar automaticamente políticas de acesso e desempenho conforme usuários mudam de localização.
- b. Que tipo de habilidades de programação você acha que precisará para implantar redes baseadas em intenção?
  - Lógica de programação e pensamento algorítmico: Capacidade de traduzir intenções de alto nível em regras e fluxos de decisão.
  - Linguagens de script e programação: Conhecimento em linguagens como Python, JavaScript ou Go para automação e integração.
  - Uso de APIs e modelos de dados: Experiência com APIs REST, JSON, YAML e modelos como YANG.
  - Automação e infraestrutura como código: Familiaridade com ferramentas como Ansible, Terraform ou similares.
  - Conceitos de redes e protocolos: Entendimento sólido de redes, segurança, roteamento e QoS.
  - Noções de IA e análise de dados (diferencial): Conhecimento básico de IA/ML para interpretação de dados e automação avançada.
# Laboratório - Pesquisa de Ameaças à segurança da rede   <img src="./0-aux/logo_course.png" alt="lab_053" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../labs/">labs</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="./">lab_053 (Laboratório - Pesquisa de Ameaças à segurança da rede)   <img src="./0-aux/logo_course.png" alt="lab_053" width="auto" height="25"></a>

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

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">Parte 1: Explorar o Site do SANS</a><br>
  1.1 <a href="#item01.01">Etapa 1: Encontrar recursos do SANS.</a><br>
  1.2 <a href="#item01.02">Etapa 2: Localize o link para os controles críticos de segurança do CIS.</a><br>
  1.3 <a href="#item01.03">Etapa 3: Localizar o menu Newsletters (Informativos).</a><br>
2. <a href="#item02">Parte 2: Identificar as Ameaças à Segurança de Redes Recentes</a><br>
  2.1 <a href="#item02.01">Etapa 1: Localizar o @Risk: Consensus Security Alert Newsletter Archive.</a><br>
  2.2 <a href="#item02.02">Etapa 2: Identificar sites que fornecem informações recentes sobre ameaças à segurança.</a><br>
3. <a href="#item03">Parte 3: Detalhar uma Ameaça à Segurança de Redes Específica</a><br>
  3.1 <a href="#item03.01">Etapa 1: Preencher o formulário a seguir para o ataque à rede selecionado.</a><br>
  3.2 <a href="#item03.02">Etapa 2: Seguir as diretrizes do instrutor para finalizar a apresentação.</a><br>
4. <a href="#item04">Perguntas para reflexão</a><br>

---

### Objective:
Este laboratório teve como objetivo capturar e analisar tráfego HTTP e HTTPS utilizando as ferramentas **tcpdump** e **Wireshark** na máquina virtual **Cisco CyberOps Workstation**, a fim de compreender as diferenças entre comunicações não criptografadas e criptografadas.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: Explorar o Site do SANS</h4></a>[Back to summary](#item00)

Na Parte 1, acesse o site do SANS e explore os recursos disponíveis.

<a name="item01.01"><h4>1.1 Etapa 1: Encontrar recursos do SANS.</h4></a>[Back to summary](#item00)

- a. Pesquise SANS na Internet. Na home page SANS, clique em Recursos GRÁTIS.
- b. Relacione três recursos disponíveis.
  - Na seção de Recursos GRÁTIS da SANS, estão disponíveis webinars, white papers e posters com cheat sheets para apoio em cibersegurança.

<a name="item01.02"><h4>1.2 Etapa 2: Localize o link para os controles críticos de segurança do CIS.</h4></a>[Back to summary](#item00)

- a. Os Controles Críticos de Segurança da CIS vinculados no site da SANS são o culminar de uma parceria público-privada envolvendo o Departamento de Defesa (DoD), a Associação Nacional de Segurança, o Centro de Segurança na Internet (CIS) e o Instituto SANS. A lista foi desenvolvida para priorizar os controles de segurança digital e os gastos do DoD. Tornou-se a peça central para programas eficazes de segurança para o governo dos Estados Unidos. No menu Resources (Recursos), selecione Critical Security Controls (Controles de segurança críticos) ou atividade similar. O documento CIS Críticos Security Controls está hospedado no site do Center for Internet Security (CIS) e requer registro gratuito para acessar. Há um link na página de controles de segurança CIS no SANS para baixar o pôster de controles críticos de segurança SANS 2014, que fornece uma breve descrição de cada controle. 
  - Infelizmente, o link “Critical Security Controls” mencionado no enunciado não está mais disponível no site atual da SANS. Por esse motivo, foi necessário localizar o documento diretamente no site oficial do Center for Internet Security (CIS), por meio da página de lista dos controles críticos de segurança:([https://www.cisecurity.org/controls/cis-controls-list](https://www.cisecurity.org/controls/cis-controls-list)).
- b. Selecione um dos controles e liste as sugestões de implementação para esse controle.
  - O controle selecionado foi o Controle 3 – Proteção de Dados. As sugestões de implementação para esse controle incluem o desenvolvimento de processos e controles técnicos capazes de identificar, classificar, armazenar, manusear com segurança, reter adequadamente e descartar corretamente os dados da organização.

<a name="item01.03"><h4>1.3 Etapa 3: Localizar o menu Newsletters (Informativos).</h4></a>[Back to summary](#item00)

- a. Destaque o menu Resources, selecione Newsletters. Descreva brevemente cada um dos três boletins informativos disponíveis.
  - Os três boletins informativos disponíveis são o NewsBites, que apresenta um resumo semissemanal das principais notícias de cibersegurança com comentários de especialistas; o @RISK, que fornece um resumo semanal sobre novos vetores de ataque, vulnerabilidades e exploits ativos; e o OUCH!, um boletim mensal gratuito voltado à conscientização em segurança, com dicas práticas para o público em geral.

<a name="item02"><h4>2. Parte 2: Identificar as Ameaças à Segurança de Redes Recentes</h4></a>[Back to summary](#item00)

Na Parte 2, você pesquisará ameaças à segurança de rede recentes usando o site do SANS para identificar outros sites que contenham informações sobre as ameaças de segurança.

<a name="item02.01"><h4>2.1 Etapa 1: Localizar o @Risk: Consensus Security Alert Newsletter Archive.</h4></a>[Back to summary](#item00)

- a. Na página Newsletters, selecione Archive no @RISK: The Consensus Security Alert. Role para baixo até Archives Volumes e selecione um boletim informativo semanal recente. Analise as seções Notable Recent Security Issues e Most Popular Malware Files.
- b. Liste algumas vulnerabilidades recentes. Consulte vários boletins informativos recentes, se necessário.
  - Entre as vulnerabilidades recentes identificadas no boletim semanal de 9 de abril, destacam-se a CVE-2026-35616, que permite execução de código não autorizada no Fortinet FortiClient EMS; a CVE-2025-30208, relacionada ao Vite, que possibilita burlar restrições de acesso a arquivos; a CVE-2026-3429, no Keycloak, que permite a exclusão indevida de credenciais MFA; e a CVE-2026-34162, no FastGPT, que expõe um endpoint HTTP sem autenticação, permitindo acesso completo como proxy.

<a name="item02.02"><h4>2.2 Etapa 2: Identificar sites que fornecem informações recentes sobre ameaças à segurança.</h4></a>[Back to summary](#item00)

- a. Além do site do SANS, identifique outros sites que forneçam informações recentes sobre ameaças à segurança.
  - Além do site da SANS, outros sites que fornecem informações recentes sobre ameaças à segurança são o NIST National Vulnerability Database (NVD), o CISA Known Exploited Vulnerabilities Catalog, o SecurityWeek, o The Hacker News e o BleepingComputer, todos amplamente utilizados para acompanhar vulnerabilidades, ataques em andamento e alertas de segurança.
- b. Relacione algumas ameaças à segurança recentes detalhadas nesses sites.
  - Entre as ameaças recentes detalhadas nesses sites, destaca-se a vulnerabilidade CVE-2026-34162, que afeta o FastGPT. Essa falha expõe um endpoint HTTP sem autenticação, permitindo que um invasor realize requisições ao servidor como se fosse um proxy completo, caracterizando risco crítico de SSRF e possível acesso indevido a recursos internos.

<a name="item03"><h4>3. Parte 3: Detalhar uma Ameaça à Segurança de Redes Específica</h4></a>[Back to summary](#item00)

Na Parte 3, você pesquisará um ataque específico à rede que tenha ocorrido e criará uma apresentação com base em suas constatações. Preencha o formulário abaixo com base em suas constatações. 

<a name="item03.01"><h4>3.1 Etapa 1: Preencher o formulário a seguir para o ataque à rede selecionado.</h4></a>[Back to summary](#item00)

- a. Formulário:
  - Nome do ataque: Exploração de SSRF sem autenticação no FastGPT (CVE-2026-34162).
  - Tipo do ataque: Server-Side Request Forgery (SSRF) com bypass de autenticação.
  - Data dos ataques: Vulnerabilidade publicada em 31/03/2026, com risco de exploração remota imediata após a divulgação.
  - Computadores/organizações afetados: Servidores e organizações que utilizam versões do FastGPT anteriores à 4.14.9.5, especialmente ambientes expostos à Internet.
  - Como funciona e o que fez: A falha ocorre porque o endpoint /api/core/app/httpTools/runTool estava acessível sem autenticação. Um invasor podia enviar URLs, métodos HTTP, cabeçalhos e corpo da requisição, fazendo o servidor agir como um proxy HTTP completo, permitindo acesso indevido a serviços internos, APIs privadas e possível roubo de informações sensíveis.
  - Opções de mitigação: Atualizar o FastGPT para a versão 4.14.9.5 ou superior, restringir o acesso externo ao endpoint vulnerável, aplicar autenticação obrigatória, limitar comunicações internas do servidor e monitorar logs para identificar requisições suspeitas.
  - Links para referências e informações: NVD ([https://nvd.nist.gov/vuln/detail/CVE-2026-34162](https://nvd.nist.gov/vuln/detail/CVE-2026-34162)) e GitHub Security Advisory ([https://github.com/labring/FastGPT/security/advisories/GHSA-w36r-f268-pwrj](https://github.com/labring/FastGPT/security/advisories/GHSA-w36r-f268-pwrj)).

<a name="item03.02"><h4>3.2 Etapa 2: Seguir as diretrizes do instrutor para finalizar a apresentação.</h4></a>[Back to summary](#item00)

Não foi necessário criar uma apresentação.

<a name="item04"><h4>4. Perguntas para reflexão</h4></a>[Back to summary](#item00)

- a. Que etapas você pode adotar para proteger seu computador?
  - Para proteger meu computador, posso adotar medidas como manter o sistema operacional e os programas sempre atualizados, utilizar antivírus e firewall, criar senhas fortes com autenticação em dois fatores, evitar abrir links ou arquivos suspeitos, realizar backups periódicos e usar redes confiáveis. Também é importante limitar permissões de programas e monitorar comportamentos incomuns no sistema.
- b. Quais são algumas etapas importantes que as organizações podem adotar para proteger seus recursos?
  - As organizações podem proteger seus recursos adotando políticas de segurança da informação, controle de acesso por níveis de privilégio, uso de firewalls e sistemas de detecção de intrusão, atualizações constantes de servidores e aplicações, backups e planos de recuperação de desastres, segmentação de rede, criptografia de dados e treinamentos frequentes de conscientização para os colaboradores sobre phishing e outras ameaças.
# Laboratório - Estudos de caso de cibersegurança   <img src="./0-aux/logo_course.png" alt="lab_026" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../labs/">labs</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="./">lab_026 (Laboratório - Estudos de caso de cibersegurança)   <img src="./0-aux/logo_course.png" alt="lab_026" width="auto" height="25"></a>

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

1. <a href="#item01">Parte 1: Realizar pesquisa de ataques cibernéticos de alto perfil.</a><br>
2. <a href="#item02">Parte 2: Escreva uma análise de um ataque cibernético.</a><br>

---

### Objective:
Pesquisar e analisar incidentes de segurança cibernética.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: Realizar pesquisa de ataques cibernéticos de alto perfil.</h4></a>[Back to summary](#item00)

- a. Usando seu mecanismo de busca favorito, realize uma pesquisa para cada um dos ataques cibernéticos listados abaixo. Sua pesquisa provavelmente irá aparecer vários resultados, variando de artigos de notícias a artigos técnicos. Observação: Você pode usar o navegador da Web na máquina virtual instalada em um laboratório anterior para pesquisar o hack. Ao usar a máquina virtual, você pode impedir que malware seja instalado em seu computador. 
  - Vírus Stuxnet (2010):
    - O Stuxnet foi um malware altamente sofisticado, considerado o primeiro ciberataque conhecido a causar danos físicos reais. Ele foi projetado para atacar sistemas industriais (SCADA), especificamente centrífugas nucleares iranianas usadas no enriquecimento de urânio.
  - Violação de Dados da Marriott (2014–2018, divulgada em 2018):
    - A violação da Marriott afetou o banco de dados da rede Starwood Hotels, adquirida pela Marriott. O ataque ficou ativo por anos sem ser detectado.
  - Violação de Dados das Nações Unidas (2019):
    - As Nações Unidas sofreram uma violação em seus sistemas internos, resultando no vazamento de dados confidenciais de funcionários e parceiros.
  - Violação do Banco de Dados de Suporte ao Cliente da Microsoft (2020):
    - A Microsoft revelou que um banco de dados de suporte ao cliente foi exposto na internet devido a uma configuração incorreta de um servidor.
  - Violação de Dados da LifeLabs (2019):
    - A LifeLabs, empresa canadense de exames laboratoriais, sofreu um ataque de ransomware que resultou no vazamento de dados altamente sensíveis.
- b. Leia os artigos encontrados em sua pesquisa no Passo 1a e esteja preparado para discutir e compartilhar sua pesquisa sobre quem, o que, quando, onde e por que de cada ataque.

<a name="item02"><h4>2. Parte 2: Escreva uma análise de um ataque cibernético.</h4></a>[Back to summary](#item00)

Selecione um dos ataques cibernéticos de alto perfil da Etapa 1a e escreva uma análise do ataque que inclua respostas às perguntas abaixo.
  - Vírus Stuxnet (2010):
    - a. Quem foram as vítimas dos ataques?
      - Instalações nucleares do Irã (usinas de enriquecimento de urânio).
    - b. Quais tecnologias e ferramentas foram usadas no ataque?
      - Malware avançado, exploits zero-day do Windows, PLCs Siemens (SCADA).
    - c. Quando o ataque aconteceu dentro da rede?
      - Por volta de 2009–2010, permanecendo oculto por meses.
    - d. Quais sistemas foram direcionados?
      - Sistemas industriais SCADA e controladores lógicos programáveis (PLCs).
    - e. Qual foi a motivação dos atacantes neste caso? O que eles esperavam alcançar? 
      - Sabotar o programa nuclear iraniano sem uso de ataque militar direto.
    - f. Qual foi o resultado do ataque? (dados roubados, resgate, danos no sistema, etc.) 
      - Danos físicos a centrífugas e atraso no programa nuclear.
  - Violação de Dados da Marriott (2014–2018, divulgada em 2018):
    - a. Quem foram as vítimas dos ataques?
      - Clientes da rede Starwood/Marriott.
    - b. Quais tecnologias e ferramentas foram usadas no ataque?
      - Acesso persistente não detectado (APT), roubo de dados de banco de dados.
    - c. Quando o ataque aconteceu dentro da rede?
      - Entre 2014 e 2018.
    - d. Quais sistemas foram direcionados?
      - Banco de dados de reservas da Starwood.
    - e. Qual foi a motivação dos atacantes neste caso? O que eles esperavam alcançar? 
      - Espionagem e coleta massiva de dados pessoais.
    - f. Qual foi o resultado do ataque? (dados roubados, resgate, danos no sistema, etc.) 
      - Vazamento de dados de cerca de 500 milhões de hóspedes.
  - Violação de Dados das Nações Unidas (2019):
    - a. Quem foram as vítimas dos ataques?
      - Funcionários e parceiros da ONU.
    - b. Quais tecnologias e ferramentas foram usadas no ataque?
      - Exploração de sistemas desatualizados e possíveis acessos não autorizados.
    - c. Quando o ataque aconteceu dentro da rede?
      - Descoberto em 2019.
    - d. Quais sistemas foram direcionados?
      - Sistemas internos administrativos da ONU.
    - e. Qual foi a motivação dos atacantes neste caso? O que eles esperavam alcançar? 
      - Espionagem e obtenção de informações sensíveis.
    - f. Qual foi o resultado do ataque? (dados roubados, resgate, danos no sistema, etc.) 
      - Exposição de dados internos e pessoais.
  - Violação do Banco de Dados de Suporte ao Cliente da Microsoft (2020):
    - a. Quem foram as vítimas dos ataques?
      - Clientes que utilizaram o suporte da Microsoft.
    - b. Quais tecnologias e ferramentas foram usadas no ataque?
      - Exploração de banco de dados mal configurado (sem autenticação).
    - c. Quando o ataque aconteceu dentro da rede?
      - Exposição detectada em 2020.
    - d. Quais sistemas foram direcionados?
      - Banco de dados de tickets de suporte ao cliente.
    - e. Qual foi a motivação dos atacantes neste caso? O que eles esperavam alcançar? 
      - Acesso a informações para possíveis ataques de phishing.
    - f. Qual foi o resultado do ataque? (dados roubados, resgate, danos no sistema, etc.) 
      - Exposição de ~250 milhões de registros, sem senhas.
  - Violação de Dados da LifeLabs (2019):
    - a. Quem foram as vítimas dos ataques?
      - Pacientes da LifeLabs no Canadá.
    - b. Quais tecnologias e ferramentas foram usadas no ataque?
      - Ransomware e acesso indevido a sistemas internos.
    - c. Quando o ataque aconteceu dentro da rede?
      - Em 2019.
    - d. Quais sistemas foram direcionados?
      - Sistemas de dados laboratoriais e bancos de dados médicos.
    - e. Qual foi a motivação dos atacantes neste caso? O que eles esperavam alcançar? 
      - Ganho financeiro por meio de extorsão (resgate).
    - f. Qual foi o resultado do ataque? (dados roubados, resgate, danos no sistema, etc.) 
      - Vazamento de dados médicos e pagamento de resgate.
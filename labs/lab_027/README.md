# Laboratório - Aprendendo os detalhes dos ataques   <img src="./0-aux/logo_course.png" alt="lab_027" width="auto" height="45">

### Cisco: <a href="../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../self_paced/">self-paced</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="./">lab_027 (Laboratório - Aprendendo os detalhes dos ataques)   <img src="./0-aux/logo_course.png" alt="lab_027" width="auto" height="25"></a>

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

1. <a href="#item01">Parte 1: Conduzir uma pesquisa de vulnerabilidades de aplicativos IoT</a><br>

---

### Objective:
Pesquisar e analisar vulnerabilidades de aplicativos IoT.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: Conduzir uma pesquisa de vulnerabilidades de aplicativos IoT</h4></a>[Back to summary](#item00)

Usando seu mecanismo de pesquisa favorito, realize uma pesquisa de vulnerabilidades da Internet das Coisas (IoT). Durante a pesquisa, encontre um exemplo de vulnerabilidade de IoT para cada uma das verticais de IoT: indústria, sistemas de energia, saúde e governo. Esteja preparado para discutir quem pode explorar a vulnerabilidade e o porquê, o que causou a vulnerabilidade e o que pode ser feito para limitar a vulnerabilidade. 

Observação: você pode usar o navegador da Web na máquina virtual instalada em um laboratório anterior para pesquisar problemas de segurança. Ao usar a máquina virtual, você pode impedir que malware seja instalado em seu computador. 

Em sua pesquisa, escolha uma vulnerabilidade de IoT e responda às seguintes perguntas: 
- Indústria: 
  - a. Qual é a vulnerabilidade?
    - Uma vulnerabilidade crítica em controladores industriais PLC (Controladores Lógicos Programáveis) como CVE-2023-22357 permite que um atacante remoto sem autenticação leia e escreva em áreas arbitrárias da memória do dispositivo, podendo sobrescrever o firmware ou executar código malicioso.
  - b. Quem poderia explorá-lo? Explique.
    - Ataques remotos de criminosos cibernéticos, APTs (Advanced Persistent Threats) ou atores que tenham acesso à rede industrial podem explorá-la sem credenciais.
    - Um invasor que consiga se conectar ao PLC via internet ou através de uma rede interna comprometida poderia usá-la para assumir o dispositivo.
  - c. Por que a vulnerabilidade existe?
    - O dispositivo tem código de depuração ativo e ausência de validações adequadas na lógica de autorização, o que permite comandos inesperados serem executados sem autenticação.
    - Esses controladores foram projetados mais para performance industrial do que para segurança cibernética robusta.
  - d. O que poderia ser feito para limitar a vulnerabilidade? 
    - Atualizar firmware e aplicar patches de segurança fornecidos pelo fabricante.
    - Isolar redes industriais (segurança de perímetro, VLANs) e restringir acesso externo.
    - Monitorar tráfego com sistemas IDS/IPS e limitar protocolos de rede não essenciais.
- Sistemas de Energia:
  - a. Qual é a vulnerabilidade?
    - Uma vulnerabilidade generalizada nos dispositivos IoT conectados à rede elétrica, como sensores de carga e sistemas de medição inteligente, é a ausência de autenticação forte e comunicação criptografada, deixando dados e comandos suscetíveis a intercepção ou manipulação.
  - b. Quem poderia explorá-lo? Explique.
    - Hackers ou grupos patrocinados por nações que queiram interferir no funcionamento de redes de energia para fins políticos ou econômicos.
    - Hacktivistas ou grupos criminosos com capacidade técnica para capturar tráfego de rede e injetar comandos maliciosos em dispositivos IoT.
  - c. Por que a vulnerabilidade existe?
    - Dispositivos IoT muitas vezes implementam comunicação sem criptografia ou com autenticação insuficiente para economizar recursos computacionais, aumentando a superfície de ataque da rede elétrica.
  - d. O que poderia ser feito para limitar a vulnerabilidade? 
    - Uso de protocolos seguros (TLS, autenticação de vários fatores).
    - Segmentar redes de energia para isolar sensores e dispositivos críticos.
    - Atualizações regulares de software e auditorias de segurança.
- Saúde:
  - a. Qual é a vulnerabilidade?
    - Dispositivos médicos IoT (como monitores cardíacos, bombas de infusão) frequentemente têm sistemas operacionais desatualizados, credenciais padrão ou transferência de dados sem criptografia, expondo-os a ataques ou acesso não autorizado.
  - b. Quem poderia explorá-lo? Explique.
    - Cibercriminosos buscando dados privados de pacientes ou tentando extorquir hospitais via ransomware.
    - Ataques direcionados que manipulam configurações do dispositivo ou interrompem dados vitais, se conectados à rede hospitalar.
  - c. Por que a vulnerabilidade existe?
    - Esses dispositivos normalmente têm uma vida útil longa e não recebem atualizações de segurança frequentes.
    - Muitos vendem hardware com credenciais padrão que não podem ser alteradas ou com protocolos inseguros para reduzir custos.
  - d. O que poderia ser feito para limitar a vulnerabilidade? 
    - Criptografar todas as comunicações de dispositivos médicos.
    - Implementar redes separadas para dispositivos IoT e sistemas clínicos.
    - Forçar políticas de atualização e exigências de segurança por regulamentações.
- Governo:
  - a. Qual é a vulnerabilidade?
    - IoT usados em cidades inteligentes e infraestrutura pública, como câmeras de segurança, sensores de tráfego e sistemas de IoT de serviços públicos, podem ter interfaces web inseguras ou falta de segmentação de rede, permitindo acesso e manipulação não autorizados.
  - b. Quem poderia explorá-lo? Explique.
    - Ataques políticos ou espionagem digital por atores estatais que queiram manipular sistemas críticos.
    - Hackers independentes que buscam perturbar serviços públicos (como tráfego, iluminação pública) ou roubar dados sensíveis.
  - c. Por que a vulnerabilidade existe?
    - Essas aplicações podem não ter sido projetadas com segurança por padrão, priorizando conectividade e integração rápida.
    - Recursos públicos nem sempre têm avaliações de risco contínuas ou investimentos em segurança robusta.
  - d. O que poderia ser feito para limitar a vulnerabilidade? 
    - Implementar frameworks de segurança com autenticação reforçada e segmentação de rede.
    - Auditorias independentes de segurança e monitoramento contínuo de dispositivos.
    - Políticas públicas que obrigam atualizações e revisões de segurança em todos os sistemas de IoT governamentais.
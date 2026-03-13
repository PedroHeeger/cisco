# Introdução à Cibersegurança - Módulo 2   <img src="../0-aux/logo_course.png" alt="sfp_004" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="../">sfp_004 (Introdução à Cibersegurança)   <img src="../0-aux/logo_course.png" alt="sfp_004" width="auto" height="25"></a>
### Module: 2. Ataques, Conceitos e Técnicas

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

### Course Module 2 Structure:
2. <a name="item02">Ataques, Conceitos e Técnicas</a><br>
2.1 <a href="#item02.01">Analisando um ataque cibernético</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.1.1 <a href="#item02.01.01">O Que Você Acha?</a><br>
2.2 <a href="#item02.02">Métodos de infiltração</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.2.1 <a href="#item02.02.01">Quebra de senha de acesso à rede WiFi</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.2.2 <a href="#item02.02.02">Tempos de Cracking</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.2.3 <a href="#item02.02.03">Agora é com você...</a><br>
2.3 <a href="#item02.03">Exploits e vulnerabilidades de segurança</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.3.1 <a href="#item02.03.01">O Que Você Acha?</a><br>
2.4 <a href="#item02.04">O Cenário de Cibersegurança</a><br>
2.5 Questionário<br>

---

### Objective:
O objetivo do módulo foi compreender as diferentes classes de malware e os métodos de infiltração utilizados por invasores, analisando técnicas de engenharia social, ataques de rede e a exploração de vulnerabilidades lógicas e físicas para fortalecer a detecção de ameaças e a manutenção da integridade dos sistemas.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item02.01"><h4>2.1 Analisando um ataque cibernético</h4></a>[Back to summary](#item02)

🦠 Análise e Classificação de Malwares   
O termo malware, derivado de Malicious Software, refere-se a qualquer código desenvolvido com o intuito de comprometer sistemas, furtar informações, evadir controles de segurança ou causar danos operacionais. A compreensão de suas variantes e métodos de propagação é essencial para processos de contenção e remediação.

⚠️ Tipos Comuns de Softwares Maliciosos   
- Spyware: Atua no monitoramento das atividades do usuário, sendo capaz de capturar digitação (keylogging) e dados bancários. Opera alterando configurações de segurança e costuma estar oculto em softwares aparentemente legítimos.
- Adware: Focado na exibição invasiva de anúncios, geralmente via navegador. É comum que se apresente de forma conjunta ao spyware para coletar dados de navegação.
- Backdoor: Estabelece um acesso secundário ao sistema, ignorando protocolos de autenticação. Permite o controle remoto e a execução de comandos sem o conhecimento do usuário, operando de forma silenciosa.
- Ransomware: Restringe o acesso aos dados ou ao sistema completo, geralmente por meio de criptografia, exigindo um resgate financeiro para a liberação. Disseminado frequentemente via phishing ou exploração de falhas de software.
- Scareware: Utiliza técnicas de manipulação psicológica, exibindo alertas falsos sobre riscos iminentes no sistema para induzir o usuário a baixar programas maliciosos sob o pretexto de reparação.
- Rootkit: Modifica estruturas do sistema operacional para ocultar sua presença e criar acessos remotos com privilégios elevados. Sua detecção é complexa, pois altera ferramentas de monitoramento, exigindo muitas vezes a formatação completa do dispositivo.
- Vírus: Código que se anexa a arquivos executáveis e depende da ação do usuário para ser ativado. Pode realizar desde ações inofensivas até a exclusão total de dados, propagando-se por mídias físicas ou compartilhamentos de rede.
- Cavalo de Troia (Trojan): Disfarça-se de software legítimo (jogos, imagens ou áudios) para enganar o usuário. Diferente do vírus, não se replica sozinho, utilizando-se das permissões do usuário para executar atividades nocivas.
- Worms: Softwares autorreplicáveis que se espalham de forma autônoma pelas redes, sem necessidade de um arquivo hospedeiro ou intervenção humana. Exploram vulnerabilidades de rede para causar danos em larga escala.

🔍 Sintomas de Infecção no Sistema   
A presença de códigos maliciosos costuma manifestar indícios técnicos que servem de alerta para a equipe de segurança:
- Desempenho Comprometido: Aumento injustificado no uso da CPU, lentidão geral, congelamentos e travamentos frequentes.
- Anomalias de Rede: Queda na velocidade de navegação e problemas de conectividade sem causa aparente.
- Alterações de Dados: Arquivos modificados, excluídos ou surgimento de ícones e programas desconhecidos no desktop.
- Comportamento Autônomo: Processos desconhecidos em execução, fechamento repentino de softwares, reconfigurações automáticas e envio de e-mails sem autorização do titular.

<a name="item02.01.01"><h4>2.1.1 O Que Você Acha?</h4></a>[Back to summary](#item02)

Para corresponder cada uma das descrições ao tipo de malware correto, selecione uma resposta em cada menu suspenso e clique em Enviar.
- Malware projetado para rastrear sua atividade on-line e capturar seus dados.
  - Spyware.
- Software que entrega anúncios automaticamente.
  - Adware.
- Malware que mantém um sistema de computador cativo até que um pagamento seja feito ao invasor.
  - Ransomware.
- Código mal-intencionado que anexa a programas legítimos e geralmente se espalha por unidades USB, mídia óptica, compartilhamentos de rede ou e-mail.
  - Vírus.
- Código malicioso que se replica de forma independente, explorando vulnerabilidades em redes.
  - Worms.

<a name="item02.02"><h4>2.2 Métodos de infiltração</h4></a>[Back to summary](#item02)

🧠 Técnicas de Manipulação e Ataques de Rede   
A segurança da informação enfrenta desafios que vão além das falhas de software, envolvendo a exploração da psicologia humana e a interrupção proposital de fluxos de comunicação.

👥 Métodos de Engenharia Social   
A engenharia social baseia-se na manipulação de indivíduos para que executem ações ou revelem dados sigilosos. Invasores exploram traços como prestatividade, ganância, vaidade ou o respeito à autoridade.
- Pretexting: O atacante cria um cenário fictício (um pretexto) por telefone ou mensagem para convencer a vítima a confirmar dados privilegiados, como informações financeiras ou de identidade.
- Tailgating (Carona): Prática física em que um indivíduo não autorizado segue de perto uma pessoa autorizada para entrar em áreas restritas.
- Quid Pro Quo (Algo por Algo): O invasor oferece um benefício, como um brinde ou serviço gratuito, em troca de informações confidenciais do usuário.

🚫 Interrupção de Disponibilidade: DoS e DDoS   
Os ataques de Negação de Serviço (DoS) visam tornar sistemas, aplicações ou redes inacessíveis para usuários legítimos.
- Volume de Tráfego: Sobrecarga de um dispositivo ou link com uma quantidade de dados superior à sua capacidade de processamento, causando lentidão ou colapso.
- Pacotes Mal-intencionados: Envio de dados formatados incorretamente que o sistema receptor não consegue interpretar, resultando em erros ou desligamento do serviço.
- DDoS (Negação de Serviço Distribuída): Variante mais complexa que utiliza múltiplas fontes coordenadas. O invasor gerencia uma Botnet (rede de computadores "zumbis" infectados) para inundar o alvo simultaneamente, dificultando a mitigação do ataque.

🛡️ Defesa Contra Botnets   
Dispositivos de segurança modernos utilizam filtros de inteligência para identificar a comunicação entre dispositivos infectados e seus servidores de Comando e Controle (C&C). Soluções como firewalls avançados recebem atualizações constantes da nuvem para bloquear tráfego de redes zumbis conhecidas e alertar as equipes de resposta.

🕵️ Interceptação de Comunicação (MitM)   
Ataques do tipo "Homem no Meio" ocorrem quando um invasor intercepta e, por vezes, altera a troca de dados entre duas partes sem que elas percebam.
- Man-in-the-Middle (MITM): O criminoso assume o controle de um nó da comunicação, capturando credenciais e dados financeiros antes que cheguem ao destino.
- Man-in-the-Mobile (MITMO): Focado em dispositivos móveis, este ataque é frequentemente utilizado para burlar a autenticação de dois fatores, capturando mensagens de SMS com códigos de verificação.

🔍 Envenenamento de Mecanismos de Busca (SEO Poisoning)   
Enquanto empresas legítimas usam a Otimização de Mecanismos de Busca (SEO) para ganhar visibilidade, invasores utilizam a técnica para elevar a classificação de sites maliciosos em termos de pesquisa populares. O objetivo é induzir o usuário a clicar em links que aparecem no topo dos resultados, direcionando o tráfego para páginas que hospedam malwares ou aplicam golpes de engenharia social.

🔐 Vulnerabilidades e Ataques a Sistemas de Senhas   
O uso de credenciais compostas por nome de usuário e senha permanece como um dos métodos de autenticação mais difundidos, o que o torna um alvo primário para agentes maliciosos. A obtenção dessas chaves de acesso permite que invasores comprometam dados sensíveis com baixo esforço técnico inicial.

🔑 Métodos de Comprometimento de Credenciais   
- Password Spraying (Pulverização): Técnica que consiste em testar uma única senha comum (como "Senha123") em uma vasta lista de nomes de usuário. Ao contrário de testar várias senhas em uma única conta, essa estratégia evita o bloqueio automático por excesso de tentativas e dificulta a detecção pelos sistemas de segurança.
- Ataque de Dicionário: O invasor utiliza listas automatizadas contendo palavras de dicionários, termos populares e senhas vazadas anteriormente para tentar obter acesso a contas protegidas.
- Força Bruta (Brute Force): Método exaustivo onde o atacante utiliza softwares para testar todas as combinações possíveis de caracteres, números e símbolos até encontrar a sequência correta.
- Ataques de Tabela Arco-íris (Rainbow Tables): Sistemas seguros armazenam senhas em formato de hash (valores criptográficos) em vez de texto claro. O invasor utiliza tabelas pré-computadas que relacionam senhas comuns aos seus respectivos hashes, permitindo a identificação da senha original por comparação direta, o que é mais rápido que o cálculo individual.
- Interceptação de Tráfego: Consiste na captura de dados durante a transmissão. Senhas enviadas sem criptografia ou armazenadas em texto simples podem ser lidas por qualquer pessoa ou ferramenta que intercepte a comunicação entre o usuário e o servidor.

🏹 Ameaças Persistentes Avançadas (APT)   
As APTs representam operações ofensivas de longo prazo, caracterizadas por serem furtivas e altamente direcionadas a alvos específicos, como grandes corporações ou infraestruturas nacionais. Diferente de ataques genéricos, as APTs exigem alto investimento financeiro e expertise técnica elevada. O objetivo central não é apenas a invasão, mas a implantação de malwares customizados que permitam a permanência do invasor no sistema por períodos prolongados sem ser detectado, visando espionagem comercial ou política.

<a name="item02.02.01"><h4>2.2.1 Quebra de senha de acesso à rede WiFi</h4></a>[Back to summary](#item02)

Você está aproveitando o almoço na cantina quando um colega se aproxima de você. Eles parecem angustiados. Eles explicam que parecem não conseguir se conectar ao Wi-Fi público no telefone e perguntam se você tem a senha de Wi-Fi privada em mãos para que possam verificar se o telefone está funcionando. Como você responderá? Selecione a resposta correta e clique em Enviar.
- Opções:
  - "Mmm... Não tenho certeza se estamos autorizados a usar a rede Wi-Fi privada. Deixe-me falar com meu gerente primeiro. ” (V)
  - “Sim, claro. Me dê seu telefone e eu vou colocá-lo para você. (F)
  - “Claro. É Xgfi76dB. ” (F)

<a name="item02.02.02"><h4>2.2.2 Tempos de Cracking</h4></a>[Back to summary](#item02)

Parece que os hackers estão tentando de tudo para quebrar a senha Wi-Fi privada da Apollo. Precisamos garantir que a senha seja forte o suficiente para suportar o ataque! Veja as seguintes senhas. Clique nos números para colocá-los na ordem correta de acordo com quanto tempo você acha que um invasor levaria para quebrar cada um usando força bruta, em que 1 é o menor período de tempo e 4, o maior.
- Opções:
  - K4km9n2R (3)
  - H $ 1gh # 7iD @ 3 (4)
  - 3trawberry (2)
  - Senha (1)

<a name="item02.02.03"><h4>2.2.3 Agora é com você...</h4></a>[Back to summary](#item02)

Ufa! Isso é muito difícil de entender e os hackers certamente têm muitas ferramentas à sua disposição. É importante que você saiba o que é isso para que possa se proteger e à @Apollo. Você se lembra de algumas das atividades suspeitas que você viu recentemente na empresa. Com base no que você aprendeu neste tópico, que tipo de ataque pode ser cada um desses cenários? Não se apresse com esta. Você tem a chance de ganhar alguns pontos de defensor muito necessários. Selecione a resposta correta nas listas suspensas e depois envie.
- Opções:
  - No caminho para o escritório, uma pessoa que você nunca viu antes pede que você feche a porta - ela esqueceu o cartão de acesso.
    - Engenharia Social.
  - Você recebeu uma mensagem de erro ao acessar o computador: “Sua conexão foi interrompida. Uma alteração na rede foi detectada.
    - DoS.
  - Você pesquisou o site da @ Apollo no Google, mas ao clicar no resultado superior foi redirecionado para uma página que anuncia software antivírus
    - Seo Poising.

<a name="item02.03"><h4>2.3 Exploits e vulnerabilidades de segurança</h4></a>[Back to summary](#item02)

🛠️ Gestão de Vulnerabilidades e Explorações de Sistema   
A segurança cibernética baseia-se na identificação de falhas em ativos tecnológicos para evitar que agentes maliciosos comprometam a integridade organizacional. Para isso, é essencial compreender a distinção entre conceitos fundamentais:
- Vulnerabilidade: Refere-se a qualquer defeito ou fragilidade lógica (software) ou física (hardware).
- Exploit: É o código ou programa desenvolvido especificamente para se aproveitar de uma vulnerabilidade conhecida.
- Ataque: É o ato de utilizar um exploit contra uma vulnerabilidade para obter acesso indevido a sistemas ou recursos.

💻 Vulnerabilidades de Hardware e Canais Laterais   
Falhas de hardware originam-se em erros de projeto nos componentes físicos, sendo muitas vezes inerentes à arquitetura do dispositivo.
- Interferência Elétrica (Rowhammer): Baseia-se na proximidade de capacitores em memórias RAM. O acesso repetitivo a uma linha de memória gera interferências que corrompem os dados de linhas vizinhas.
- Ataques de Canal Lateral (Meltdown e Spectre): Descobertas em 2017, estas falhas afetam a maioria das CPUs modernas. Permitem que invasores leiam a memória do sistema e de outras aplicações em execução, extraindo dados confidenciais através da observação do comportamento físico do processador.

Embora graves, vulnerabilidades de hardware são geralmente exploradas em ataques altamente direcionados. Para o usuário comum, a segurança física dos dispositivos e o uso de proteções contra malwares tradicionais costumam ser suficientes.

📂 Vulnerabilidades de Software e Falhas de Código   
As falhas de software surgem de erros de programação em sistemas operacionais ou aplicativos. Um exemplo histórico é o SYNful Knock, que permitia o controle remoto de roteadores empresariais através de versões modificadas do sistema operacional (IOS), permitindo o monitoramento de todo o tráfego da rede.

As principais categorias de falhas de software incluem:
- Estouro de Buffer (Buffer Overflow): Ocorre quando dados excedem o limite de memória alocada para um programa, permitindo o acesso a áreas de memória de outros processos ou a execução de códigos com privilégios elevados.
- Entrada não Validada: Programas que aceitam dados externos sem verificação rigorosa podem ser forçados a comportamentos anômalos por arquivos mal-intencionados (ex: imagens com dimensões inválidas).
- Condição de Corrida (Race Condition): Falha que ocorre quando o sistema depende da execução de eventos em uma ordem específica, mas essa sequência é alterada ou desincronizada.
- Fragilidade em Práticas de Segurança: Ocorre quando desenvolvedores tentam criar algoritmos próprios de criptografia ou ignoram bibliotecas verificadas, introduzindo fraquezas no sistema.
- Controle de Acesso Inadequado: Má gestão sobre quem pode visualizar ou editar recursos. Nota-se que o acesso físico ao equipamento pode anular quase todas as proteções lógicas, permitindo a leitura direta de discos.

🔄 Manutenção e Resposta Proativa   
A aplicação constante de atualizações e patches de segurança é a principal defesa contra a exploração de vulnerabilidades conhecidas. Fabricantes de sistemas e desenvolvedores de aplicativos lançam correções regularmente para fechar brechas identificadas. 

Além das correções reativas, grandes organizações mantêm iniciativas proativas. O Project Zero do Google é uma equipe dedicada à pesquisa de vulnerabilidades em softwares de terceiros, visando a correção de falhas antes que estas sejam exploradas em larga escala. No cenário atual, novas ameaças como o cryptojacking (mineração não autorizada de criptomoedas) demonstram a evolução contínua dos riscos digitais.

<a name="item02.03.01"><h4>2.3.1 O que você acha?</h4></a>[Back to summary](#item02)

Isso fez você pensar sobre algumas das vulnerabilidades que podem existir no @Apollo. Após algumas investigações, você observou alguns possíveis problemas. Você consegue identificar em qual categoria cada uma dessas vulnerabilidades se encaixa? Você tem a chance de ganhar alguns pontos de defensor aqui e proteger ainda mais @Apollo, então tome seu tempo. Escolha a resposta correta em cada uma das opções e clique em Enviar.
- Opções:
  - Ao iniciar no @Apollo, sua senha de rede foi enviada para você em texto sem formatação e você não foi solicitado a alterá-la.
    - Fragilidade nas práticas de segurança.
  - Os funcionários antigos ainda têm acesso ao banco de dados de clientes da @Apollo.
    - Problemas de controle de acesso.
  - Novos usuários podem fazer login na conta @Apollo, mesmo que tenham se inscrito com um endereço de e-mail formatado incorretamente.
    - Entrada não validada.

<a name="item02.04"><h4>2.4 O Cenário de Cibersegurança</h4></a>[Back to summary](#item02)

🪙 Fundamentos das Criptomoedas e Blockchain   
A criptomoeda é uma forma de ativos digitais utilizada para a aquisição de bens e serviços, fundamentada em técnicas avançadas de criptografia para garantir a segurança e a integridade das operações financeiras. Instituições bancárias, órgãos governamentais e grandes corporações globais têm reconhecido a relevância tecnológica e econômica desse sistema.

💰 Mecânica das Transações Digitais   
- Carteiras Digitais: O armazenamento desses ativos ocorre em carteiras virtuais criptografadas, que funcionam como repositórios pessoais para o capital digital.
- Descentralização (Blockchain): As transações são registradas em um livro-razão descentralizado denominado blockchain. Esse modelo permite o autogerenciamento das operações com alto nível de anonimato, eliminando a necessidade de intermediários ou controle por bancos centrais.
- Processo de Mineração: Periodicamente, dados das transações recentes são agrupados e convertidos em desafios matemáticos complexos. A validação desses dados é realizada por uma rede global de "mineradores", que utilizam hardware de alta performance para autenticar as transações.
- Atualização do Registro: Após a verificação técnica, o livro-razão é atualizado e distribuído eletronicamente por toda a rede, garantindo que todos os participantes possuam uma cópia idêntica e atualizada do histórico de operações.

⚠️ A Ameaça do Cryptojacking   
O cryptojacking representa um risco crescente à segurança de dispositivos pessoais e servidores. Trata-se de uma técnica em que invasores utilizam sub-repticiamente o poder de processamento (CPU e GPU) de máquinas de terceiros para realizar a mineração de criptomoedas sem autorização. Muitas vezes, a detecção dessa invasão é tardia, sendo percebida apenas pelo aumento excessivo no consumo de energia ou pela degradação severa do desempenho do hardware. Embora a economia digital ofereça novas oportunidades, ela também amplia a superfície de ataque para criminosos interessados no desvio de recursos computacionais e financeiros.
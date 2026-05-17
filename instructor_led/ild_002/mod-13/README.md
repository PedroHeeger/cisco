# CyberOps Associate - Módulo 13   <img src="../0-aux/logo_course.png" alt="ild_002" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="../">ild_002 (CyberOps Associate)   <img src="../0-aux/logo_course.png" alt="ild_002" width="auto" height="25"></a>
### Module: 13. Invasores e suas ferramentas

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

### Course Module 13 Structure:

13. <a name="item13">Invasores e suas ferramentas</a><br>
  13.1 <a href="#item13.01">Introdução</a><br>
  13.2 <a href="#item13.02">Quem está atacando nossa rede?</a><br>
  13.3 <a href="#item13.03">Ferramentas do agente da ameaça</a><br>
  13.4 <a href="#item13.04">Resumo de invasores e suas ferramentas</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item13.01"><h4>13.1 Introdução</h4></a>[Back to summary](#item13)

🔹 Perfis de Ameaça e Vetores de Ataque Cibernético   
A identificação das motivações e dos perfis dos indivíduos que tentam comprometer as infraestruturas digitais é o primeiro passo para estabelecer uma defesa sólida. Este módulo explora a classificação dos agentes de ameaça, diferenciando suas abordagens éticas e objetivos, além de apresentar o arsenal tecnológico disponível para a execução de intrusões. O entendimento dessas dinâmicas permite antecipar movimentos adversários e compreender o ecossistema de vulnerabilidades que desafia a segurança das redes modernas.

🎯 Objetivo Geral:   
- Analisar os métodos e os perfis responsáveis pela execução de ofensivas contra infraestruturas de rede.

✅ Objetivos Específicos:   
- Quem está atacando nossa rede: Investigar a trajetória histórica e a sofisticação crescente das ameaças que visam os ativos de rede.
- Ferramentas do agente da ameaça: Categorizar os diferentes utilitários e softwares empregados por atacantes para explorar brechas e comprometer sistemas.

<a name="item13.02"><h4>13.2 Quem está atacando nossa rede?</h4></a>[Back to summary](#item13)

🛡️ Fundamentos e Terminologia de Segurança   
A proteção de uma organização começa pelo entendimento do que está em risco e como esses ativos podem ser atingidos. Ativos são todos os bens valiosos, desde dados intelectuais e servidores até dispositivos móveis.

Para navegar na área de segurança, é preciso dominar os seguintes conceitos:
- Ameaça: Qualquer perigo em potencial que possa prejudicar um ativo.
- Vulnerabilidade: Uma falha ou fraqueza no projeto ou na implementação de um sistema.
- Superfície de Ataque: O conjunto total de pontos vulneráveis que um invasor pode tentar explorar. Quanto mais softwares sem atualização (patches), maior será essa superfície.
- Exploit: O meio ou ferramenta usada para tirar proveito de uma vulnerabilidade. Pode ser remoto (via rede, sem acesso prévio) ou local (exige uma conta ou acesso interno ao sistema).
- Risco: A chance real de uma ameaça explorar uma vulnerabilidade e causar um dano.
- Contramedida: Ações e controles aplicados para diminuir o risco ou mitigar a ameaça.

⚖️ Estratégias de Gestão de Riscos   
Gerenciar riscos é encontrar o equilíbrio entre o custo da proteção e o valor do ativo. Existem quatro abordagens principais:
- Aceitação: O custo para mitigar o risco é maior que o prejuízo potencial. O risco é mantido sem ações adicionais.
- Prevenção: Elimina-se a causa do risco (ex: desligar um serviço perigoso), embora isso também remova os benefícios desse serviço.
- Redução (Mitigação): A estratégia mais comum, onde medidas são tomadas para diminuir a probabilidade ou o impacto do ataque.
- Transferência: O risco é passado para outra entidade, como a contratação de um seguro cibernético.

🎩 O Espectro dos Hackers   
O termo "hacker" evoluiu de programadores brilhantes para perfis distintos, frequentemente classificados por "chapéus" que indicam sua ética e intenção:
- White Hat (Chapéu Branco): Hackers éticos. Usam suas habilidades legalmente para descobrir falhas e ajudar organizações a corrigi-las antes que criminosos as encontrem.
- Gray Hat (Chapéu Cinzento): Atuam em uma zona moral ambígua. Podem invadir sistemas sem permissão, mas geralmente não visam lucro pessoal, focando em expor falhas publicamente ou avisar o proprietário após a invasão.
- Black Hat (Chapéu Preto): Criminosos motivados por intenções maliciosas ou ganho financeiro. Eles exploram vulnerabilidades para roubar dados ou destruir sistemas.

🎭 Perfis de Atores de Ameaça   
A motivação dos atacantes mudou drasticamente desde o início das invasões telefônicas (phreaking) nos anos 60. Hoje, os perfis incluem:
- Script Kiddies: Atacantes inexperientes que usam ferramentas e scripts criados por outros para causar danos, geralmente por diversão ou reconhecimento.
- Corretores de Vulnerabilidades: Especialistas que buscam falhas para reportar a fabricantes em troca de recompensas (Bug Bounties).
- Hacktivistas: Atuam por motivações políticas ou sociais, usando invasões para protestar ou vazar informações confidenciais de governos e empresas.
- Criminosos Cibernéticos: Profissionais (autônomos ou em grupos organizados) focados no lucro financeiro através de fraudes e roubo de dados.
- Patrocinados pelo Estado: Agentes que operam a mando de governos para espionagem, sabotagem de infraestrutura estrangeira e roubo de segredos nacionais. São considerados os atacantes mais sofisticados e bem financiados.
 
💰 O Ecossistema do Crime Cibernético   
Criminosos virtuais são motivados essencialmente pelo lucro financeiro. Embora alguns atuem sozinhos, a maioria faz parte de organizações criminosas estruturadas que movimentam bilhões de dólares anualmente, vitimando desde usuários domésticos até grandes corporações.

Este grupo opera em uma verdadeira "economia paralela" no submundo da internet, onde:
- Comércio de Dados: Informações pessoais e propriedades intelectuais roubadas são vendidas como mercadoria.
- Mercado de Ferramentas: Invasores compram e vendem exploits e softwares maliciosos prontos para uso.
- Alvos Diversificados: Ninguém está imune; pequenas empresas são visadas tanto quanto setores estratégicos, devido à vulnerabilidade de seus sistemas.

🛡️ Responsabilidade Compartilhada e Prevenção   
A segurança no ambiente digital não é apenas uma tarefa técnica, mas um dever de todos os usuários. Adotar uma postura consciente é o primeiro passo para reduzir o sucesso das ameaças.

Ações Essenciais para Organizações: 
- Para proteger ativos e clientes, as empresas devem seguir protocolos rígidos, como:
  - Utilizar autenticação de dois fatores (2FA) e senhas complexas.
  - Manter softwares de segurança e políticas internas sempre atualizados.
  - Realizar cópias de segurança (backups) frequentes em nuvem e mídia física.
  - Executar testes de invasão periódicos para identificar falhas antes dos criminosos.

🔍 Inteligência contra Ameaças: IOC e IOA   
A defesa moderna baseia-se na análise de evidências e comportamentos para identificar invasões:
- Indicadores de Comprometimento (IOC): São as evidências de que um ataque já ocorreu. Incluem endereços IP de servidores maliciosos, nomes de arquivos de vírus ou alterações suspeitas no sistema. Compartilhar esses dados ajuda a comunidade a bloquear ataques similares rapidamente.
- Indicadores de Ataque (IOA): Focam na estratégia e motivação do invasor. Ao entender como e por que um criminoso age, é possível criar uma defesa proativa, impedindo futuros ataques que utilizem táticas parecidas, mesmo que as ferramentas mudem.

🌐 Cooperação Internacional e Governamental   
Governos ao redor do mundo têm criado agências para centralizar a defesa cibernética e promover a conscientização pública:
- CISA (EUA): Lidera a automação do compartilhamento de informações entre os setores público e privado através do sistema AIS, permitindo respostas em tempo real a ameaças verificadas.
- ENISA (União Europeia): Desempenha papel semelhante à CISA, oferecendo soluções e consultoria em segurança para os estados-membros da UE.
- Campanhas de Conscientização: Iniciativas como o Mês da Conscientização sobre Cibersegurança promovem práticas seguras, como o cuidado com redes sociais, privacidade em aplicativos e segurança em compras online, reforçando que o usuário é a peça central da proteção digital.

<a name="item13.03"><h4>13.3 Ferramentas do agente da ameaça</h4></a>[Back to summary](#item13)

🛠️ Evolução das Ferramentas e Conhecimento Técnico   
A relação entre a complexidade das invasões e a habilidade do atacante mudou drasticamente. Antigamente, era necessário um profundo saber técnico para criar e executar um ataque. Hoje, com a automação e ferramentas altamente sofisticadas, invasores com pouco conhecimento (como os script kiddies) conseguem realizar ataques complexos com apenas alguns cliques.

🧰 Categorias de Ferramentas de Teste e Exploração   
Tanto profissionais de segurança ética (white hats) quanto criminosos (black hats) utilizam um arsenal variado para analisar ou comprometer redes:
- Crackers de Senha: Ferramentas focadas em descobrir credenciais através de tentativas repetidas, remoção de senhas originais ou contorno de criptografia. Exemplos: John the Ripper, Ophcrack e Hydra.
- Hacking Sem Fio: Equipamentos e softwares usados para invadir redes Wi-Fi e identificar falhas de segurança específicas do meio sem fio. Exemplos: Aircrack-ng, Kismet e NetStumbler.
- Varredura de Rede (Scanning): Investigam dispositivos e servidores em busca de portas TCP ou UDP que estejam abertas e vulneráveis. Exemplos: Nmap, Angry IP Scanner e SuperScan.
- Elaboração de Pacotes: Utilizadas para criar pacotes forjados e testar a resistência e as regras de filtragem de firewalls. Exemplos: Hping, Scapy e Netcat.
- Sniffers de Pacotes: Capturam e analisam o tráfego de dados em redes locais ou sem fio para visualizar o conteúdo das comunicações. Exemplos: Wireshark, Tcpdump e Ettercap.
- Detectores de Rootkit: Verificadores de integridade que monitoram arquivos e diretórios em busca de rootkits instalados no sistema. Exemplos: AIDE e Netfilter.
- Fuzzers de Vulnerabilidades: Ferramentas que injetam dados aleatórios em sistemas para forçar falhas e descobrir novas brechas de segurança. Exemplos: Skipfish e W3af.
- Exploração de Vulnerabilidades: Softwares que confirmam se um host remoto é realmente suscetível a um ataque específico. Exemplos: Metasploit, Sqlmap e Core Impact.
- Scanners de Vulnerabilidades: Sistemas que examinam redes, máquinas virtuais e bancos de dados em busca de vulnerabilidades conhecidas. Exemplos: Nessus, OpenVAS e SAINT.
- Sistemas Operacionais de Hacking: Distribuições customizadas que já vêm nativamente carregadas com diversas ferramentas de auditoria. Exemplos: Kali Linux, Parrot OS e BackBox.

🕵️ Ferramentas Forenses e de Análise   
Para os defensores, algumas ferramentas são vitais no pós-ataque ou na análise de códigos maliciosos:
- Forense: Usadas para coletar evidências digitais e rastros deixados em sistemas invadidos (Sleuth Kit, Encase).
- Depuradores (Debuggers): Permitem a engenharia reversa de programas para entender como um malware funciona ou como um exploit foi escrito (IDA Pro, GDB).
- Criptografia: Essenciais para proteger a confidencialidade dos dados em repouso ou em trânsito (VeraCrypt, OpenVPN).

⚔️ Estratégias Comuns de Ataque de Rede   
Os agentes de ameaça selecionam técnicas específicas com base no ativo que desejam comprometer. Abaixo, as principais metodologias de ataque explicadas de forma direta:
- Eavesdropping (Escuta ou Sniffing): Consiste na interceptação passiva de tráfego de rede não criptografado. O objetivo é monitorar e capturar dados sensíveis, como senhas e mensagens, sem que as partes percebam a presença do invasor.
- Modificação de Dados: O atacante captura os pacotes em trânsito e altera seu conteúdo original. A informação manipulada é enviada ao destino final, enganando tanto o remetente quanto o receptor sobre a integridade da mensagem.
- Spoofing de Endereço IP: Técnica de falsificação onde o invasor mascara pacotes com um endereço IP de origem legítimo. Isso permite que o atacante se passe por um dispositivo confiável da rede interna para burlar firewalls e filtros de acesso.
- Ataques Baseados em Senha: Ocorre quando credenciais válidas são obtidas para acessar o sistema. Com o login em mãos, o invasor pode escalar privilégios, alterar configurações de servidores ou extrair informações confidenciais agindo como um usuário comum.
- Negação de Serviço (DoS): Focado em interromper a disponibilidade de um recurso. O alvo é inundado com um volume massivo de tráfego ou requisições até que o sistema fique sobrecarregado e pare de responder aos usuários legítimos.
- Man-in-the-Middle (MITM): O agente de ameaça se posiciona entre a origem e o destino da comunicação. Ele atua como um intermediário invisível que pode monitorar, capturar e até injetar novos dados na sessão de forma transparente.
- Ataque de Chave Comprometida: Ocorre quando uma chave de criptografia secreta é descoberta pelo invasor. Com esse acesso, ele consegue descriptografar comunicações protegidas sem a necessidade de quebrar o algoritmo, mantendo a invasão oculta por longos períodos.

<a name="item13.04"><h4>13.4 Resumo de invasores e suas ferramentas</h4></a>[Back to summary](#item13)

⚖️ Fundamentos da segurança   
A proteção digital exige a compreensão de conceitos como falhas sistêmicas, exposição de ativos e a probabilidade de danos reais. O gerenciamento dessas ameaças envolve um equilíbrio financeiro entre o custo das defesas e o valor do que está sendo protegido, podendo a organização decidir por mitigar o perigo, evitá-lo totalmente, transferir a responsabilidade para terceiros ou simplesmente aceitar a possibilidade de impacto.

🎭 Categorias de invasores   
O termo que define quem realiza invasões é subdividido em perfis baseados na ética e no objetivo da ação. Existem profissionais que atuam dentro da lei para fortalecer defesas, indivíduos que operam em áreas cinzentas sem intenção de dano direto, e criminosos focados em benefício próprio ou prejuízo alheio, que exploram redes para comprometer dados e sistemas por motivações puramente maliciosas.

👥 Perfis de criminosos   
O cenário de riscos é composto por uma variedade de agentes, desde iniciantes que utilizam roteiros prontos até grupos altamente organizados e financiados por governos para espionagem. Para combater esses ataques, instituições globais incentivam o compartilhamento de evidências de invasão e promovem diretrizes de defesa que ajudam empresas e nações a se protegerem contra táticas de comprometimento cada vez mais complexas.

🛠️ Arsenal de ataque   
As ferramentas utilizadas para comprometer redes evoluíram para sistemas automatizados e sofisticados, muitos deles baseados em ambientes de software aberto. Esse conjunto de recursos inclui programas para quebra de senhas, simuladores de tráfego, capturadores de dados e scanners que buscam brechas automáticas, tornando essencial que o defensor conheça essas tecnologias para antecipar os movimentos do invasor.

📂 Tipos de investidas   
Os ataques são organizados em grupos conforme o método utilizado, abrangendo desde a espionagem silenciosa e a alteração indevida de informações até o bloqueio total de serviços essenciais. Outras táticas comuns envolvem o roubo de credenciais, a interceptação de comunicações no meio do trajeto e a falsificação de identidades digitais para enganar sistemas de controle e obter acesso a áreas restritas.
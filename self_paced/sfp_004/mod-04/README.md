# Introdução à Cibersegurança - Módulo 4   <img src="../0-aux/logo_course.png" alt="sfp_004" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="../">sfp_004 (Introdução à Cibersegurança)   <img src="../0-aux/logo_course.png" alt="sfp_004" width="auto" height="25"></a>
### Module: 4. Protegendo a Organização

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

### Course Module 4 Structure:
4. <a name="item04">Protegendo a Organização</a><br>
4.1 <a href="#item04.01">Dispositivos e Tecnologias de segurança cibernética</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;4.1.1 <a href="#item04.01.01">Qual é?</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;4.1.2 <a href="#item04.01.02">Qual é?</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;4.1.3 <a href="#item04.01.03">O que isso significa?</a><br>
4.2 <a href="#item04.02">Abordagem comportamental à segurança cibernética</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;4.2.1 <a href="#item04.02.01">Sua vez de</a><br>
4.3 <a href="#item04.03">Abordagem da Cisco para segurança cibernética</a><br>
4.4 Questionário<br>

---

### Objective:
O objetivo do módulo foi compreender o ecossistema de defesa corporativa, identificando o papel de dispositivos como firewalls, IPS e VPNs, além de explorar metodologias de análise comportamental, testes de intrusão e gestão de riscos para estruturar uma resposta eficiente a incidentes de segurança.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item04.01"><h4>4.1 Dispositivos e Tecnologias de segurança cibernética</h4></a>[Back to summary](#item04)

🛡️ Ecossistema de Defesa Cibernética   
A segurança de uma rede organizacional não depende de uma única tecnologia, mas de um conjunto estratégico de ferramentas que atuam de forma complementar. Esses dispositivos podem ser equipamentos físicos dedicados ou soluções de software integradas.

🛠️ Categorias de Dispositivos de Segurança   
- Roteadores: Além de conectar segmentos de rede, realizam filtragem básica de tráfego para controlar a comunicação entre diferentes áreas.
- Firewalls: Analisam o tráfego detalhadamente para bloquear comportamentos maliciosos com base em políticas sofisticadas.
- Sistemas de Prevenção de Invasão (IPS): Utilizam assinaturas de ataques conhecidos para identificar e interromper ameaças em tempo real.
- Redes Privadas Virtuais (VPN): Criam túneis criptografados para garantir conexões seguras de funcionários remotos ou filiais à sede.
- Antimalware de Próxima Geração: Realizam análise comportamental e de assinaturas para impedir a execução de códigos nocivos.
- Gestão de Segurança: Inclui ferramentas de descriptografia, servidores de controle de acesso e segurança específica para e-mail e web.

🔥 Tipos e Evolução de Firewalls   
O firewall atua como um filtro de entrada e saída, podendo proteger um único computador (baseado em host) ou uma rede inteira (baseado em rede).
- Camada de Rede: Filtra dados baseando-se nos endereços IP de origem e destino.
- Camada de Transporte: Analisa portas de dados e o estado das conexões.
- Camada de Aplicação: Monitora o tráfego de programas e serviços específicos.
- Sensível ao Contexto: Considera o usuário, dispositivo e perfil da ameaça para filtrar o acesso.
- Servidores Proxy: Atuam como intermediários, filtrando conteúdos web como URLs e domínios.
- NAT: Oculta os endereços IP privados da rede interna contra o mundo exterior.

🔍 Varredura de Portas e Reconhecimento   
Cada aplicação em um dispositivo utiliza um número de porta para identificação. A varredura de portas é o processo de sondar essas entradas para identificar serviços ativos ou vulnerabilidades.
- Status Aberto: Indica que o serviço está acessível e pode ser explorado ou utilizado.
- Status Fechado: O serviço não está em execução, impossibilitando a exploração.
- Status Filtrado: Um firewall está protegendo a porta, bloqueando o acesso e a sondagem.

Nota-se que administradores utilizam ferramentas como Zenmap ou Nmap para validar políticas de segurança, enquanto atacantes as usam para mapear o sistema operacional do alvo.

🛡️ Detecção e Prevenção: IDS vs IPS   
Embora parecidos, esses sistemas possuem funções distintas na proteção de dados.
- IDS (Detecção): Monitora o tráfego em busca de anomalias e gera alertas. Ele funciona "fora da linha" (offline) para evitar atrasos na rede (latência), apenas relatando o ocorrido sem interrompê-lo.
- IPS (Prevenção): Atua diretamente no fluxo de dados, bloqueando o tráfego malicioso imediatamente ao detectar uma correspondência de regra ou assinatura.

⚡ Proteção em Tempo Real e Dia Zero   
Ataques de Dia Zero exploram falhas de software antes que os desenvolvedores criem correções. A detecção em tempo real é o objetivo final da segurança, exigindo análise de comportamento e integração com centros globais de inteligência de ameaças.

Ataques de DDoS são especialmente desafiadores, pois utilizam milhares de dispositivos infectados ("zumbis") para sobrecarregar servidores com tráfego que parece legítimo.

📊 Soluções Corporativas e Resposta   
Ferramentas como o Cisco AMP (Advanced Malware Protection) ajudam a combater Ameaças Persistentes Avançadas (APTs) através da análise de milhões de arquivos e seus comportamentos.
- Equipe SOC: Centraliza a coleta de dados para monitoramento contínuo.
- Resposta a Incidentes: Utiliza informações forenses para conter invasões com rapidez.
- Inteligência de Ameaças: Melhora a segurança de forma proativa com base em análises globais.

✅ Boas Práticas e Governança   
A conformidade com diretrizes de órgãos como o NIST fortalece a postura de segurança organizacional:
- Gestão de Riscos: Avaliar o valor dos ativos para justificar investimentos em defesa.
- Segurança Física: Restringir o acesso aos equipamentos e servidores.
- Backups e Atualizações: Testar regularmente a recuperação de dados e manter sistemas corrigidos.
- Educação de Usuários: Treinar funcionários para evitar falhas humanas (ex: Instituto SANS).

<a name="item04.01.01"><h4>4.1.1 Qual é?</h4></a>[Back to summary](#item04)

Isto é interessante! Você se pergunta qual sistema de segurança está sendo implementado na @Apollo. Você pergunta ao Chief Technology Officer (CTO), que explica que os seguintes dispositivos de segurança estão instalados. Você consegue identificar em qual categoria cada uma delas se encaixa? Você tem a chance de ganhar alguns pontos de defensor, então escolha suas respostas com cuidado. Selecione uma opção em cada um dos menus suspensos e clique em Enviar.
- Opções:
  - O Cisco ISR 4000 oferece roteamento, filtragem e criptografia em uma única plataforma.
    - Roteador.
  - O Cisco Firepower 4100 Series mostra o que está acontecendo na rede para que você possa agir com mais rapidez diante de um ataque cibernético.
    - Firewall.
  - O AnyConnect Secure Mobility Client da Cisco capacita funcionários remotos com acesso altamente seguro à rede de @Αpollo de qualquer dispositivo, a qualquer hora e em qualquer local.
    - VPN.
  - O AMP da Cisco oferece proteção de endpoint de próxima geração, varredura e monitoramento constante de arquivos em relação a comportamentos mal-intencionados.
    - Antimalware.

<a name="item04.01.02"><h4>4.1.2 Qual é?</h4></a>[Back to summary](#item04)

O CTO esqueceu de mencionar que o @Apollo tem alguns firewalls implementados. Com base nas seguintes afirmações, você consegue identificar qual é a categoria de firewall? Responda corretamente para ganhar pontos de defensor valiosos que ajudarão a proteger @Apollo de ataques. Selecione uma opção em cada um dos menus suspensos e clique em Enviar.
- Opções:
  - Uma pequena rede de área local interna com computadores requer acesso à Internet usando uma única conexão com a Internet
    - NAT firewall.
  - Por padrão, o Windows tenta bloquear o acesso a aplicativos em execução em computadores Windows de outros computadores na rede
    - Firewall baseado em host.
  - Os funcionários que usam computadores na rede não têm acesso a URLs específicas, como sites de jogos
    - Servidor proxy.

<a name="item04.01.03"><h4>4.1.3 O que isso significa?</h4></a>[Back to summary](#item04)

Seu gerente pede que você avalie o firewall da rede de computadores da @Apollo e a segurança de porta. Você executa uma varredura de porta, que retorna uma resposta de estado "aberto". Complete a frase abaixo preenchendo os espaços em branco de cada um dos menus suspensos para entender o que isso significa.

A varredura de portas reportou uma resposta de estado "aberto". Isso significa que o serviço em execução na rede - Selecione uma opção - por outros dispositivos de rede. Portanto, se o serviço contiver uma vulnerabilidade, ele - Selecione uma opção - pode ser explorado por um atacante.
- Opções:
  - pode ser acessado (V)
  - não pode ser acessado (F)
  - está bloqueado (F)
  - pode ser explorado (V)
  - não pode ser explorado (F)

<a name="item04.02"><h4>4.2 Abordagem comportamental à segurança cibernética</h4></a>[Back to summary](#item04)

🔍 Análise Comportamental e Testes de Intrusão   
A detecção de ameaças evoluiu para além da simples busca por vírus conhecidos. Atualmente, a segurança baseada em comportamento monitora o fluxo de comunicações para identificar desvios nos padrões normais, tratando qualquer anomalia como um potencial ataque em curso.

🍯 Ferramentas de Detecção Comportamental   
- Honeypots: São sistemas "chamariz" configurados para atrair invasores. Ao simular vulnerabilidades, permitem que os administradores capturem e analisem as táticas dos criminosos em um ambiente controlado, fortalecendo as defesas reais.
- Tecnologia NetFlow: Utilizada para coletar metadados sobre quem, como e quando a rede é acessada. Switches e roteadores equipados com essa tecnologia enviam dados para coletores que estabelecem uma "linha de base" de comportamento normal, facilitando a identificação de atividades suspeitas em mais de 90 atributos técnicos.

🛡️ O Processo de Teste de Penetração (Pen Test)   
O Pen Test é uma avaliação ativa onde especialistas tentam burlar as defesas de uma organização para descobrir falhas antes que criminosos o façam. O processo segue cinco etapas rigorosas:
- Planejamento: Coleta de informações e reconhecimento passivo sobre o alvo para identificar vetores de ataque.
- Varredura: Uso de ferramentas para investigar portas abertas, vulnerabilidades de software e enumeração de contas de usuário.
- Obtenção de Acesso: Fase de exploração real, utilizando engenharia social, quebra de criptografia Wi-Fi ou payloads para invadir o sistema.
- Manutenção do Acesso: O testador instala backdoors ou rootkits para garantir permanência e descobrir quais dados valiosos podem ser extraídos sem detecção.
- Análise e Relatório: Entrega de um documento técnico com recomendações de correções em produtos, políticas e treinamentos.

🚨 Resposta e Gestão de Incidentes   
Quando uma violação é confirmada, a rapidez e a transparência da organização são vitais para mitigar danos à reputação e à operação.
- Transparência e Responsabilidade: A empresa deve comunicar o problema interna e externamente de forma honesta, assumindo a responsabilidade por falhas eventuais.
- Ação Forense: Identificar a causa raiz da invasão e garantir que todos os sistemas estejam limpos de backdoors deixados pelos invasores.
- Mitigação de Danos: Informar aos clientes quais dados foram expostos e, frequentemente, arcar com custos de proteção contra roubo de identidade para os afetados.

📈 Gerenciamento de Riscos   
O risco cibernético não pode ser totalmente eliminado, mas deve ser gerenciado através de um processo formal que equilibra o custo da proteção com o valor do ativo protegido.
- Definição: Identificar ameaças que podem causar interrupção de serviços, perdas legais ou danos à imagem.
- Classificação: Priorizar riscos através de análise quantitativa (financeira) ou qualitativa (impacto operacional).
- Resposta: Decidir se o risco será eliminado (removendo a causa), mitigado (reduzindo o impacto), transferido (seguros) ou aceito (assumindo a perda potencial).
- Monitoramento: Análise contínua das ameaças aceitas ou mitigadas para garantir que os níveis de segurança permaneçam adequados.

Nota-se que grandes organizações mantêm equipes especializadas de Resposta a Incidentes de Segurança (CSIRT) para atuar exclusivamente na proteção e contenção de ataques digitais.

<a name="item04.02.01"><h4>4.2.1 Sua vez de</h4></a>[Back to summary](#item04)

Você foi encarregado de realizar um teste interno para verificar a rede de computadores da @Apollo em busca de vulnerabilidades. Como você conduzirá o teste? Faça isso direito e ganhe alguns muito necessários pontos de defensor. Coloque as etapas a seguir na ordem correta e depois envie.
- Opções:
  - Reúna o máximo de informações possível sem ser detectado (4)
  - Explore todas as vulnerabilidades identificadas na rede simulando um ataque (3)
  - Identifique possíveis vulnerabilidades exploráveis (2)
  - Investigue a rede para encontrar maneiras de invadir (1)
  - Relate suas descobertas para a equipe (5)

<a name="item04.03"><h4>4.3 Abordagem da Cisco para segurança cibernética</h4></a>[Back to summary](#item04)

🛡️ Gestão de Resposta a Incidentes e Prevenção Estratégica   
A maturidade da segurança digital em grandes organizações exige planos estruturados para a preparação, contenção e recuperação de violações. A utilização de equipes especializadas e ferramentas de automação é o diferencial para minimizar danos operacionais e reputacionais.

👥 Atuação das Equipes CSIRT   
As Equipes de Resposta a Incidentes de Segurança Computacional (CSIRT) são responsáveis pelo recebimento, análise e resolução de eventos críticos. Diferente de modelos puramente reativos, as equipes modernas atuam na frente de prevenção:
- Ações Proativas: Realizam avaliações constantes de ameaças, planejam mitigações, analisam tendências de ataques e revisam a arquitetura de segurança.
- Colaboração Global: A troca de inteligência com fóruns internacionais (como o FIRST e o DNS-OARC) garante que as organizações estejam atualizadas sobre novos métodos de exploração e vulnerabilidades.

📖 O Manual de Segurança (Playbook)   
Um manual de segurança é um documento técnico que padroniza os processos de detecção e resposta. Ele serve como um guia de execução para a equipe de segurança e deve abranger:
- Automação de Resposta: Definição de como identificar e responder automaticamente a malwares, comportamentos anômalos de rede e falhas de autenticação.
- Métricas e Estatísticas: Fornecimento de relatórios resumidos, tendências e acesso rápido a indicadores de desempenho (KPIs).
- Correlação de Dados: Integração de eventos provenientes de diversas fontes para uma visão holística do incidente.

🛠️ Ferramentas de Monitoramento e Proteção   
Para a execução das políticas de segurança, utilizam-se sistemas avançados que centralizam e protegem o fluxo de informações:
- SIEM (Gestão de Eventos e Informações de Segurança): Coleta e analisa logs e alertas em tempo real. Sua função é correlacionar dados históricos e atuais para permitir a detecção precoce de invasões.
- DLP (Prevenção de Perda de Dados): Sistema focado em impedir a exsudação de informações sensíveis. O monitoramento ocorre em três estados: dados em uso (acesso ativo), em movimento (tráfego de rede) e inativos (armazenamento permanente).

🔐 Controle de Acesso e Identidade   
A implementação de políticas de segurança pode ser complexa, exigindo soluções que automatizem o controle de usuários. O uso de tecnologias como o Cisco ISE (Identity Services Engine) e o TrustSec permite o reforço da segurança através de políticas baseadas em funções. Isso significa que o acesso aos recursos da rede não é concedido de forma genérica, mas de acordo com o papel específico de cada colaborador, dispositivo ou aplicação, garantindo o princípio do privilégio mínimo.

<a name="item04.03.01"><h4>4.3.1 Conheça a linguagem</h4></a>[Back to summary](#item04)

Este módulo contém muitas informações técnicas e jargões que você precisa saber para desenvolver sua carreira em segurança digital. Então, antes de prosseguir, vamos verificar sua compreensão de alguns desses termos-chave. É a sua última chance de ganhar pontos de defensor, então pense bem antes de fazer suas escolhas. Faça corresponder as descrições a seguir ao termo de segurança digital correto e envie.
- Opções:
  - Bloqueia ou nega o tráfego com base em uma correspondência de regra ou assinatura positiva.
    - IPS.
  - Um sistema projetado para impedir que dados confidenciais sejam roubados ou escapem de uma rede.
    - DLP.
  - Um sistema que coleta e analisa alertas de segurança, registros e outros dados históricos e em tempo real de dispositivos de segurança na rede.
    - SIEM.
  - Verifica os dados em um banco de dados de regras ou assinaturas de ataque, registra quaisquer detecções e cria um alerta para o administrador da rede.
    - IDS.
# Digital Safety and Security Awareness - Módulo 1   <img src="../0-aux/logo_course.png" alt="sfp_006" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="../">sfp_006 (Digital Safety and Security Awareness)   <img src="../0-aux/logo_course.png" alt="sfp_006" width="auto" height="25"></a>
### Module: 1. Há agentes maliciosos - Fique de olho!

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

### Course Module 1 Structure:
1. <a name="item01">Há agentes maliciosos - Fique de olho!</a><br>
1.1 <a href="#item01.01">Avaliação de Riscos</a><br>
1.2 <a href="#item01.02">Salvaguardar hoje e amanhã</a><br>
1.3 <a href="#item01.03">Falsificações & Filtros: Em Busca da Realidade</a><br>
1.4 <a href="#item01.04">Dicas para resolução de problemas</a><br>

---

### Objective:
O objetivo do módulo foi explorar os principais riscos e ameaças à segurança digital — como malware, phishing, engenharia social, deepfakes e roubo de identidade —, além de debater o impacto das pegadas digitais, os desafios das redes sociais e a interseção entre literacia digital e sustentabilidade ambiental.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01.01"><h4>1.1 Avaliação de Riscos</h4></a>[Back to summary](#item01)

🛡️ Impactos das Ameaças Digitais   
A proliferação de vetores de ataque no ambiente cibernético acarreta consequências operacionais, financeiras e reputacionais para indivíduos e corporações.
- Perda e Comprometimento de Dados: Incidentes decorrentes de invasões, malwares ou falhas operacionais resultam na interrupção de serviços, destruição de ativos de informação e sanções regulatórias.
- Roubo de Identidade e Fraudes Financeiras: A exfiltração de credenciais, dados bancários e identificadores pessoais viabiliza transações não autorizadas, comprometimento de contas e exaustão de recursos financeiros.
- Danos Reputacionais e Perda de Confiança: A exposição pública de falhas de segurança degrada a imagem institucional, resultando na perda de clientes, sanções legais e estigmatização interpessoal.

☣️ Principais Vetores e Táticas de Ataque   
Os agentes maliciosos empregam diferentes metodologias para explorar sistemas e fatores humanos:
- Malware: Softwares maliciosos (vírus, worms, trojans e ransomware) projetados para interromper operações, exfiltrar dados ou sequestrar sistemas mediante criptografia não autorizada.
- Phishing e Engenharia Social: Táticas baseadas em manipulação psicológica (como pretexting e baiting) e falsificação de identidade para induzir a entrega voluntária de dados sensíveis ou execução de artefatos nocivos.
- Ataques DDoS (Distributed Denial of Service): Inundação de tráfego direcionada a servidores ou redes para esgotar recursos de infraestrutura e indisponibilizar serviços.
- Credential Stuffing: Automação de testes massivos de combinações de usuário e senha vazadas previamente em múltiplos serviços para explorar a reutilização de credenciais.
- Explorações de Dia Zero (Zero-Day): Ataques direcionados a vulnerabilidades de software ainda desconhecidas pelos desenvolvedores, inexistindo correções ou patches de segurança disponíveis no momento da exploração.
- Ameaças Internas (Insider Threats): Comprometimento causado por colaboradores ou terceiros com acesso autorizado, atuando com intenção maliciosa ou por negligência operacional.

🔍 Tipologias de Ameaças e Mecanismos de Detecção   
A identificação prévia de anomalias operacionais permite mitigar invasões e mitigar a degradação de ativos tecnológicos:

🕵️ Spyware e Adware   
Programas voltados ao monitoramento não autorizado de atividades ou à exibição intrusiva de anúncios. Apresentam como sinais de infecção a degradação do desempenho do sistema, o surgimento de janelas pop-up e alterações de comportamento em aplicações. A mitigação envolve o uso de ferramentas de proteção endpoint e restrição de fontes de download.

🐴 Cavalo de Troia (Trojan)   
Artefato malicioso disfarçado de software legítimo. A execução concede aos atacantes controle parcial do sistema ou acesso persistente. Requer verificação rigorosa de integridade e autenticidade de instaladores antes da execução.

🌐 Pharming e Escutas em Redes Wi-Fi   
O pharming manipula o redirecionamento de tráfego DNS para direcionar conexões a instâncias falsas. As escutas em redes sem fio não seguras capturam tráfego não cifrado. O controle dessas ameaças exige a validação de certificados HTTPS, verificação de URLs e o uso de redes virtuais privadas (VPN).

📥 Downloads Drive-By e Deepfakes   
Os downloads drive-by executam scripts maliciosos de forma automatizada durante a navegação em sites comprometidos, exigindo mantenedores de navegação atualizados. Os deepfakes utilizam mídias sintéticas para manipulação e ataques de phishing avançados, demandando verificação multifatorial de identidade.

<a name="item01.02"><h4>1.2 Salvaguardar hoje e amanhã</h4></a>[Back to summary](#item01)

👶 Proteção Digital Infantil e Mecanismos de Controle   
A exposição precoce a recursos tecnológicos exige a implementação de estratégias preventivas para neutralizar riscos de ciberassédio, acesso a conteúdos inadequados e interação com perfis maliciosos.
- Filtros e Controles Parentais: Configuração de restrições de conteúdo em nível de sistema operacional, limitação de tempo de tela e emprego de softwares dedicados para monitoramento de tráfego e bloqueio de aplicações não autorizadas.
- Comunicação e Educação Orientada: Estabelecimento de diretrizes sobre privacidade de dados, conscientização acerca dos riscos da divulgação de informações pessoais e incentivo à notificação imediata de incidentes de cyberbullying.
- Gestão de Saúde e Atividades: Limitação de horas de exposição a telas para mitigar impactos no desenvolvimento cognitivo, distúrbios do sono e sedentarismo, promovendo o equilíbrio com atividades desconectadas.

👣 Pegada Digital e Impactos de Longo Prazo   
A persistência dos registros de navegação e de interações em ambientes virtuais molda a reputação do usuário, com reflexos permanentes na esfera pessoal e profissional.

📜 Immutabilidade e Visibilidade dos Dados   
Atividades em redes sociais, fóruns e plataformas de comunicação permanecem indexadas em repositórios digitais. Mesmo após a exclusão formal de publicações, o histórico mantido por serviços de terceiros pode ser resgatado por processos de auditoria ou indexação.

💼 Consequências Reputacionais e Profissionais   
Processos seletivos acadêmicos e corporativos empregam a análise de presença digital como critério de verificação comportamental. O histórico de postagens inadequadas, linguagem ofensiva ou conteúdos controversos pode resultar na desqualificação de candidatos ou em danos de imagem institucional.

🔒 Gestão Responsável da Identidade Virtual   
A administração consciente da presença online minimiza a exposição a riscos reputacionais e maximiza a utilidade da rede.
- Ajuste Restritivo de Privacidade: Configuração rigorosa dos níveis de visibilidade de perfis para restringir o acesso de dados pessoais apenas a conexões autorizadas.
- Avaliação de Impacto Pré-Publicação: Análise crítica quanto ao caráter das informações compartilhadas antes da veiculação de textos, imagens ou opiniões.
- Construção de Histórico Positivo: Utilização de plataformas digitais para o registro de projetos acadêmicos, iniciativas comunitárias e interações construtivas, consolidando um portfólio digital favorável.

<a name="item01.03"><h4>1.3 Falsificações & Filtros: Em Busca da Realidade</h4></a>[Back to summary](#item01)

🎭 Mídias Sintéticas e Tecnologia Deepfake   
A geração de conteúdo sintético por meio de algoritmos de Inteligência Artificial impõe desafios à autenticidade da informação e à integridade de dados biométricos.

🤖 Arquitetura das Redes Geradoras Adversárias (GANs)   
A criação de mídias sintéticas baseia-se no treinamento concorrente entre dois modelos de aprendizado de máquina:
- Gerador: Cria amostras de dados (imagens, áudios ou vídeos) com o objetivo de mimetizar distribuições reais.
- Discriminador: Avalia as amostras geradas em relação aos dados autênticos, buscando identificar falsificações.

O ajuste iterativo entre os modelos resulta em artefatos sintéticos de alta fidelidade e de difícil detecção por métodos convencionais.

⚠️ Riscos operacionais e sociais   
A disseminação descontrolada de deepfakes viabiliza fraudes de identidade, campanhas de desinformação massiva, extorsão e a erosão da confiança em evidências digitais (liar's dividend).

📱 Dinâmicas de Consumo em Redes Sociais   
As plataformas de compartilhamento de mídia estruturam a comunicação digital por meio da curadoria visual de conteúdo, impactando o comportamento dos usuários e a percepção da realidade.
- Filtros e Idealização Visual: A edição digital e a seleção deliberada de recortes de estilo de vida geram padrões irrealistas, demandando análise crítica por parte dos consumidores de conteúdo.
- Diversidade e Representatividade: Plataformas abertas viabilizam a democratização de narrativas e o alcance de públicos específicos sem a intermediação de veículos tradicionais de comunicação.
- Consumo Crítico da Informação: Prática de avaliação consciente das publicações, reduzindo o impacto psicológico adverso provocado pela comparação social contínua.

🌿 Alfabetização Digital e Sustentabilidade Tecnológica   
A interseção entre o uso de tecnologias digitais e a consciência ambiental exige a aplicação de critérios rigorosos na verificação de dados e na gestão do impacto ecológico da infraestrutura de TI.

🛡️ Mitigação de Desinformação Ambiental e Greenwashing   
O combate à disseminação de dados ambientais incorretos requer a checagem de fontes e a validação de certificações independentes em alegações corporativas de sustentabilidade, indo além de estratégias de marketing digital.

🔋 Pegada Ecológica da Infraestrutura Digital   
O funcionamento de ecossistemas tecnológicos gera impactos ambientais diretos que demandam práticas de mitigação:
- Consumo Energético de Data Centers: Processamento e armazenamento de dados em grande escala exigem alto consumo de eletricidade e sistemas de refrigeração.
- Descarte de Lixo Eletrônico (e-waste): A substituição precipitada de dispositivos requer fluxos adequados de reciclagem e descarte de componentes nocivos.
- Gestão Eficiente de Armazenamento: A eliminação de dados ociosos reduz a carga de processamento e a demanda por infraestrutura física de armazenamento.

<a name="item01.04"><h4>1.4 Dicas para resolução de problemas</h4></a>[Back to summary](#item01)

🛡️ Protocolos de Resolução de Incidentes e Mitigação de Riscos   
A identificação tempestiva de vetores de vulnerabilidade permite a aplicação de procedimentos corretivos para a preservação da integridade de sistemas e dados operacionais.

✉️ Resposta a Tentativas de Phishing Corporativo   
O recebimento de mensagens eletrônicas com solicitações atípicas de dados sigilosos exige a validação do cabeçalho do remetente e a abstenção de interação com hyperlinks ou anexos. A notificação imediata à equipe de resposta a incidentes de TI e a participação contínua em programas de conscientização reduzem a superfície de ataque associada à engenharia social.

🔐 Contenção de Comprometimento de Contas   
A identificação de acessos não autorizados em perfis de serviços online requer a redefinição imediata de credenciais de acesso e a sobreposição da autenticação multifator (2FA). A revogação de sessões ativas em dispositivos não reconhecidos e o alerta ao suporte da plataforma interrompem a persistência do atacante no ambiente.

🛒 Validação de Autenticidade em E-commerce   
A prevenção contra fraudes em transações eletrônicas baseia-se na verificação de certificados de segurança (HTTPS), inspeção de anomalias sintáticas nos nomes de domínio (typosquatting) e na seleção restrita de plataformas de comércio eletrônico consolidadas.
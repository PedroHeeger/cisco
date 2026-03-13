# Introdução à Cibersegurança - Módulo 1   <img src="../0-aux/logo_course.png" alt="sfp_004" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="../">sfp_004 (Introdução à Cibersegurança)   <img src="../0-aux/logo_course.png" alt="sfp_004" width="auto" height="25"></a>
### Module: 1. Introdução à Segurança Cibernética

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
1. <a name="item01">Introdução à Segurança Cibernética</a><br>
1.1 <a href="#item01.01">O mundo da segurança cibernética</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;1.1.1 <a href="#item01.01.01">Sua Identidade On-Line</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;1.1.2 <a href="#item01.01.02">O que os hackers querem?</a><br>
1.2 <a href="#item01.02">Dados organizacionais</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;1.2.1 <a href="#item01.02.01">O Que Você Acha?</a><br>
1.3 <a href="#item01.03">O que foi roubado?</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;1.3.1 <a href="#item01.03.01">O Que Aconteceu?</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;1.3.2 <a href="#item01.03.02">Quais Exploits?</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;1.3.3 <a href="#item01.03.03">Retrospectiva...</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;1.3.4 <a href="../../../labs/files/lab_049/">Laboratório - O que foi roubado?</a><br>
1.4 <a href="#item01.04">Invasores cibernéticos</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;1.4.1 <a href="#item01.04.01">Que é a Cor do Meu Chapéu?</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;1.4.2 <a href="#item01.04.02">O que você acha?</a><br>
1.5 <a href="#item01.05">Guerra cibernética</a><br>
1.6 Questionário<br>

---

### Objective:
O objetivo do módulo foi compreender os fundamentos da proteção de dados nos níveis pessoal, corporativo e governamental, identificando os diferentes perfis de invasores e as vulnerabilidades de tecnologias emergentes para mitigar os impactos de violações e conflitos no ciberespaço.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01.01"><h4>1.1 O mundo da segurança cibernética</h4></a>[Back to summary](#item01)

🛡️ Fundamentos da Segurança Cibernética   
A segurança cibernética é definida como um esforço contínuo e sistemático voltado à proteção de indivíduos, organizações e esferas governamentais contra ataques digitais. A preservação da integridade de dados e sistemas exige uma atuação em múltiplas camadas.

💻 Níveis de Proteção da Informação   
- Nível Particular: Foca na salvaguarda da identidade individual, dos dados pessoais e dos dispositivos de computação contra acessos não autorizados.
- Nível Corporativo: Estabelece a responsabilidade coletiva de proteger a reputação institucional, a base de dados e a privacidade dos clientes da organização.
- Nível Governamental: Prioriza a segurança nacional, a estabilidade econômica e o bem-estar dos cidadãos por meio da proteção de informações críticas coletadas e compartilhadas pelo Estado.

👤 A Identidade no Contexto Offline   
A identidade offline compreende as informações da vida cotidiana apresentadas em ambientes físicos, como residência, instituições de ensino ou locais de trabalho. Dados como nome completo, idade e endereço compõem esse perfil, sendo compartilhados com círculos sociais próximos. A negligência na proteção desses dados físicos facilita a atuação de criminosos especializados em furto de identidade.

🌐 A Natureza da Identidade Online   
A identidade online extrapola a utilização de um nome simples, abrangendo a forma como o indivíduo se projeta em ambientes digitais. Ela é composta por nomes de usuário, pseudônimos e a identidade social estabelecida em comunidades virtuais e redes sociais. Nota-se que a existência de uma identidade online não depende da criação voluntária de perfis em redes sociais; o simples uso da rede mundial de computadores gera um rastro digital. A recomendação técnica consiste em limitar rigorosamente a quantidade de informações pessoais reveladas nesses meios.

📄 Composição e Vulnerabilidade dos Dados Pessoais   
Os dados pessoais compreendem qualquer informação capaz de identificar um indivíduo, abrangendo desde registros oficiais, como números de identificação governamental e data de nascimento, até conteúdos privados, como mensagens e fotografias trocadas em ambientes digitais. A posse desses dados por criminosos virtuais viabiliza a falsidade ideológica e a violação da privacidade, resultando em danos severos à reputação e à segurança financeira do sujeito exposto.

🏥 Registros Médicos e de Saúde   
- Prontuários Eletrônicos (EHRs): Informações sobre saúde física e mental são armazenadas digitalmente em cada consulta, exigindo cautela sobre o volume de dados compartilhados em ambientes online.
- Tecnologias Vestíveis: Dispositivos como rastreadores de fitness e smartwatches coletam dados clínicos contínuos, incluindo frequência cardíaca e níveis glicêmicos. Estas informações são frequentemente armazenadas na nuvem, integrando o histórico médico do usuário.
- Compartilhamento Institucional: Dados médicos podem ser legitimamente compartilhados entre consultórios e seguradoras para fins de faturamento e auditoria, expandindo o número de entidades com acesso à informação.

🎓 Registros Educacionais e Profissionais   
- Esfera Acadêmica: Incluem qualificações, históricos de saúde escolar, registros de imunização e programas de educação individualizada (IEPs).
- Esfera Laboral: Dados sobre empregos anteriores e avaliações de desempenho atuais são alvos de interesse para a coleta de informações estratégicas por terceiros.

💳 Registros Financeiros e Hábitos de Consumo   
- Dados Econômicos: Extratos bancários, movimentações via aplicativos móveis, classificações de crédito e registros fiscais constituem informações de alto risco se não protegidas.
- Perfis de Consumo: Cartões de fidelidade em estabelecimentos comerciais são utilizados para mapear o comportamento de compra do usuário, permitindo o direcionamento de ofertas por parceiros de marketing.

🌐 A Dispersão de Dados e o Rastro Digital   
A replicação de dados ocorre de forma acelerada no ambiente digital. Uma fotografia capturada em um dispositivo móvel e compartilhada com terceiros pode ser baixada, replicada e publicada em servidores globais sem o consentimento do proprietário original. Nota-se que o acesso a serviços digitais muitas vezes ocorre mediante a cessão da privacidade. Empresas de mídia social utilizam algoritmos para extrair dados e direcionar publicidade, tratando a privacidade como a moeda de troca pela conveniência tecnológica oferecida.

⚠️ Riscos do Roubo de Identidade e Rastreamento Digital   
A atuação de criminosos digitais transcende o ganho financeiro imediato, focando estrategicamente no roubo de identidade para exploração de longo prazo. Essa prática compromete a integridade civil do indivíduo e pode gerar repercussões persistentes em diversas esferas da vida pessoal.

🏥 Exploração de Dados Médicos e Bancários   
- Fraude em Seguros de Saúde: O acesso indevido a dados de seguros permite que terceiros utilizem benefícios médicos. Como consequência, procedimentos realizados pelo criminoso são registrados permanentemente no histórico clínico da vítima, corrompendo seus prontuários.
- Comprometimento Financeiro e Fiscal: A posse de dados privados viabiliza o acesso a contas bancárias e cartões de crédito. Criminosos podem emitir declarações fiscais fraudulentas para reter reembolsos, além de contratar empréstimos que resultam na degradação do índice de crédito do titular legítimo.

🔍 Monitoramento e Comercialização de Dados por Entidades Legais   
Além de agentes maliciosos, diversas organizações monitoram a atividade digital com finalidades comerciais ou regulatórias:
- Provedores de Serviços de Internet (ISPs): Empresas de conectividade rastreiam o tráfego online e, dependendo da jurisdição, comercializam esses perfis para publicitários ou fornecem dados a órgãos de vigilância governamental por determinação legal.
- Mecanismos de Busca e Redes Sociais: Plataformas digitais consolidam informações sobre gênero, localização, contatos e inclinações ideológicas. Esses metadados, extraídos do histórico de navegação, são convertidos em ativos financeiros através da venda para o setor de publicidade.
- Publicitários e Sites Terceiros: O uso de cookies e ferramentas de rastreamento permite o monitoramento de hábitos de consumo e preferências. O rastro deixado pelo usuário é utilizado para criar anúncios direcionados e experiências personalizadas, frequentemente resultando no compartilhamento desses dados entre múltiplas redes de marketing.

A sofisticação das técnicas de obtenção de dados pessoais demonstra que a ameaça não se limita ao usuário individual, expandindo-se também para o ambiente de dados organizacionais.

<a name="item01.01.01"><h4>1.1.1 Sua Identidade On-Line</h4></a>[Back to summary](#item01)

É o seu primeiro dia de trabalho e é hora de escolher um nome de usuário para sua identidade on-line. Qual das seguintes opções você escolheria? Esta é a sua primeira chance de ganhar alguns pontos valiosos de defensor na empresa de eLearning @Apollo, então pense bem antes de fazer suas escolhas. Escolha duas respostas corretas e, em seguida, Enviar.
- Opções:
  - jdoe (V)
  - j.doe12 (V)
  - jane.doe (F)
  - jdoe.IT (F)
  - jdoe1990 (F)

<a name="item01.01.02"><h4>1.1.2 O que os hackers querem?</h4></a>[Back to summary](#item01)

Então, com todas essas informações disponíveis on-line, o que os hackers querem? Claro, eles querem seu dinheiro. Você consegue pensar em um exemplo do qual você já passou por experiência própria ou sobre o qual ouviu ou leu,  onde os criminosos digitais acessaram ou tentaram acessar informações financeiras on-line? Compartilhe seu exemplo na caixa abaixo e depois clique em Enviar. Depois de inserir seu exemplo, selecione Mostrar resposta para exibir um resumo.
- Um exemplo comum ocorre quando criminosos digitais enviam e-mails ou mensagens falsas que parecem ser de bancos ou empresas conhecidas, solicitando que a pessoa clique em um link e informe seus dados bancários ou senha. Ao acessar esse link e inserir as informações, os dados são enviados aos hackers, que podem utilizá-los para acessar contas bancárias ou realizar transações financeiras indevidas.

<a name="item01.02"><h4>1.2 Dados organizacionais</h4></a>[Back to summary](#item01)

💼 Classificação e Gestão de Dados Organizacionais   
Para a implementação de protocolos de segurança eficazes, é fundamental identificar a natureza das informações mantidas por uma organização. No contexto corporativo, os ativos de dados são categorizados em dois grupos principais.

📦 Categorias de Dados Corporativos   
- Dados Tradicionais: Compreendem o conjunto de informações fundamentais para a operação e competitividade.
  - Propriedade Intelectual: Inclui patentes, marcas e projetos de inovação. A proteção desses segredos comerciais é vital para a manutenção da vantagem competitiva.
  - Dados Financeiros: Relatórios de fluxo de caixa, balanços patrimoniais e demonstrativos de resultados que refletem a viabilidade econômica da instituição.
- IoT e Big Data: A expansão da Internet das Coisas (IoT) através de sensores e dispositivos conectados gera um volume massivo de informações. Esse fenômeno, aliado ao armazenamento em nuvem e virtualização, impulsiona o conceito de Big Data, exigindo novas estratégias de tratamento de dados.

🧊 O Modelo de Segurança: Cubo de McCumber   
Desenvolvida em 1991, esta estrutura fornece uma metodologia tridimensional para avaliar e estabelecer iniciativas de segurança da informação, dividindo-se em princípios fundamentais, estados do dado e medidas de proteção.

🛡️ Dimensão 1: Princípios Fundamentais (Tríade CID)   
- Confidencialidade: Garante que o acesso à informação seja restrito a entes autorizados. É assegurada por métodos como criptografia e autenticação de dois fatores (2FA).
- Integridade: Protege os dados contra alterações indevidas, sejam elas acidentais ou maliciosas. O uso de funções hash e somas de verificação (checksum) são práticas comuns para validar a precisão dos registros.
- Disponibilidade: Assegura que sistemas e informações estejam acessíveis sempre que necessário para usuários legítimos. Envolve manutenção preventiva de hardware, atualizações de software e rotinas de backup.

💾 Dimensão 2: Estados da Informação   
- Em Processamento (Dados em Processo): Informações que estão sendo manipuladas ativamente por operações de sistema ou bancos de dados.
- Em Armazenamento (Dados em Repouso): Dados retidos em suportes físicos ou digitais, como discos rígidos, memórias permanentes ou unidades USB.
- Em Transmissão (Dados em Trânsito): Informações em movimento, trafegando entre sistemas através de redes de comunicação.

⚙️ Dimensão 3: Medidas de Segurança   
- Educação e Conscientização: Iniciativas voltadas ao treinamento de usuários para o reconhecimento de ameaças e adoção de comportamentos seguros.
- Tecnologia: Implementação de soluções de hardware e software, como firewalls e sistemas de monitoramento, para a detecção de incidentes.
- Políticas e Procedimentos: Controles administrativos que definem as diretrizes de governança, incluindo planos de resposta a incidentes e manuais de boas práticas.

⚠️ Vulnerabilidades em Infraestruturas de Nuvem e IoT   
A exploração de falhas em configurações de nuvem e dispositivos conectados representa um dos maiores riscos para a integridade de dados organizacionais. Incidentes reais demonstram que configurações incorretas em clusters de nuvem podem expor segmentos inteiros de uma infraestrutura à internet pública. No caso de exposições prolongadas, informações de clientes podem ser coletadas por agentes maliciosos para a execução de ataques de engenharia social e fraudes sofisticadas. Tais eventos reforçam a necessidade de uma postura proativa e vigilante quanto à segurança de instâncias de armazenamento e redes virtuais.

🤖 O Impacto de Botnets e Ataques Distribuídos   
O crescimento da Internet das Coisas (IoT) expandiu a superfície de ataque para criminosos digitais. Um exemplo notável é o botnet Persirai, que comprometeu milhares de modelos de câmeras IP através de portas de comunicação abertas. O método de ataque envolveu a injeção de comandos que forçavam o download de malwares executados diretamente na memória do dispositivo para evitar detecção. Uma vez sequestrados, esses equipamentos foram utilizados para realizar ataques de Negação de Serviço Distribuído (DDoS), sobrecarregando recursos de sistemas alvo sem que os proprietários dos dispositivos percebessem a atividade.

📉 Vulnerabilidades em Aplicações Web e Domínios   
Falhas em softwares de aplicações web podem servir de porta de entrada para o acesso a dados sensíveis em larga escala, como demonstrado no incidente da agência Equifax. A resposta inadequada a uma crise de segurança também pode gerar novos riscos. Ao utilizar domínios alternativos para auxiliar vítimas, empresas podem facilitar a criação de sites fraudulentos por atacantes. Esses endereços clonados enganam os usuários, induzindo-os a fornecer dados que permitem a usurpação completa de identidade, tornando a contestação de fraudes extremamente complexa para o cliente legítimo.

🛡️ Medidas de Vigilância e Mitigação de Danos   
A proteção contra os impactos de violações de dados exige atenção constante do usuário e das organizações.
- Monitoramento de Crédito: É necessário revisar relatórios financeiros regularmente para identificar solicitações de crédito ou compras não autorizadas.
- Validação de Canais: Em momentos de crise, deve-se verificar rigorosamente a autenticidade de sites antes de inserir informações de identificação pessoal.
- Relato de Incidentes: Qualquer atividade suspeita ou informação falsa deve ser comunicada imediatamente às autoridades financeiras e instituições competentes para minimizar o impacto da exposição.

📉 Impactos e Consequências das Violações de Segurança   
As repercussões de um incidente de segurança digital são profundas e podem comprometer a continuidade de uma organização. A análise dos danos revela que o impacto financeiro é apenas uma das dimensões afetadas, estendendo-se para a esfera moral e competitiva.

🏢 Danos à Reputação e Credibilidade   
- Perda de Confiança: A exposição de dados negativos pode destruir a imagem institucional construída ao longo de anos. Clientes afetados frequentemente buscam compensações financeiras ou migram para concorrentes que demonstrem maior robustez em segurança.
- Evasão de Talentos: Crises de segurança e escândalos corporativos podem desmotivar o corpo técnico e administrativo, levando à saída de funcionários qualificados.
- Reparação de Imagem: O processo de recuperação da confiança do mercado é lento e exige investimentos significativos em comunicação e transparência após a notificação dos envolvidos.

🎨 Vandalismo Digital e Desinformação   
Grupos de invasores podem comprometer a integridade de sites corporativos para publicar informações falsas. Alterações sutis em dados de contato, como endereços ou números de telefone, são táticas de difícil detecção imediata que projetam uma imagem de amadorismo e reduzem a credibilidade da organização perante o público.

💸 Perdas Financeiras e Roubo de Ativos   
- Subtração de Dados e Valores: Violações frequentemente resultam no furto de informações sensíveis que são vendidas ou utilizadas para a apropriação indébita de recursos financeiros e identidades.
- Interrupção de Operações: Ataques que tornam sites e sistemas indisponíveis impedem a realização de negócios online, paralisando a geração de receita.
- Custos Regulatórios: A negligência na proteção de dados pode acarretar multas severas e penalidades aplicadas por órgãos reguladores, além da necessidade de gastos emergenciais na reestruturação da infraestrutura de segurança.

💡 Comprometimento da Propriedade Intelectual   
A competitividade de uma empresa é severamente prejudicada quando segredos comerciais, patentes e documentos estratégicos são acessados por terceiros. A perda do controle sobre a propriedade intelectual pode anular vantagens de mercado e beneficiar diretamente a concorrência.

🛠️ A Resposta a Incidentes como Prioridade   
Nota-se que a proteção absoluta contra todos os ataques digitais é tecnicamente inviável, visto que métodos de invasão evoluem continuamente. Diante da inevitabilidade de tentativas de ataque, a função dos profissionais de segurança digital reside na capacidade de monitoramento constante e na rapidez da resposta aos incidentes para mitigar danos e restaurar a normalidade operacional.

<a name="item01.02.01"><h4>1.2.1 O Que Você Acha?</h4></a>[Back to summary](#item01)

Um cliente preocupado encaminhou o que acredita ser um e-mail fraudulento. Parece que foi enviado por @Apollo, mas algo parece um pouco “phish-y”. Dê uma olhada no e-mail. Qual das seguintes opções indica que na verdade é um e-mail de phishing? Não se esqueça, você tem a chance de ganhar pontos de defensor valiosos se responder a isso corretamente 
Selecione as quatro respostas corretas e clique em Enviar.
- Opções:
  - O idioma, a ortografia e a gramática (V)
  - Gráficos (V)
  - Endereço de e-mail (V)
  - Nome do cliente (F)
  - Link da URL (V)

<a name="item01.03"><h4>1.3 O que foi roubado?</h4></a>[Back to summary](#item01)

🛡️ Definição e Prevenção de Violações de Segurança   
Uma violação de segurança é caracterizada como um incidente que possibilita o acesso não autorizado a dados, aplicações, serviços ou dispositivos. Tal exposição compromete informações privadas, as quais são frequentemente exploradas por invasores para a obtenção de vantagens financeiras ou benefícios estratégicos. Para a mitigação desses riscos, é fundamental a adoção de medidas protetivas tanto no âmbito individual quanto no corporativo. A segurança robusta baseia-se nos seguintes pilares:
- Consciência de Ameaças: É necessário manter-se atualizado sobre os métodos e vetores de ataques digitais mais comuns.
- Vigilância Contínua: A adoção de uma postura atenta na manipulação de informações sensíveis reduz as probabilidades de sucesso de ações maliciosas.
- Implementação de Defesas: O uso de práticas recomendadas de segurança atua como uma barreira preventiva, impedindo que usuários e organizações se tornem alvos vulneráveis.

<a name="item01.03.01"><h4>1.3.1 O Que Aconteceu?</h4></a>[Back to summary](#item01)

Cenário 1: Hoje, as violações de segurança são muito comuns, com os invasores constantemente encontrando maneiras novas e inovadoras de se infiltrar nas empresas em busca de informações valiosas. Role para baixo para ler a última notícia de segurança.

De acordo com nossas fontes, uma conhecida cadeia de hotéis que opera em todo o mundo relatou uma violação de dados enorme, com as informações pessoais de mais de três milhões de hóspedes expostas a hackers. O hotel descobriu que os hackers obtiveram acesso ao banco de dados de clientes usando os detalhes de login de um de seus funcionários. Neste momento, o hotel não acredita que os hackers puderam acessar senhas de contas ou informações financeiras. Hóspedes recentes são incentivados a verificar o portal web da cadeia de hotéis para ver se eles foram afetados por essa violação. Este é um cenário fictício. Neste exemplo, o que os hackers pegaram? Selecione a resposta correta e clique em Enviar.
- Opções:
  - As informações de pagamento com cartão de mais de três milhões de hóspedes (F)
  - O nome de usuário e a senha de todos os funcionários do hotel (F)
  - Os nomes, endereço de e-mail e números de telefone de mais de três milhões de hóspedes do hotel (V)
  - A reputação da rede de hotéis (F)

<a name="item01.03.02"><h4>1.3.2 Quais Exploits?</h4></a>[Back to summary](#item01)

Cenário 2: Plataformas de eLearning em risco! A equipe da @Apollo está preocupada. As plataformas de eLearning estão se tornando os principais alvos dos invasores, à medida que mais e mais empresas migram para a aprendizagem digital. Selecione as setas para saber mais sobre um caso recente. 

Uma plataforma de treinamento on-line popular admitiu ter deixado os dados pessoais de milhões de seus alunos (muitos deles menores) expostos em um banco de dados em nuvem publicamente acessível. Os hackers conseguiram acessar diretamente os nomes completos dos alunos, endereços de e-mail, números de telefone e detalhes de matrícula na escola pela Internet! Embora não esteja claro o que os hackers fizeram com essas informações adquiridas, é seguro dizer que eles têm tudo o que precisam para realizar ataques generalizados de phishing ou malware.

Quais exploits os hackers usaram nesse caso para obter acesso a informações pessoais valiosas? Selecione a resposta correta e clique em Enviar.
- Opções:
  - Ignorando os métodos de controle de acesso da plataforma (F)
  - Tirando vantagem de informações do aluno não sendo validadas corretamente na plataforma (F)
  - Extração de informações quando o volume de dados do aluno exceder a capacidade de armazenamento do buffer de memória da plataforma (F)
  - Fragilidade nas práticas de segurança da plataforma (V)

<a name="item01.03.03"><h4>1.3.3 Retrospectiva...</h4></a>[Back to summary](#item01)

Toda empresa corre o risco de sofrer um ataque digital e, portanto, deve tomar as medidas necessárias para se proteger. Considerando cada um dos dois exemplos de violação de segurança descritos acima, que medidas essas empresas poderiam ter implementado para evitar essas violações de segurança? Escreva sua opinião na caixa abaixo e depois envie. Selecione Mostrar resposta para verificar sua resposta.
- Para o cenário 1, a empresa poderia ter implementado uma política de senha forte e autenticação de dois fatores para os funcionários, além de monitoramento contínuo de atividades suspeitas no banco de dados. Para o cenário 2, a plataforma de eLearning deveria ter configurado corretamente as permissões do banco de dados em nuvem, evitando acesso público e permitindo acesso apenas a usuários autorizados, além de utilizar criptografia de dados e auditorias regulares de segurança para identificar vulnerabilidades.

<a name="item01.04"><h4>1.4 Invasores cibernéticos</h4></a>[Back to summary](#item01)

🕵️ Classificação e Perfil dos Agentes Invasores   
Invasores cibernéticos são indivíduos ou grupos que buscam identificar e explorar falhas em sistemas para obter benefícios próprios, sejam eles financeiros, pessoais ou políticos. O alvo desses agentes varia desde dados bancários até segredos industriais complexos.

💻 Categorias de Hackers por Conduta   
A comunidade de segurança frequentemente utiliza uma analogia baseada em cores de "chapéus" para diferenciar as motivações e a legalidade das ações dos hackers:
- Invasores White Hat (Chapéu Branco): Atuam de forma ética e legal. São especialistas contratados para realizar testes de intrusão e identificar vulnerabilidades com a autorização dos proprietários, visando fortalecer as defesas do sistema.
- Invasores Gray Hat (Chapéu Cinzento): Operam em uma zona cinzenta de legalidade. Podem identificar falhas sem permissão, mas o reporte dessas vulnerabilidades depende de seus interesses pessoais. Em certos casos, expõem as falhas publicamente, o que pode facilitar ataques por terceiros.
- Invasores Black Hat (Chapéu Preto): Agem com intenções puramente maliciosas e ilegais. Exploram qualquer fragilidade encontrada para obter lucros ilícitos, exercer influência política ou causar danos diretos às vítimas.

👤 Hackers Amadores (Script Kiddies)   
O termo, consolidado na década de 1990, descreve indivíduos com pouco conhecimento técnico profundo que utilizam softwares e scripts prontos, disponíveis na internet, para realizar ataques. Embora careçam de expertise para criar as próprias ferramentas, a atuação desses amadores pode causar prejuízos significativos, sendo motivada por curiosidade ou pelo desejo de exibir habilidades técnicas em comunidades online.

🏢 Hackers Organizados e Estruturados   
Este grupo representa a ameaça mais sofisticada e persistente, contando com alta organização e, muitas vezes, financiamento robusto:
- Criminosos Virtuais: Operam o crime digital como um modelo de negócio, chegando a oferecer ataques como serviço para outros agentes ilícitos.
- Hacktivistas: Realizam invasões e vazamentos para promover causas ideológicas ou políticas, visando atrair atenção pública para temas específicos.
- Agentes Patrocinados pelo Estado: Hackers altamente treinados que atuam sob o comando de governos nacionais. O foco desses profissionais reside na espionagem, coleta de inteligência estratégica ou sabotagem de infraestruturas críticas de outras nações.

🌍 Origens das Ameaças Cibernéticas   
Os ataques digitais podem ser classificados de acordo com o seu ponto de origem em relação ao perímetro da organização. Compreender se a ameaça é interna ou externa é fundamental para a definição de estratégias de defesa e controle de acesso.

🏢 Ameaças Internas   
As ameaças internas são originadas por indivíduos que possuem ou possuíam acesso legítimo aos sistemas, como funcionários, prestadores de serviços ou parceiros comerciais. Estas ações podem ocorrer de forma deliberada ou por negligência:
- Manuseio Inadequado de Dados: Manipulação incorreta ou exposição de informações sensíveis sem intenção maliciosa.
- Uso de Mídia Infectada: Introdução de códigos maliciosos na infraestrutura ao conectar dispositivos USB ou periféricos comprometidos.
- Fator Humano e Engenharia Social: Facilitação da entrada de malware na rede corporativa através do clique em links de e-mails de phishing ou acesso a sites mal-intencionados.
- Sabotagem Operacional: Ações direcionadas a comprometer o funcionamento de servidores internos ou equipamentos de infraestrutura de rede.

🌐 Ameaças Externas   
As ameaças externas provêm de agentes sem autorização prévia, variando de amadores a grupos altamente qualificados, que operam fora dos limites da empresa:
- Exploração de Vulnerabilidades: Identificação e uso de falhas técnicas na rede para ganhar acesso ilícito.
- Bloqueio de Acesso: Tentativas de impedir que usuários legítimos acessem seus próprios dados ou recursos computacionais.
- Engenharia Social Externa: Uso de técnicas de manipulação psicológica para induzir colaboradores a revelarem credenciais ou dados organizacionais críticos.

<a name="item01.04.01"><h4>1.4.1 Que é a Cor do Meu Chapéu?</h4></a>[Back to summary](#item01)

Agora que você conhece os diferentes tipos de invasores e suas motivações para fazer o que eles fazem, você pode identificar qual cor de chapéu é usada pelo invasor em cada um dos seguintes cenários? Essa é uma tarefa complicada, mas lembre-se, você pode ganhar pontos de defensor valiosos se responder corretamente. Selecione a resposta correta nas listas suspensas e depois envie.
- Depois de invadir sistemas ATM remotamente usando um laptop, esse invasor trabalhou com os fabricantes de ATMs para resolver as vulnerabilidades de segurança identificadas.
  - Gray Hat.
- Esse invasor transferiu US$ 10 milhões para sua conta bancária usando a conta do cliente e as credenciais de PIN obtidas de gravações.
  - Black Hat.
- O trabalho desse invasor é identificar pontos fracos no sistema de computadores de uma empresa.
  - White Hat.
- Este invasor usou malware para comprometer o sistema de uma empresa e roubar informações de cartão de crédito que foram vendidas pelo lance mais alto.
  - Black Hat.
- Ao realizar algumas pesquisas, esse invasor encontrou uma vulnerabilidade de segurança na rede de uma empresa que está autorizado a acessar.
  - White Hat.

<a name="item01.04.02"><h4>1.4.2 O que você acha?</h4></a>[Back to summary](#item01)

Lembra do e-mail de phishing que você recebeu anteriormente de um de seus clientes? Uma investigação sobre este e-mail revelou que as contas de usuário e os privilégios de acesso de um ex-funcionário não foram totalmente removidos dos sistemas de TI ao sair da empresa. Na verdade, esse ex-funcionário, que agora trabalha para um concorrente, fez login no banco de dados de clientes da @Apollo há apenas três dias. Ocorreu uma ameaça à segurança interna ou externa? Selecione uma resposta e depois Enviar.
- Opções:
  - Interno (V)
  - Externo (F)

<a name="item01.05"><h4>1.5 Guerra cibernética</h4></a>[Back to summary](#item01)

🌐 Conceitos e Impactos da Guerra Cibernética   
A guerra cibernética caracteriza-se pelo emprego estratégico de meios tecnológicos para infiltrar, comprometer e desabilitar redes e sistemas computacionais de outras nações. Diferente do crime digital comum, o objetivo central é a sabotagem em escala nacional, visando a interrupção de serviços essenciais e a geração de danos físicos ou operacionais.

Um marco histórico nesse cenário foi o uso do malware Stuxnet, desenvolvido para ultrapassar as barreiras de sistemas digitais e atuar diretamente na destruição de equipamentos industriais físicos. O caso demonstrou que ataques virtuais podem paralisar instalações críticas, como usinas de enriquecimento nuclear, sem a necessidade de intervenção militar presencial.

🛡️ Objetivos Estratégicos do Conflito Digital   
As nações utilizam as capacidades ofensivas no ciberespaço para obter vantagens sobre adversários através de frentes específicas:
- Espionagem e Coleta de Inteligência: Busca-se a captura de segredos de defesa, planos militares e inovações tecnológicas para reduzir disparidades entre potências. Além disso, o acesso a informações confidenciais permite a chantagem de figuras governamentais.
- Sabotagem de Infraestrutura Crítica: O foco reside na criação de caos social e econômico. Ataques direcionados a redes elétricas, por exemplo, podem paralisar o tráfego urbano, interromper o comércio, impedir atendimentos médicos de emergência e cortar o acesso à comunicação global.
- Desestabilização Nacional: A guerra digital permite afetar o comércio internacional e erodir a confiança da população em suas instituições governamentais sem que ocorra uma invasão física do território.

🚀 A Demanda por Profissionais de Segurança   
Dada a gravidade das consequências e a disseminação crescente dessas táticas, a proteção de cidadãos e infraestruturas tornou-se uma prioridade de segurança nacional. O contexto atual exige especialistas capacitados para antecipar ameaças e responder a incidentes em ambientes de alta complexidade técnica.
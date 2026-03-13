# Introdução à Cibersegurança - Módulo 3   <img src="../0-aux/logo_course.png" alt="sfp_004" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="../">sfp_004 (Introdução à Cibersegurança)   <img src="../0-aux/logo_course.png" alt="sfp_004" width="auto" height="25"></a>
### Module: 3. Protegendo seus dados e privacidade

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

### Course Module 3 Structure:
3. <a name="item03">Protegendo seus dados e privacidade</a><br>
3.1 <a href="#item03.01">Como proteger a rede e os dispositivos</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.1.1 <a href="#item03.01.01">O Que Você Acha?</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.1.2 <a href="#item03.01.02">Segurança de senha</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.1.3 <a href="#item03.01.03">Verificação de senha</a><br>
3.2 <a href="#item03.02">Manutenção de dados</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.2.1 <a href="#item03.02.01">Eles realmente desapareceram?</a><br>
3.3 <a href="#item03.03">Quem é o dono dos seus dados?</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.3.1 <a href="#item03.03.01">Termos de serviço</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.3.2 <a href="#item03.03.02">O que você está concordando? | Qual é a Política de Uso de Dados?</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.3.3 <a href="#item03.03.03">Configurações de privacidade</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.3.4 <a href="#item03.03.04">Proteja seus dados</a><br>
3.4 <a href="#item03.04">Como proteger a privacidade on-line</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.4.1 <a href="#item03.04.01">Compartilhamento social</a><br>
3.5 <a href="#item03.05">Descobrir seu próprio comportamento on-line arriscado</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.5.1 <a href="#item03.05.01">Cenário 1</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.5.2 <a href="#item03.05.02">Cenário 2</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.5.3 <a href="#item03.05.03">Cenário 3</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.5.4 <a href="#item03.05.04">Cenário 4</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.5.5 <a href="#item03.05.05">Cenário 5</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.5.6 <a href="#item03.05.06">Cenário 6</a><br>
3.6 Questionário<br>

---

### Objective:
O objetivo do módulo foi compreender as estratégias essenciais para a proteção de dispositivos e redes, abordando desde a criação de credenciais robustas e o uso de autenticação de múltiplos fatores até a implementação de criptografia e backups, visando garantir a soberania sobre os dados pessoais e a segurança da identidade no ambiente digital.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item03.01"><h4>3.1 Como proteger a rede e os dispositivos</h4></a>[Back to summary](#item03)

🛡️ Proteção e Higiene Digital de Dispositivos   
A segurança online fundamenta-se na adoção de medidas preventivas que transformam os dispositivos computacionais em barreiras contra o acesso não autorizado. Como os dispositivos móveis e desktops funcionam como portais para dados pessoais e armazenamento em nuvem, sua proteção é a primeira linha de defesa do usuário.

🖥️ Configurações Essenciais de Segurança   
- Ativação de Firewalls: É fundamental a utilização de ao menos uma camada de firewall (seja via software no sistema operacional ou hardware no roteador). Esta ferramenta monitora o tráfego e bloqueia tentativas de invasão externa.
- Software Antimalware: A instalação de antivírus e antispyware de fontes confiáveis é indispensável. Estes programas identificam códigos que visam destruir dados, sequestrar contas para envio de spam ou monitorar hábitos de navegação. A atualização constante é o que garante a proteção contra novas variantes de ameaças.
- Manutenção do Ecossistema: Hackers exploram falhas conhecidas em sistemas operacionais e navegadores. Recomenda-se configurar o nível de segurança para "médio" ou "superior" e aplicar imediatamente patches e atualizações de segurança fornecidos pelos fabricantes.

🔐 Gestão de Acessos e Criptografia   
Todos os equipamentos, incluindo tablets e smartphones, devem possuir proteção por senha. Dados sensíveis devem ser criptografados para garantir que, em caso de perda ou roubo físico, o conteúdo permaneça ilegível. Nota-se que o comprometimento de um dispositivo local pode dar aos criminosos acesso total a serviços de armazenamento em nuvem, como Google Drive ou iCloud, ampliando o alcance do dano.

📡 Segurança em Redes Sem Fio e Bluetooth   
As redes Wi-Fi residenciais exigem configurações que vão além da simples ocultação do SSID. Hackers possuem ferramentas para identificar redes ocultas e senhas padrão de fábrica.
- Criptografia WPA2: Este protocolo deve estar habilitado, mas é necessário cautela, pois vulnerabilidades como o ataque KRACK (reinstalação de chave) podem interromper a cifragem entre o roteador e o dispositivo.
- Mitigação de Riscos Wi-Fi: Para maior segurança, deve-se priorizar conexões cabeadas (NIC), utilizar serviços de VPN confiáveis e manter o firmware dos roteadores atualizado.
- Uso de Bluetooth: O protocolo Bluetooth pode ser explorado para espionagem e controle remoto. Recomenda-se manter esta funcionalidade desativada quando não houver uso ativo.

🌐 Cuidados em Redes Públicas (Hotspots)   
O uso de Wi-Fi público apresenta riscos elevados de interceptação de dados (eavesdropping). Em redes abertas, as seguintes diretrizes são fundamentais:
- Restrição de Tráfego: Evitar o acesso a contas bancárias ou envio de informações confidenciais.
- Desativação de Compartilhamento: Garantir que o compartilhamento de arquivos e mídia esteja desligado nas configurações do sistema.
- Uso de VPN: A utilização de um túnel VPN criptografado é a medida mais eficaz para impedir que terceiros interceptem e decifrem a comunicação entre o dispositivo e a internet.

🏠 Desafios da Internet das Coisas (IoT)   
Diferente de computadores e smartphones, muitos dispositivos de IoT (como câmeras e eletrodomésticos inteligentes) raramente recebem atualizações de software, permanecendo vulneráveis a falhas de fabricação por longos períodos. Uma vez comprometido, um dispositivo IoT pode servir como porta de entrada para a rede local da residência. A prática técnica recomendada consiste em isolar esses dispositivos em uma rede segmentada, impedindo que uma falha em um sensor comprometa o acesso a computadores principais.

🔐 Estratégias para Criação de Credenciais Robustas   
A segurança de contas e sistemas depende diretamente da complexidade das credenciais de acesso. Senhas frágeis são a principal porta de entrada para invasões, tornando essencial a adoção de padrões que dificultem ataques automatizados de dicionário ou força bruta.

📋 Diretrizes para Senhas Fortes   
- Extensão Mínima: Recomenda-se a utilização de sequências com mais de dez caracteres.
- Diversidade de Caracteres: Deve-se incluir símbolos especiais (como !, @, #, $) para elevar a entropia da senha.
- Evitar Padrões Óbvios: É necessário abster-se do uso de nomes de usuários, nomes de computadores, palavras dicionarizadas (em qualquer idioma) ou erros ortográficos comuns de termos conhecidos.

💬 Uso de Frases Secretas (Passphrases)   
Uma alternativa eficaz ao uso de senhas curtas é a adoção de frases secretas. Elas consistem em sentenças que, embora fáceis de memorizar para o usuário, são extremamente difíceis de serem quebradas por softwares de ataque devido à sua extensão.
- Personalização: Deve-se escolher afirmações com significado pessoal, evitando citações famosas ou letras de músicas populares.
- Complexidade Estrutural: A inserção de caracteres especiais dentro da frase potencializa sua segurança.
- Resistência: Por serem mais longas, as frases secretas oferecem uma defesa superior contra tentativas de exaustão de caracteres.

🏛️ Padrões Modernos do NIST   
O Instituto Nacional de Padrões e Tecnologia (NIST) estabeleceu diretrizes atualizadas que visam equilibrar a segurança técnica com a usabilidade para o usuário final. Estes requisitos são amplamente adotados por governos e setores corporativos de alta criticidade.
- Limites de Caracteres: As senhas devem possuir entre 8 e 64 caracteres.
- Simplificação de Regras: O NIST desencoraja regras rígidas de composição (obrigatoriedade de maiúsculas/minúsculas) e períodos de expiração arbitrários, que muitas vezes levam o usuário a criar senhas previsíveis.
- Acessibilidade e Precisão: É recomendado que o sistema permita a visualização da senha durante a digitação para evitar erros e que aceite todos os tipos de caracteres e espaços.
- Eliminação de Métodos Inseguros: Práticas como "dicas de senha" e "perguntas de segurança" baseadas em conhecimento pessoal devem ser abolidas, pois são facilmente pesquisáveis por engenharia social.

<a name="item03.01.01"><h4>3.1.1 O Que Você Acha?</h4></a>[Back to summary](#item03)

Você acabou de receber o novo laptop da @Apollo e está se preparando para configurá-lo. Quais etapas você tomaria para protegê-lo antes de usá-lo? Escreva sua opinião na caixa abaixo e depois envie. Depois de inserir as etapas, selecione Mostrar resposta para exibir o feedback.
- Antes de começar a usar o laptop, eu configuraria uma senha forte para o sistema e habilitaria a autenticação de dois fatores, se disponível. Em seguida, instalaria todas as atualizações do sistema operacional, ativaria o firewall, instalaria um antivírus confiável e garantiria que o disco estivesse criptografado para proteger os dados. Também evitaria conectar o dispositivo a redes Wi-Fi públicas sem proteção e manteria backups regulares dos arquivos importantes.

<a name="item03.01.02"><h4>3.1.2 Segurança de senha</h4></a>[Back to summary](#item03)

Você fez login no seu novo laptop e ele solicitou que você alterasse sua senha de rede. Você já se esforça para lembrar as poucas senhas que usa para suas contas pessoais online. Você pede conselhos a um de seus colegas. Eles dizem para você usar uma das senhas usadas nas suas contas pessoais - isso é o que elas fazem! Eles mantêm suas senhas pessoais anotadas no final de seu diário, caso as esqueçam. Como você classificaria a atitude de seu colega em relação à segurança de senha em uma escala de 1 (prática inadequada) a 5 (prática recomendada)? Faça sua escolha deslizando o marcador na escala e depois enviando.
- Opção:
  - Prática Inadequada (1)

<a name="item03.01.03"><h4>3.1.3 Verificação de senha</h4></a>[Back to summary](#item03)

Com base em todas essas informações, você está pronto para atualizar sua senha de rede. Você está considerando várias opções possíveis. Dê uma olhada em cada uma das senhas e decida se acha que é uma opção forte ou fraca. Faça isso da maneira certa e você vai melhorar as configurações de privacidade. Selecione Iniciar para começar.
- Opções:
  - Am@z0nPa55 (Forte)
  - April012000 (Fraca)
  - 1q2w3e4r (Fraca)
  - Password123 (Fraca)
  - !Lik 3MySch001 (Forte)
  - J0n@than#81 (Forte)
  - Iloveyou (Fraca)

<a name="item03.02"><h4>3.2 Manutenção de dados</h4></a>[Back to summary](#item03)

🔐 Criptografia e Salvaguarda de Dados Pessoais   
A criptografia é o mecanismo técnico essencial para garantir que informações sensíveis não sejam acessadas por indivíduos não autorizados. O processo consiste em transformar dados legíveis em um formato codificado, que só pode ser revertido à sua forma original por meio de uma chave secreta ou senha específica. Nota-se que a criptografia atua na proteção do conteúdo, mas não impede a interceptação do arquivo ou ataques de ransomware, nos quais criminosos utilizam a própria criptografia para bloquear o acesso do proprietário aos dados em troca de resgate.

📁 Implementação de Criptografia em Sistemas Operacionais   
Sistemas como o Windows oferecem ferramentas nativas para a proteção de arquivos e diretórios, como o EFS (Encrypting File System). Este recurso vincula a proteção diretamente à conta do usuário, restringindo o acesso apenas ao titular da credencial.
- Processo de Ativação: O usuário deve selecionar os itens desejados, acessar as 'Propriedades' via clique direito, entrar no menu 'Avançado' e habilitar a opção de criptografia de conteúdo. No Windows, arquivos protegidos por este método são visualmente identificados pela cor verde.

💾 Estratégias de Backup e Continuidade   
A realização de cópias de segurança é a única garantia contra a perda definitiva de informações em casos de furto, perda de hardware ou falhas técnicas. O backup exige a replicação periódica dos dados para um local de armazenamento distinto do original.
- Rede e Armazenamento Local: Oferece controle total sobre o hardware e os dados. Pode envolver o uso de dispositivos NAS (Network Attached Storage), discos rígidos externos, fitas ou mídias removíveis. A manutenção e os custos operacionais são de responsabilidade integral do proprietário.
- Armazenamento em Nuvem: Serviços como AWS permitem a custódia dos dados em servidores remotos. A principal vantagem é a resiliência contra incidentes físicos locais, como incêndios ou roubos. O acesso é condicionado à conexão de rede e às credenciais da conta, com custos proporcionais ao volume armazenado.

🗑️ Eliminação Segura de Informações   
A simples exclusão de um arquivo não garante sua remoção permanente, permitindo que especialistas ou criminosos recuperem os dados do disco. Para assegurar a irrecuperabilidade, os dados devem ser sobrescritos múltiplas vezes por padrões binários.
- Ferramentas de Exclusão Lógica: Softwares como SDelete (Windows), Shred (Linux) ou Secure Empty Trash (macOS) executam a sobrescrita necessária para apagar rastros digitais.
- Destruição Física: É o único método que oferece garantia absoluta de que os dados não serão recuperados. Discos rígidos e dispositivos de armazenamento devem ser inutilizados fisicamente antes do descarte.
- Dados em Nuvem: É necessário garantir que cópias armazenadas em servidores de terceiros também sejam excluídas ao encerrar serviços ou remover arquivos confidenciais.

<a name="item03.02.01"><h4>3.2.1 Eles realmente desapareceram?</h4></a>[Back to summary](#item03)

Você fez login no seu laptop, mas ele contém algumas fotos do usuário anterior, que não trabalha mais na @Apollo. Seu gerente pede que você as exclua. Você arrasta as fotos para a lixeira, abre a lixeira, seleciona-as e clica em “Excluir” novamente. Isso deve funcionar! Você acha que as fotos realmente sumiram do laptop? Selecione a resposta correta e clique em Enviar.
- Opções:
  - Sim, as fotos não podem mais ser recuperadas (F)
  - Não, as fotos estão apenas inacessíveis no sistema operacional (V)

<a name="item03.03"><h4>3.3 Quem é o dono dos seus dados?</h4></a>[Back to summary](#item03)

📋 Análise de Termos de Serviço e Privacidade Online   
A adesão a qualquer serviço digital pressupõe a aceitação de um contrato que define as regras de interação entre o usuário e o provedor. Compreender esses documentos é vital para garantir que a custódia das informações pessoais seja tratada com a transparência e segurança necessárias.

🔍 Componentes Fundamentais dos Acordos Digitais   
- Política de Uso de Dados: Detalha os métodos de coleta, a finalidade do processamento e as condições sob as quais o provedor pode compartilhar as informações do usuário com terceiros ou parceiros comerciais.
- Configurações de Privacidade: Define as ferramentas disponíveis para que o titular da conta gerencie a visibilidade do seu perfil e restrinja quem possui autorização para acessar seus dados de interação.
- Política de Segurança: Apresenta as medidas técnicas e administrativas adotadas pela organização para salvaguardar os ativos digitais contra acessos não autorizados e violações.

🤔 Fatores Críticos para Avaliação de Serviços   
Antes de realizar o cadastro em uma plataforma, nota-se que o usuário deve considerar questões estratégicas sobre a soberania de seus dados:
- Direitos de Propriedade: É necessário verificar se o provedor reivindica direitos sobre o conteúdo enviado (upload) pelo usuário.
- Portabilidade: Deve-se confirmar se existe a possibilidade de solicitar e baixar uma cópia integral dos dados armazenados.
- Ciclo de Vida da Informação: É fundamental entender qual é o destino das informações após o encerramento da conta e se a exclusão dos servidores é definitiva.

A leitura atenta dessas cláusulas constitui uma camada de proteção preventiva, assegurando que o usuário mantenha o controle sobre sua pegada digital.

<a name="item03.03.01"><h4>3.3.1 Termos de serviço</h4></a>[Back to summary](#item03)

Você foi solicitado a configurar uma conta de armazenamento e compartilhamento de fotos on-line para ser usada para colaboração criativa com o departamento de design e outras equipes da @Apollo. Ao se inscrever, você será solicitado a assinar um contrato de serviço com o provedor. Você não pensa muito sobre isso e concorda com todos os termos sem lê-los. Você acabou de assinar um contrato de Termos de Serviço. Mas você sabe o que é isso? Considere as opções a seguir e escolha a que você achar melhor descreve um contrato de termos de serviço. Selecione a resposta correta e clique em Enviar.
- Opções:
  - Um contrato descrevendo os serviços que você espera receber do provedor e como você usará o serviço. (F)
  - Uma organização informal que define as regras do relacionamento entre você, o provedor de serviços e outras pessoas que usam o serviço. (F)
  - Um contrato que vincula legalmente as regras de relacionamento entre você, o provedor de serviços e outras pessoas que usam o serviço. (V)

<a name="item03.03.02"><h4>3.3.2 O que você está concordando? | Qual é a Política de Uso de Dados?</h4></a>[Back to summary](#item03)

Você criou a conta @Apollo e concordou com os Termos de Serviço da empresa de compartilhamento de fotos on-line. Mas você realmente sabe pelo que se inscreveu? Vamos analisar detalhadamente.

A política de uso de dados da empresa que você usou para configurar a conta afirma que, para qualquer conteúdo que você publique: “você nos concede uma licença não exclusiva, transferível, sublicenciável, isenta de direitos autorais e mundial para hospedar, usar, distribuir , modificar, executar, copiar, executar ou exibir publicamente, traduzir e criar trabalhos derivados do seu conteúdo (compatível com as configurações de privacidade e do aplicativo)”. O que essa declaração realmente significa? Selecione a resposta correta e clique em Enviar.
- Opções:
  - Você não é mais o proprietário do conteúdo, e a empresa de compartilhamento de fotos pode reutilizá-lo, mas apenas em circunstâncias específicas. (F)
  - Você é o proprietário do conteúdo, mas a empresa de compartilhamento de fotos pode reutilizá-lo para qualquer finalidade. (V)
  - Você é o proprietário do conteúdo e a empresa de compartilhamento de fotos precisa obter permissão para reutilizar o conteúdo. (F)

<a name="item03.03.03"><h4>3.3.3 Configurações de privacidade</h4></a>[Back to summary](#item03)

Como você não definiu as configurações de privacidade antes de aceitar os termos, as configurações padrão foram aplicadas. Qual das seguintes opções você acha que é mais provável? Selecione a resposta correta e clique em Enviar.
- Opções:
  - Ninguém poderá ver informações sobre você e acessar seu perfil até que você altere as preferências nas configurações de privacidade. (F)
  - Qualquer pessoa poderá ver informações sobre você e acessar seu perfil até que você altere as configurações de privacidade. (V)

<a name="item03.03.04"><h4>3.3.4 Proteja seus dados</h4></a>[Back to summary](#item03)

Você sempre deve tomar as medidas adequadas para proteger seus dados e proteger sua conta. Voltando aos exemplos dos Termos de serviço descritos acima, o que você pode fazer para se proteger ao entrar em um contrato com um provedor de serviços on-line? O que você pode fazer para proteger sua conta e seus dados? Escreva sua opinião na caixa abaixo e depois envie. Selecione Mostrar resposta para verificar sua resposta.
- Para se proteger ao entrar em um contrato com um provedor de serviços on-line, é importante ler os termos de serviço e a política de privacidade para entender como seus dados serão coletados, usados e protegidos. Além disso, deve-se utilizar senhas fortes, habilitar autenticação de dois fatores, evitar compartilhar credenciais com outras pessoas e manter as configurações de segurança e privacidade da conta sempre atualizadas para reduzir riscos de acesso não autorizado.

<a name="item03.04"><h4>3.4 Como proteger a privacidade on-line</h4></a>[Back to summary](#item03)

🛡️ Mecanismos de Autenticação e Navegação Segura   
A proteção de contas digitais evoluiu para um modelo de camadas, onde a simples combinação de nome de usuário e senha é considerada insuficiente. Grandes provedores de serviços adotam protocolos que exigem múltiplas provas de identidade para autorizar o acesso.

🔐 Autenticação de Dois Fatores (2FA)   
A autenticação de dois fatores adiciona uma barreira extra ao exigir, além do conhecimento da senha (PIN), um segundo elemento de verificação. Este token pode assumir diversas formas:
- Posse Física: Uso de dispositivos como telefones celulares, cartões inteligentes ou chaves de segurança (fobs).
- Biometria: Validação por meio de características biológicas únicas, como reconhecimento facial, impressões digitais ou padrões de voz.
- Tokens Temporários: Códigos numéricos enviados instantaneamente via e-mail ou mensagens SMS.

Nota-se que, embora o 2FA eleve significativamente o nível de segurança, ele não torna a conta imune. Técnicas de engenharia social, malwares específicos e campanhas de phishing ainda podem ser empregadas para interceptar esses códigos ou enganar o usuário.

🌐 Protocolos de Autorização Aberta (OAuth)   
O OAuth é um padrão técnico que permite ao usuário acessar aplicações de terceiros utilizando credenciais de contas já existentes (como Google ou Facebook). Este método oferece conveniência ao eliminar a necessidade de criar novas senhas para cada serviço e, fundamentalmente, aumenta a segurança ao não compartilhar a senha original com o novo aplicativo. O portal de destino recebe apenas um token de autorização, preservando a integridade das credenciais primárias.

🕵️ Privacidade e Navegação Privada   
A navegação convencional deixa rastros digitais que podem ser acessados por qualquer pessoa com acesso físico ao dispositivo ou roteador. Além disso, e-mails enviados sem proteção podem ser lidos em qualquer ponto da cadeia de transmissão digital.

O modo de navegação privada (conhecido como Incógnito ou InPrivate, dependendo do navegador) atua da seguinte forma:
- Gestão de Cookies: Desabilita o armazenamento de pequenos arquivos que identificam os sites visitados.
- Limpeza Automática: Remove arquivos temporários e apaga o histórico de navegação assim que a sessão é encerrada.
-Rastreamento e Publicidade: Dificulta a coleta de dados por empresas que buscam criar perfis de consumo para anúncios direcionados.

É necessário observar que a navegação privada não garante anonimato absoluto. Provedores de internet, administradores de rede e dispositivos intermediários (como roteadores) ainda podem registrar o tráfego. Além disso, técnicas modernas de "impressão digital do dispositivo" (fingerprinting) permitem o rastreamento comportamental mesmo sem o uso de cookies. A segurança digital é uma responsabilidade individual que exige a aplicação constante de diretrizes preventivas para salvaguardar a identidade e os ativos computacionais.

<a name="item03.04.01"><h4>3.4.1 Compartilhamento social</h4></a>[Back to summary](#item03)

Você decide atualizar seu novo cargo nas redes sociais. Ao fazer isso, um dos sites solicita que você atualize suas informações de perfil para garantir que você receba o conteúdo que realmente não quer perder! Dê uma olhada nos campos ausentes. Quais você deve preencher? Lembre-se, responder corretamente melhorará suas configurações de privacidade, então pense cuidadosamente nas informações que deseja compartilhar online. Selecione as duas respostas corretas e, em seguida, Enviar.
- Opções:
  - Data de nascimento. (F)
  - Sua foto de perfil. (V)
  - Endereço de e-mail. (F)
  - O nome e as informações de contato do seu gerente. (F)
  - Telefone celular. (F)
  - Nome da organização. (V)
  - Nomes e informações de contato de seus colegas. (F)

<a name="item03.05"><h4>3.5 Descobrir seu próprio comportamento on-line arriscado</h4></a>[Back to summary](#item03)

<a name="item03.05.01"><h4>3.5.1 Cenário 1</h4></a>[Back to summary](#item03)

Você sabe quais informações são seguras para compartilhar nas mídias sociais? É surpreendente o que as pessoas publicam nas mídias sociais sem pensar! Quais das seguintes opções você acha que representa um risco se publicado em mídias sociais? Selecione as três respostas corretas e clique em Enviar.
- Opções:
  - RI com os amigos. (F)
  - Ainda pagando meu novo par de sapatos LOL! (V)
  - Adeus, 23 Brookbank Street. Olá, las vegas! Vacation time pelas três semanas! (V)
  - Amando meu novo protetor de tela. Benson é o melhor cachorro de todos os tempos! (F)
  - Mal posso esperar para usar meus novos diamantes. O restaurante Fontana em Bridgetown na Quinta à noite. #worth$$$ (V)

<a name="item03.05.02"><h4>3.5.2 Cenário 2</h4></a>[Back to summary](#item03)

Ao criar uma nova conta em um serviço online, qual senha você usa? É segura? Com suas próprias palavras, descreva o que é um aplicativo gerenciador de senhas, como funciona e por que é benéfico. Se você já usou um gerenciador de senhas, descreva alguns detalhes e compartilhe sua experiência. Escreva sua opinião na caixa e depois envie. Selecione Mostrar resposta para verificar sua resposta.
- Ao criar uma nova conta em um serviço online, é importante utilizar uma senha forte e única, combinando letras maiúsculas e minúsculas, números e caracteres especiais. Um gerenciador de senhas é um aplicativo que armazena e organiza todas as suas senhas de forma segura em um cofre digital protegido por uma senha principal. Ele funciona criptografando as informações e preenchendo automaticamente as credenciais quando necessário, o que facilita o uso de senhas diferentes para cada serviço. Isso é benéfico porque aumenta a segurança das contas, reduz o risco de reutilização de senhas e torna mais fácil gerenciar várias credenciais.

<a name="item03.05.03"><h4>3.5.3 Cenário 3</h4></a>[Back to summary](#item03)

A conexão a um hotspot de Wi-Fi aberto pode tornar seu sistema e dados vulneráveis a um ataque. A gerente de vendas da @Apollo está viajando para encontrar um cliente. Ela se esqueceu de baixar o contrato do servidor de @Apollo para trazer para a reunião com ela. O trem tem uma rede Wi-Fi aberta. Ela entra em contato com você para perguntar o que deve fazer. O que você recomendaria?
- Opções:
  - Ela deve acessar a rede Wi-Fi aberta do trem e se conectar aos servidores @Apollo usando a conexão VPN em seu laptop de trabalho. (V)
  - Ela deve esperar até chegar ao escritório do cliente e solicitar o código de acesso à rede Wi-Fi e acessar o serviço @Apollo diretamente no laptop de trabalho. (F)
  - Ela deve usar a conexão 4G no telefone para encontrar uma rede Wi-Fi aberta alternativa. (F)
  - Ela deve esquecer o contrato da reunião e acompanhar outros trabalhos on-line usando o Wi-Fi aberto do trem para acessar os sites https de que ela precisa. (F)

<a name="item03.05.04"><h4>3.5.4 Cenário 4</h4></a>[Back to summary](#item03)

Você está ciente dos riscos que surgem ao baixar uma versão de avaliação de um programa? Um designer da @Apollo precisa instalar um software de manipulação de imagem. O aplicativo tradicional é muito caro e só é necessário para uma pequena parte de um projeto único. O gerente de design diz que isso não seria uma compra econômica e, em vez disso, instala um aplicativo gratuito alternativo - o gerente não se importa se for de uma fonte não confiável, pois acredita que os riscos são baixos. O projetista deve seguir o conselho do gerente? Selecione a resposta correta e clique em Enviar.
- Opções:
  - Obviamente, o gerenciador recebeu instruções do gerente, então não há problema em instalar o aplicativo gratuito. Isso vai economizar dinheiro para a empresa! (F)
  - Não, o designer deve verificar com um membro da equipe de TI antes de instalar qualquer aplicação de uma fonte não confiável. (V)
  - Sim, o gerente de design considera que o risco é baixo, então isso deve ser certo! (F)
  - Não, o designer deve comprar o aplicativo confiável do principal provedor de software e pagar por isso usando seu próprio dinheiro. (F)

<a name="item03.05.05"><h4>3.5.5 Cenário 5</h4></a>[Back to summary](#item03)

Você já recebeu uma mensagem de aviso para baixar um programa de diagnóstico que protegerá seu computador? Você deve estar ciente dos riscos. Esta mensagem aparece enquanto você está online. Quais das seguintes ações você deve tomar? Selecione a resposta correta em cada lista suspensa e clique em Enviar.
- Opções:
  - Feche o pop-up ou o navegador -> Clicar em "X".
  - Proteja seu sistema, que ainda não foi corrompido -> Executando uma verificação do sistema com seu software antivírus confiável.
  - Verifique se uma atualização de aplicativo legítima de uma fonte confiável é necessária -> Verificando se você tem o aplicativo SOCIALACCESSNOW e, em caso afirmativo, acesse o site oficial.

<a name="item03.05.06"><h4>3.5.6 Cenário 6</h4></a>[Back to summary](#item03)

Clicar em links em um e-mail pode parecer seguro, mas muitas vezes nem tudo é o que parece. Você deve conhecer os sinais que devem ser observados! A @Apollo viu um aumento no número de e-mails de phishing sendo recebidos por sua equipe. Eles decidem implementar um exercício de treinamento rápido para ajudar os funcionários a identificar os sinais de um e-mail inseguro. Vá em frente! Ao clicar em Iniciar, você verá algumas seções diferentes de e-mails que afirmam ser de @Apollo. Para cada uma delas, clique em “SEGURO” se achar que isso indica que o e-mail é seguro ou clique em “NÃO SEGURO” se achar que isso indica que o e-mail é suspeito.
- Opções:
  - Subject: Instalação urgente /*& isso agora do seu serviço de TI -> Não Seguro.
  - Clique para baixar o conteúdo deste e-mail -> Não Seguro.
  - Este e-mail foi enviado de dentro da sua organização. -> Seguro.
  - Este e-mail foi enviado de fora da sua organização. Clique para enviar para sau pasta de lixo eletrônico. -> Não Seguro.
  - john@ap0ll0-admin.org -> Não Seguro.
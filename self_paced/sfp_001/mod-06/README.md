# Gerenciamento de Ameaças Cibernéticas - Módulo 6   <img src="../0-aux/logo_course.png" alt="curso_150" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="../">curso_150 (Gerenciamento de Ameaças Cibernéticas)   <img src="../0-aux/logo_course.png" alt="curso_150" width="auto" height="25"></a>
### Module: 6. Análise Forense Digital e Análise e Resposta a Incidentes

---

### Theme:
- Cybersecurity

### Used Tools:
- Operating System (OS): 
  - Windows 11 <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/windows11.png" alt="windows11" width="auto" height="25">
- Cloud:
  - Amazon Web Services (AWS)   <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="aws" width="auto" height="25">
- Cloud Services:
  - Amazon Elastic Compute Cloud (EC2)   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/cloud/aws_ec2.svg" alt="aws_ec2" width="auto" height="25">
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

### Course Module 6 Structure:
6. <a name="item06">Análise Forense Digital e Análise e Resposta a Incidentes</a><br>
  6.1 <a href="#item06.01">Introdução</a><br>
  6.2 <a href="#item06.02">Manuseio de evidências e atribuição de ataque</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;6.2.1 <a href="#item06.02.01">Laboratório - Coletar informações do sistema depois de um incidente</a><br>
  6.3 <a href="#item06.03">O Cyber Kill Chain</a><br>
  6.4 <a href="#item06.04">O modelo Diamond de análise de intrusão</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;6.4.1 <a href="#item06.04.01">Laboratório - Análise de ataque</a><br>
  6.5 <a href="#item06.05">Resposta a incidentes</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;6.5.1 <a href="#item06.05.01">Laboratório - Tratamento de Incidentes</a><br>
  6.6 <a href="#item06.06">Recuperação de desastres</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;6.6.1 <a href="#item06.06.01">Packet Tracer - Investigar la Recuperación ante un Desastre</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;6.6.2 <a href="#item06.06.02">Laboratório - Recomende Medidas de Recuperação de Desastres</a><br>
  6.7 <a href="#item06.07">Análise forense digital e análise de incidentes e resumo de resposta</a><br>

---

### Objective:
O objetivo deste módulo foi apresentar os principais fundamentos da resposta a incidentes e da recuperação de desastres em segurança cibernética, destacando a importância de identificar e analisar rapidamente eventos que possam comprometer sistemas e dados. Foram exploradas práticas de forense digital para coletar, preservar e examinar evidências, além de estratégias para detectar, conter e erradicar ameaças, garantindo a restauração segura das operações. O módulo abordou também a aplicação de frameworks e modelos, como NIST 800-61r2, Cyber Kill Chain e Modelo Diamond, para estruturar a resposta de forma organizada e eficaz. Por fim, foram discutidos planos de continuidade e recuperação de desastres, enfatizando a avaliação de riscos, a priorização de processos críticos e a validação de procedimentos que assegurem a integridade de sistemas e dados mesmo diante de incidentes complexos.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item06.01"><h4>6.1 Introdução</h4></a>[Back to summary](#item06)

Este módulo aborda o que deve ser feito quando um ataque realmente acontece. Até aqui foram estudados vetores de ataque, ferramentas e práticas de proteção. Agora, o foco passa a ser a resposta a incidentes e o uso de técnicas forenses para investigar e mitigar impactos.  

🧾 Tratamento de Evidências e Atribuição de Ataques   
O processo de forense digital desempenha um papel essencial na coleta, preservação e análise de evidências. Ele permite reconstruir a sequência dos eventos, identificar a origem do ataque e associar a atividade maliciosa a possíveis responsáveis, sempre seguindo práticas que garantam a integridade dos dados.  

🕵️ The Cyber Kill Chain   
O modelo Cyber Kill Chain descreve as etapas de um ataque cibernético, permitindo identificar em qual fase a intrusão pode ser interrompida. Ele ajuda a mapear o comportamento do adversário desde o reconhecimento inicial até a execução e o impacto final.  

💎 Modelo Diamond de Análise de Intrusão   
O Diamond Model fornece uma estrutura para analisar eventos de intrusão considerando quatro componentes principais: adversário, infraestrutura, capacidade e vítima. Essa abordagem permite classificar incidentes de forma mais clara e identificar relações entre diferentes ataques.  

🚨 Resposta a Incidentes   
O framework NIST 800-61r2 define diretrizes para lidar com incidentes de segurança. Ele abrange preparação, detecção, análise, contenção, erradicação, recuperação e aprendizado pós-incidente. Aplicar esses procedimentos garante uma resposta estruturada e eficaz.  

🛠️ Recuperação de Desastres   
Quando ocorrem falhas críticas ou interrupções, a recuperação de desastres torna-se vital. Procedimentos de backup e restauração de arquivos, assim como a retomada das operações de rede, asseguram a continuidade dos serviços e a minimização de perdas.  

<a name="item06.02"><h4>6.2 Manuseio de evidências e atribuição de ataque</h4></a>[Back to summary](#item06)

🔍 Tratamento de Evidências Digitais   
A perícia digital trata da recuperação, preservação e exame de dados em dispositivos e redes. O objetivo é documentar o incidente e, quando necessário, apoiar ações legais. É essencial preservar arquivos, memória volátil, pacotes de rede e logs para análise. Sempre deve-se trabalhar em cópias (imagens bit-a-bit) e manter a integridade dos metadados.

⚖️ Procedimentos Formais e Legais   
Investigações podem ser internas (envolvendo colaboradores) ou externas (envolvendo invasores). Em casos legais, a organização pode ter de envolver autoridades, e a investigação torna-se pública. Manipular ou destruir evidências pode gerar responsabilidade criminal, por isso é indispensável manter procedimentos documentados e formais.

🗂️ Fases da Forense Digital   
- **Coleta:** identificar fontes de dados e armazenar evidências sem alteração.  
- **Exame:** extrair e filtrar informações relevantes.  
- **Análise:** correlacionar pessoas, eventos e fontes para tirar conclusões.  
- **Relatório:** documentar resultados de forma imparcial, indicando limitações e próximos passos.  

⛓️ Cadeia de Custódia   
É fundamental registrar quem coletou e manuseou cada evidência, em que momento e por qual motivo. Isso garante validade legal e integridade do processo investigativo.

📶 Ordem de Volatilidade (RFC 3227)   
A coleta deve seguir a ordem da volatilidade dos dados:  
1. Memória e caches.  
2. Estados do kernel, tabelas de roteamento/ARP.  
3. Fluxos e sistemas temporários.  
4. Discos fixos e mídias removíveis.  
5. Logs remotos.  
6. Backups e arquivos em arquivamento.  

🕵️‍♂️ Atribuição de Ataques   
O processo de atribuição busca identificar os responsáveis, mas deve ser feito com cautela. Evidências forenses raramente são diretas, sendo necessário correlacionar táticas, técnicas e procedimentos (TTPs) com explorações conhecidas. É importante evitar viés e especulações durante a investigação.

🔗 Inteligência e Modelos de Apoio   
- **Indicadores:** localização de hosts/domínios, artefatos de código, ferramentas utilizadas e padrões comportamentais.  
- **Logs de rede e infraestrutura:** ajudam a rastrear dispositivos e usuários internos.  
- **MITRE ATT&CK:** cataloga TTPs e auxilia a relacionar incidentes com grupos e atores conhecidos, fortalecendo a detecção e resposta.  

<a name="item06.02.01"><h4>6.2.1 Laboratório - Coletar informações do sistema depois de um incidente</h4></a>[Back to summary](#item06)

Este laboratório foi desenvolvido em quatro partes, cada uma composta por várias etapas. Algumas etapas foram documentadas diretamente neste arquivo README, enquanto outras exigiram a criação de arquivos específicos. O objetivo do laboratório foi analisar vulnerabilidades identificadas em uma empresa fictícia, classificá-las por ordem de criticidade, desenvolver uma política de segurança da informação para a vulnerabilidade mais crítica, criar um procedimento detalhado para sua implementação e, por fim, elaborar um plano para disseminar e avaliar as políticas de segurança da empresa. Além disso, foi realizado uma análise conceitual dos documentos de segurança da informação para melhor compreensão e entendimento.

##### Parte 1: Revisão do cenário




<a name="item06.03"><h4>6.3 O Cyber Kill Chain</h4></a>[Back to summary](#item06)

💥 O Modelo Cyber Kill Chain   
A Cyber Kill Chain, criada pela Lockheed Martin, descreve as etapas que um invasor percorre desde o reconhecimento até alcançar o objetivo final. Entender cada fase ajuda a detectar e interromper o ataque o mais cedo possível — quanto mais cedo, menos dano e menos aprendizado por parte do atacante.

🔎 Reconhecimento   
É a pesquisa do alvo: coleta de emails, perfis em redes sociais, servidores públicos, endereços IP e portas abertas. O invasor decide se vale a pena atacar e quais vetores usar.  
- Táticas: varreduras, coleta pública de informações, mineração de perfis sociais.  
- Defesas: monitorar sinais de reconhecimento (logs web, scouting), criar detectores de comportamento e priorizar proteção de alvos prováveis.

🛠️ Armamento   
O atacante combina exploits, backdoors e cargas para formar a “arma” que será entregue ao alvo. Pode usar malware pronto ou criar variantes para evitar detecção.  
- Táticas: empacotar payloads, criar documentos maliciosos, configurar infraestrutura C2.  
- Defesas: análise e sandboxing de amostras, regras IDS/IPS atualizadas, coleta de artefatos de armamento.

📤 Entrega   
É o envio da carga ao alvo (anexo de email, drive USB, site comprometido). Se a entrega falhar, o ataque não progride.  
- Táticas: phishing, malvertising, mídias removíveis, exploits contra serviços web.  
- Defesas: filtragem de e-mail e web, bloqueio por reputação, captura de evidências de entrega (emails, pcaps).

⚠️ Exploração   
A arma é executada para explorar a vulnerabilidade — pode ser execução remota, abuso de usuário (abrir anexo) ou falha de software.  
- Táticas: exploits contra aplicações/SO ou engenharia social.  
- Defesas: hardening, testes de vulnerabilidade, treinamentos de phishing, detecção de comportamentos de exploit.

🔗 Instalação   
O atacante estabelece persistência no sistema (webshells, serviços, chaves de AutoRun) para manter acesso após reinicializações.  
- Táticas: criar backdoors persistentes, modificar timestamps, instalar serviços.  
- Defesas: auditoria de endpoints, HIPS/HIDS, monitoramento de criação de serviços e arquivos suspeitos.

📡 Comando e Controle (C2)   
O malware estabelece um canal para receber comandos e exfiltrar dados — via HTTP, DNS, IRC etc. Detectar C2 é crítico para encontrar hosts comprometidos.  
- Táticas: comunicação bidirecional com infraestrutura C2 (domínios, DNS dinâmico, proxies).  
- Defesas: análise de tráfego, bloqueio de domínios suspeitos, sinkholing, análise estática/dinâmica de malware.

🎯 Ações sobre Objetivos   
Fase final: exfiltração de dados, escalonamento de privilégios, movimento lateral, destruição ou uso do ambiente (spam, mineração). Aqui o atacante alcança seus objetivos e fica muito mais difícil removê-lo.  
- Táticas: coleta de credenciais, lateral movement, encriptação/exfiltração de dados.  
- Defesas: detecção forense (endpoints, pcaps), resposta imediata a alertas, contenção segmentada e análise de danos.

<a name="item06.04"><h4>6.4 O modelo Diamond de análise de intrusão</h4></a>[Back to summary](#item06)

💎 Modelo Diamond de Análise de Intrusão   
O Modelo Diamond representa um evento de intrusão como uma relação entre quatro elementos principais: adversário, capacidade, infraestrutura e vítima. Ele ajuda a visualizar quem atacou, com que ferramenta, por qual caminho e contra quem — facilitando a correlação de eventos e a construção de cadeias de ataque.

🔷 Componentes do Modelo Diamond   
- **Adversário:** a entidade (pessoa, grupo ou Estado) responsável pela ação maliciosa.  
- **Capacidade:** a ferramenta, exploit ou técnica que o adversário usa para executar o ataque (por exemplo, malware ou script).  
- **Infraestrutura:** os recursos de rede e sistemas usados para suportar o ataque — servidores C2, domínios, proxies, etc.  
- **Vítima:** o alvo do evento; pode ser um usuário, host ou serviço (e uma vítima também pode virar infraestrutura para ataques futuros).

🧭 Meta-recursos (extensões úteis)   
O modelo incorpora elementos adicionais que enriquecem a análise:
- **Timestamp:** início e fim do evento — essencial para agrupar atividades.  
- **Fase:** qual estágio da cadeia de ataque (ex.: reconhecimento, entrega, exploração).  
- **Resultado:** impacto alcançado (confidencialidade, integridade, disponibilidade).  
- **Direção:** como o fluxo do evento percorre o modelo (ex.: infraestrutura → vítima).  
- **Metodologia:** classificação do tipo de ataque (phishing, portscan, DDoS, etc.).  
- **Recursos:** ativos externos usados pelo adversário (código, know-how, financiamento, hardware).

🧩 Uso prático e encadeamento de eventos   
O Diamond é ideal para mapear como eventos individuais se conectam: um adversário usa uma capacidade através de uma infraestrutura para comprometer uma vítima; em seguida pode pivotar e reutilizar essa vítima como infraestrutura para novos ataques. Diagramar cada evento facilita identificar padrões, TTPs e relações entre incidentes aparentemente separados.

🔁 Exemplo simplificado (fluxo de ataque encadeado)   
1. Adversário pesquisa a organização alvo e identifica domínios e funcionários.  
2. Envia spear-phishing para administradores usando um anexo malicioso.  
3. Um administrador abre o anexo → exploração bem-sucedida; host comprometido.  
4. Malware no host registra-se num servidor C2 (infraestrutura) e recebe comandos.  
5. O host comprometido passa a atuar como proxy, permitindo ao adversário alcançar novas vítimas via contatos do administrador.  
6. Segundo alvo é spear-phishado usando a infraestrutura já comprometida — novo compromisso e possível exfiltração.

Esse encadeamento mostra como eventos Diamond separados (cada compromisso) se ligam verticalmente pela Kill Chain e horizontalmente ao reutilizar infraestrutura/vítimas. Diagramar cada nó e suas conexões ajuda a traçar o ataque, priorizar contenção e suportar atribuição.

<a name="item06.04.01"><h4>6.4.1 Laboratório - Análise de ataque</h4></a>[Back to summary](#item06)

Este laboratório foi desenvolvido em quatro partes, cada uma composta por várias etapas. Algumas etapas foram documentadas diretamente neste arquivo README, enquanto outras exigiram a criação de arquivos específicos. O objetivo do laboratório foi analisar vulnerabilidades identificadas em uma empresa fictícia, classificá-las por ordem de criticidade, desenvolver uma política de segurança da informação para a vulnerabilidade mais crítica, criar um procedimento detalhado para sua implementação e, por fim, elaborar um plano para disseminar e avaliar as políticas de segurança da empresa. Além disso, foi realizado uma análise conceitual dos documentos de segurança da informação para melhor compreensão e entendimento.

##### Parte 1: Revisão do cenário


<a name="item06.05"><h4>6.5 Resposta a incidentes</h4></a>[Back to summary](#item06)

🧭 O que é resposta a incidentes   
Resposta a incidentes são métodos, políticas e procedimentos usados para detectar, conter, analisar e recuperar de ataques cibernéticos. O objetivo é limitar o impacto, avaliar danos e restaurar operações, por isso é crítico manter planos detalhados e equipes responsáveis pela execução.

📚 NIST 800-61r2   
O NIST SP 800-61r2 é a referência para tratamento de incidentes: define preparação, detecção, análise, contenção, erradicação, recuperação e lições aprendidas. Seguir essas diretrizes ajuda a padronizar ações independentemente de plataformas ou tecnologias.

🏢 Estabelecendo um CSIRC (Capacidade de Resposta)   
O primeiro passo é criar políticas, planos e procedimentos formais para um CSIRC/CSIRT. A política de resposta deve refletir missão, escopo e autoridade da organização e ser revisada periodicamente.

⚙️ Elementos da política de resposta a incidentes   
Uma política eficaz inclui: declaração de compromisso da gestão; objetivos; escopo; definição de incidentes; estrutura organizacional (papéis e autoridades); priorização por gravidade; métricas de desempenho; e formulários/contatos de comunicação.

📋 Plano de resposta a incidentes   
O plano operacionaliza a política: define missão, estratégias e objetivos, aprovação executiva, comunicação interna/externa, métricas de capacidade e integração com a organização. Um bom plano minimiza confusão durante o estresse de um incidente.

🧰 Procedimentos (SOPs)   
Os procedimentos detalham passos técnicos, técnicas e checklists operacionais. SOPs claros e praticados reduzem erros e garantem que cada membro saiba suas ações e como colaborar.

🤝 Partes interessadas e colaboração interna   
Várias áreas devem cooperar com o CSIRT antes de um incidente:  
- **Gerência:** define políticas, orçamento e coordenação com stakeholders.  
- **Garantia de Informação:** pode alterar regras de firewall ou políticas durante contenção/recuperação.  
- **Suporte de TI:** executa ações técnicas, preserva evidências e mitiga falhas.  
- **Juridico:** revisa políticas, orienta sobre compliance e apoia ações legais.  
- **Assuntos Públicos / Mídia:** responsável por comunicações ao público quando necessário.  
- **Recursos Humanos:** trata de medidas disciplinares em incidentes internos.  
- **Planejamento de Continuidade:** ajusta planos de continuidade e avalia impacto organizacional.  
- **Segurança Física / Facilities:** apoia investigações que envolvem acesso físico e preservação de evidências.

🛡️ CMMC e resposta a incidentes (contexto DoD)   
O CMMC avalia maturidade de segurança para fornecedores do DoD. Inclui um domínio de resposta a incidentes com requisitos como: plano de resposta, detecção/relato, execução de respostas, revisões pós-incidente e testes. Os níveis refletem maturidade crescente:
- **Nível 2:** estabelecer plano conforme NIST; detectar, relatar e responder; analisar causas.  
- **Nível 3:** documentar e comunicar incidentes; testar capacidades de resposta.  
- **Nível 4:** usar TTPs conhecidos para aprimorar respostas; estabelecer SOC 24/7.  
- **Nível 5:** aplicar coleta forense sistemática e respostas manuais/automatizadas em tempo real seguindo padrões.

🌀 Ciclo de Vida da Resposta a Incidentes   
O NIST define quatro etapas principais no ciclo de vida da resposta a incidentes:  
- **Preparação**: o CSIRT é treinado, adquire ferramentas e mantém-se atualizado sobre novas ameaças.  
- **Detecção e Análise**: monitoramento contínuo para identificar, validar e compreender incidentes.  
- **Contenção, Erradicação e Recuperação**: execução de procedimentos para limitar os danos, eliminar o impacto e restaurar sistemas usando backups. Essa fase pode retornar à análise para ampliar o escopo da investigação.  
- **Atividades Pós-Incidente**: documentação do ocorrido, ajustes nos processos e medidas para evitar repetições.  

Esse ciclo funciona como um processo de aprendizado contínuo, em que cada incidente melhora a preparação para os próximos.

🧰 Preparação do CSIRT   
Na fase de preparação, são definidos processos, adquiridos recursos e treinada a equipe. Exemplos de ações:  
- Definição de canais de comunicação (contatos de stakeholders, aplicação da lei, rastreamento de incidentes, criptografia).  
- Criação de instalações para o SOC e espaços de resposta.  
- Aquisição de hardware e software de análise (ferramentas forenses, servidores, dispositivos de backup, sniffers, analisadores de protocolo).  
- Realização de avaliações de risco para implementar controles preventivos.  
- Validação de segurança em dispositivos de usuários, servidores e rede.  
- Desenvolvimento de materiais de conscientização em segurança.  

📂 Recursos de Apoio   
Recursos adicionais podem incluir:  
- Inventário de ativos críticos.  
- Diagramas de rede e lista de portas utilizadas.  
- Hashes de arquivos essenciais.  
- Leituras de linha de base de sistemas e redes.  
- Imagens limpas de sistemas operacionais e instaladores de aplicativos.  

🎒 Jump Kit   
Muitas equipes mantêm um **jump kit**, uma caixa portátil com recursos para resposta rápida. Pode conter:  
- Laptop configurado com softwares de análise.  
- Mídia de backup.  
- Hardware e software de recuperação.  
- Documentação essencial.  

O kit deve ser inspecionado e atualizado regularmente, além de praticado em exercícios para que todos saibam utilizá-lo corretamente.

🎯 Vetores de Ataque Mais Comuns   
Embora incidentes sejam variados, é importante focar nos tipos mais frequentes:  
- **Web**: ataques originados em sites ou aplicativos web.  
- **E-mail**: phishing ou anexos maliciosos.  
- **Perda ou Roubo**: dispositivos comprometidos que podem expor dados.  
- **Personificação**: uso de identidade falsa para ações maliciosas.  
- **Atrição**: ataques de força bruta contra redes ou serviços.  
- **Mídia Removível**: dispositivos externos usados como vetor de malware.  

🔍 Detecção de Incidentes   
A detecção é uma das fases mais desafiadoras no processo de resposta a incidentes, pois alguns incidentes são facilmente identificáveis, enquanto outros podem passar despercebidos por meses.  

Formas de detecção:   
- **Automatizadas:** softwares antivírus, sistemas de detecção de intrusão (IDS).  
- **Manuais:** relatórios de usuários ou equipes internas.  

Sinais de incidente:   
1. **Precursores** – indicam que um incidente pode ocorrer no futuro. Medidas preventivas podem ser aplicadas para evitar o ataque.  
   - Exemplo: logs mostrando resposta a varredura de portas ou vulnerabilidade recém-descoberta em um servidor web.  
2. **Indicadores** – sinalizam que um incidente já ocorreu ou está ocorrendo.  
   - Exemplo: host infectado com malware, múltiplos logins falhos de origem desconhecida, alerta de IDS.  

🧠 Análise de Incidentes   
A análise é complexa porque nem todos os indicadores são precisos. Alguns eventos podem ocorrer por razões não relacionadas à segurança, como falhas de hardware.  

Abordagens para análise:   
- Uso de algoritmos e aprendizado de máquina para validar incidentes, especialmente em grandes organizações com milhares ou milhões de eventos diários.  
- Criação de perfis de rede e sistemas, registrando padrões esperados de atividade para detectar alterações anômalas.  

Mesmo quando um indicador parece correto, é essencial investigar se houve um incidente legítimo, considerando causas alternativas, como falhas de hardware ou software.  

📊 Determinação do Escopo   
Quando um incidente é considerado real, o CSIRT realiza uma análise inicial para definir:  
- Sistemas, redes ou aplicativos afetados.  
- Origem do incidente.  
- Modo de ocorrência.  

Essa análise permite priorizar ações subsequentes, como contenção e investigação aprofundada dos efeitos do incidente.

📢 Notificação de Incidentes   
Após análise e priorização, as partes interessadas devem ser notificadas para execução de suas funções.  

Exemplos de partes notificadas:   
- CIO (Diretor executivo de informações)  
- Chefe de segurança da informação  
- Oficial de segurança da informação local  
- Outras equipes de resposta a incidentes internas  
- Equipes externas de resposta a incidentes (quando aplicável)  
- Proprietário do sistema  
- Recursos Humanos (para incidentes envolvendo funcionários, como assédio por e-mail)  
- Assuntos públicos (para incidentes que possam gerar publicidade)  
- Departamento jurídico (para incidentes com implicações legais)  
- US-CERT (para agências federais ou sistemas operados para o governo federal)  
- Aplicação da lei (quando necessário)  

🛑 Contenção, erradicação e recuperação   
Após a detecção e validação de um incidente de segurança, é essencial contê-lo para minimizar impactos. Estratégias e procedimentos de contenção devem estar definidos antes que qualquer dano significativo ocorra. A contenção ajuda a limitar a propagação do incidente e fornece tempo para ações corretivas mais detalhadas.

⚙️ Estratégia de contenção   
Cada incidente exige uma estratégia específica de contenção. Para defini-la, considere:  
- Quanto tempo levará para implementar a solução?  
- Quantos recursos serão necessários?  
- Como preservar as evidências do incidente?  
- É possível redirecionar o invasor para um ambiente controlado para análise segura?  
- Qual será o impacto sobre a disponibilidade dos serviços?  
- Qual a extensão dos danos aos ativos?  
- Quão eficaz é a estratégia?

📌 Danos adicionais durante a contenção   
Nem sempre é recomendável desconectar imediatamente o host comprometido da rede. Processos maliciosos podem perceber a desconexão e executar ações como apagamento de dados ou criptografia. A experiência da equipe é crucial para conter o incidente sem causar danos adicionais.

📝 Evidências   
Durante um incidente, é fundamental coletar e preservar evidências. Elas são importantes tanto para a resolução do incidente quanto para investigações legais futuras. A documentação deve ser clara e seguir regulamentos específicos. Após a coleta, as evidências devem ser registradas corretamente na cadeia de custódia. Elementos importantes a documentar incluem:  
- Local de recuperação e armazenamento de cada evidência.  
- Critérios de identificação (número de série, endereço MAC, hostname, IP, etc.).  
- Identificação das pessoas que manusearam ou coletaram as evidências.  
- Data e hora de cada etapa de coleta e manipulação.  

É essencial treinar todos os envolvidos para preservar as evidências corretamente.

🕵️ Identificação do invasor   
Embora secundária à contenção, erradicação e recuperação, identificar o invasor ajuda a minimizar impactos futuros. Algumas ações incluem:  
- Pesquisar atividades relacionadas em bancos de dados de incidentes (internos ou comunitários, como VERIS).  
- Validar o endereço IP do invasor para verificar se é viável ou se foi reatribuído.  
- Pesquisar na internet informações sobre ataques anteriores relacionados ao IP.  
- Monitorar canais de comunicação usados por invasores, como IRC, tratando informações obtidas como pistas e não fatos confirmados.

🚑 Erradicação, recuperação e remediação   
Após a contenção, identifique todos os hosts afetados e elimine todos os efeitos do incidente, incluindo malware e contas comprometidas. Corrija as vulnerabilidades exploradas para evitar reincidência. Para a recuperação:  
- Use backups limpos ou reinstale sistemas se não houver backups confiáveis.  
- Atualize e corrija sistemas operacionais e softwares.  
- Altere todas as senhas de hosts e sistemas críticos conforme a política de segurança.  
- Aproveite para validar e atualizar a segurança da rede, estratégias de backup e políticas de segurança.  

O foco deve ser corrigir rapidamente os sistemas e operações críticas, prevenindo novos ataques.

📖 Atividades pós-incidente   
Após a erradicação das ameaças e a recuperação dos sistemas, é importante reunir todas as partes envolvidas para analisar os eventos e as ações tomadas durante o incidente. Essa reunião proporciona aprendizado sobre o que foi feito corretamente, o que deu errado e o que pode ser melhorado.

📝 Reunião de lições aprendidas   
Depois de um incidente significativo, a organização deve conduzir uma reunião de “lições aprendidas” para avaliar a eficácia do processo de resposta a incidentes e identificar melhorias nos controles e práticas de segurança. Perguntas úteis para essa análise incluem:  
- O que aconteceu e quando?  
- Como a equipe e a gerência reagiram ao incidente?  
- Os procedimentos documentados foram seguidos e foram adequados?  
- Quais informações faltaram?  
- Houve ações que dificultaram a recuperação?  
- O que faria diferente em incidentes futuros?  
- Como melhorar o compartilhamento de informações com outras organizações?  
- Que medidas corretivas podem evitar incidentes semelhantes?  
- Quais precursores ou indicadores devem ser monitorados no futuro?  
- Que ferramentas ou recursos adicionais seriam úteis para detectar, analisar e mitigar incidentes futuros?

📊 Avaliação de dados do incidente   
Os dados coletados durante o incidente ajudam a determinar custos, medir a eficácia do CSIRT e identificar falhas de segurança. Apenas informações acionáveis devem ser registradas.  
- Um alto número de incidentes pode indicar falhas na metodologia ou incompetência da equipe.  
- Um número baixo pode mostrar melhoria na segurança ou falhas na detecção.  
- Dividir incidentes por tipo ajuda a identificar pontos fortes e fracos específicos.  
- O tempo de cada incidente e o tempo até a primeira resposta fornecem insights sobre recursos e eficiência do processo.

🔍 Avaliação objetiva do incidente   
Cada incidente deve ser analisado objetivamente para medir sua resolução e eficácia. Exemplos de atividades incluem:  
- Analisar logs, relatórios e documentação para verificar a adesão a políticas e procedimentos.  
- Identificar quais precursores e indicadores foram registrados.  
- Determinar se houve danos antes da detecção.  
- Identificar a causa, vetor de ataque, vulnerabilidades exploradas e sistemas afetados.  
- Verificar se o incidente é recorrente.  
- Estimar o dano monetário.  
- Comparar avaliação de impacto inicial e final.  
- Identificar medidas que poderiam ter prevenido o incidente.  
- Avaliação subjetiva: a equipe avalia seu desempenho e de outros membros, além do feedback de proprietários de recursos afetados.

📦 Retenção de evidências   
É necessário definir políticas para retenção de evidências de incidentes:  
- Processo: se houver ação legal, mantenha as evidências até o encerramento do processo.  
- Tipo de dados: e-mails ou textos podem ser retidos por 90 dias; dados críticos, por 3 anos ou mais.  
- Custo: armazenar mídia por longos períodos pode ser caro, especialmente com mudanças tecnológicas.  
A equipe jurídica deve consultar regulamentos governamentais para definir responsabilidades de relato e comunicação com partes interessadas, como clientes e parceiros.

🌐 Compartilhamento de informações   
Além das exigências legais, recomenda-se coordenar com outras organizações para compartilhar detalhes do incidente. Recomendações do NIST incluem:  
- Planejar a coordenação externa antes do incidente.  
- Consultar o departamento jurídico antes de compartilhar informações.  
- Compartilhar dados durante todo o ciclo de vida do incidente.  
- Automatizar o máximo possível o compartilhamento.  
- Equilibrar benefícios do compartilhamento com a proteção de informações confidenciais.  

O compartilhamento deve ser feito de forma segura e apropriada, visando aprendizado mútuo e prevenção de incidentes futuros.

<a name="item06.05.01"><h4>6.5.1 Laboratório - Tratamento de Incidentes</h4></a>[Back to summary](#item06)

Este laboratório foi desenvolvido em quatro partes, cada uma composta por várias etapas. Algumas etapas foram documentadas diretamente neste arquivo README, enquanto outras exigiram a criação de arquivos específicos. O objetivo do laboratório foi analisar vulnerabilidades identificadas em uma empresa fictícia, classificá-las por ordem de criticidade, desenvolver uma política de segurança da informação para a vulnerabilidade mais crítica, criar um procedimento detalhado para sua implementação e, por fim, elaborar um plano para disseminar e avaliar as políticas de segurança da empresa. Além disso, foi realizado uma análise conceitual dos documentos de segurança da informação para melhor compreensão e entendimento.

##### Parte 1: Revisão do cenário



<a name="item06.06"><h4>6.6 Recuperação de desastres</h4></a>[Back to summary](#item06)

🌪️ Desastres   
Um desastre é qualquer evento natural ou provocado por humanos que danifica ativos ou propriedades e prejudica a capacidade operacional da empresa.  

🗻 Desastres naturais   
Eles variam de acordo com a localização e podem ser difíceis de prever. Exemplos:  
- Geológicos: terremotos, deslizamentos, vulcões, tsunamis.  
- Meteorológicos: furacões, tornados, tempestades de neve, raios, granizo.  
- Saúde: pandemias, quarentenas, doenças disseminadas.  
- Diversos: incêndios, inundações, tempestades solares, avalanches.  

👥 Desastres provocados por seres humanos   
Envolvem ações de pessoas ou organizações, como:  
- Eventos trabalhistas: greves, passeatas, “operações tartaruga”.  
- Eventos sócio-políticos: vandalismo, protestos, sabotagem, terrorismo, guerra.  
- Eventos materiais: incêndios, derramamentos perigosos.  
- Interrupções de serviços essenciais: falhas de energia, comunicação, escassez de combustível, precipitação radioativa.  

📄 Plano de Recuperação de Desastres (DRP)   
O DRP é ativado durante o desastre, garantindo que sistemas essenciais permaneçam online. Ele define atividades para avaliar, recuperar, reparar e restaurar instalações ou ativos danificados.  

Perguntas fundamentais para criar um DRP:  
- Quem é responsável pelo processo?  
- O que o responsável precisa para executar o processo?  
- Onde o processo é realizado?  
- Qual é o procedimento do processo?  
- Por que o processo é essencial?  

⚡ Priorização de processos   
O DRP identifica os processos mais críticos da empresa. Durante a recuperação, os sistemas essenciais são restaurados primeiro. Controles de recuperação minimizam os efeitos de um desastre, permitindo que recursos e processos retomem a operação.

🛡️ Tipos de controles   
- Preventivos: evitam a ocorrência de desastres, identificando e mitigando riscos.  
- De detecção: descobrem eventos indesejados e novas ameaças.  
- Corretivos: restauram sistemas após um desastre ou evento adverso.  

🔄 Continuidade dos negócios   
Mesmo com prevenção, desastres podem ocorrer. Um plano de continuidade dos negócios (BCP) é essencial, garantindo operações contínuas mesmo enquanto sistemas e instalações originais estão sendo restaurados. 

O BCP inclui:  
- Levar sistemas essenciais para outro local temporariamente.  
- Continuar os processos comerciais até retomar operações normais.  
- Realizar uma análise de impacto nos negócios (BIA) para identificar processos críticos, recursos e dependências.  

⏱️ Métricas importantes da continuidade   
- RTO (Recovery Time Objective): tempo máximo que um sistema pode ficar indisponível.  
- RPO (Recovery Point Objective): ponto de recuperação de dados antes da falha.  
- MTTR (Mean Time to Repair): tempo médio para reparar um componente com falha.  
- MTBF (Mean Time Between Failures): tempo médio entre falhas de um componente.  

👨‍💻 Operacionalização do BCP   
Além de backups e hardware redundante, a continuidade depende de:  
- Colocação das pessoas certas nos lugares certos.  
- Documentação de configurações.  
- Estabelecimento de canais de comunicação alternativos.  
- Garantia de fornecimento de energia.  
- Compreensão das dependências de processos e aplicativos.  
- Capacidade de automatizar tarefas manualmente quando necessário.  

📚 Diretrizes do NIST para BCP   
1) Escrever uma política de continuidade e atribuir funções.  
2) Realizar avaliação de impacto nos negócios (BIA) e priorizar processos críticos.  
3) Calcular riscos, identificando vulnerabilidades e ameaças.  
4) Implementar controles para reduzir riscos.  
5) Desenvolver estratégias de recuperação para sistemas essenciais.  
6) Criar plano de contingência com procedimentos para operação em caos.  
7) Testar o plano em cenários reais.  
8) Manter e atualizar o plano regularmente.  

🧪 Testes e exercícios do DRP   
- Tabletop (Topo de Mesa): discussão de cenários sem execução real de procedimentos.  
- Testes funcionais: testam aspectos específicos do plano e a preparação da equipe.  
- Exercícios operacionais: simulações completas que interrompem serviços para validar o plano em situações reais.

<a name="item06.06.01"><h4>6.6.1 Packet Tracer - Investigar la Recuperación ante un Desastre</h4></a>[Back to summary](#item06)

Este laboratório foi desenvolvido em quatro partes, cada uma composta por várias etapas. Algumas etapas foram documentadas diretamente neste arquivo README, enquanto outras exigiram a criação de arquivos específicos. O objetivo do laboratório foi analisar vulnerabilidades identificadas em uma empresa fictícia, classificá-las por ordem de criticidade, desenvolver uma política de segurança da informação para a vulnerabilidade mais crítica, criar um procedimento detalhado para sua implementação e, por fim, elaborar um plano para disseminar e avaliar as políticas de segurança da empresa. Além disso, foi realizado uma análise conceitual dos documentos de segurança da informação para melhor compreensão e entendimento.

##### Parte 1: Revisão do cenário




<a name="item06.06.02"><h4>6.6.2 Laboratório - Recomende Medidas de Recuperação de Desastres</h4></a>[Back to summary](#item06)

Este laboratório foi desenvolvido em quatro partes, cada uma composta por várias etapas. Algumas etapas foram documentadas diretamente neste arquivo README, enquanto outras exigiram a criação de arquivos específicos. O objetivo do laboratório foi analisar vulnerabilidades identificadas em uma empresa fictícia, classificá-las por ordem de criticidade, desenvolver uma política de segurança da informação para a vulnerabilidade mais crítica, criar um procedimento detalhado para sua implementação e, por fim, elaborar um plano para disseminar e avaliar as políticas de segurança da empresa. Além disso, foi realizado uma análise conceitual dos documentos de segurança da informação para melhor compreensão e entendimento.

##### Parte 1: Revisão do cenário


<a name="item06.07"><h4>6.7 Recuperação de desastres</h4></a>[Back to summary](#item06)

🖥️ Perícia Digital   
A perícia digital consiste na recuperação e investigação de informações encontradas em dispositivos digitais relacionadas a atividades criminosas. Indicadores de comprometimento (IoCs) são evidências de que ocorreu um incidente de segurança cibernética. Essas evidências devem ser preservadas para análises futuras e atribuição do ataque.  

📑 Procedimentos e normas   
Uma organização precisa criar processos e procedimentos bem documentados para análise forense digital. O NIST 800-86, Guia para integração de técnicas forenses em resposta a incidentes, é um recurso valioso. O processo forense envolve quatro etapas: coleta, exame, análise e relatórios.  

A RFC 3227 do IETF descreve a ordem de coleta de evidências digitais com base na volatilidade dos dados. A cadeia de custódia garante a coleta, manuseio e armazenamento seguro das evidências.  

🕵️‍♂️ Identificação de atores   
A identificação dos responsáveis pela ameaça ocorre por investigação sistemática baseada em evidências. A equipe de resposta a incidentes correlaciona Táticas, Técnicas e Procedimentos (TTP) usados no incidente com explorações conhecidas. Fontes de inteligência de ameaças ajudam a mapear TTPs para ataques semelhantes. Descobrir os dispositivos de origem do ataque pode levar diretamente ao ator da ameaça. Modelar o comportamento do ator de ameaça é uma forma de atribuir ataques.  

O MITRE ATT&CK (Adversarial Tactics, Techniques & Common Knowledge) permite detectar táticas, técnicas e procedimentos do atacante como parte da defesa e atribuição de incidentes.  

💀 Cyber Kill Chain   
A Cyber Kill Chain descreve sete etapas do ataque, ajudando analistas a entender técnicas, ferramentas e procedimentos dos atores de ameaça. O objetivo é detectar e interromper o ataque o mais cedo possível.  

Etapas da Kill Chain:  
1. **Reconhecimento:** Pesquisa, coleta de inteligência e seleção de alvos pelo ator de ameaça.  
2. **Armamento:** Desenvolvimento de uma arma baseada nas informações do reconhecimento.  
3. **Entrega:** Transmissão da arma ao alvo através de um vetor de entrega.  
4. **Exploração:** Uso da arma para explorar vulnerabilidades e ganhar controle do alvo.  
5. **Instalação:** Estabelecimento de backdoors para acesso contínuo sem alertar usuários ou analistas.  
6. **Command and Control (CNC):** Estabelecimento de controle remoto sobre o sistema comprometido.  
7. **Ações sobre os Objetivos:** Realização do objetivo final, como roubo de dados, ataque DDoS, envio de spam ou mineração de criptomoedas.  

💎 Modelo Diamond de Análise de Intrusão   
O Modelo Diamond representa um evento de segurança cibernética. Um evento é uma atividade temporária em que um adversário usa uma capacidade sobre uma infraestrutura para atacar uma vítima e alcançar um resultado.  

Características principais de um evento de intrusão:  
- Adversário: Quem realiza o ataque ou causa o incidente.  
- Capacidade: Ferramentas, técnicas e recursos usados pelo adversário.  
- Infraestrutura: Meios ou sistemas utilizados para conduzir o ataque.  
- Vítima: O alvo ou recurso afetado pelo ataque.  

Meta-recursos adicionais incluem:  
- Timestamp: Data e hora do evento.  
- Fase: Etapa do ataque dentro do ciclo de intrusão.  
- Resultado: Consequência ou efeito do evento.  
- Direção: Origem e destino do ataque.  
- Metodologia: Como o ataque foi realizado.  
- Recursos: Qualquer recurso externo utilizado pelo adversário no ataque. 

🔗 Encadeamento de eventos   
Os analistas podem usar o Modelo Diamond para diagramar uma série de eventos. Adversários geralmente encadeiam múltiplos eventos, e cada um deve ser concluído antes do próximo. Esse encadeamento pode ser mapeado com a Cyber Kill Chain, conectando análise de intrusão com prevenção de ataques.

🛡️ Resposta a incidentes   
A resposta a incidentes envolve métodos, políticas e procedimentos usados por uma organização para reagir a ataques cibernéticos. O objetivo é limitar impactos, avaliar danos e implementar recuperação. Planos detalhados e pessoal designado são essenciais. O NIST detalha práticas recomendadas na Publicação Especial 800-61, revisão 2.

👥 Capacidade de resposta a incidentes (CSIRC)   
O primeiro passo é criar um CSIRC, estabelecendo políticas, planos e procedimentos. Partes interessadas incluem: gerenciamento, TI, jurídico, relações públicas, RH, segurança física e continuidade de negócios. A equipe jurídica avalia obrigações legais e a retenção de evidências. Compartilhamento de informações com outras organizações também é recomendado.

🎯 CMMC e maturidade em segurança cibernética   
O CMMC avalia organizações que trabalham para o Departamento de Defesa dos EUA, protegendo a cadeia de suprimentos militar. Possui 17 domínios com recursos específicos. A organização é certificada pelo nível de maturidade alcançado em cada domínio.

🔄 Ciclo de vida da resposta a incidentes   
O NIST define quatro etapas:
1. Preparação  
   - Criar e treinar o CSIRT;  
   - Adquirir e implementar ferramentas e ativos necessários;  
2. Detecção e análise  
   - Identificar incidentes por precursores (sinais de possíveis ataques futuros) ou indicadores (incidentes ocorrendo);  
   - Uso de algoritmos e aprendizado de máquina para validar incidentes;  
   - Criar perfis de rede e sistema para detectar alterações suspeitas;  
3. Contenção, erradicação e recuperação  
   - Determinar o escopo: sistemas, redes, aplicativos afetados e origem do incidente;  
   - Notificar partes interessadas internas e externas;  
   - Preservar evidências de forma documentada;  
   - Identificação de invasores é secundária à contenção;  
   - Corrigir vulnerabilidades exploradas e restaurar sistemas afetados;  
4. Atividades pós-incidente  
   - Realizar reuniões de “lições aprendidas”;  
   - Avaliar a eficácia da resposta e fortalecer controles e práticas de segurança;  

🌪️ Desastres naturais e provocados por humanos   
Desastres naturais variam conforme a localização e são, às vezes, difíceis de prever. Desastres causados por seres humanos envolvem pessoas ou organizações. O DRP (Plano de Recuperação de Desastres) engloba atividades para avaliar, recuperar, reparar e restaurar instalações ou ativos danificados.

🛠️ Controles de recuperação de desastres   
- Controles preventivos: evitam a ocorrência de desastres.  
- Controles de detecção: descobrem eventos indesejados e possíveis ameaças.  
- Controles corretivos: restauram sistemas após desastres ou eventos.  

📊 Continuidade dos negócios   
Os controles vão além de backups e hardware redundante. Um plano de continuidade começa com a análise de impacto nos negócios (BIA), identificando processos críticos, recursos e relacionamentos entre sistemas. A BIA avalia consequências da interrupção para funções essenciais e considera:  
- RTO (Objetivo de Tempo de Recuperação): tempo máximo tolerável que um sistema pode ficar indisponível antes de causar impacto significativo ao negócio.  
- RPO (Objetivo de Ponto de Recuperação): quantidade máxima de dados que pode ser perdida, ou seja, até que ponto os dados precisam ser recuperados.  
- MTTR (Tempo Médio de Reparo): tempo médio necessário para reparar um sistema ou componente após uma falha.  
- MTBF (Tempo Médio entre Falhas): tempo médio esperado entre uma falha e a próxima, indicando a confiabilidade de um sistema.

O NIST fornece melhores práticas para continuidade dos negócios.

🎯 Treinamento e testes do DRP   
- Exercícios de mesa (Tabletop): discussão de cenários e processos sem execução real.  
- Testes funcionais: verificam como determinados aspectos do plano funcionam e a preparação do pessoal.  
- Exercícios operacionais completos: simulam interrupções reais para testar se todos os aspectos do plano são eficazes e suficientes para responder ao incidente.
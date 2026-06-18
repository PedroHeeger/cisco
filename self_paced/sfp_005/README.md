# Introduction To Splunk   <img src="./0-aux/logo_course.png" alt="sfp_005" width="auto" height="45">

### Cisco: <a href="../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../self_paced/">self-paced</a>
### Software/Subject: splunk   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/splunk.png" alt="splunk" width="auto" height="25"></a>
### Course: <a href="./">sfp_005 (Introduction To Splunk)   <img src="./0-aux/logo_course.png" alt="sfp_004" width="auto" height="25"></a>

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
- Cibersecurity:
  - Splunk   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/splunk.png" alt="splunk" width="auto" height="25">

---

<!-- ### Course Strcuture: -->
<h3><a name="item00">Course Strcuture:</a><br></h3>
1. <a href="#item01">Whatis Splunk?</a><br>
2. <a href="#item02">Using Splunk Web</a><br>
3. <a href="#item03">Using Search</a><br>
4. <a href="#item04">Exploring Events</a><br>
5. <a href="#item05">Using Search Terms</a><br>
6. <a href="#item06">What are Commands?</a><br>
7. <a href="#item07">What are Knowledge Objects?</a><br>
8. <a href="#item08">Creating Reports</a><br>
9. <a href="#item09">Creating Dashboards</a><br>
10. <a href="#item10">Dashboard Studio</a><br>
11. <a href="#item11">Additional Resources</a><br>

---

### Objective:
O objetivo deste curso foi apresentar o Splunk, a ferramenta de SIEM da Cisco, mostrando suas principais funcionalidades e recursos, como a ferramenta é instalada e utilizada. O foco foi nos Search Jobs, em como executá-los e em como, através dos dados fornecidos, construir relatórios e dashboards que geram insights.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, contendo todo conteúdo teórico do curso.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:
O desenvolvimento deste curso foi estruturado com base na organização do próprio conteúdo. Como era módulo único, todo o conteúdo foi inserido diretamente aqui, sem a criação de pastas de módulos. Apesar de apresentar uma abordagem voltada à prática, este curso foi teórico, não havendo atividades a serem realizadas.

<a name="item01"><h4>1 Whatis Splunk?</h4></a>[Back to summary](#item00)

🔍 Introdução ao Splunk   
O Splunk consiste em uma plataforma robusta desenvolvida para a coleta, indexação, busca e análise de grandes volumes de dados gerados por máquinas em tempo real. A ferramenta opera de forma centralizada, convertendo registros de logs complexos e dados de infraestrutura em informações estruturadas e acionáveis. A sua aplicação abrange desde o monitoramento contínuo até a investigação detalhada de incidentes, fornecendo visibilidade ponta a ponta sobre o comportamento de aplicações, servidores e dispositivos de rede.

⚙️ Áreas de Aplicação Estratégica   
O uso da plataforma reflete diretamente na eficiência de três pilares fundamentais da infraestrutura de tecnologia modernos:
- ITOps (Operações de TI): Atua na sustentação, estabilidade e disponibilidade dos ambientes tecnológicos. A análise de dados viabiliza a administração preditiva de servidores, redes e rotinas de backup, otimizando o suporte operacional.
- DevOps: Apoia a cultura de integração e implantação contínuas ao unificar as frentes de desenvolvimento e operações. A visibilidade dos dados acelera o ciclo de entrega de software por meio da automação e do monitoramento compartilhado.
- SecOps: Funde a segurança da informação às operações diárias para mitigar riscos sem mitigar a velocidade do negócio. O foco reside na detecção proativa de ameaças, resposta rápida a incidentes e conformidade de controles de segurança.

<a name="item02"><h4>2 Using Splunk Web</h4></a>[Back to summary](#item00)

🏠 Interface Inicial e Navegação   
O ponto de partida na plataforma é a página inicial, um painel centralizado projetado para a exploração inicial do ambiente. Essa interface inicial viabiliza a inicialização e o gerenciamento de aplicações, o acesso direto à documentação técnica e a definição de painéis personalizados como visualização padrão. A partir desse ecossistema, perfis com privilégios administrativos possuem a capacidade de incorporar novas fontes de dados e estender as funcionalidades do sistema.

A navegação global é sustentada por componentes estruturais que permanecem acessíveis em todo o sistema:
- Splunk Bar: Barra superior presente em todas as páginas da plataforma. Agrega funções de alternância entre aplicações, edição de preferências da conta do usuário, exibição de mensagens do sistema, gerenciamento de configurações gerais, monitoramento do progresso de tarefas de busca e suporte técnico.
- Applications Menu: Elemento localizado na extremidade superior esquerda da barra principal, dedicado exclusivamente à troca rápida de contexto entre os diferentes aplicativos instalados.
- Apps Bar: Barra de navegação secundária posicionada imediatamente abaixo da barra principal. Concentra os atalhos para os módulos operacionais de busca, análise, conjuntos de dados, relatórios, alertas e painéis.

🔍 O Aplicativo de Busca e Relatórios   
O módulo de busca e relatórios constitui a interface padrão para a análise detalhada e a execução de consultas sobre os dados indexados. A composição dessa área de trabalho baseia-se em elementos especializados para a filtragem e extração de informações:
- Mecanismos de Consulta e Tempo: A barra de busca recebe as instruções de consulta para processamento imediato. Associado a ela, o seletor de intervalo de tempo delimita o escopo temporal dos eventos que serão recuperados na pesquisa.
- Histórico de Buscas: Menu dedicado à revisão e reexecução de consultas anteriores. O recurso dispõe de filtros textuais e temporais específicos para segmentar buscas processadas no dia corrente, nos últimos sete dias ou nos últimos 30 dias.
- Painel de Instruções e Sumário de Dados: Espaço que disponibiliza documentação de apoio e tutoriais. O acionamento do sumário de dados detalha a volumetria indexada com base em três metadados fundamentais: o host (nome da máquina, endereço IP ou domínio de origem), a fonte (arquivo, diretório, porta de rede ou script gerador) e o tipo de fonte (sourcetype).
- Visualizações em Tabela: Recursos baseados em interface gráfica que permitem a exploração e a preparação de dados de forma visual, dispensando a escrita direta em linguagem de processamento de buscas.

👥 Gerenciamento de Perfis e Permissões   
O controle de acesso e o nível de interação com os recursos do sistema são determinados por papéis funcionais. O ambiente nativo do produto estabelece três perfis de privilégios predefinidos:
- Administrador: Perfil de maior privilégio no ambiente, detendo autonomia para a instalação de aplicações, ingestão de novas fontes de dados e criação de objetos de conhecimento globais.
- Power: Perfil intermediário com capacidade de desenvolver e compartilhar objetos de conhecimento entre usuários de uma mesma aplicação, além de possuir permissão para executar buscas em tempo real.
- Usuário: Perfil restrito à visualização de objetos de conhecimento próprios ou explicitamente compartilhados com a sua conta.

☁️ Modelos de Implantação e Ecossistema   
O software distribui-se em diferentes arquiteturas de implantação para atender a requisitos variados de infraestrutura e governança:
- Splunk Enterprise: Modelo implantado e gerenciado localmente em servidores próprios ou máquinas virtuais da organização. Garante o controle total sobre atualizações, políticas de armazenamento, segurança e dimensionamento de infraestrutura, sendo amplamente adotado em centros de operações de segurança.
- Splunk Cloud: Modalidade de software como serviço em que a infraestrutura subjacente é totalmente administrada, atualizada e mantida pelo provedor. A experiência operacional assemelha-se à versão local, porém adota papéis adicionais específicos para nuvem, incluindo permissões voltadas para exclusão de dados, autenticação baseada em tokens e gestão restrita de aplicações.
- Splunkbase: Repositório centralizado que disponibiliza centenas de aplicações homologadas e complementos desenvolvidos pela comunidade ou parceiros para estender as capacidades nativas da plataforma.

<a name="item03"><h4>3 Using Search</h4></a>[Back to summary](#item00)

🔍 Execução de Consultas e o Ciclo de Vida do Search Job   
A execução de uma consulta dentro do aplicativo de busca e relatórios baseia-se na escrita de instruções estruturadas em Search Processing Language (SPL). Durante a digitação na barra de pesquisas, o recurso Splunk Search Assistant fornece suporte em tempo real ao exibir termos correspondentes, sugestões contextuais e documentação sintática para os comandos utilizados. A delimitação temporal da pesquisa por meio do seletor de intervalo de tempo constitui uma prática fundamental para otimizar o desempenho do sistema e acelerar o retorno dos resultados.

A submissão de uma consulta inicia um processo interno denominado Search Job. Este componente técnico representa a execução física da pesquisa e encapsula dados de progresso, métricas de desempenho (como tempo de processamento e volume de dados analisados), estatísticas e os resultados temporariamente armazenados. Por padrão, um Search Job permanece ativo na memória por 10 minutos. Caso o gatilho de compartilhamento seja acionado, esse ciclo de vida é estendido para sete dias, permitindo que outros usuários visualizem exatamente o mesmo conjunto de dados original sem a necessidade de reprocessamento.

🖥️ Componentes da Interface de Resultados   
Após o disparo de um Search Job, a interface de usuário habilita um conjunto de ferramentas analíticas e de controle operacional:

Abas de Resultados (Search Result Tabs)   
A exibição dos dados resultantes segmenta-se em quatro visões especializadas:
  - Events: Apresenta a listagem detalhada dos logs recuperados e destaca os campos extraídos na barra lateral dedicada.
  - Patterns: Identifica tendências e recorrências estruturais nos dados para facilitar a compreensão de comportamentos anômalos no ambiente.
  - Statistics: Exibe tabelas de dados tabulados quando a consulta emprega comandos de transformação (transforming commands), que convertem eventos brutos em matrizes estatísticas.
  - Visualization: Renderiza gráficos e elementos visuais baseados nas estatísticas geradas. Caso a busca não seja transformativa, a interface exibe links para ferramentas assistidas como Pivot e relatórios rápidos.

Seletores e Painéis de Controle   
- Search Mode Selector: Controla o balanço entre desempenho e profundidade de análise através de três modos:
  - Fast Mode: Desabilita a descoberta automática de campos, retornando apenas os metadados padrões e os campos explicitamente requisitados na busca para maximizar a velocidade.
  - Verbose Mode: Ativa a descoberta máxima de campos e extrai o maior volume possível de dados dos eventos, priorizando o detalhamento em detrimento da velocidade.
  - Smart Mode: Configuração padrão que alterna automaticamente o comportamento do sistema entre os modos rápido e detalhado com base na complexidade da consulta executada.
- Timeline: Representação gráfica e volumétrica dos eventos distribuídos ao longo do tempo. Os segmentos são gerados dinamicamente e permitem interações como cliques para filtragem direta ou o uso de ferramentas de zoom para estreitar o escopo da investigação.
- Search Action Buttons: Conjunto de controles operacionais que viabiliza pausar, interromper, inspecionar o desempenho ou enviar a execução da busca para segundo plano (background).
- Save As Menu: Permite persistir a consulta estruturada, convertendo-a em um objeto de conhecimento reutilizável dentro da plataforma.
- Export Icon: Permite a extração física dos dados retornados pelo trabalho de busca nos formatos estruturados CSV, XML, JSON ou em formato de texto bruto (raw).

🛡️ Cenário Prático: Investigação de Acesso Indevido   
Em um cenário de resposta a incidentes, como a suspeita de um acesso não autorizado a um servidor corporativo, as ferramentas operam de maneira integrada:
- O analista acessa o aplicativo de busca e relatórios.
- A consulta é inserida na barra de buscas filtrando pelo termo failed associado aos eventos de autenticação do servidor afetado.
- O seletor de tempo é ajustado para delimitar a busca à última semana, otimizando o tempo de resposta do Search Job.
- A linha do tempo indica os picos volumétricos de falhas, permitindo isolar o momento exato do ataque.
- Os dados são analisados na aba de eventos para identificar a origem das requisições e, posteriormente, exportados em formato JSON para subsidiar o relatório de auditoria.

<a name="item04"><h4>4 Exploring Events</h4></a>[Back to summary](#item00)

📄 Composição e Interação na Lista de Eventos   
A conclusão de uma busca resulta na exibição da lista de eventos, disposta por padrão em ordem cronológica inversa, o que prioriza a visualização dos registros mais recentes. O termo ou argumento pesquisado é automaticamente realçado no corpo do texto de cada log para agilizar a identificação visual. Embora os dados contidos no indexador sejam padronizados em um formato temporal consistente, a estampa de tempo (timestamp) exibida na interface é ajustada dinamicamente com base no fuso horário configurado no perfil do usuário.

A interação direta com os dados exibidos permite refinar e expandir a estratégia de busca sem a necessidade de digitação manual:
- Inclusão e Exclusão Dinâmica: Ao posicionar o cursor sobre qualquer segmento de texto de um evento, o termo é destacado. O clique sobre esse elemento abre opções para incorporá-lo à consulta atual, excluí-lo dos resultados ou iniciar uma nova pesquisa em uma janela de navegação separada.
- Metadados Inferiores: Na base de cada bloco de evento, são exibidos os campos selecionados ativos. Como padrão de fábrica, o sistema apresenta os metadados host, source e sourcetype.

ℹ️ Painel de Informações do Evento e Ações de Campo   
O acionamento do botão de informações (info button), localizado ao lado esquerdo de cada registro, expande uma interface detalhada com todos os campos estruturados que foram extraídos automaticamente daquele log específico.

Nesse painel expandido, os campos definidos como ativos exibem uma marca de seleção ao lado de seus respectivos nomes. A interface disponibiliza menus suspensos específicos para a execução de tarefas avançadas:
- Event Actions: Permite aplicar tratamentos ou fluxos de trabalho diretamente ao log selecionado.
- Field Actions: Atalho técnico que possibilita configurar novas regras de extração, criar aliases ou vincular o campo a links e ferramentas externas de análise.

<a name="item05"><h4>5 Using Search Terms</h4></a>[Back to summary](#item00)

📝 Sintaxe e Operadores de Busca em SPL   
A construção de consultas na plataforma baseia-se em regras sintáticas específicas que determinam a abrangência e a precisão do Search Job. O comportamento dos argumentos de busca segue diretrizes padronizadas de interpretação:
- Insensibilidade a Maiúsculas e Minúsculas: Os termos de busca comuns não diferenciam maiúsculas de minúsculas (case-insensitive). Desse modo, a inserção de um argumento em qualquer variação de caixa retornará os mesmos resultados correspondentes.
- Busca por Frases Exatas: A delimitação de termos compostos por meio de aspas duplas força o sistema a procurar pela sequência textual exata. Caso o próprio conteúdo a ser pesquisado contenha aspas, utiliza-se o caractere de escape barra invertida (\\) imediatamente antes das aspas internas.
- Uso de Curingas: O caractere asterisco (\*) atua como curinga para expandir o escopo da pesquisa. A sua inserção ao final de um radical, como fail*, instrui o motor de busca a retornar qualquer variação que inicie com aquele fragmento, incluindo fail, failure e failed.

⚖️ Operadores Lógicos e Ordem de Avaliação   
A combinação de múltiplos critérios de filtragem é realizada através de operadores booleanos, os quais exigem obrigatoriamente a escrita em letras maiúsculas: AND, OR e NOT.
- AND: Operador implícito padrão. Caso nenhum operador seja explicitado entre dois termos na barra de busca, o sistema assume a conjunção AND, exigindo a presença de ambos os argumentos no evento.
- OR: Utilizado para ampliar a pesquisa, retornando registros que contenham pelo menos um dos termos especificados.
- NOT: Empregado para excluir eventos que apresentem o termo subsequente à cláusula.

Os operadores booleanos possuem uma ordem de precedência nativa para a avaliação das expressões. O motor de busca processa prioritariamente as cláusulas NOT, seguidas pelas instruções OR e, por fim, pelas operações AND. Essa ordem lógica padrão pode ser alterada ou explicitamente controlada mediante o emprego de parênteses, priorizando o conteúdo contido em seu interior.

<a name="item06"><h4>6 What are Commands?</h4></a>[Back to summary](#item00)

🏗️ Anatomia da Search Processing Language (SPL)   
A Search Processing Language (SPL) é estruturada a partir de cinco componentes lógico-sintáticos essenciais que definem o comportamento e o fluxo de transformação dos dados:
- Search Terms (Termos de Busca): Constituem a base fundamental de qualquer consulta, atuando como os filtros iniciais para localizar os registros desejados no indexador.
- Commands (Comandos): Instruem o motor de busca sobre a ação a ser executada com os resultados obtidos, englobando a criação de gráficos, computação de estatísticas e formatação de saídas.
- Functions (Funções): Determinam os métodos específicos de cálculo, avaliação ou plotagem que serão aplicados aos dados.
- Arguments (Argumentos): Representam as variáveis ou valores fornecidos como entrada para que uma função possa operar.
- Clauses (Cláusulas): Definem a forma de agrupamento, ordenação ou limitação dos resultados gerados.

O fluxo de processamento ocorre de maneira sequencial da esquerda para a direita. Utiliza-se o caractere pipe (|) para indicar que o resultado obtido pelo componente anterior deve ser direcionado e injetado diretamente como entrada para o componente subsequente.

No exemplo clássico `index=network sourcetype=cisco_wsa_squid usage=Violation | stats count(usage) as Visits`, os termos de busca iniciais filtram a massa de dados e o caractere pipe encaminha esses registros para o comando stats, que emprega a função count associada ao argumento usage e à cláusula de renomeação as Visits.

🚀 Boas Práticas de Desempenho e Otimização   
A eficiência na execução de consultas correlaciona-se diretamente com a correta aplicação de filtros e o entendimento de como o sistema processa a informação. As seguintes diretrizes garantem a otimização de performance:
- Diferenciação de Caixa: Os nomes de comandos, cláusulas e funções não diferenciam maiúsculas de minúsculas. Contudo, se um comando fizer referência a um valor específico extraído de um evento, a correspondência desse valor exato será sensível à caixa (case-sensitive).
- Limitação Temporal: A restrição do intervalo de tempo é o mecanismo de filtragem mais eficiente. Reduzir o volume de dados que o motor precisa varrer acelera significativamente o tempo de resposta do sistema.
- Uso de Campos Indexados: Após o fator tempo, os metadados padrões index, source, host e sourcetype são os filtros mais poderosos, pois são extraídos no momento da ingestão (index-time) e dispensam processamento computacional para extração durante a busca.
- Especificidade e Inclusão: Fornecer mais detalhes ao motor de busca melhora o direcionamento dos resultados (buscar por failed password é mais eficiente do que buscar apenas por password). Adicionalmente, estratégias de inclusão apresentam melhor rendimento do que exclusões (adotar access denied é superior a computar NOT access granted).
- Substituição de Curingas: Sempre que aplicável, deve-se priorizar o uso dos operadores lógicos OR ou IN em detrimento do uso do caractere curinga asterisco (*).
- Filtragem Precoce: Os comandos de filtragem devem ser inseridos o mais cedo possível na linha de comando de busca. Isolar e reduzir a volumetria de eventos logo no início da esteira de processamento otimiza o desempenho de manipulações subsequentes.

<a name="item07"><h4>7 What are Knowledge Objects?</h4></a>[Back to summary](#item00)

🧩 Conceito e Importância dos Objetos de Conhecimento   
Os objetos de conhecimento (knowledge objects) consistem em entidades criadas por usuários para enriquecer, classificar e extrair inteligência dos dados indexados durante o tempo de busca (search-time mapping). A relevância desses componentes reside na capacidade de reutilização e compartilhamento baseado em permissões, permitindo que regras de negócio complexas sejam encapsuladas e consumidas por múltiplos analistas ou aplicações distintas simultaneamente.

A governança desse ecossistema é conduzida pelos Gerentes de Conhecimento (Knowledge Managers). Estes profissionais são responsáveis por supervisionar o ciclo de vida dos objetos, implementar padronizações de nomenclatura, normalizar os registros de eventos e estruturar modelos de dados. Essa atuação garante a eficiência operacional do ambiente, mantendo os recursos organizados e otimizados para o uso geral da plataforma.

🗂️ Categorização dos Objetos de Conhecimento   
Os objetos de conhecimento são classificados em cinco grandes categorias funcionais de acordo com o objetivo analítico que cumprem no sistema:

- Interpretação de Dados (Data Interpretation):
  - Focada na identificação e isolamento de informações específicas contidas no corpo dos logs brutos.
  - Campos Extraídos: Embora o sistema capture metadados automaticamente com base no tipo de fonte (sourcetype), novos campos podem ser extraídos manualmente para isolar variáveis críticas.
  - Campos Calculados: Expressões matemáticas ou lógicas aplicadas aos eventos em tempo de execução, gerando um novo campo cujo valor decorre da manipulação de variáveis já existentes no registro.
- Classificação de Dados (Data Classification):
  - Destinada a agrupar e categorizar informações para simplificar a organização lógica do ambiente.
  - Tipos de Eventos (Event Types): Mecanismo de rotulação de logs que atende a critérios específicos de uma consulta, facilitando a busca subsequente por categorias inteiras de eventos.
  - Transações: Agrupamentos lógicos de múltiplos eventos conceitualmente relacionados que se estendem ao longo do tempo, como o rastreamento completo de uma sessão de compra de ponta a ponta.
- Enriquecimento de Dados (Data Enrichment):
  - Adiciona contexto externo ou inteligência operacional aos logs que já foram indexados.
  - Consultas (Lookups): Cruzamento de dados que injeta novos campos e valores aos eventos a partir de fontes externas (como tabelas CSV ou bancos de dados), sem alterar o dado armazenado no indexador.
  - Ações de Fluxo de Trabalho (Workflow Actions): Criação de hiperlinks dinâmicos dentro dos eventos que permitem interagir com ferramentas externas de suporte ou refinar instantaneamente o escopo da busca atual.
- Normalização de Dados (Data Normalization):
  - Padroniza a nomenclatura de termos provenientes de fontes distintas para viabilizar análises correlacionadas.
  - Aliases de Campo (Field Aliases): Atribuição de codinomes a campos extraídos de diferentes origens. Permite correlacionar logs de firewalls de fabricantes distintos, por exemplo, unificando os termos sob uma mesma nomenclatura de campo.
  - Tags: Rótulos descritivos vinculados a pares de chave-valor específicos, funcionando como etiquetas de busca rápida para identificar conjuntos particulares de dados.
- Modelos de Dados (Data Models):
  - Estruturas hierárquicas compostas por conjuntos de dados estruturados que combinam eventos, buscas salvas e transações. Esses modelos servem como base simplificada e abstrata para alimentar relatórios e viabilizar a criação de painéis por usuários da ferramenta de análise assistida Pivot.

<a name="item08"><h4>8 Creating Reports</h4></a>[Back to summary](#item00)

📊 Geração e Gerenciamento de Relatórios (Reports)   
A conversão de uma consulta técnica em um relatório (report) constitui o método padrão para a persistência e o compartilhamento de resultados dentro da plataforma. O processo de criação ocorre por meio do acionamento da opção correspondente dentro do menu Save As. A interface de configuração exige a definição de um título estruturado, descrição opcional, confirmação do modelo de exibição visual e a escolha sobre a inclusão do seletor de intervalo de tempo na interface final.

Para assegurar a governança e a manutenibilidade do ambiente, as organizações devem adotar convenções estritas de nomenclatura antes da consolidação desses objetos. Recomenda-se uma estrutura padronizada que contemple o departamento demandante, o tipo de objeto de conhecimento e uma descrição concisa do escopo de análise (ex: Seguranca_Relatorio_FalhasLoginSsh).

Os relatórios consolidados ficam centralizados na aba Reports da barra de navegação. Ao acessar um relatório, o motor de busca processa uma nova consulta em tempo real, trazendo dados atualizados. Caso o seletor de tempo tenha sido habilitado na criação, o analista operacional possui a flexibilidade de modificar o escopo temporal da análise diretamente na interface de visualização do relatório.

🔐 Permissões, Governança e Modos de Execução   
Por padrão de fábrica, todo relatório nasce configurado como privado, sendo visível exclusivamente para o seu criador. A expansão do menu de detalhes do objeto permite elevar o nível de visibilidade para o escopo do aplicativo (App), tornando-o acessível para os demais integrantes daquela área de trabalho (como o módulo Search & Reporting). A ampliação do acesso para o nível global (visível em todas as aplicações do sistema) é uma atribuição exclusiva de contas com perfil de administrador.

A definição do contexto de segurança para a execução do relatório baseia-se na diretiva Run As, que dispõe de dois modos operacionais:
- Owner (Proprietário): O relatório executa utilizando os privilégios e permissões de acesso a dados da conta que o criou. Sob essa configuração, existe o risco de expor logs confidenciais a usuários comuns caso o criador possua acessos privilegiados no indexador.
- User (Usuário): A consulta processa estritamente sob o escopo de segurança e visibilidade do usuário que disparou a execução no momento atual, omitindo registros para os quais ele não possua credenciais de leitura.

⏱️ Agendamento de Consultas e Otimização Ambiental   
O agendamento de relatórios em intervalos programados (horários, diários, semanais, mensais ou via sintaxe cron customizada) atua como um mecanismo crítico de otimização de infraestrutura. Essa prática reduz o estresse computacional gerado por buscas simultâneas e repetitivas de caráter ad-hoc, sendo altamente recomendada para relatórios consumidos por múltiplos analistas ou integrados a painéis operacionais.

A ativação do agendamento impõe alterações estruturais automáticas no comportamento do objeto:
- Restrição de Interface: O seletor de intervalo de tempo é removido da visualização final, fixando o escopo temporal definido na janela de agendamento.
- Precedência de Execução: A ativação do agendamento sobrescreve as diretivas personalizadas de Run As.
- Janela de Agendamento (Schedule Window): Recurso utilizado para definir uma margem temporal tolerável para o disparo da busca. Isso evita gargalos de processamento quando há concorrência de múltiplos relatórios agendados para o mesmo horário exato.

Os relatórios agendados podem disparar ações de resposta automatizadas (trigger actions) baseadas nos resultados obtidos. As integrações nativas englobam o envio dos dados tabulados por correio eletrônico (e-mail), o disparo de requisições HTTP para URLs externas via webhooks ou a execução de scripts customizados desenvolvidos para a automação de fluxos de trabalho da organização.

<a name="item09"><h4>9 Creating Dashboards</h4></a>[Back to summary](#item00)

📊 Visualizações e Criação de Painéis (Dashboards)   
A transformação de dados estatísticos em elementos visuais constitui um dos recursos mais poderosos para a análise de dados na plataforma. Qualquer consulta que retorne valores tabulares e estruturados por meio de comandos de transformação pode ser convertida diretamente em gráficos. A interface disponibiliza uma ampla variedade de representações visuais, permitindo ajustar o formato para melhor expor o comportamento dos dados, incluindo recursos interativos como a exibição de métricas detalhadas ao posicionar o cursor sobre segmentos específicos de um gráfico.

Para consolidar e compartilhar essas visualizações de forma unificada, os elementos são agrupados em painéis (dashboards). O processo de criação inicia-se no menu Save As, selecionando a opção de salvar em um painel novo ou existente. Durante a configuração inicial, define-se o título do painel, uma descrição opcional e o nível de permissão de acesso. É uma prática recomendada manter o status como privado durante a fase de desenvolvimento, alterando a visibilidade para o escopo do aplicativo ou global apenas após a validação de todo o conteúdo.

🏗️ Frameworks e Estrutura de Painéis   
A plataforma disponibiliza dois frameworks distintos para a construção e estilização de painéis:
- Classic Dashboards: Modelo tradicional baseado em estruturas rígidas de linhas e colunas, amplamente utilizado pela compatibilidade com versões anteriores e simplicidade de layout.
- Dashboard Studio: Ambiente moderno de design que oferece total liberdade de customização visual, permitindo o uso de imagens de fundo personalizadas, posicionamento livre de componentes e recursos avançados de design corporativo.

Ao incorporar um novo painel de exibição, o sistema vincula a visualização a uma consulta em linha (inline search). No menu de configurações avançadas (Advanced Panel Settings), o administrador pode gerenciar essa dependência e verificar se o comportamento de detalhamento está ativo.

🛠️ Edição Avançada e Interatividade   
A evolução de um painel estático para uma ferramenta analítica interativa ocorre por meio do modo de edição. Dentro desse ambiente de desenvolvimento, novos blocos de informação podem ser acoplados ao painel através do menu Add Panel, que oferece quatro métodos de inserção:
- Criação de uma nova visualização do zero, sem a necessidade de retornar à tela de buscas global.
- Vinculação direta de um relatório (report) já existente e homologado.
- Clonagem de um painel pertencente a outro dashboard corporativo.
- Inclusão de um bloco de visualização pré-construído (prebuilt panel).

O modo de edição estende a capacidade técnica do analista ao permitir a manipulação direta do código-fonte em formato XML, a aplicação de temas visuais (como o modo escuro) e a introdução de elementos de entrada de dados (inputs), como caixas de texto e seletores de tempo globais que filtram todos os blocos do painel simultaneamente.

A interatividade é refinada por meio do editor de detalhamento (drilldown editor). Esse recurso mapeia a ação do usuário ao clicar em um ponto do gráfico, direcionando o fluxo analítico para cinco destinos possíveis:
- Execução da consulta estruturada original no módulo de buscas.
- Redirecionamento para outro painel operacional correlacionado.
- Abertura de um relatório específico.
- Encaminhamento para uma URL externa customizada.
- Manipulação de variáveis de memória (tokens) para atualizar dinamicamente outros elementos do próprio painel em tempo real.

<a name="item10"><h4>10 Dashboard Studio</h4></a>[Back to summary](#item00)

🎨 Evolução de Painéis no Dashboard Studio   
O Dashboard Studio representa a evolução na camada de apresentação visual da plataforma, fornecendo recursos avançados de design que superam as limitações estruturais do modelo Classic Dashboard. Um painel tradicional pode ser migrado para este novo framework por meio da funcionalidade de clonagem (Clone in Dashboard Studio), mantendo as propriedades de metadados como título, descrição e permissões de acesso, mas habilitando uma nova suíte de ferramentas de edição.

O desenvolvimento dentro deste ecossistema exige a seleção entre dois modos de disposição de layout, os quais determinam como os elementos visuais interagem com a tela de pintura (canvas):
- Modo de Grade (Grid Layout):
  - Projetado para uma construção rápida e estruturada, este modo organiza os elementos automaticamente por meio de mecanismos de alinhamento magnético (snap to alignment).
  - Comportamento: Os painéis são confinados em linhas e colunas organizadas de forma responsiva.
  - Customização: A redimensionalização de um bloco é realizada arrastando as suas bordas diretamente com o cursor, fazendo com que todos os componentes vizinhos se ajustem de maneira coordenada para preencher o espaço.
  - Indicação: Ideal para cenários operacionais padrão que demandam rapidez na entrega e foco na legibilidade das tabelas e gráficos estatísticos.
- Modo Absoluto (Absolute Layout):
  - Oferece total liberdade criativa ao analista por meio de um controle de posicionamento preciso ao nível de pixel (pixel-perfect), eliminando restrições de alinhamento automático.
  - Recursos de Design: Permite a definição livre do tamanho da tela, alteração de cores de fundo ou aplicação de imagens de preenchimento complexas.
  - Elementos Gráficos: Suporta a sobreposição de camadas, inserção de formas geométricas personalizadas, ícones dinâmicos e upload de arquivos de imagem de até 16 megabytes.
  - Indicação: Recomendado para a criação de painéis executivos (C-Level) de alta fidelidade visual ou centros de controle de operações (SOC) que utilizam topologias de rede ou mapas de calor como plano de fundo.

🛠️ Interface de Controle e Configuração   
Uma vez inicializado o ambiente de edição no Dashboard Studio, a barra de ferramentas superior centraliza os comandos de governança do painel, permitindo interações diretas sem a necessidade de alternar entre diferentes menus do sistema:
- Gerenciamento de Entradas e Fontes: Ícones dedicados à inserção de filtros de entrada (inputs) e à configuração centralizada das fontes de dados (data sources) que alimentam as buscas em segundo plano.
- Enriquecimento Textual: Suporte nativo para a inclusão de blocos de texto formatados em sintaxe Markdown para documentação ou inserção de notas operacionais diretamente no painel.
- Configuração Contextual: O painel lateral de propriedades exibe parâmetros dinâmicos que se alteram automaticamente com base no tipo de visualização selecionada, permitindo customizar eixos, legendas e cores de maneira isolada.
- Manipulação em Código: Substitui o antigo formato XML do modelo clássico pela definição estruturada em JSON, viabilizando a exportação, importação e edição direta de toda a declaração lógica do painel através de um editor de texto embutido.

<a name="item11"><h4>11 Additional Resources</h4></a>[Back to summary](#item00)

📚 Ecossistema Oficial de Aprendizado e Suporte Técnico   
A consolidação do conhecimento e a resolução de desafios complexos na plataforma são sustentadas por canais oficiais de capacitação, documentação e compartilhamento de boas práticas. Esses recursos são segmentados para atender desde a formação profissional até a implementação estratégica de soluções corporativas:
- Splunk Documentation: Consiste no repositório técnico oficial da plataforma. Centraliza manuais detalhados e referências completas sobre os processos de instalação, arquitetura de infraestrutura, administração de instâncias, segurança e o catálogo integral de comandos e sintaxes da Search Processing Language (SPL).
- Splunk Training & Certification: Portal dedicado à capacitação estruturada e trilhas de formação profissional. Constitui a vertente oficial para a preparação de exames e obtenção de certificações técnicas reconhecidas pelo mercado, cobrindo níveis que vão do perfil de usuário analista até funções especializadas de administração e arquitetura.
- Splunk Lantern: Centro de Sucesso do Cliente voltado para a disseminação de estratégias práticas e guias de implementação. O foco deste ecossistema reside na apresentação de casos de uso reais e metodologias de negócio, auxiliando as organizações a extraírem o máximo valor operacional dos dados indexados.
- Splunk How-To: Canal multimídia focado em instruções visuais e demonstrações passo a passo. Reúne tutoriais dinâmicos desenvolvidos para ilustrar recursos específicos da interface, metodologias de busca rápida e configurações práticas do dia a dia de forma simplificada.
# Networking Devices and Initial Configuration - Módulo 2   <img src="../0-aux/logo_course.png" alt="sfp_008" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">sfp_008 (Networking Devices and Initial Configuration)   <img src="../0-aux/logo_course.png" alt="sfp_008" width="auto" height="25"></a>
### Module: 2. Nuvem e virtualização

---

### Theme:
- Network

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
2. <a name="item02">Nuvem e virtualização</a><br>
  2.1 <a href="#item02.01">Introdução</a><br>
  2.2 <a href="#item02.02">Nuvem e Serviços de Nuvem</a><br>
  2.3 <a href="#item02.03">Virtualização</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.3.1 <a href="../../../labs/files/lab_056/">Laboratório - Instalar o Linux em uma Máquina Virtual e Explorar a GUI</a><br>
  2.4 <a href="#item02.04">Resumo de Nuvem e Virtualização</a><br>
  
---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item02.01"><h4>2.1 Introdução</h4></a>[Back to summary](#item02)

☁️ Computação em Nuvem e Virtualização   
A modernização da infraestrutura tecnológica corporativa baseia-se na migração de servidores físicos para ambientes abstratos e centralizados. A integração de serviços em nuvem e tecnologias de virtualização permite que as organizações reduzam custos operacionais com espaço físico, consumo energético e manutenção de hardware, além de otimizar a segurança e a continuidade dos negócios por meio de mecanismos eficientes de redundância e recuperação de dados.

🎯 Objetivo do módulo:   
- Explicar os conceitos, o funcionamento e os benefícios das tecnologias de virtualização e dos modelos de computação em nuvem.

📘 Tópicos do módulo:   
- Nuvem e Serviços de Nuvem: Análise das características fundamentais, modalidades de implantação e tipos de serviços fornecidos sob demanda por provedores externos.
- Virtualização: Descrição técnica do propósito, funcionamento de hipervisores e métodos de emulação de múltiplos sistemas operacionais independentes em um único hardware físico.

<a name="item02.02"><h4>2.2 Nuvem e Serviços de Nuvem</h4></a>[Back to summary](#item02)

☁️ Os Quatro Modelos de Implantação em Nuvem   
A computação em nuvem não é uma estrutura de tamanho único. Para atender a diferentes requisitos de orçamento, privacidade e conformidade, a infraestrutura é classificada em quatro modelos principais de entrega:
- Nuvem Pública: Serviços hospedados por provedores terceiros e disponibilizados para qualquer pessoa ou empresa via internet. O modelo financeiro baseia-se na escalabilidade e no pagamento pelo uso real (pay-as-you-go), como no caso de armazenamento web compartilhado.
- Nuvem Privada: Um ambiente digital exclusivo para uma única organização (como agências governamentais ou grandes corporações). Pode ser mantida localmente na infraestrutura própria da empresa — o que demanda alto investimento em hardware e manutenção — ou terceirizada para um provedor que garanta isolamento e perímetros de segurança rigorosos.
- Nuvem Híbrida: A união simbiótica de duas ou mais topologias de nuvem (como a integração entre uma nuvem privada e uma pública). Embora permaneçam como entidades independentes, elas são conectadas por uma arquitetura padronizada, permitindo a portabilidade de dados e níveis de acesso customizados para os usuários.
- Nuvem Comunitária: Uma infraestrutura compartilhada de forma restrita por organizações que possuem objetivos ou obrigações em comum. A grande diferença para a nuvem pública é a personalização para atender a nichos específicos, como o setor de saúde, que exige conformidade estrita com leis de sigilo e autenticação avançada (como a norma HIPAA).

🏗️ Virtualização: O Alicerce Oculto da Nuvem   
É comum confundir os conceitos de computação em nuvem e virtualização, mas eles operam em camadas distintas: a virtualização é a tecnologia habilitadora da nuvem. Sem ela, a nuvem moderna simplesmente não existiria.

Em termos práticos, virtualizar significa usar software para criar uma representação digital e abstrata de um recurso físico — como simular e executar um sistema operacional Linux dentro de uma máquina cujo sistema nativo é o Windows. Essa revolução ganhou força com tecnologias pioneiras que permitiram a um único hardware de servidor hospedar múltiplos sistemas operacionais clientes de forma simultânea e isolada.

📉 O Antigo Modelo Físico e Seus Gargalos   
Para compreender o valor da virtualização, é preciso olhar para o modelo tradicional de Data Centers de décadas atrás, onde a arquitetura era rígida: um sistema operacional instalado diretamente em um hardware dedicado. Essa abordagem centralizada gerava dois problemas críticos de engenharia:
- O Ponto Único de Falha (SPOF): Como todos os recursos de processamento (CPU), memória RAM e armazenamento estavam vinculados a uma única máquina física dedicada a uma função (como e-mail ou servidor web), a quebra de qualquer componente de hardware interrompia o serviço por completo, derrubando a aplicação instantaneamente.
- Expansão Desordenada e Ociosidade (Server Sprawl): Servidores dedicados costumavam passar a maior parte do tempo ociosos, operando bem abaixo de sua capacidade máxima enquanto aguardavam picos de requisições. Essa subutilização resultava em desperdício massivo de energia elétrica, refrigeração e espaço físico nos racks, um fenômeno técnico conhecido como server sprawl.

A virtualização resolve esse cenário ao fragmentar o hardware físico em várias máquinas virtuais, maximizando a eficiência energética e a resiliência operacional da infraestrutura.

<a name="item02.03"><h4>2.3 Virtualização</h4></a>[Back to summary](#item02)

📉 O Impacto Econômico da Consolidação   
A transição de servidores físicos para ambientes virtuais gera uma redução imediata nas despesas operacionais (OpEx) e de capital (CapEx). Esse ganho financeiro fundamenta-se em três fatores:
- Otimização de Hardware: Concentrar a carga de trabalho em menos equipamentos reduz os custos de aquisição e as despesas com contratos de manutenção de hardware.
- Eficiência Energética: A diminuição de servidores físicos ativos resulta em uma queda direta no consumo de eletricidade e alivia a demanda dos sistemas de refrigeração.
- Aproveitamento de Espaço: Minimiza a quantidade de racks necessários nos Data Centers, permitindo maior densidade computacional por metro quadrado.

🚀 Ganhos Operacionais e Resiliência de Infraestrutura   
Além da economia básica, a virtualização eleva a agilidade e a segurança da operação de TI através de recursos específicos:
- Prototipagem Ágil: Permite a criação instantânea de laboratórios e ambientes de teste completamente isolados da rede de produção.
- Provisionamento Veloz: O tempo necessário para implantar uma nova máquina virtual é drasticamente menor do que o processo de configurar um servidor físico do zero.
- Alta Disponibilidade (Uptime): Mecanismos integrados de redundância e tolerância a falhas garantem a continuidade dos serviços mesmo em caso de pane no hardware.
- Recuperação de Desastres: Facilita a automação e o teste de processos de failover, preparando a infraestrutura para mitigar impactos antes que ocorra um incidente real.
- Ciclo de Vida de Sistemas Legados: Estende a sobrevida de aplicações e sistemas operacionais antigos que não rodam em hardwares modernos, garantindo tempo para uma migração planejada.

🎛️ O Hypervisor e as Arquiteturas de Virtualização   
O hypervisor é o componente de software ou firmware encarregado de criar a camada de abstração sobre os recursos físicos. Ele gerencia e distribui CPU, memória RAM, controladores de disco e interfaces de rede para as Máquinas Virtuais (VMs), permitindo que cada uma opere com um sistema operacional independente.

Essa tecnologia viabiliza cenários de alta densidade, como consolidar a carga de trabalho de 100 servidores tradicionais em apenas 10 servidores físicos robustos. A arquitetura divide-se em dois tipos:
- Hipervisor Tipo 1 (Bare-Metal): Nesta abordagem, o software é instalado diretamente sobre o hardware do servidor, sem nenhum sistema operacional intermediário.
  - Foco: Ambientes corporativos e Data Centers.
  - Diferencial: Por possuir acesso direto aos componentes físicos, entrega o máximo desempenho disponível, maior escalabilidade e robustez.
- Hipervisor Tipo 2 (Hospedado): O software opera como uma aplicação comum, rodando em cima de um sistema operacional base já instalado na máquina (como Windows, Linux ou macOS).
  - Foco: Computadores de desenvolvimento, laboratórios pessoais e estações de trabalho.
  - Diferencial: Dispensa consoles complexos de gerência, mas exige que a máquina hospedeira possua hardware robusto para suportar o consumo de recursos das VMs sem travar o sistema principal.

<a name="item02.04"><h4>2.4 Resumo de Nuvem e Virtualização</h4></a>[Back to summary](#item02)

☁️ Os Pilares da Nuvem   
A computação em nuvem baseia-se na união de infraestruturas robustas de data centers, no fornecimento de recursos sob demanda e na tecnologia de virtualização. Enquanto organizações de grande porte constroem e mantêm suas próprias instalações com alta capacidade de energia e refrigeração, a maioria das empresas opta por terceirizar essas demandas, alugando a capacidade computacional diretamente de provedores especializados.

📦 Modelos de Serviço em Nuvem   
A entrega de soluções na nuvem é estruturada em três categorias principais que definem o nível de controle do usuário. O modelo SaaS fornece aplicações completas e prontas para uso direto no navegador; o PaaS disponibiliza ambientes e ferramentas otimizadas para que desenvolvedores criem seus sistemas; já o IaaS entrega o controle direto de recursos básicos de computação, como redes, armazenamento e servidores virtuais.

🌐 Modelos de Implantação   
A infraestrutura de nuvem pode ser organizada de quatro maneiras distintas para atender a diferentes necessidades de acesso. As nuvens públicas oferecem recursos abertos para qualquer usuário ou empresa na internet, enquanto as nuvens privadas são exclusivas para uma única organização corporativa ou governamental. A abordagem híbrida conecta esses dois mundos em uma estrutura unificada, e a nuvem comunitária atende a um grupo fechado de entidades com interesses e requisitos funcionais regulatórios em comum.

📉 Benefícios Econômicos da Virtualização   
A virtualização funciona como o motor da nuvem ao permitir que um hardware físico atue como múltiplos computadores virtuais simultâneos. Essa consolidação traz vantagens financeiras imediatas para as empresas, pois diminui drasticamente a necessidade de adquirir novos servidores físicos, o que reduz o espaço físico ocupado nos racks, os gastos com manutenção de hardware e o consumo de eletricidade com energia e sistemas de climatização.

🛠️ Vantagens Operacionais e Resiliência   
Além da economia, criar ambientes virtuais otimiza a rotina das equipes de TI. O provisionamento de novos servidores leva minutos em vez de dias, e a criação de laboratórios isolados facilita testes de protótipos de forma segura. A virtualização também melhora a continuidade dos negócios através de ferramentas avançadas de replicação, recuperação rápida de desastres e capacidade de manter sistemas legados antigos funcionando em hardwares modernos.

🎛️ Papel do Hypervisor   
O gerenciamento e a criação das máquinas virtuais são feitos por um componente de software ou hardware chamado hypervisor. Ele atua como uma camada de abstração sobre os componentes físicos do servidor, dividindo recursos como processador, memória RAM e placas de rede entre as diversas instâncias virtuais, garantindo que cada máquina opere com um sistema operacional totalmente independente e isolado dos demais.

🖥️ Hypervisors Tipo 1 (Bare-Metal)   
Os hypervisors do Tipo 1 são projetados para ambientes corporativos de alta performance e data centers. Eles recebem o nome de bare-metal porque são instalados diretamente sobre o hardware físico da máquina, sem a necessidade de um sistema operacional intermediário. Essa arquitetura garante acesso direto aos recursos do servidor, oferecendo máxima eficiência, estabilidade e menor tempo de resposta para as aplicações virtuais.

💻 Hypervisors Tipo 2 (Hospedados)   
O Tipo 2 funciona como um software comum que o usuário instala em cima do seu sistema operacional atual, como rodar um programa de virtualização dentro do Windows ou macOS para testar o Linux. Chamado de hospedado, esse modelo é ideal para computadores pessoais e desenvolvedores por dispensar consoles complexos de gerenciamento e permitir o uso simultâneo do sistema operacional padrão do computador junto com as máquinas virtuais.
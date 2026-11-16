# Networking Devices and Initial Configuration - Módulo 1   <img src="../0-aux/logo_course.png" alt="sfp_008" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">sfp_008 (Networking Devices and Initial Configuration)   <img src="../0-aux/logo_course.png" alt="sfp_008" width="auto" height="25"></a>
### Module: 1. Design de rede

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

### Course Module 1 Structure:
1. <a name="item01">Design de rede</a><br>
  1.1 <a href="#item01.01">Introdução</a><br>
  1.2 <a href="#item01.02">Redes confiáveis</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;1.2.1 <a href="../../../labs/files/lab_055/">Laboratório – Exibição de informações da placa de rede com e sem fio</a><br>
  1.3 <a href="#item01.03">Projeto de rede hierárquica</a><br>
  1.4 <a href="#item01.04">Resumo de Design de Rede</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01.01"><h4>1.1 Introdução</h4></a>[Back to summary](#item01)

🏗️ Arquitetura e Confiabilidade de Projetos de Rede   
A expansão de uma infraestrutura de rede para suportar novos serviços corporativos — como monitoramento por vídeo, telefonia IP e plataformas de comércio eletrônico — exige um planejamento estruturado que supere as limitações de redes planas. Para garantir que o crescimento do negócio ocorra sem interrupções operacionais, o projeto de engenharia de redes deve fundamentar-se em pilares de alta disponibilidade e em modelos arquiteturais que facilitem a gerência e a divisão eficiente do tráfego de dados.

🎯 Objetivo do módulo:   
- Explicar os fundamentos da arquitetura hierárquica e os critérios de qualidade necessários para a concepção de redes corporativas resilientes.

📘 Tópicos do módulo:   
- Redes confiáveis: Análise dos quatro pilares fundamentais para a estabilidade de sistemas: tolerância a falhas, escalabilidade, qualidade de serviço (QoS) e segurança.
- Projeto de rede hierárquica: Estudo das funções, características e atribuições técnicas das camadas de Acesso, Distribuição e Núcleo (Core) no modelo estruturado de três camadas.

<a name="item01.02"><h4>1.2 Redes confiáveis</h4></a>[Back to summary](#item01)

🏢 Fundamentos da Arquitetura e Confiabilidade de Rede   
A infraestrutura de comunicação evoluiu de sistemas exclusivos para dados para plataformas convergentes, capazes de integrar voz, vídeo e informações em tempo real. A eficiência e a expansão desse ecossistema dependem de uma arquitetura de rede padronizada, composta por hardware físico, softwares de gerenciamento e protocolos que regulam o fluxo de tráfego. Para atender às expectativas operacionais e garantir a continuidade dos serviços, o desenvolvimento de redes modernas baseia-se em quatro pilares fundamentais.

🛡️ 1. Tolerância a Falhas e Redundância   
Uma infraestrutura tolerante a falhas é projetada para mitigar o impacto de interrupções, isolando incidentes e assegurando o restabelecimento imediato dos serviços. Esse princípio baseia-se na redundância, ou seja, na disponibilização de caminhos alternativos entre a origem e o destino.

A comutação de pacotes desempenha um papel crucial nessa dinâmica:
- Fragmentação: As mensagens são divididas em unidades menores chamadas pacotes, contendo dados de endereçamento de origem e destino.
- Roteamento Dinâmico: Os roteadores encaminham os pacotes de forma independente, selecionando trajetórias com base nas condições instantâneas da rede. Caso um link falhe, o tráfego é desviado automaticamente sem interrupção perceptível para as aplicações finais.

📈 2. Escalabilidade   
A escalabilidade define a capacidade de uma rede de crescer e absorver novos dispositivos, usuários e aplicações de forma rápida. O objetivo central é realizar essa expansão sem que ocorra a degradação do desempenho dos serviços já usufruídos pela estrutura existente. Essa expansão fluida é viabilizada pela aderência estrita a padrões universais e protocolos abertos. Essa conformidade regulatória permite que diferentes fabricantes desenvolvam soluções de hardware e software interoperáveis, facilitando a acoplagem de novas sub-redes sem a necessidade de reconfiguração das regras globais de operação.

🚦 3. Qualidade de Serviço (QoS)   
A convergência de mídias distintas em um mesmo canal físico exige mecanismos de controle para evitar gargalos operacionais. O congestionamento surge sempre que a demanda por largura de banda — mensurada em bits por segundo (bps) — supera a capacidade máxima de vazão do link de comunicação.

Quando o limite de transmissão é atingido, os ativos de rede retêm os pacotes excedentes em buffers de memória. A implementação de políticas de QoS atua no gerenciamento dessas filas, priorizando o tráfego sensível ao tempo (como chamadas de voz e transmissões de vídeo ao vivo) em detrimento de dados tolerantes a atrasos (como navegação web e e-mails). O critério de diferenciação baseia-se estritamente na categoria do tráfego, e não no teor da informação.

🔒 4. Segurança da Infraestrutura e da Informação   
A proteção de ativos de rede abrange duas esferas essenciais de controle: a integridade física e lógica dos equipamentos de conectividade (segurança da infraestrutura) e a salvaguarda dos dados armazenados ou em trânsito (segurança da informação).

A governança de segurança orienta-se por três requisitos mandatórios:
- Confidencialidade: Garantia de que o acesso e a leitura dos dados sejam restritos exclusivamente aos destinatários autorizados.
- Integridade: Assegura que as informações permaneçam exatamente iguais às originais durante todo o trajeto de transmissão.
- Disponibilidade: Certifica o acesso tempestivo, confiável e contínuo aos recursos e serviços por parte dos usuários validados.

<a name="item01.03"><h4>1.3 Projeto de rede hierárquica</h4></a>[Back to summary](#item01)

🗺️ Endereçamento Hierárquico e a Estrutura de Design de Rede   
Para que a comunicação global ocorra de forma organizada, os sistemas de rede utilizam uma estratégia de endereçamento duplo, dividida entre identificação permanente e localização variável. Essa lógica é o pilar que sustenta a escalabilidade da internet.

🆔 Identidade Física vs. Localização Lógica    
A comunicação entre dispositivos exige dois tipos de informações, comparáveis aos dados de correspondência do mundo real:
- Endereço MAC (Físico): Funciona como o nome de uma pessoa. Ele é gravado diretamente na placa de rede (NIC) durante a fabricação e nunca se altera, independentemente do local onde o dispositivo seja conectado. Contudo, o MAC revela quem o dispositivo é, mas não onde ele está na topologia global.
- Endereço IP (Lógico): Assemelha-se ao endereço residencial. Ele é mutável e atribuído dinamicamente (ou manualmente por um administrador) com base na rede em que o host se encontra no momento.

🧬 A Anatomia do Endereço IP   
Cada endereço IP é subdividido em duas partes essenciais que viabilizam o roteamento:
- Porção de Rede: Identifica o segmento local compartilhado. Todos os dispositivos conectados à mesma rede local possuem exatamente a mesma porção de rede em seus IPs.
- Porção de Host: Garante a exclusividade. Identifica individualmente aquela máquina específica dentro daquele segmento de rede.

🌪️ O Perigo das Redes Planas (Flat Networks)   
Caso a infraestrutura global dependesse exclusivamente dos endereços MAC para encaminhar dados, a internet se tornaria inviável. Localizar um único dispositivo entre bilhões exigiria tabelas de mapeamento infinitas.

Além disso, a tecnologia Ethernet baseia-se fortemente em transmissões de difusão (broadcast) para aproximar dispositivos. Se o mundo inteiro fizesse parte de uma única rede plana, o volume de tráfego de broadcast consumiria instantaneamente toda a largura de banda disponível, gerando o colapso do desempenho através de tempestades de difusão. A solução para esse impasse é a fragmentação em sub-redes menores gerenciadas por um design hierárquico.

🏢 O Modelo Hierárquico de Três Camadas   
A Cisco adota um modelo estrutural para organizar o tráfego IP, dividindo as responsabilidades de hardware em três camadas distintas: acesso, distribuição e núcleo.
- 1 - Camada de Acesso (Access Layer): Representa a fronteira final da rede, onde os dispositivos dos usuários (PCs, laptops, impressoras e pontos de acesso) realizam a conexão inicial. Através de switches de Camada 2, ela agrupa os hosts locais. Se a porção de rede do IP de destino aponta para um vizinho local, o switch resolve a entrega internamente. Caso o destino seja externo, o tráfego é despachado para a próxima camada.
- 2 - Camada de Distribuição (Distribution Layer): Funciona como a fronteira de controle e interconexão de sub-redes. Composta por roteadores e switches multicamadas (Layer 3), esta camada avalia os pacotes vindos do acesso, aplicando políticas de segurança, filtragem de tráfego e regras de roteamento. Ela determina como e se os dados podem transitar entre diferentes departamentos ou sub-redes antes de enviá-los ao núcleo.
- 3 - Camada de Núcleo (Core Layer): É o backbone (espinha dorsal) de alta velocidade da infraestrutura. Sua única e exclusiva função é comutar e transportar volumes massivos de dados entre as diferentes redes de distribuição da forma mais rápida possível. Por ser focada em velocidade máxima e alta disponibilidade, ela conta com links redundantes e evita o processamento pesado de pacotes (como filtragens complexas ou inspeções de segurança), que devem ser tratados estritamente na distribuição.

<a name="item01.04"><h4>1.4 Resumo de Design de Rede</h4></a>[Back to summary](#item01)

📐 Pilares do Projeto de Rede   
O planejamento de infraestruturas modernas baseia-se em quatro qualidades fundamentais para satisfazer as necessidades dos usuários. Os engenheiros devem projetar sistemas que resistam a panes, cresçam de forma organizada, gerenciem a prioridade de serviços essenciais e protejam os ativos contra acessos não autorizados ou corrupção de dados.

🛡️ Resiliência e Tolerância a Falhas   
Uma rede resiliente é estruturada para minimizar o impacto de quebras de hardware ou rompimentos de cabos. Utilizando rotas redundantes entre os pontos, o sistema consegue desviar o tráfego de maneira imediata por um caminho alternativo caso o link principal apresente problemas, garantindo a continuidade do serviço sem que o usuário final perceba a falha.

📈 Capacidade de Escalabilidade   
A escalabilidade permite que a rede cresça e receba novos dispositivos ou sistemas sem que haja perda de qualidade para quem já está conectado. Esse desenvolvimento ordenado é viabilizado pelo uso de arquiteturas padronizadas e protocolos universais, que facilitam a expansão modular da infraestrutura conforme a demanda da empresa aumenta.

🚦 Mecanismos de Qualidade de Serviço (QoS)   
Com a unificação de tráfegos distintos como voz, vídeo e dados no mesmo canal, o QoS torna-se vital para evitar gargalos em momentos de alta demanda. Essa tecnologia atua classificando o tráfego por urgência, garantindo que aplicações sensíveis a atrasos, como chamadas telefônicas e transmissões ao vivo, passem na frente de downloads comuns.

🔒 Segurança e a Tríade CIA   
A proteção da rede abrange tanto os equipamentos físicos quanto as informações que trafegam ou estão guardadas neles. Para garantir um ambiente seguro, os administradores baseiam-se em três princípios fundamentais: manter os dados visíveis apenas a pessoas autorizadas, assegurar que as informações não sejam alteradas no caminho e garantir o acesso constante aos recursos.

🧱 Identidade Lógica e Física   
A comunicação depende do uso conjunto de duas identificações: o endereço MAC, que funciona como o nome fixo gravado de fábrica na placa de rede, e o endereço IP, que funciona como a localização geográfica dinâmica. O IP possui uma estrutura dupla que separa a identificação da rua (rede) e do número da casa (host), permitindo o roteamento eficiente de pacotes.

💻 Central de Gerenciamento Local   
Sistemas operacionais de computadores pessoais disponibilizam painéis gráficos para monitorar o status das conexões ativas. Através dessas centrais, o usuário consegue verificar se o acesso ocorre via cabo ou sinal sem fio, checar as propriedades das placas instaladas e alterar parâmetros essenciais de rede para ajustar a comunicação local e externa.

🏗️ Design de Rede Hierárquico   
Trabalhar com milhões de dispositivos exige uma organização em camadas para evitar o caos administrativo e técnico. O modelo hierárquico substitui estruturas planas complexas por divisões de funções bem definidas, segmentando o processamento de pacotes de dados em três níveis distintos para facilitar a gerência, o suporte e a expansão do ambiente.

🔌 Camada de Acesso   
Este nível funciona como a periferia da rede, sendo a porta de entrada onde computadores, smartphones e impressoras se conectam fisicamente através de switches ou pontos de acesso sem fio. Os dispositivos presentes nesta camada geralmente compartilham a mesma faixa lógica de endereçamento e dependem desse ponto para iniciar qualquer comunicação.

🏢 Camada de Distribuição   
Atuando como intermediária, esta camada recebe o tráfego vindo dos switches de acesso e gerencia a comunicação entre as diferentes sub-redes da organização. Ela é composta por roteadores ou switches avançados que filtram pacotes, aplicam políticas de segurança e barram transmissões desnecessárias, organizando o fluxo antes de enviá-lo para o centro da rede.

⚡ Camada de Núcleo (Core)   
O núcleo funciona como a rodovia de alta velocidade da infraestrutura, ligando os grandes blocos da rede corporativa. Equipado com conexões redundantes e hardwares de altíssimo desempenho, seu único objetivo é encaminhar volumes massivos de dados o mais rápido possível, evitando processamentos complexos que possam causar lentidão no backbone.
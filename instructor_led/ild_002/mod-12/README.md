# CyberOps Associate - Módulo 12  <img src="../0-aux/logo_course.png" alt="ild_002" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="../">ild_002 (CyberOps Associate)   <img src="../0-aux/logo_course.png" alt="ild_002" width="auto" height="25"></a>
### Module: 12. Infraestrutura de segurança de rede

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

### Course Module 12 Structure:

12. <a name="item12">Infraestrutura de segurança de rede</a><br>
  12.1 <a href="#item12.01">Introdução</a><br>
  12.2 <a href="#item12.02">Topologia de rede</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;12.2.1 <a href="../../../pkt/pkt_???/">Packet Tracer - Identificar Fluxo</a><br>
  12.3 <a href="#item12.03">Dispositivos de segurança</a><br>
  12.4 <a href="#item12.04">Serviços de segurança</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;12.4.1 <a href="../../../pkt/pkt_???/">Packet Tracer - Demonstração da ACL</a><br>
  12.5 <a href="#item12.05">Resumo da infraestrutura de segurança de rede</a><br>
  12.6 Exame de ponto de verificação: Exame de grupo de segurança de infraestrutura de rede<br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item12.01"><h4>12.1 Introdução</h4></a>[Back to summary](#item12)

🔹 Arquitetura e Dispositivos de Defesa Cibernética   
A proteção de ativos digitais e a continuidade dos serviços exigem um planejamento estratégico da infraestrutura de rede. Este módulo aborda como a disposição lógica e física dos componentes influencia a segurança das transmissões, apresentando os modelos de design recomendados pelo setor para criar ambientes resilientes. São explorados os mecanismos que permitem a conectividade de ponta a ponta, integrando equipamentos especializados e protocolos de monitoramento para garantir que o tráfego de dados ocorra de forma íntegra e eficiente.

🎯 Objetivo Geral:   
- Analisar a aplicação de equipamentos e protocolos voltados ao fortalecimento das defesas em infraestruturas de rede.

✅ Objetivos Específicos:   
- Topologias de rede: Descrever como o design e o arranjo dos componentes impactam o direcionamento e a segurança do tráfego de informações.
- Dispositivos de segurança: Investigar o papel de ferramentas dedicadas, como firewalls e sistemas de detecção, na mitigação de ameaças externas e internas.
- Serviços de segurança: Demonstrar como os processos de monitoramento e controle de acesso contribuem para a manutenção da estabilidade e proteção da rede.

<a name="item12.02"><h4>12.2 Topologia de rede</h4></a>[Back to summary](#item12)

🗺️ Representações e Topologias de Rede   
A visualização da estrutura de uma rede é essencial para arquitetos e administradores, permitindo identificar conexões, localizações e o funcionamento dos componentes. Para isso, utilizam-se diagramas de topologia que padronizam a representação de dispositivos através de símbolos técnicos.
- Dispositivos Finais: São os pontos de origem ou destino dos dados, como computadores, impressoras, telefones IP e tablets.
- Dispositivos Intermediários: Responsáveis por conectar os dispositivos finais e garantir o fluxo de dados entre redes, incluindo roteadores, switches e firewalls.
- Meios de Rede: Representam as conexões físicas ou sem fio, como cabos de rede (LAN), links de longa distância (WAN) ou sinais de rádio.

🏗️ Componentes de Conexão e Terminologia   
A interação entre os dispositivos e os meios de rede ocorre através de elementos específicos:
- Placa de Interface de Rede (NIC): Componente que realiza a conexão física entre o dispositivo final e o meio.
- Porta Física: O ponto de encaixe ou conector no hardware para o cabo de rede.
- Interface: Termo técnico para portas em dispositivos de rede, como roteadores, que interconectam diferentes redes.

📐 Tipos de Diagramas de Topologia   
A documentação visual de uma rede é classificada em duas categorias principais:
- Topologia Física: Detalha a localização geográfica real dos equipamentos, identificando salas, racks e o caminho percorrido pelos cabos.
- Topologia Lógica: Foca no fluxo de dados, identificando portas, esquemas de endereçamento IP e como os dispositivos se comunicam logicamente, independentemente da sua posição física.

🌐 Escopo e Dimensões das Redes   
As redes são dimensionadas de acordo com a área que atendem e o volume de usuários:
- Redes Domésticas e SOHO: Estruturas simples para compartilhamento local de recursos ou acesso remoto ao trabalho (Small Office/Home Office).
- LAN (Rede Local): Atende áreas geográficas limitadas (casas, escolas ou prédios), oferecendo alta velocidade sob administração única.
- WAN (Rede de Longa Distância): Interconecta LANs em grandes distâncias (cidades, países), geralmente gerenciada por provedores de serviços.
- Internet: A maior infraestrutura existente, definida como uma "rede de redes" pública e global.

🏛️ Design Hierárquico de Redes LAN   
Para aumentar a eficiência e a escalabilidade, as redes corporativas utilizam um modelo modular de camadas:
- Camada de Acesso: Ponto de entrada dos usuários e dispositivos finais na rede.
- Camada de Distribuição: Agrega o tráfego da camada de acesso e gerencia a conectividade aos serviços.
- Camada de Núcleo (Core): Responsável pelo transporte rápido de grandes volumes de tráfego entre os diversos setores da rede.

🛡️ Estratégias de Design com Firewalls   
A segurança perimetral é estruturada através da segmentação de tráfego baseada na confiabilidade das interfaces:
- Privado vs. Público: Separa a rede interna confiável da rede externa (Internet) não confiável, bloqueando acessos não originados internamente.
- Zona Desmilitarizada (DMZ): Área isolada que hospeda servidores públicos (como e-mail e web), permitindo o acesso controlado da Internet sem expor a rede privada interna.
- Firewall Baseado em Zonas (ZPF): Agrupa interfaces com funções similares em "zonas". O tráfego flui livremente dentro da mesma zona, mas é bloqueado entre zonas diferentes, a menos que existam regras explícitas.
- Zona Própria (Self Zone): Refere-se ao tráfego destinado ao próprio roteador (gerenciamento e protocolos), exigindo políticas específicas de proteção.

<a name="item12.03"><h4>12.3 Dispositivos de segurança</h4></a>[Back to summary](#item12)

🛡️ Definição e Função do Firewall   
Um firewall constitui um sistema ou conjunto de sistemas encarregado de implementar políticas de controle de acesso entre diferentes perímetros de rede. Ele atua como um filtro crítico para garantir a integridade da comunicação.

Suas propriedades fundamentais incluem:
- Resistência a Ataques: O sistema é projetado para suportar tentativas de invasão direta.
- Ponto Único de Trânsito: Toda a comunicação entre a rede interna e externa deve obrigatoriamente atravessar o firewall.
- Execução de Políticas: Atua como o executor das regras de permissão ou bloqueio de tráfego definidas pela organização.

🌟 Vantagens e Pontos de Atenção   
A implementação dessa tecnologia oferece benefícios claros, mas também apresenta desafios operacionais:

Benefícios:
- Proteção de Ativos: Blinda servidores e aplicações contra acessos de usuários não autorizados.
- Saneamento de Protocolos: Analisa o fluxo de dados para evitar que vulnerabilidades em protocolos sejam exploradas.
- Controle Centralizado: Simplifica a gestão de segurança ao concentrar o controle de acesso em pontos estratégicos da rede.

Limitações:
- Ponto Único de Falha: Erros de configuração podem interromper totalmente o serviço ou expor a rede a riscos severos.
- Impacto no Desempenho: A inspeção profunda de pacotes pode causar latência e reduzir a velocidade da rede.
- Evasão: Usuários ou softwares maliciosos podem tentar ocultar tráfego proibido dentro de pacotes aparentemente legítimos (túneis).

🔍 Tipos de Firewalls e Tecnologias   
Existem diversas abordagens para a filtragem de tráfego, variando em complexidade e nível de inspeção:
- Filtragem de Pacotes (Stateless): Atua nas camadas 3 e 4 do modelo OSI. Toma decisões simples baseadas em endereços IP e portas, sem considerar o contexto ou o histórico da conexão.
- Monitoração de Estado (Stateful): É a tecnologia mais difundida. Mantém uma tabela de estado para acompanhar conexões ativas, analisando o tráfego nas camadas de rede, transporte e sessão para validar se o pacote faz parte de uma comunicação legítima.
- Gateway de Aplicação (Proxy): Opera até a camada de aplicação (Camada 7). Age como um intermediário: o cliente conecta-se ao proxy, que por sua vez solicita o dado ao servidor, ocultando a identidade da rede interna.
- Próxima Geração (NGFW): Evolução dos modelos anteriores que integra prevenção de intrusão (IPS), controle avançado de aplicações e inteligência contra ameaças modernas e dinâmicas.

🔧 Outros Modelos de Implementação   
- Baseado em Host: Software instalado diretamente em servidores ou computadores pessoais para proteção individual.
- Transparente: Filtra o tráfego IP entre interfaces que operam em ponte (Layer 2), sem exigir reconfiguração de endereçamento na rede.
- Híbrido: Combina diferentes métodos, como a inspeção de estado aliada a gateways de aplicação, para uma proteção mais profunda.

🛡️ Defesa Ativa: IDS e IPS   
Para enfrentar ameaças cibernéticas que evoluem rapidamente, a arquitetura de rede exige sistemas de monitoramento proativos. O Sistema de Detecção de Intrusão (IDS) e o Sistema de Prevenção de Intrusão (IPS) são sensores estratégicos posicionados nos pontos de entrada e saída da rede para identificar e mitigar ataques.

Ambas as tecnologias compartilham características essenciais:
- Uso de Assinaturas: Regras que identificam padrões maliciosos conhecidos.
- Detecção de Padrões: Podem analisar desde um único pacote isolado (atômico) até sequências complexas de múltiplos pacotes (composto).

🔄 Funcionamento e Fluxo de Resposta   
Quando um tráfego malicioso tenta alcançar um host interno, o processo segue esta lógica em um sistema preventivo:
- O tráfego é roteado pela infraestrutura até encontrar o sensor.
- O dispositivo identifica a ameaça e bloqueia a passagem dos dados.
- As informações sobre o evento são enviadas para um console de gerenciamento.
- O tráfego é descartado permanentemente (processo conhecido como "Bit Bucket").

⚖️ Comparativo: IDS vs. IPS   
A escolha entre um sistema de detecção ou prevenção depende do equilíbrio entre segurança e desempenho da rede.
- IDS (Modo Offline):
  - Vantagens: Não gera latência ou falhas no fluxo de dados, pois analisa uma cópia do tráfego. Se o sensor falhar, a rede continua operando normalmente.
  - Desvantagens: É reativo. Ele não consegue impedir o primeiro pacote do ataque e é mais suscetível a técnicas de evasão.
- IPS (Modo Inline): 
  - Vantagens: Atua diretamente no caminho dos dados, permitindo interromper ameaças em tempo real e normalizar fluxos fragmentados.
  - Desvantagens: Pode introduzir latência e jitter. Caso o sensor fique sobrecarregado ou falhe, o tráfego da rede pode ser interrompido.

🖥️ Implementações: Host e Rede   
Os sistemas de segurança podem ser instalados de forma localizada ou abrangente:
- IPS Baseado em Host (HIPS): Software instalado diretamente no dispositivo final. Protege o sistema operacional e processos críticos contra alterações não autorizadas ou estouros de buffer. Atua mesmo após a descriptografia dos dados, mas exige instalação e manutenção individual em cada máquina.
- IPS Baseado em Rede: Dispositivos dedicados (ou módulos em roteadores/firewalls) que protegem todo o segmento de rede, oferecendo uma visão global dos eventos.

🛠️ Soluções Especializadas Cisco   
Além dos sistemas padrão, existem dispositivos focados em vetores de ataque específicos:
- Cisco AMP: Focado em malware avançado. Monitora arquivos antes, durante e após um ataque, utilizando inteligência global para detectar comportamentos suspeitos mesmo em arquivos previamente considerados seguros.
- Cisco WSA/CWS: Gateways de segurança web que bloqueiam sites arriscados e controlam o uso de aplicações na internet, protegendo usuários locais e remotos.
- Cisco ESA: Especializado em segurança de e-mail. Combina filtros de reputação e análise profunda para bloquear spam e mitigar ameaças enviadas por mensagens, garantindo a conformidade das comunicações externas.

<a name="item12.04"><h4>12.4 Serviços de segurança</h4></a>[Back to summary](#item12)

🛡️ Listas de Controle de Acesso (ACL)   
As ACLs funcionam como filtros inteligentes nos roteadores, determinando o destino dos pacotes (encaminhamento ou descarte) com base na análise de seus cabeçalhos. Elas são fundamentais para manter a saúde e a segurança da rede.

Principais Funções das ACLs:
- Otimização de Desempenho: Limitam o tráfego desnecessário (como bloqueio de streaming em rede corporativa), liberando largura de banda.
- Gestão de Fluxo: Controlam a propagação de atualizações de roteamento para fontes confiáveis.
- Segurança de Acesso: Segmentam a rede, permitindo que apenas usuários autorizados acessem departamentos sensíveis, como o RH.
- Filtragem por Serviço: Diferenciam o tráfego por protocolo, permitindo, por exemplo, o uso de e-mail enquanto bloqueiam o acesso via Telnet.
- Priorização (Classificação): Funcionam como um "ingresso VIP", identificando tráfego prioritário para processamento imediato em políticas de QoS.

🚦 Tipos de ACLs Cisco   
Existem duas categorias principais para o protocolo IPv4, diferenciadas pela profundidade da inspeção:
- ACL Padrão: Avalia apenas o endereço IPv4 de origem. É mais simples, mas não consegue distinguir o destino ou o tipo de serviço (porta).
- ACL Estendida: Oferece controle granular, filtrando por endereço de origem e destino, tipo de protocolo (IP, TCP, UDP, ICMP) e números de porta (origem e destino).

Ambas podem ser identificadas por números (ideal para redes pequenas) ou nomes (que facilitam a compreensão do propósito da lista). Além disso, podem ser configuradas para registrar eventos (logs) ou permitir apenas conexões TCP já estabelecidas (verificando bits ACK ou RST), impedindo que sessões externas iniciem comunicações não solicitadas.

📊 Monitoramento e Gerenciamento: SNMP   
O SNMP (Simple Network Management Protocol) é a ferramenta padrão para gerenciar o inventário e o desempenho dos dispositivos da rede.
- Estrutura do Sistema: Composta pelo Gerente SNMP (software central de controle) e pelos Agentes SNMP (dispositivos monitorados).
- Base de Dados (MIB): Cada agente possui uma MIB, que armazena estatísticas operacionais do hardware.

Ações Principais:
- Get: O gerente solicita informações do agente.
- Set: O gerente altera configurações no agente.
- Trap: O agente envia alertas automáticos e imediatos ao gerente caso ocorra um evento crítico.

📈 Análise de Fluxo com NetFlow   
Enquanto o SNMP foca na saúde do dispositivo, o NetFlow foca nas estatísticas dos pacotes. Ele monitora fluxos individuais de dados e envia os relatórios para um coletor externo.

Identificação de um Fluxo (Os 7 Campos):
- Para o NetFlow, um fluxo é único se houver variação em:
  - Endereço IP de origem.
  - Endereço IP de destino.
  - Porta de origem.
  - Porta de destino.
  - Tipo de protocolo da Camada 3.
  - Marcação de ToS (Type of Service).
  - Interface lógica de entrada.

Essa tecnologia é vital para identificar gargalos, planejar a expansão da rede e realizar faturamento baseado no consumo de dados.

🔍 Captura de Tráfego e Espelhamento de Portas   
Para analisar pacotes detalhadamente, utilizam-se softwares conhecidos como analisadores de pacotes (sniffers). Como os switches modernos isolam o tráfego entre as portas, utiliza-se o Espelhamento de Portas (Port Mirroring). O switch cria uma cópia idêntica de todo o tráfego de uma porta (ou VLAN) e a envia para uma porta específica onde o analisador ou um sensor IDS está conectado. Isso permite a inspeção profunda sem interromper o fluxo original de dados.

📝 Monitoramento e Sincronização de Rede   
Os dispositivos de rede possuem sistemas de alerta para comunicar desde eventos rotineiros até falhas críticas. O gerenciamento eficiente dessas mensagens permite que administradores antecipem problemas e mantenham a infraestrutura estável.

📜 Protocolo Syslog   
O Syslog é o padrão mais utilizado para o envio de registros (logs) de dispositivos como roteadores e firewalls para um servidor centralizado. Ele desempenha três papéis fundamentais:
- Coleta: Reúne dados para análise e resolução de problemas.
- Filtragem: Permite selecionar quais níveis de mensagens serão capturados.
- Destino: Define para onde os registros devem ser encaminhados na rede.

🕒 Network Time Protocol (NTP)   
A sincronização de horário é vital; sem ela, é impossível correlacionar eventos que ocorrem em diferentes partes da rede. O NTP automatiza esse ajuste, utilizando uma hierarquia chamada Stratum:
- Stratum 0: Fontes de tempo de altíssima precisão (relógios atômicos, GPS).
- Stratum 1: Servidores conectados diretamente às fontes de nível 0.
- Stratum 2: Dispositivos que sincronizam com o nível 1 e podem servir o horário para o nível 3, e assim por diante.
- Nota: O valor máximo de saltos é 15; o nível 16 indica que o dispositivo não está sincronizado.

🔐 Estrutura AAA (Autenticação, Autorização e Accounting)   
A arquitetura AAA oferece uma estrutura modular para garantir a segurança no acesso à rede através de três pilares:
- Autenticação: Valida a identidade do usuário (ex: login e senha).
- Autorização: Define o que o usuário pode fazer ou acessar após ser identificado.
- Accounting (Bilhetagem): Registra as atividades, o tempo de acesso e as alterações realizadas, gerando um histórico de uso.

📑 Comparação de Protocolos: TACACS+ vs. RADIUS   
Para a comunicação com servidores AAA, utilizam-se dois protocolos principais:
- TACACS+ (Cisco): Mais seguro, pois criptografa todo o pacote. Separa as funções de autenticação e autorização, permitindo controle detalhado de comandos por usuário. Utiliza o protocolo TCP.
- RADIUS (Padrão Aberto): Criptografa apenas a senha. Combina autenticação e autorização em um único processo e é amplamente utilizado para bilhetagem detalhada. Utiliza o protocolo UDP.

🌐 Redes Virtuais Privadas (VPN)   
Uma VPN estabelece um canal de comunicação seguro e privado sobre uma infraestrutura pública, como a Internet. Ela utiliza tunelamento e criptografia para garantir que os dados permaneçam confidenciais.

Tipos e Tecnologias de VPN:
- GRE (Generic Routing Encapsulation): Um protocolo da Cisco que cria túneis virtuais ponto a ponto, mas que originalmente não possui criptografia própria.
- IPsec (IP Security): Um conjunto de protocolos que fornece autenticação, integridade e confidencialidade. É a base para a maioria das VPNs seguras atuais.

Modelos de Implementação:
- Site-to-Site: Conecta escritórios inteiros (ex: matriz e filial).
- Acesso Remoto: Permite que usuários individuais (trabalhando em casa ou viajando) se conectem com segurança à rede da empresa.

As conexões lógicas de uma VPN podem ocorrer na Camada 2 ou na Camada 3 (como MPLS e IPsec), dependendo das necessidades de conectividade e roteamento da organização.

<a name="item12.05"><h4>12.5 Resumo da infraestrutura de segurança de rede</h4></a>[Back to summary](#item12)

🌐 Variedades de infraestrutura   
As redes de computadores são moldadas conforme a extensão geográfica, o volume de usuários e as funções que desempenham em cada organização. Elas são ilustradas através de mapas que detalham tanto a disposição física dos cabos e aparelhos quanto a organização lógica, que dita como as regras e protocolos orientam o fluxo de informações entre os pontos de conexão.

🏢 Hierarquia de redes   
A organização de ambientes corporativos geralmente segue um modelo de três níveis para garantir eficiência e organização no tráfego de dados. Na base, o nível de acesso conecta os aparelhos dos usuários, enquanto o nível de distribuição concentra esses acessos para gerenciar serviços, e o núcleo central foca na velocidade total para interligar as grandes divisões da infraestrutura.

🛡️ Arquitetura de defesa   
O controle do que entra e sai de uma rede é feito por perímetros de segurança que separam o ambiente privado da internet pública. Em muitos casos, utiliza-se uma zona intermediária para serviços que precisam de visibilidade externa, protegendo os dados críticos de acessos diretos através de grupos de interfaces com exigências de segurança similares.

🔥 Evolução dos firewalls   
As barreiras de segurança evoluíram de simples filtros de pacotes para sistemas inteligentes capazes de inspecionar o estado das conexões e o conteúdo das mensagens em camadas superiores. As versões mais modernas identificam o comportamento de aplicativos específicos e integram inteligência contra ameaças em tempo real para barrar ataques sofisticados antes que eles atinjam o núcleo da rede.

🚨 Vigilância e sistemas   
Sistemas especializados monitoram o tráfego em busca de invasões, podendo apenas alertar sobre perigos ou agir ativamente para barrar conexões suspeitas conforme a configuração. Existem equipamentos dedicados exclusivamente para limpar o tráfego de e-mail e proteger a navegação web, utilizando bancos de dados globais que correlacionam ataques ocorridos em todo o mundo.

📊 Monitoramento de fluxo   
Para manter a ordem, utilizam-se listas de controle que barram ou permitem pacotes conforme critérios predefinidos nos cabeçalhos de cada transmissão. Ferramentas de gerenciamento e coleta de estatísticas permitem que os administradores entendam o volume de dados circulando e identifiquem falhas, enquanto o espelhamento de portas possibilita analisar cópias das informações sem interromper o serviço original.

📋 Serviços de suporte   
A saúde da rede depende de registros centralizados de eventos e da sincronização precisa de horários entre todos os aparelhos para que os diagnósticos sejam confiáveis. Além disso, estruturas de controle de acesso verificam a identidade dos usuários e autorizam suas ações, enquanto as redes privadas virtuais garantem que as informações viajem de forma criptografada através de caminhos públicos.
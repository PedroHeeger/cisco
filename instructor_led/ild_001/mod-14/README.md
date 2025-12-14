# CCNA: Introduction to Networks - Módulo 14   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_001 (CCNA: Introduction to Networks)   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="25"></a>
### Module: 14. Camada de transporte

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

### Course Module 14 Structure:
14. <a name="item14">Camada de transporte</a><br>
  14.1 <a href="#item14.01">Introdução</a><br>
  14.2 <a href="#item14.02">Transporte de Dados</a><br>
  14.3 <a href="#item14.03">Visão geral do TCP</a><br>
  14.4 <a href="#item14.04">Visão geral do UDP</a><br>
  14.5 <a href="#item14.05">Números de porta</a><br>
  14.6 <a href="#item14.06">Processo de Comunicação TCP</a><br>
  14.7 <a href="#item14.07">Confiabilidade e controle de fluxo</a><br>
  14.8 <a href="#item14.08">Comunicação UDP</a><br>
  14.9 <a href="#item14.09">Módulo Prático e Quiz</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;14.9.1 <a href="#item14.09.01">PTTA - Comunicações TCP e UDP</a><br>

---

### Objective:
O objetivo deste módulo foi apresentar os fundamentos da governança em segurança digital, destacando políticas, papéis e responsabilidades na administração de dados. Também foram exploradas as principais leis, regulamentações e normas internacionais aplicáveis à proteção da informação. Além disso, foram abordados os princípios éticos na tomada de decisões em ambientes digitais e introduzidos frameworks e controles essenciais, como ISO 27000, NIST, CIS e CSA, para garantir conformidade, proteção de dados e integridade operacional em organizações.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item14.01"><h4>14.1 Introdução</h4></a>[Back to summary](#item14)

🚚 Camada de Transporte   
A camada de transporte é responsável por movimentar dados entre hosts de forma organizada e funcional. É nela que os protocolos TCP e UDP operam, garantindo que as aplicações possam trocar informações por meio de mecanismos confiáveis ou rápidos, conforme a necessidade. Cada protocolo oferece um conjunto distinto de comportamentos, desde controle de conexão até entrega simples e ágil, permitindo que diferentes tipos de tráfego sejam atendidos adequadamente. Este módulo aprofunda o funcionamento desses protocolos e apresenta recursos visuais para reforçar o entendimento.

🎯 Objetivo do módulo   
Comparar as operações dos protocolos da camada de transporte no suporte da comunicação de ponta a ponta.

📘 Tópicos do módulo   
- Transporte de dados: Apresentar o papel da camada de transporte no envio, recebimento e gerenciamento dos fluxos de dados entre hosts.
- Visão geral do TCP: Explicar características do TCP, incluindo confiabilidade, controle de conexão e mecanismos que garantem entrega ordenada.
- Visão geral do UDP: Descrever as propriedades do UDP, focado em simplicidade, baixo atraso e ausência de confirmação ou controle de sessão.
- Números de porta: Mostrar como TCP e UDP utilizam portas para identificar serviços e permitir que múltiplas aplicações funcionem simultaneamente.
- Processo de comunicação TCP: Explicar como a criação e finalização de uma sessão TCP organizam o envio confiável de dados.
- Confiabilidade e controle de fluxo: Detalhar como o TCP assegura que todos os segmentos sejam entregues e reconhecidos, evitando sobrecarga no receptor.
- Comunicação UDP: Comparar a operação do UDP com a do TCP, destacando situações em que a entrega rápida supera a necessidade de confiabilidade.

<a name="item14.02"><h4>14.2 Transporte de Dados</h4></a>[Back to summary](#item14)

🔗 A Camada de Transporte e a Comunicação Lógica   
A Camada de Transporte atua como um elo vital entre os programas da Camada de Aplicação e as camadas de rede inferiores. Sua responsabilidade é gerenciar a comunicação lógica entre as aplicações que rodam em hosts diferentes. Em outras palavras, ela cuida dos detalhes de como os dados de uma aplicação de origem chegam corretamente à aplicação de destino, o que pode envolver o estabelecimento de uma sessão temporária e a garantia da entrega das informações.

É importante notar que a Camada de Transporte atua de forma independente de fatores de rede, como o tipo de meio físico, o caminho percorrido pelos dados, o congestionamento na rede ou a arquitetura do host de destino.

📋 Responsabilidades Principais da Camada de Transporte   
A Camada de Transporte tem várias funções cruciais para gerenciar a troca de dados entre aplicações:
- Rastreamento de Conversações Individuais: Um host pode executar vários programas simultaneamente, todos se comunicando pela rede. Cada fluxo de dados entre um aplicativo de origem e um aplicativo de destino é tratado como uma conversa separada. A Camada de Transporte é responsável por manter o controle e monitorar essas múltiplas conversas de forma independente.
- Segmentação e Remontagem de Dados: Como existe um limite para a quantidade de dados que pode ser encapsulada em um único pacote de rede, a Camada de Transporte deve dividir os dados do aplicativo em blocos menores e gerenciáveis. Esses blocos são chamados de Segmentos se o TCP for usado. Eles são chamados de Datagramas se o UDP for usado. No host de destino, a camada de transporte é responsável por remontar esses blocos em um fluxo de dados completo para a aplicação receptora.
- Adição de Informações de Cabeçalho: A camada adiciona um cabeçalho contendo dados binários a cada bloco (segmento ou datagrama). Os valores presentes nesses campos do cabeçalho são o que permitem aos protocolos de transporte (TCP/UDP) realizar suas funções, como garantir a ordem e direcionar os dados para a aplicação correta.
- Identificação de Aplicações (Portas): Para garantir que os fluxos de dados sejam entregues à aplicação correta, a Camada de Transporte utiliza um identificador chamado número da porta. Cada processo de software que precisa acessar a rede recebe um número de porta exclusivo para aquele host.
- Multiplexação de Conversas: Enviar um grande volume de dados (como um streaming de vídeo) como um fluxo único e contínuo pode monopolizar toda a largura de banda. A Camada de Transporte utiliza a segmentação e a multiplexação para intercalar os blocos de diferentes conversas na mesma rede simultaneamente, maximizando a eficiência.

🔄 Protocolos de Transporte: TCP vs. UDP   
A arquitetura TCP/IP oferece dois protocolos de transporte para atender a diferentes necessidades de confiabilidade e desempenho das aplicações. É o protocolo da Camada de Transporte, e não o IP, que determina como o transporte da mensagem ocorrerá, e ele é responsável por gerenciar os requisitos de confiabilidade da conversa.

✅ Protocolo TCP (Transmission Control Protocol)   
O TCP é um protocolo confiável e orientado a conexão, o que significa que ele deve primeiro estabelecer uma conexão (handshake) entre o remetente e o receptor antes de transmitir os dados.
- Confiabilidade: O TCP garante que todos os dados cheguem ao destino e na ordem correta, análogo ao envio de pacotes rastreados que exigem confirmação de recebimento.
- Sobrecarga: Os campos adicionais de controle de confiabilidade e fluxo no cabeçalho exigem um processamento extra dos hosts.
- Operações de Confiabilidade: O TCP fornece confiabilidade e controle de fluxo por meio de um conjunto de operações:
  - Numerar e rastrear os segmentos de dados.
  - Confirmar os dados recebidos (ACK).
  - Retransmitir os dados não confirmados após um timeout.
  - Reordenar os dados que possam ter chegado fora de sequência.
  - Gerenciar o fluxo de dados para que o remetente não sobrecarregue o receptor.
- Exemplos de Uso: É ideal para aplicações onde a perda de dados é inaceitável, como navegadores web (HTTP/HTTPS), clientes de e-mail (SMTP/IMAP) e aplicações de banco de dados.

⏩ Protocolo UDP (User Datagram Protocol)   
O UDP é um protocolo simplificado, sem conexão e sem estado, focado em velocidade e baixa sobrecarga. Ele é conhecido como um protocolo de "melhor esforço", pois envia os dados sem exigir confirmação de recebimento ou garantia de entrega. Suas principais características e aplicações incluem:
- Velocidade e Leveza: Por não realizar handshake, retransmissão ou sequenciamento complexo, o cabeçalho UDP é pequeno e o processamento é muito rápido.
- Tolerância a Perdas: O UDP "dispara e esquece". Se um pacote se perder, ele não é reenviado, o que evita atrasos causados pela espera de retransmissões.
- Aplicações Típicas: É a escolha ideal para aplicações sensíveis a atrasos (delay) onde uma pequena perda de dados é preferível a uma pausa na transmissão. Exemplos incluem VoIP (Telefonia IP), Streaming em Tempo Real e serviços de consulta rápida como DNS.

<a name="item14.03"><h4>14.3 Visão geral do TCP</h4></a>[Back to summary](#item14)









<a name="item14.04"><h4>14.4 Visão geral do UDP</h4></a>[Back to summary](#item14)








<a name="item14.05"><h4>14.5 Números de porta</h4></a>[Back to summary](#item14)









<a name="item14.06"><h4>14.6 Processo de Comunicação TCP</h4></a>[Back to summary](#item14)









<a name="item14.07"><h4>14.7 Confiabilidade e controle de fluxo</h4></a>[Back to summary](#item14)











<a name="item14.08"><h4>14.8 Comunicação UDP</h4></a>[Back to summary](#item14)










<a name="item14.09"><h4>14.9 Módulo Prático e Quiz</h4></a>[Back to summary](#item14)

🚚 Função da Camada de Transporte   
A camada de transporte conecta os aplicativos às partes responsáveis pela transmissão na rede, garantindo comunicação lógica entre hosts. Ela utiliza TCP e UDP para mover dados, definir requisitos de confiabilidade, segmentar informações, remontar tudo no destino, adicionar cabeçalhos, identificar aplicativos e permitir múltiplas conversas simultâneas.

🔐 Características do TCP e UDP   
O TCP mantém estado, confirma recebimento, retransmite perdas e entrega dados na ordem correta, sendo comum em e-mail e navegação web. O UDP trabalha sem estado, é mais ágil, não confirma recebimento, não reenviará perdas e entrega conforme os dados chegam, sendo usado em VoIP e DNS.

📦 Estrutura do TCP   
O TCP cria sessões confiáveis, controla fluxo e preserva a ordem da entrega. Cada segmento inclui cerca de 20 bytes extras no cabeçalho, contendo portas, números de sequência e reconhecimento, tamanho de janela e outros campos. Aplicações como HTTP, FTP, SMTP e Telnet dependem desse protocolo.

📨 Estrutura do UDP   
O UDP não estabelece sessões e não verifica recursos do destino. Seus datagramas incluem portas de origem e destino, tamanho e soma de verificação. Como não reenvia perdas nem controla ordem, é ideal para serviços como DHCP, DNS, SNMP, TFTP, VoIP e videoconferência.

🔢 Portas e Sockets   
TCP e UDP utilizam números de porta para organizar múltiplas conversas ao mesmo tempo. As portas são gravadas nos segmentos e, junto aos endereços IP de origem e destino, formam um socket, que identifica claramente o serviço solicitado. As portas variam de 0 a 65535 e se dividem em faixas específicas, com algumas reservadas para protocolos amplamente usados. O utilitário netstat permite visualizar conexões ativas.

🖥️ Processos e Conexões TCP   
Cada aplicação recebe uma porta automaticamente ou configurada manualmente. Clientes e servidores trocam solicitações usando portas de origem e destino. Para encerrar uma sessão TCP, quatro trocas finalizam a conexão. O estabelecimento ocorre com o handshake de três vias, que confirma a presença do destino, a disponibilidade do serviço e a intenção de iniciar comunicação. Os bits de controle usados nesse processo são URG, ACK, PSH, RST, SYN e FIN.

📊 Sequência, Perdas e SACK   
Para que a mensagem final faça sentido, todos os segmentos devem chegar e ser remontados conforme a ordem original. Cada pacote recebe um número de sequência para permitir essa organização. Quando ocorre perda, o TCP oferece mecanismos de retransmissão. O recurso SACK, negociado durante a conexão, permite reconhecer exatamente quais partes chegaram, facilitando o reenvio apenas do que faltou.

🌊 Controle de Fluxo e Congestionamento   
A confiabilidade do TCP também depende do ajuste da taxa de envio entre origem e destino, controlado pelo tamanho da janela declarado no cabeçalho. O processo de envio e reconhecimento contínuo forma as chamadas janelas deslizantes. O MSS, normalmente de 1460 bytes, indica o tamanho máximo de dados por segmento. Para lidar com congestionamento, o TCP reduz a quantidade de bytes pendentes de confirmação para manter a entrega eficiente.

📡 Funcionamento do UDP em Trânsito   
O UDP envia datagramas que podem seguir caminhos distintos e chegar fora de ordem. Ele não usa números de sequência para reorganizar dados; apenas repassa ao aplicativo na ordem em que chegam. Se a sequência for importante, o próprio aplicativo deve tratá-la. Servidores que usam UDP escutam portas bem conhecidas, enquanto clientes escolhem portas de origem de forma dinâmica e mantêm o mesmo par de portas durante toda a comunicação. Quando o servidor responde, as portas se invertem no cabeçalho.
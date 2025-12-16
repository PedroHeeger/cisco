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

🛡️ Recursos e Funcionalidades do TCP   
A compreensão das diferenças entre TCP e UDP fundamenta-se na análise de como cada protocolo implementa a confiabilidade e o rastreamento de conversas. Além de executar as funções básicas de segmentação e remontagem de dados, o TCP oferece serviços específicos que garantem a integridade da comunicação. Os principais recursos fornecidos pelo TCP incluem:
- Estabelecimento de Sessão: O TCP é um protocolo orientado à conexão. Antes do encaminhamento de qualquer tráfego, uma conexão (ou sessão) permanente é negociada e estabelecida entre os dispositivos de origem e destino, permitindo o gerenciamento atento da comunicação.
- Garantia de Entrega Confiável: Durante a transmissão pela rede, segmentos podem ser corrompidos ou perdidos. O TCP assegura que cada segmento enviado pela fonte seja efetivamente recebido no destino.
- Entrega Ordenada: Como as redes podem utilizar rotas distintas com taxas de transmissão variadas, os dados podem chegar fora de ordem. O TCP numera e sequencia os segmentos, garantindo que sejam remontados na ordem exata em que foram enviados.
- Suporte ao Controle de Fluxo: Dispositivos de rede possuem recursos limitados de memória e processamento. O TCP pode solicitar que a aplicação emissora reduza a taxa de fluxo de dados ao perceber sobrecarga no receptor, evitando a perda de dados e a necessidade de retransmissão.

💾 Protocolo com Estado (Stateful)   
O TCP é classificado como um protocolo stateful (com estado), pois mantém o controle do estado da sessão de comunicação. Para isso, o protocolo registra quais informações foram enviadas e quais foram confirmadas. Uma sessão com estado possui um ciclo de vida definido: inicia-se com o estabelecimento da conexão, mantém-se durante a transferência e encerra-se ao final da comunicação.

📦 Estrutura do Cabeçalho TCP   
O segmento TCP adiciona uma sobrecarga de 20 bytes (160 bits) ao encapsular os dados da camada de aplicação. O cabeçalho é composto por dez campos principais, descritos a seguir:
- Porta de Origem (16 bits): Identifica o aplicativo de origem por meio do número da porta.
- Porta de Destino (16 bits): Identifica o aplicativo de destino por meio do número da porta.
- Número de Sequência (32 bits): Utilizado para fins de reordenação e remontagem dos dados.
- Número de Confirmação (32 bits): Indica que os dados foram recebidos e aponta qual é o próximo byte esperado da fonte.
- Comprimento do Cabeçalho (4 bits): Conhecido como "offset de dados", indica o tamanho total do cabeçalho do segmento TCP.
- Reservado (6 bits): Campo reservado para uso futuro.
- Bits de Controle (6 bits): Inclui códigos de bits (flags) que indicam a finalidade e a função do segmento.
- Tamanho da Janela (16 bits): Indica o número de bytes que podem ser aceitos de uma só vez pelo receptor.
- Checksum (16 bits): Utilizado para a verificação de erros tanto do cabeçalho quanto dos dados do segmento.
- Urgente (16 bits): Sinaliza se os dados contidos no segmento possuem prioridade.

🤝 Independência das Aplicações   
O TCP exemplifica a divisão de tarefas no conjunto de protocolos TCP/IP. Ele assume todas as responsabilidades associadas à divisão do fluxo de dados, garantia de confiabilidade, controle de fluxo e reordenação. Isso libera a camada de aplicação da necessidade de gerenciar tais tarefas complexas. Aplicações como FTP, HTTP, SMTP e SSH simplesmente enviam o fluxo de dados à camada de transporte e utilizam os serviços do TCP.

<a name="item14.04"><h4>14.4 Visão geral do UDP</h4></a>[Back to summary](#item14)

⚡ Características Fundamentais do UDP   
O User Datagram Protocol (UDP) opera sob o conceito de "melhor esforço" (best-effort). Diferentemente do TCP, que prioriza a garantia de entrega, o UDP foca na leveza e na velocidade de transmissão. Embora realize as funções básicas da camada de transporte, como a segmentação e a remontagem de dados, ele dispensa mecanismos complexos de controle de fluxo e verificação de confiabilidade. Por ser um protocolo sem estado (stateless), nem o cliente nem o servidor mantêm registros sobre a sessão de comunicação. Isso significa que a responsabilidade por garantir a integridade dos dados — caso seja necessária — é transferida inteiramente para a aplicação, e não gerida pelo protocolo de transporte.

🚫 Modo de Operação e Limitações   
O funcionamento do UDP é frequentemente definido pela ausência dos recursos restritivos encontrados no TCP, o que resulta em um processamento mais ágil. As principais características operacionais incluem:
- Ausência de Sessão: Não há o processo de estabelecimento de conexão (handshake) antes do envio dos dados.
- Entrega Não Ordenada: Os dados são reagrupados e processados na exata ordem em que chegam. Se chegarem fora de sequência, não há reordenação automática.
- Sem Retransmissão: Segmentos perdidos ou corrompidos durante o trajeto não são reenviados pelo protocolo.
- Envio Contínuo: O remetente não verifica se o destinatário está disponível ou sobrecarregado; os dados são enviados continuamente.

📦 Estrutura Simplificada do Cabeçalho   
A eficiência do UDP reflete-se na simplicidade do seu cabeçalho. Enquanto o TCP possui um cabeçalho extenso e complexo, o UDP utiliza apenas 8 bytes (64 bits) de sobrecarga para empacotar os dados da aplicação. Os blocos de comunicação aqui são denominados datagramas. O cabeçalho é composto por apenas quatro campos:
- Porta de Origem (16 bits): Identifica a aplicação remetente.
- Porta de Destino (16 bits): Identifica a aplicação destinatária.
- Comprimento (16 bits): Define o tamanho total do datagrama (cabeçalho + dados).
- Checksum (16 bits): Realiza uma verificação básica de integridade do cabeçalho e dos dados.

🎬 Cenários de Uso Ideais   
A escolha do UDP é estratégica para situações onde a velocidade é crítica e pequenas perdas de dados são aceitáveis. Existem três categorias principais de aplicações que se beneficiam deste protocolo:
- Multimídia em Tempo Real: Aplicações de voz e vídeo, como VoIP e transmissões ao vivo, priorizam o fluxo contínuo. Uma pausa para retransmitir um pacote perdido causaria travamentos perceptíveis, o que é pior do que uma pequena falha visual ou de áudio momentânea.
- Transações Simples (Solicitação/Resposta): Protocolos que envolvem trocas rápidas de pequenas quantidades de informação, onde o host envia uma pergunta e espera uma resposta imediata. Exemplos clássicos são o DNS e o DHCP.
- Confiabilidade Gerida pela Aplicação: Situações em que a própria aplicação possui mecanismos para lidar com erros ou onde a comunicação é unidirecional e não exige confirmação. Exemplos incluem SNMP e TFTP.

🔀 Flexibilidade e Exceções   
Embora certos protocolos como DNS e SNMP utilizem UDP por padrão devido à eficiência, essa não é uma regra absoluta. O DNS, por exemplo, alternará para o uso de TCP caso a resposta da consulta exceda 512 bytes (comum em resoluções complexas ou com segurança DNSSEC). Da mesma forma, administradores de rede podem configurar o SNMP para operar sobre TCP quando a confiabilidade da gestão da rede for prioritária sobre a velocidade.

<a name="item14.05"><h4>14.5 Números de porta</h4></a>[Back to summary](#item14)

🔢 Números de Porta e Gerenciamento de Conversas   
Independentemente de se utilizar TCP ou UDP, ambos os protocolos da camada de transporte dependem de números de porta para gerenciar múltiplas conversas simultâneas. Nos cabeçalhos de ambos os protocolos, existem campos específicos que identificam a Porta de Origem e a Porta de Destino.

A função desses números é distinta para cada extremidade da comunicação:
- Porta de Origem: Está associada à aplicação no host local (o remetente). Geralmente, é gerada dinamicamente pelo dispositivo para identificar aquela conversa específica de forma exclusiva. Cada nova solicitação (como abrir uma nova aba no navegador) recebe um número de porta de origem diferente, permitindo que várias conexões ocorram ao mesmo tempo sem conflito.
- Porta de Destino: Identifica o serviço específico que está sendo requisitado no servidor remoto. Por exemplo, ao solicitar uma página web, o número 80 é inserido na porta de destino, informando ao servidor que a requisição deve ser encaminhada ao serviço de servidor web (HTTP).

Graças a esse mecanismo, um único servidor pode oferecer diversos serviços simultaneamente (como FTP na porta 21 e Web na porta 80), pois o número da porta direciona os dados para a aplicação servidora correta.

🔌 O Conceito de Socket   
Para que a comunicação ocorra, os segmentos da camada de transporte (que contêm as portas) são encapsulados dentro de pacotes IP (que contêm os endereços lógicos). A combinação de um Endereço IP com um Número de Porta é denominada Socket. O socket serve para identificar de forma única o dispositivo e o serviço específico em execução.
- Exemplo de Socket de Cliente: 192.168.1.5:1099 (Onde 192.168.1.5 é o IP do host e 1099 é a porta de origem gerada dinamicamente).
- Exemplo de Socket de Servidor: 192.168.1.7:80 (Onde 192.168.1.7 é o IP do servidor e 80 é a porta do serviço web).

A comunicação ativa entre dois dispositivos é definida por um Par de Sockets, consistindo no socket de origem e no socket de destino. Esse par permite que múltiplos processos no cliente se diferenciem, e que o servidor gerencie múltiplas conexões de diferentes clientes simultaneamente. A porta atua, essencialmente, como um "endereço de retorno" para que a camada de transporte saiba exatamente para qual aplicativo entregar a resposta recebida.

🗂️ Classificação de Portas pela IANA   
A Internet Assigned Numbers Authority (IANA) é a entidade responsável pela padronização e atribuição dos números de porta. O campo de 16 bits permite um intervalo que vai de 0 a 65.535. A IANA divide esse intervalo em três grupos distintos:
- Portas Bem Conhecidas (0 a 1.023): Reservadas para serviços e aplicações essenciais e populares (como navegadores web e clientes de e-mail). O uso dessas portas estáticas permite que clientes identifiquem facilmente o serviço necessário em um servidor.
- Portas Registradas (1.024 a 49.151): Atribuídas pela IANA a entidades que solicitam o uso para aplicações específicas. Geralmente referem-se a aplicações instaladas pelo usuário, e não a serviços de infraestrutura básica. Exemplo: A porta 1812 é registrada pela Cisco para o processo de autenticação RADIUS.
- Portas Dinâmicas ou Privadas (49.152 a 65.535): Também chamadas de portas efêmeras. Estas são atribuídas dinamicamente pelo sistema operacional do cliente quando uma conexão é iniciada, servindo para identificar a aplicação durante aquela sessão específica.

Nota: Alguns sistemas operacionais podem utilizar o intervalo de portas registradas para atribuição dinâmica, variando conforme a implementação.

📌 Portas de Serviços Comuns   
É fundamental reconhecer as portas associadas aos serviços de rede mais utilizados. Abaixo estão listadas algumas das principais portas TCP e UDP:
- 20 e 21 (TCP): FTP (Transferência de Arquivos) - Dados e Controle, respectivamente.
- 22 (TCP): SSH (Secure Shell) - Acesso remoto seguro.
- 23 (TCP): Telnet - Acesso remoto não seguro.
- 25 (TCP): SMTP - Envio de e-mail.
- 53 (UDP/TCP): DNS - Resolução de nomes de domínio. (Usa UDP para consultas padrão e TCP para transferências de zona ou respostas grandes).
- 67 e 68 (UDP): DHCP - Configuração dinâmica de host (Servidor e Cliente).
- 69 (UDP): TFTP - Transferência trivial de arquivos.
- 80 (TCP): HTTP - Navegação web padrão.
- 110 (TCP): POP3 - Recebimento de e-mail.
- 143 (TCP): IMAP - Acesso a e-mail no servidor.
- 161 (UDP): SNMP - Gerenciamento de redes.
- 443 (TCP): HTTPS - Navegação web segura.

🕵️ Monitoramento com Netstat   
Conexões TCP desconhecidas podem representar riscos de segurança, indicando a presença de softwares maliciosos ou acessos não autorizados ao host local. Para auditar essas atividades, utiliza-se o utilitário de rede netstat. Este comando lista os protocolos em uso, os endereços e portas locais, os endereços e portas externas (remotas) e o estado atual da conexão (como ESTABLISHED ou LISTENING). Por padrão, o netstat tenta resolver os IPs para nomes de domínio e as portas para nomes de serviços conhecidos. Para visualizar os dados em sua forma numérica bruta (IPs e números de portas), utiliza-se a opção `-n`.

<a name="item14.06"><h4>14.6 Processo de Comunicação TCP</h4></a>[Back to summary](#item14)

🖥️ Processos do Servidor TCP   
A compreensão da função dos números de porta é essencial para entender os detalhes da comunicação TCP. Nos servidores, cada aplicação em execução é configurada para utilizar um número de porta específico, que pode ser atribuído automaticamente ou definido manualmente por um administrador. É uma regra fundamental que um servidor individual não pode atribuir o mesmo número de porta a dois serviços distintos dentro da mesma camada de transporte. Por exemplo, um host não pode executar simultaneamente um servidor Web e um servidor de transferência de arquivos utilizando a mesma porta (como a porta 80). Quando uma aplicação de servidor é atribuída a uma porta, diz-se que essa porta está aberta. Isso significa que a camada de transporte do servidor está escutando, aceitando e processando segmentos endereçados a ela. Qualquer solicitação de cliente que chegue ao socket correto é aceita e os dados são encaminhados para a aplicação correspondente.

Fluxo de Solicitação e Resposta:
- Requisição do Cliente: Ao solicitar um serviço (como Web na porta 80 ou E-mail na porta 25), o cliente gera dinamicamente uma porta de origem única (ex: 49152) para identificar aquela conversa.
- Resposta do Servidor: Ao responder, o servidor inverte os papéis. A porta de origem da resposta torna-se a porta do serviço (80 ou 25) e a porta de destino torna-se a porta dinâmica gerada pelo cliente (49152). Isso garante que o tráfego retorne para a aba ou janela correta no dispositivo do usuário.

🤝 Estabelecimento de Conexão: O Handshake de Três Vias   
O TCP é um protocolo full-duplex, onde cada conexão é composta por duas sessões de comunicação unidirecionais. Antes que qualquer dado seja transmitido, os hosts devem estabelecer a conexão através de um processo conhecido como Handshake de Três Vias (Three-Way Handshake). Este processo desempenha três funções vitais:
- Verifica se o dispositivo de destino está presente na rede.
- Confirma se o dispositivo de destino possui um serviço ativo e está aceitando solicitações na porta desejada.
- Informa ao destino que o cliente de origem pretende iniciar uma sessão de comunicação.

Etapas do Handshake:
- Passo 1 (SYN): O cliente iniciador envia um segmento com a flag SYN (Sincronização) ativa, solicitando uma sessão com o servidor.
- Passo 2 (SYN + ACK): O servidor recebe a solicitação, confirma a sessão do cliente (com a flag ACK) e, simultaneamente, solicita sua própria sessão de volta para o cliente (com a flag SYN).
- Passo 3 (ACK): O cliente iniciador responde com uma flag ACK, confirmando a sessão do servidor. Após isso, a conexão está estabelecida.

🛑 Término da Sessão TCP   
Para encerrar uma conexão, é necessário desligar a flag de controle FIN (Finish). Como o TCP é full-duplex, o encerramento deve ocorrer em ambas as direções, exigindo um processo de quatro etapas (ou dois handshakes duplos). Qualquer um dos hosts pode iniciar o término:
- Passo 1 (FIN): O host que deseja encerrar envia um segmento com a flag FIN ativa.
- Passo 2 (ACK): O outro host confirma o recebimento do FIN. (A sessão em uma direção é encerrada).
- Passo 3 (FIN): O segundo host envia seu próprio segmento FIN para encerrar a sessão na direção oposta.
- Passo 4 (ACK): O primeiro host confirma o recebimento. (A conexão é totalmente encerrada).

🚩 Bits de Controle (Flags)   
O cabeçalho do segmento TCP possui um campo de 6 bits reservado para os Bits de Controle, também chamados de Flags. Esses bits indicam o status e o propósito do segmento na gestão da conexão. As seis flags principais são:
- URG: Indica que o campo de "ponteiro urgente" é significativo.
- ACK: A flag de confirmação, usada para validar o recebimento de dados e durante o handshake.
- PSH: Função Push, instruindo o receptor a processar os dados imediatamente.
- RST: Reset, usado para reinicializar uma conexão quando ocorre um erro ou falha.
- SYN: Sincronização, usada para iniciar e estabelecer conexões.
- FIN: Finish, indica que não há mais dados a serem enviados e inicia o encerramento da sessão.

<a name="item14.07"><h4>14.7 Confiabilidade e controle de fluxo</h4></a>[Back to summary](#item14)

🛡️ Confiabilidade do TCP: Ordenação e Entrega Garantida   
A preferência pelo TCP em determinadas aplicações justifica-se pela sua capacidade de garantir a entrega e a ordem correta dos dados, diferentemente do UDP. O protocolo não apenas recupera pacotes perdidos, mas também gerencia o fluxo para evitar a sobrecarga dos dispositivos finais. Para assegurar que a mensagem original seja compreendida, mesmo que os segmentos cheguem fora de ordem ou por rotas distintas, o TCP utiliza Números de Sequência. Este número é atribuído no cabeçalho de cada pacote e representa o primeiro byte de dados daquele segmento específico.

O processo de sequenciamento funciona da seguinte forma:
- Número de Sequência Inicial (ISN): Durante o estabelecimento da sessão, um valor inicial aleatório é definido. Isso visa prevenir ataques maliciosos de previsão de sequência.
- Rastreamento de Bytes: À medida que os dados são transmitidos, o número de sequência é incrementado com base na quantidade de bytes enviados. Isso permite que cada segmento seja identificado e confirmado individualmente.
- Buffer de Recepção: O processo TCP no receptor armazena os segmentos em um buffer. Dados fora de ordem são retidos até que os segmentos faltantes cheguem, momento em que são reordenados corretamente e passados para a camada de aplicação.

🔄 Gerenciamento de Perdas e Retransmissão (ACK e SACK)   
A perda de dados é um evento possível em qualquer rede. O TCP gerencia essas ocorrências através de mecanismos de confirmação e retransmissão. O protocolo utiliza o Número de Sequência (SEQ) e o Número de Confirmação (ACK) em conjunto. O ACK é uma "confirmação antecipatória", ou seja, informa à origem qual é o próximo byte que o destino espera receber.

A evolução dos métodos de confirmação trouxe melhorias significativas na eficiência:
- Método Tradicional: Originalmente, o TCP apenas confirmava o próximo byte esperado em sequência. Se os segmentos 1, 2, 5, 6 e 7 chegassem, mas o 3 e 4 se perdessem, o receptor confirmaria apenas o recebimento até o 2 (pedindo o 3). O remetente, sem saber que o 5, 6 e 7 já haviam chegado, retransmitiria tudo do 3 ao 7, gerando duplicidade e desperdício de banda.
- Reconhecimento Seletivo (SACK): Atualmente, sistemas operacionais modernos negociam o uso do SACK durante o handshake de três vias. Com o SACK, o receptor pode confirmar explicitamente blocos de dados descontínuos. No exemplo anterior, ele informaria que precisa do 3 e 4, mas que já possui do 5 ao 7. Assim, a origem retransmite apenas os dados estritamente necessários.

🌊 Controle de Fluxo: Janelas Deslizantes   
O controle de fluxo é o mecanismo que impede que o remetente sobrecarregue o receptor, enviando mais dados do que este consegue processar. Isso é gerenciado através do campo Tamanho da Janela (Window Size) no cabeçalho TCP (16 bits).
- Janela de Envio: O tamanho da janela define quantos bytes podem ser enviados antes que uma confirmação (ACK) seja exigida. Este valor é negociado inicialmente no handshake.
- Conceito de Janelas Deslizantes: O receptor não precisa esperar a janela inteira encher para enviar um ACK. À medida que processa os dados, ele envia confirmações. Quando a origem recebe um ACK, ela "desliza" a janela, permitindo o envio de mais bytes.
- Ajuste Dinâmico: Se o buffer do receptor começar a encher (por falta de memória ou processamento lento), ele pode reduzir o tamanho da janela informado nos ACKs, forçando a origem a diminuir a taxa de transmissão.

📏 Tamanho Máximo do Segmento (MSS)   
O MSS (Maximum Segment Size) define a maior quantidade de dados (payload) que um dispositivo pode receber em um único segmento TCP, excluindo o cabeçalho. Este valor é definido no campo de opções do cabeçalho TCP durante o handshake. O cálculo do MSS é baseado na Unidade Máxima de Transmissão (MTU) da interface de rede:
- Cálculo Padrão (IPv4/Ethernet):
  - MTU Ethernet: 1500 bytes.
  - Menos Cabeçalho IPv4: 20 bytes.
  - Menos Cabeçalho TCP: 20 bytes.
  - MSS Resultante: 1460 bytes.

🚦 Prevenção de Congestionamento   
Enquanto o controle de fluxo lida com a capacidade do receptor, a prevenção de congestionamento lida com a capacidade da rede (roteadores e links intermediários). Quando ocorre congestionamento, roteadores sobrecarregados descartam pacotes. A origem detecta o congestionamento indiretamente:
- Sintoma: A ausência de confirmações (ACKs) em tempo hábil ou o recebimento de ACKs duplicados.
- Reação: Ao perceber a perda de pacotes, a origem assume que a rede está congestionada e reduz automaticamente a taxa de envio (diminuindo o número de bytes não confirmados na rede), independentemente do tamanho da janela anunciado pelo receptor.
- Objetivo: Essa redução evita o colapso da rede, impedindo que retransmissões excessivas agravem o tráfego já saturado.

<a name="item14.08"><h4>14.8 Comunicação UDP</h4></a>[Back to summary](#item14)

⚡ Eficiência e Baixa Sobrecarga do UDP   
O UDP destaca-se como o protocolo ideal para comunicações sensíveis a atrasos, como o VoIP (Voz sobre IP), devido à sua arquitetura simplificada. A principal característica que confere essa agilidade é o fato de o UDP não estabelecer uma conexão prévia. Ao contrário do TCP, que exige negociações iniciais, o UDP inicia a transmissão de dados imediatamente. Isso resulta em um transporte de baixa sobrecarga, caracterizado por um cabeçalho de datagrama pequeno e pela ausência de tráfego de gerenciamento de rede (como handshakes ou confirmações).

🔀 Reagrupamento de Datagramas   
Quando múltiplos datagramas UDP são enviados a um destino, é comum que percorram caminhos de rede distintos, resultando em tempos de chegada variados e, consequentemente, fora da ordem original de envio. Diferentemente do TCP, o UDP não utiliza números de sequência para rastrear ou reordenar os pacotes. O comportamento padrão do protocolo é remontar os dados exatamente na ordem em que são recebidos e encaminhá-los imediatamente para a camada de aplicação. Portanto, se a sequência correta dos dados for crítica para a interpretação da mensagem, a responsabilidade recai sobre a aplicação. É o software na camada de aplicação que deve ser projetado para identificar a sequência adequada e processar os dados corretamente, compensando a simplicidade do protocolo de transporte.

🖥️ Processos e Portas do Servidor UDP   
Aplicações de servidor baseadas em UDP operam escutando números de portas "bem conhecidas" ou registradas. Quando um serviço é iniciado no servidor, ele aceita qualquer dado que chegue marcado com o número de porta atribuído a ele. O protocolo UDP recebe o datagrama, verifica a porta de destino e encaminha os dados para a aplicação correspondente.

Exemplo de Serviço: O servidor RADIUS (Remote Authentication Dial-In User Service), frequentemente utilizado para serviços de Autenticação, Autorização e Auditoria (AAA), opera tipicamente na porta registrada UDP 1812.

🔄 Fluxo de Comunicação Cliente-Servidor   
O processo de comunicação é iniciado pela aplicação cliente, que seleciona dinamicamente um número de porta (a partir da faixa de portas dinâmicas/privadas) para usar como porta de origem. A porta de destino será a porta fixa do serviço desejado no servidor. A mecânica de endereçamento durante a troca de mensagens ocorre da seguinte forma:
- Envio da Solicitação:
  - O Cliente 1 deseja resolver um nome de domínio. Ele envia um datagrama para a porta de destino 53 (DNS) e utiliza uma porta de origem dinâmica, por exemplo, 49152.
  - O Cliente 2 deseja autenticação. Ele envia um datagrama para a porta de destino 1812 (RADIUS) e utiliza uma porta de origem dinâmica, por exemplo, 51152.
- Retorno da Resposta:
  - Ao responder, o servidor inverte os endereços para garantir o retorno correto.
  - Para o Cliente 1, a resposta do servidor DNS terá como destino a porta 49152 e origem a porta 53.
  - Para o Cliente 2, a resposta do servidor RADIUS terá como destino a porta 51152 e origem a porta 1812.

Desta forma, o servidor consegue gerenciar múltiplas solicitações simultâneas e encaminhar as respostas para os processos clientes exatos que as originaram.

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
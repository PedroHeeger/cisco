# CyberOps Associate - Módulo 7   <img src="../0-aux/logo_course.png" alt="ild_002" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="../">ild_002 (CyberOps Associate)   <img src="../0-aux/logo_course.png" alt="ild_002" width="auto" height="25"></a>
### Module: 7. Verificação de conectividade

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

### Course Module 7 Structure:

7. <a name="item07">Verificação de conectividade</a><br>
  7.1 <a href="#item07.01">Introdução</a><br>
  7.2 <a href="#item07.02">ICMP</a><br>
  7.3 <a href="#item07.03">Utilitários Ping e Traceroute</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;7.3.1 <a href="../../../pkt/pkt_027/">Packet Tracer - Verificar endereçamento IPv4 e IPv6</a><br>
  7.4 <a href="#item07.04">Resumo de Verificação de Conectividade</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item07.01"><h4>7.1 Introdução</h4></a>[Back to summary](#item07)

🔹 Diagnóstico de Rede e Protocolos de Teste   
A disponibilidade contínua de uma infraestrutura digital não é garantida, tornando essencial a existência de mecanismos voltados à verificação de integridade e desempenho. O protocolo de mensagens de controle (ICMP) atua como um recurso de diagnóstico, permitindo que especialistas em defesa cibernética estabeleçam padrões de comportamento esperado para a rede. Através da análise dessas respostas, é possível diferenciar fluxos operacionais comuns de possíveis anomalias ou falhas críticas de comunicação.

🎯 Objetivo Geral   
- Empregar utilitários baseados no protocolo de controle para a validação da conectividade entre pontos da rede.

✅ Objetivos Específicos   
- ICMP: Analisar o papel das mensagens de controle na execução de testes e na sinalização de erros durante o transporte de dados.
- Utilitários Ping e Traceroute: Utilizar ferramentas nativas para medir a latência e mapear o trajeto percorrido pelos pacotes até o destino final.

<a name="item07.02"><h4>7.2 ICMP</h4></a>[Back to summary](#item07)

📣 O Papel do ICMP: Feedback, não Confiabilidade   
É crucial entender que o ICMP não existe para tornar o IP "confiável" (quem cuida disso é o TCP). O objetivo dele é reportar erros e fornecer informações sobre o processamento dos pacotes.
- ICMPv4: Utilizado em redes IPv4.
- ICMPv6: Utilizado em redes IPv6, trazendo funções extras como a configuração automática de endereços.
- Nota de Segurança: Por expor detalhes da rede, muitos administradores bloqueiam mensagens ICMP para evitar que invasores mapeiem a infraestrutura.

📡 Mensagens Comuns de Diagnóstico   
Existem diversos tipos de mensagens, mas quatro delas são o principais de qualquer analista de rede:
- Confirmação de Host (Echo): É a base do famoso comando ping. O host de origem envia um Echo Request (solicitação) e, se o destino estiver "vivo" e configurado para responder, ele devolve um Echo Reply (resposta).
- Destino Inalcançável (Unreachable): Quando um roteador ou o próprio host de destino não consegue entregar o pacote, ele avisa a origem. O ICMPv4 usa códigos específicos para dizer onde o problema ocorreu:
  - Código 0: Rede inacessível (problema de roteamento).
  - Código 1: Host inacessível (o dispositivo não responde).
  - Código 2: Protocolo inacessível.
  - Código 3: Porta inacessível (o serviço não está rodando naquela porta).
- Tempo Excedido (Time Exceeded): Para evitar que um pacote fique circulando eternamente em um "loop" de rede, existe um contador.
  - No IPv4 (TTL): O campo Time to Live é reduzido em 1 a cada roteador (salto). Se chegar a zero, o roteador descarta o pacote e avisa o remetente.
  - No IPv6 (Hop Limit): Funciona da mesma forma, mas o campo mudou de nome para Limite de Salto.
- Redirecionamento de Rota: Usado por roteadores para avisar um host que existe um caminho mais curto ou eficiente para chegar a um determinado destino.

📡 O Protocolo de Descoberta de Vizinhos (NDP)   
O NDP substitui funções antigas e adiciona novas capacidades de comunicação entre dispositivos e roteadores na rede local. Ele utiliza quatro tipos principais de mensagens:
- Diálogo entre Roteador e Host (RS e RA): Este par de mensagens permite que um dispositivo se configure automaticamente sem precisar de um servidor central (SLAAC).
  - RA (Router Advertisement - Anúncio de Roteador): Os roteadores enviam essa mensagem periodicamente ou quando solicitados. Ela contém o "mapa da mina": o prefixo da rede, o tamanho desse prefixo, endereços de DNS e o domínio. É aqui que o host descobre quem é seu gateway padrão.
  - RS (Router Solicitation - Solicitação de Roteador): Quando um dispositivo acaba de entrar na rede e não quer esperar pelo próximo anúncio periódico, ele grita um RS. Basicamente, ele pergunta: "Tem algum roteador aí que possa me passar as configurações da rede?".
- Diálogo entre Dispositivos Locais (NS e NA): No IPv6, o ARP (Address Resolution Protocol) não existe mais. Quem faz o trabalho de descobrir endereços físicos é o ICMPv6 através dessas mensagens:
  - NS (Neighbor Solicitation - Solicitação de Vizinho): O dispositivo envia um NS quando conhece o IP do colega, mas precisa descobrir o endereço MAC (endereço físico) para enviar o quadro Ethernet.
  - NA (Neighbor Advertisement - Anúncio de Vizinho): É a resposta ao NS. O dispositivo alvo responde confirmando seu endereço MAC. É o famoso: "Sou eu mesmo, e aqui está o meu endereço físico".

🛡️ Detecção de Endereço Duplicado (DAD)   
Como o IPv6 permite que os dispositivos criem seus próprios endereços (via SLAAC), existe o risco de dois aparelhos gerarem o mesmo IP. Para evitar esse conflito, usa-se o processo DAD:
- O dispositivo gera seu endereço IP.
- Antes de começar a usá-lo, ele envia uma mensagem NS para a rede, mas usando o seu próprio endereço recém-criado como destino.
- Se ninguém responder, o endereço é único e ele pode usar.
- Se alguém responder com um NA, significa que aquele IP já tem dono. O dispositivo emissor precisa parar e gerar um novo endereço para evitar o conflito.

Nota Técnica: Embora o DAD não seja estritamente obrigatório em todos os cenários, ele é altamente recomendado pelas normas internacionais (RFC 4861) para garantir a integridade da rede.

<a name="item07.03"><h4>7.3 Utilitários Ping e Traceroute</h4></a>[Back to summary](#item07)

📡 Utilitário Ping e Mensagens ICMP   
O ping é um utilitário de diagnóstico para redes IPv4 e IPv6 que utiliza o protocolo ICMP para verificar a comunicação entre dispositivos. O processo consiste no envio de uma solicitação de eco (Echo Request) para um endereço específico. Caso o destino receba o pacote, uma resposta de eco (Echo Reply) é retornada ao emissor.

🔍 Categorias de Teste de Conectividade   
A execução do comando permite validar diferentes estágios da infraestrutura de rede:
- Loopback Local: Realizado através do endereço 127.0.0.1 (IPv4) ou ::1 (IPv6). Este teste verifica se a pilha de protocolos TCP/IP está instalada e funcional internamente no host. Uma resposta positiva indica que a camada de rede do sistema operacional responde adequadamente, embora não valide configurações de hardware ou endereçamento físico.
- Gateway Padrão: O envio de pings para o endereço do roteador local testa a integridade do segmento de rede local. O sucesso nesta etapa confirma que a placa de rede do host e a interface do roteador estão operacionais. Falhas neste ponto sugerem problemas no cabeamento, configurações de IP locais incorretas ou restrições de segurança na interface do gateway.
- Host Remoto: Utilizado para testar a comunicação através de redes interconectadas ou da internet. O êxito confirma o funcionamento do gateway, de todos os roteadores intermediários e da capacidade do destino externo em processar e responder pacotes.

⏱️ Análise de Desempenho e Respostas   
O utilitário fornece dados quantitativos sobre a qualidade da conexão:
- Tempo de Resposta (RTT): Indica o intervalo entre o envio da solicitação e o recebimento da resposta, servindo como métrica para o desempenho e latência da rede.
- Tempo Limite (Timeout): Ocorre quando o host não recebe a resposta dentro do período esperado. As causas podem variar entre falhas físicas, congestionamento ou a necessidade inicial de resolução de endereços (ARP ou ND).
- Restrições de Segurança: Em redes corporativas, a ausência de resposta é frequentemente causada por firewalls ou configurações que bloqueiam o tráfego ICMP por motivos de proteção contra varreduras de rede.

🛤️ Utilitário Traceroute e Mapeamento de Saltos   
O traceroute (conhecido como tracert em sistemas Windows) é um utilitário de diagnóstico que identifica a rota detalhada percorrida por um pacote até o destino. Diferente do ping, que apenas valida a conectividade básica, o traceroute fornece a lista de todos os roteadores intermediários, denominados saltos, presentes no caminho.

⏱️ Tempo de Ida e Volta (RTT) e Diagnóstico   
A ferramenta registra o tempo necessário para que um pacote alcance cada salto e retorne a resposta.
- Identificação de Falhas: Caso um roteador não responda, o utilitário exibe um asterisco (*), indicando perda de pacote ou restrição de segurança (firewall).
- Análise de Desempenho: Tempos de resposta elevados em um salto específico sinalizam possíveis gargalos, conexões sobrecarregadas ou processamento excessivo no roteador em questão.
- Localização de Erros: O endereço do último roteador a responder serve como indicador geográfico ou lógico de onde a comunicação foi interrompida ou bloqueada.

⚙️ Mecanismo de Funcionamento: TTL e Limite de Saltos   
O funcionamento baseia-se na manipulação dos campos TTL (Time to Live) no IPv4 ou Limite de Saltos no IPv6, em conjunto com mensagens de erro do protocolo ICMP.
- Início do Rastreamento: O host de origem envia o primeiro pacote com TTL definido como 1. O primeiro roteador processa o pacote, decrementa o valor para 0, descarta o dado e retorna uma mensagem ICMP Time Exceeded (Tempo Excedido).
- Incremento Progressivo: O utilitário aumenta sucessivamente o valor do TTL (2, 3, 4...). Isso força a expiração do pacote em roteadores cada vez mais distantes, revelando a interface de cada dispositivo no trajeto.
- Finalização: O processo encerra quando o pacote atinge o host de destino final. Neste ponto, o destino responde com uma mensagem de Porta Inalcançável ou Resposta de Eco, indicando a conclusão do caminho.

📑 Estrutura e Segurança do ICMP   
O ICMP é encapsulado diretamente em pacotes IP na Camada 3 (Rede). A distinção entre as funções é feita através de códigos de mensagem:
- Código 0: Echo Reply (Resposta de eco).
- Código 3: Destination Unreachable (Destino inalcançável).
- Código 8: Echo Request (Solicitação de eco).
- Código 11: Time Exceeded (Tempo excedido/TTL igual a 0).

No contexto da segurança cibernética, o campo opcional de carga útil (payload) das mensagens ICMP exige monitoramento, pois pode ser explorado por agentes maliciosos como vetor para a exfiltração de dados de forma furtiva dentro da rede.

<a name="item07.04"><h4>7.4 Resumo de Verificação de Conectividade</h4></a>[Back to summary](#item07)

📡 Mensagens de Diagnóstico   
O protocolo ICMP atua como um sistema de avisos que reporta falhas de entrega ou problemas de rota durante o transporte de pacotes. Embora existam versões específicas para cada protocolo de rede, ambas compartilham funções vitais como confirmar se um destino está ativo ou avisar quando um serviço está inacessível, sendo frequentemente restringidas em infraestruturas corporativas para evitar o mapeamento da rede por invasores.

🤝 Descoberta de Vizinhança   
No ambiente IPv6, o sistema de mensagens evoluiu para incluir o protocolo NDP, que facilita a comunicação automática entre roteadores e dispositivos locais. Através de solicitações e anúncios específicos, os equipamentos conseguem identificar a presença de roteadores na rede e localizar outros dispositivos vizinhos, permitindo que a configuração e a troca de informações ocorram de forma dinâmica e sem intervenção manual.

🧪 Teste de Conectividade   
O utilitário Ping utiliza pedidos e respostas de eco para verificar se existe comunicação funcional entre dois pontos da rede. Essa ferramenta é fundamental para validar se a interface interna do computador está operando corretamente, se o portão de saída para a internet está alcançável ou se um servidor localizado em outra parte do mundo consegue responder aos chamados do sistema.

🗺️ Rastreamento de Saltos   
Para identificar o caminho exato que um dado percorre, o comando Traceroute mapeia cada roteador intermediário até o destino final, utilizando contadores de tempo de vida do pacote. Quando um desses contadores expira, o roteador envia um aviso de tempo excedido, permitindo que o analista visualize cada etapa da viagem e identifique exatamente em qual ponto da infraestrutura está ocorrendo uma falha ou lentidão.
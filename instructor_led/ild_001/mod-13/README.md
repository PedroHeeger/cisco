# CCNA: Introduction to Networks - Módulo 13   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_001 (CCNA: Introduction to Networks)   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="25"></a>
### Module: 13. ICMP

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

### Course Module 13 Structure:
13. <a name="item13">ICMP</a><br>
  13.1 <a href="#item13.01">Introdução</a><br>
  13.2 <a href="#item13.02">Mensagens ICMP</a><br>
  13.3 <a href="#item13.03">Testes de Ping e Traceroute</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;13.3.1 <a href="../../../pkt/files/pkt_040/">Packet Tracer - Verifique o endereçamento IPv4 e IPv6</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;13.3.2 <a href="../../../pkt/files/pkt_041/">Packet Tracer - Use Ping e Traceroute para testar a conectividade de rede</a><br>
  13.4 <a href="#item13.04">Módulo Prático e Quiz</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;13.4.1 <a href="../../../pkt/files/pkt_042/">Packet Tracer - Usar ICMP para testar e corrigir conectividade de rede</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;13.4.2 <a href="../../../pkt/files/pkt_043/">Packet Tracer - Use Ping e Traceroute para testar a conectividade de rede</a><br>
  13.5 Exame de endereçamento IP<br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item13.01"><h4>13.1 Introdução</h4></a>[Back to summary](#item13)

🛰️ ICMP   
O ICMP é essencial para diagnosticar problemas em redes IPv4 e IPv6. Diferente de um sistema físico onde a falha pode ser identificada visualmente, em redes os erros não são evidentes. O ICMP fornece mensagens de controle e retorno que ajudam a identificar onde um pacote está sendo bloqueado, perdido ou atrasado. Este módulo apresenta essas mensagens e mostra como utilitários comuns usam o ICMP para verificar caminhos e conectividade.

🎯 Objetivo do módulo   
Usar várias ferramentas para testar a conectividade de rede.

📘 Tópicos do módulo   
- Mensagens ICMP: Apresentação do papel do ICMP no envio de notificações sobre erros, tempos excedidos e informações de diagnóstico ao longo do caminho de um pacote.
- Teste de ping e traceroute: Demonstração de como utilitários como ping e traceroute utilizam o ICMP para confirmar conectividade, medir resposta e identificar cada salto até o destino.

<a name="item13.02"><h4>13.2 Mensagens ICMP</h4></a>[Back to summary](#item13)

💬 Protocolos de Mensagens de Controle da Internet (ICMP)   
Embora o Protocolo IP seja considerado um protocolo de "melhor esforço" (não confiável, sem garantia de entrega), o conjunto de protocolos TCP/IP inclui mecanismos para fornecer mensagens de erro e informações sobre o processamento de pacotes. Esses mecanismos são fornecidos pelo Protocolo de Mensagens de Controle da Internet (ICMP). O objetivo do ICMP é dar feedback sobre problemas relacionados ao processamento de pacotes IP sob determinadas condições, e não transformar o IP em um protocolo confiável. Por questões de segurança, muitas vezes as mensagens ICMP são bloqueadas.

O ICMP está disponível para ambas as versões do protocolo:
- ICMPv4: O protocolo de mensagens para o IPv4.
- ICMPv6: Fornece os mesmos serviços para o IPv6, mas inclui funcionalidades adicionais.

🚨 Mensagens ICMP Comuns (v4 e v6)   
Os tipos de mensagens ICMP são numerosos, mas as mais comuns e essenciais, presentes tanto no ICMPv4 quanto no ICMPv6, são:
- Acessibilidade do Host (Echo Request/Reply)
- Destino ou Serviço Inalcançável
- Tempo Excedido (Time Exceeded)

✅ Teste de Acessibilidade (Ping)   
Uma mensagem de Echo ICMP é utilizada para verificar se um host está acessível em uma rede. O host de origem envia uma Solicitação de Echo (ICMP Echo Request). Se o host de destino estiver operacional, ele responderá com uma Resposta de Echo (Echo Reply). Este processo de Requisição/Resposta de Echo é a base da ferramenta de diagnóstico conhecida como ping.

🛑 Destino Inalcançável (Destination Unreachable)   
Quando um roteador ou host recebe um pacote IP que não consegue entregar (seja porque a rede de destino não existe ou o serviço está indisponível), ele pode enviar uma mensagem ICMP de Destino Inalcançável de volta à origem. A mensagem inclui um código que especifica a razão da falha.

Exemplos de códigos de Destino Inalcançável para ICMPv4 incluem:
- 0 = Rede inalcançável
- 1 = Host inalcançável
- 2 = Protocolo inalcançável
- 3 = Porta inalcançável

Exemplos de códigos para ICMPv6 (que são semelhantes, mas ligeiramente diferentes) incluem:
- 0 = Nenhuma rota para o destino
- 1 = Comunicação administrativamente proibida (ex: por firewall)
- 3 = Endereço inacessível
- 4 = Porta inalcançável

⏳ Tempo Excedido (Time Exceeded)   
O protocolo ICMPv4 utiliza a mensagem de Tempo Excedido quando o campo Vida Útil (TTL) de um pacote IPv4 é decrementado para zero por um roteador. Nesse caso, o roteador descarta o pacote e notifica o host de origem com a mensagem de Tempo Excedido. No ICMPv6, a mesma mensagem é enviada, mas o campo de controle de expiração usado é o Limite de Salto (Hop Limit), que substitui o TTL do IPv4. As mensagens de Tempo Excedido são fundamentais para o funcionamento da ferramenta traceroute.

🚀 Funcionalidades Aprimoradas do ICMPv6   
O ICMPv6, apesar de realizar as mesmas funções de erro e controle que o ICMPv4, possui funcionalidades aprimoradas e é essencial para o Protocolo de Descoberta de Vizinhos (Neighbor Discovery Protocol - NDP). As mensagens do ICMPv6 são encapsuladas diretamente no IPv6.

O NDP utiliza o ICMPv6 para realizar funções essenciais, como alocação dinâmica de endereços e resolução de endereços. As principais mensagens do NDP são:
- Mensagens Roteador-Dispositivo (Alocação de Endereço Dinâmico):
  - Mensagem de Solicitação de Roteador (RS): Um host (dispositivo IPv6) envia um RS ao inicializar para determinar se há roteadores IPv6 na rede e como deve obter suas informações de endereço dinamicamente (ex: se deve usar SLAAC).
  - Mensagem de Anúncio de Roteador (RA): O roteador habilitado para IPv6 envia RAs periodicamente (a cada 200 segundos) ou em resposta a um RS. O RA fornece informações cruciais para o host, como o prefixo da rede, o comprimento do prefixo e, mais importante, o endereço LLA do roteador, que será usado pelo host como seu gateway padrão (se estiver usando SLAAC).
- Mensagens Dispositivo-Dispositivo (Detecção e Resolução de Endereço):
  - Mensagem de Solicitação de Vizinhos (NS): Esta mensagem tem dois usos principais:
    - Resolução de Endereço (ARP em IPv6): Um dispositivo envia um NS para determinar o endereço MAC Ethernet de um vizinho cujo endereço IPv6 unicast é conhecido.
    - Detecção de Endereço Duplicado (DAD): Um dispositivo envia um NS para verificar se um endereço IPv6 (Global ou Link Local) que ele acabou de receber já está em uso na rede, enviando o NS para o próprio endereço que está tentando verificar.
  - Mensagem de Anúncio de Vizinhos (NA): Esta mensagem é a resposta a uma Solicitação de Vizinhos (NS). Ela é usada para:
    - Responder à Resolução de Endereço: O dispositivo de destino (que possui o endereço IPv6 solicitado) responde com o NA, fornecendo seu endereço MAC Ethernet.
    - Notificar Duplicidade: Se o NS foi enviado para DAD e outro dispositivo já possui o endereço, ele responderá com o NA, notificando o dispositivo emissor de que o endereço está em uso.
- Nota: O ICMPv6 ND também inclui uma mensagem de Redirecionamento, que possui uma função semelhante àquela usada no ICMPv4.

<a name="item13.03"><h4>13.3 Testes de Ping e Traceroute</h4></a>[Back to summary](#item13)

⚙️ Ferramentas Essenciais de Verificação: Ping e Traceroute   
Nesta aula, exploraremos as ferramentas de diagnóstico ping e traceroute (ou tracert), focando em como e quando elas são utilizadas para testar a conectividade e mapear rotas em redes IPv4 e IPv6.

📡 O Utilitário Ping   
O ping é uma ferramenta de teste fundamental que utiliza as mensagens ICMP (Internet Control Message Protocol) de Solicitação de Eco e Resposta de Eco para confirmar se a comunicação entre dois hosts é possível.
- Funcionamento: Ao enviar uma Solicitação de Eco para um endereço específico, se o host de destino estiver ativo e puder receber a mensagem, ele enviará uma Resposta de Eco.
- Métrica de Desempenho: O ping mede o Tempo de Ida e Volta (Round Trip Time – RTT), fornecendo um indicativo da performance da rede.
- Comportamento de Timeout: Se a Resposta de Eco não chegar dentro de um tempo limite, o ping reporta uma falha. Isso pode indicar um problema de conectividade ou, frequentemente, que recursos de segurança (como um firewall) estão bloqueando o tráfego ICMP. É comum o primeiro ping falhar se for necessário realizar a resolução de endereço (ARP ou ND) antes do envio do ICMP.
- Resumo: Após a conclusão, o utilitário exibe um resumo estatístico, incluindo a taxa de sucesso e o tempo médio de RTT.

🎯 Tipos de Testes de Conectividade com Ping   
O ping é usado para realizar testes em três níveis principais:
- Loopback Local: Testar a configuração interna do protocolo IP no host local.
  - Como fazer: Use o endereço de loopback local: 127.0.0.1 (IPv4) ou ::1 (IPv6).
  - Resultado: Uma resposta bem-sucedida confirma que o stack IP (TCP/IP) está instalado e funcionando corretamente na camada de rede. Não garante que endereços, máscaras ou gateways estejam corretos ou que as camadas inferiores estejam operacionais. Uma mensagem de erro indica que o TCP/IP está inoperante no host.
- Gateway Padrão ou Host Local: Testar a capacidade de comunicação dentro da rede local.
  - Como fazer: O teste mais comum é enviar um ping para o endereço IP do gateway padrão.
  - Resultado: Um sucesso indica que tanto o host local quanto a interface do roteador (que atua como gateway) estão operacionais no mesmo link local.
  - Diagnóstico: Se o gateway falhar, pode-se tentar o ping para outro host conhecido na rede. Se o outro host responder, mas o gateway não, o problema pode estar no roteador (endereço de gateway incorreto no host, ou segurança no roteador bloqueando o ICMP).
- Host Remoto: Testar a conectividade através da rede interconectada.
  - Como fazer: Enviar um ping para um endereço IPv4 ou IPv6 de um host em uma rede distante.
  - Resultado: Um ping bem-sucedido a um host remoto verifica a operação de uma grande parte da rede, confirmando: a comunicação local, a operação do gateway padrão e a operação de todos os roteadores ao longo do caminho.
  - Atenção: Muitos administradores de rede aplicam restrições de segurança que limitam ou proíbem o tráfego ICMP (ping) que entra na rede corporativa. Uma falha no ping remoto pode ser um indicativo de restrições de segurança e não, necessariamente, de uma falha de rede.

🗺️ O Utilitário Traceroute (Tracert)   
Enquanto o ping confirma a conectividade entre dois pontos, o traceroute (tracert) fornece detalhes dos dispositivos intermediários. Ele gera uma lista dos saltos (roteadores) alcançados com sucesso no caminho entre a origem e o destino.

Informação Fornecida:
- Lista de Saltos: O endereço da interface de cada roteador no caminho.
- Diagnóstico de Falhas: Se os dados falharem em um ponto, o endereço do último roteador que respondeu indica a área provável do problema ou a localização das restrições de segurança.
- Tempo de Ida e Volta (RTT): O traceroute mostra o RTT para cada salto. RTTs elevados ou asteriscos (*) indicam pacotes perdidos ou não respondidos, sugerindo que o roteador intermediário ou suas conexões estão sobrecarregados ou configurados para não responder.

⏳ Mecanismo do Traceroute (TTL e Limite de Saltos)   
O traceroute utiliza o campo TTL (Time-to-Live) no IPv4, ou o campo Limite de Saltos (Hop Limit) no IPv6, em conjunto com a mensagem ICMP Time Exceeded para mapear a rota.
- Primeiro Salto: O traceroute envia a primeira sequência de mensagens com o TTL/Limite de Saltos definido como 1. Isso garante que o pacote expire no primeiro roteador. O roteador responde com uma mensagem ICMP Time Exceeded, revelando seu endereço.
- Mapeamento Progressivo: O traceroute aumenta o valor do TTL/Limite de Saltos (2, 3, 4, etc.) para cada sequência subsequente. Isso faz com que os pacotes expirem progressivamente mais adiante no caminho, permitindo que a ferramenta colete o endereço de cada salto.
- Destino Final: O processo se repete até que o pacote alcance o destino ou atinja um valor máximo predeterminado. Ao ser alcançado, o host de destino responde com uma mensagem ICMP de Porta Inacessível ou uma Resposta de Eco, encerrando o rastreio.

<a name="item13.04"><h4>13.4 Módulo Prático e Quiz</h4></a>[Back to summary](#item13)

🌐 Mensagens ICMP   
O conjunto TCP/IP utiliza o ICMP para enviar alertas e informações sempre que surgem dificuldades no tratamento de pacotes IP. Essas mensagens fornecem retorno sobre problemas, como falha de acesso ao host, serviço indisponível ou expiração de tempo. Solicitações e respostas de eco verificam se um host está alcançável, formando a base do comando ping.

📩 Destino Inacessível   
Quando um pacote não pode ser entregue, o host ou gateway avisa a origem por meio de uma mensagem de destino inacessível, incluindo um código que explica o motivo da falha. No IPv4, também há notificações quando o TTL chega a zero; o pacote é descartado e a origem recebe um aviso. No IPv6, o princípio é o mesmo, usando o limite de saltos. Essa mecânica é essencial para o funcionamento do traceroute.

🔄 Mensagens IPv6 Específicas   
No IPv6, roteadores e dispositivos trocam mensagens adicionais para funções como autoconfiguração, incluindo RS e RA. Entre dispositivos, podem ocorrer mensagens de redirecionamento, além de NS e NA, responsáveis por confirmar endereços e vizinhança na rede.

📡 Testes com Ping   
O ping verifica conectividade enviando requisições de eco ao destino e exibindo o tempo necessário para cada resposta. Ao final, mostra estatísticas de sucesso e média de ida e volta. Ele pode validar a configuração interna do dispositivo usando o loopback, testar comunicação com o gateway padrão ou confirmar acesso a hosts remotos em diferentes redes.

🛰️ Rastreamento com Traceroute   
O traceroute lista cada salto alcançado ao longo do caminho até o destino, ajudando a identificar onde surgem falhas ou restrições. Sempre que um roteador reduz o TTL ou limite de saltos a zero, gera uma mensagem de tempo excedido que o traceroute usa para mapear o trajeto. Esse processo revela o último ponto que respondeu e facilita o diagnóstico do percurso dos pacotes.
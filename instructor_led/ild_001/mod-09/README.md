# CCNA: Introduction to Networks - Módulo 9   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_001 (CCNA: Introduction to Networks)   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="25"></a>
### Module: 9. Resolução de endereços

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

### Course Module 9 Structure:
9. <a name="item09">Resolução de endereços</a><br>
  9.1 <a href="#item09.01">Introdução</a><br>
  9.2 <a href="#item09.02">MAC e IP</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;9.2.1 <a href="../../../pkt/files/pkt_023/">Packet Tracer – Identificação de Endereços MAC e IP</a><br>
  9.3 <a href="#item09.03">ARP</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;9.3.1 <a href="../../../pkt/files/pkt_024/">Packet Tracer – Exame da Tabela ARP</a><br>
  9.4 <a href="#item09.04">Descoberta de vizinhos de IPv6</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;9.4.1 <a href="../../../pkt/files/pkt_025/">Packat Tracer - Descoberta de vizinhos de IPv6</a><br>
  9.5 <a href="#item09.05">Módulo Prático e Quiz</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item09.01"><h4>9.1 Introdução</h4></a>[Back to summary](#item09)

📘 Introdução   
Este módulo aborda os mecanismos que permitem a associação entre endereços lógicos e endereços físicos dentro de uma rede. Para que um pacote chegue ao destino correto, é necessário que dispositivos consigam identificar o endereço MAC correspondente ao endereço IP envolvido na comunicação. Esse processo, que seria inviável de ser realizado manualmente em ambientes reais, é automatizado por protocolos específicos que tratam da resolução de endereços. Compreender como esses protocolos funcionam é essencial tanto para diagnosticar falhas quanto para reconhecer comportamentos anômalos que possam indicar ameaças à rede.

🎯 Objetivo Geral   
Explicar como os protocolos ARP e Neighbor Discovery viabilizam a comunicação em redes ao mapear endereços IP para endereços físicos.

✅ Objetivos Específicos   
- Comparar as funções desempenhadas pelos endereços MAC e IP.
- Descrever a finalidade e o funcionamento do protocolo ARP em redes IPv4.
- Explicar como ocorre o processo de descoberta de vizinhança em redes IPv6 por meio do Neighbor Discovery.

<a name="item09.02"><h4>9.2 MAC e IP</h4></a>[Back to summary](#item09)

🔍 Resolução de Endereços na Rede   
Em muitas situações, um host precisa enviar uma mensagem sabendo apenas o endereço IP do dispositivo de destino. Para que o envio funcione na camada de enlace, é necessário descobrir o endereço MAC correspondente — e é exatamente isso que o processo de resolução de endereços faz.

🧩 Dois Endereços por Dispositivo na LAN   
Cada dispositivo em uma LAN Ethernet possui dois endereços essenciais:
- Endereço físico (MAC): Usado para comunicação direta entre NICs na mesma rede.
- Endereço lógico (IP): Usado para enviar o pacote da origem ao destino, seja na rede local ou em uma rede remota.

O quadro da Camada 2 usa endereços MAC para transportar o pacote encapsulado até o próximo dispositivo no mesmo enlace. Já os endereços IPv4/IPv6, na Camada 3, definem origem e destino fim a fim.

🖥️ Exemplo: Comunicação na Mesma Rede   
PC1 precisa enviar um pacote para PC2. O endereço IP de destino está na mesma rede, portanto o quadro Ethernet será montado assim:
- Quadro Ethernet (Camada 2):
  - MAC de destino: MAC do PC2 → 55-55-55
  - MAC de origem: MAC do PC1 → aa-aa-aa
- Pacote IP (Camada 3):
  - IPv4 de origem: 192.168.10.10
  - IPv4 de destino: 192.168.10.11

🌐 Exemplo: Comunicação com Rede Remota   
Agora PC1 deseja enviar um pacote para PC2, mas o destino está em outra rede. Nesse caso:
- O quadro Ethernet não usa o MAC de PC2.
- O MAC de destino passa a ser o MAC da interface do gateway padrão (o roteador).

O roteador recebe o quadro, remove o cabeçalho da Camada 2, analisa o endereço IPv4 de destino e decide o próximo salto. Então encapsula o pacote novamente com novos MACs, de acordo com a interface de saída. Esse processo se repete a cada link, até o pacote chegar ao destino.

🔗 Como IP vira MAC em cada salto?   
A associação entre endereços IP e MAC ao longo do caminho funciona assim:
- Para IPv4: usa ARP (Address Resolution Protocol)
- Para IPv6: usa ICMPv6 Neighbor Discovery (ND)

Esses protocolos permitem que cada dispositivo descubra o endereço MAC correspondente ao próximo salto, garantindo que o quadro possa ser entregue corretamente no enlace atual.

<a name="item09.03"><h4>9.3 ARP</h4></a>[Back to summary](#item09)

🔧 O que o ARP Faz em uma Rede IPv4   
Quando uma rede utiliza IPv4, o mecanismo responsável por transformar endereços IP em endereços MAC é o ARP (Address Resolution Protocol). Ele permite que um dispositivo descubra o endereço físico necessário para montar um quadro Ethernet e enviá-lo ao destino correto.

🧩 Endereços usados no Quadro Ethernet   
Ao enviar um quadro Ethernet, dois endereços MAC são obrigatórios:
- MAC de destino:
  - Se o destino estiver na mesma rede, é o MAC do próprio host de destino.
  - Se o destino estiver em outra rede, é o MAC do gateway padrão (interface do roteador).
- MAC de origem:
  - É o MAC da interface de rede do host que está enviando o quadro.

Para que isso funcione, o dispositivo precisa saber qual MAC corresponde ao endereço IPv4 envolvido na comunicação.

📚 A Função do ARP   
O ARP possui duas funções essenciais:
- Descobrir o endereço MAC associado a um endereço IPv4 local.
- Manter um cache (tabela ARP) com esses mapeamentos temporários.

Essa tabela é armazenada na memória RAM e contém linhas que ligam cada IPv4 ao MAC correspondente. Quando o host precisa enviar um quadro, ele consulta essa tabela.

🔍 Como o Dispositivo Consulta a Tabela ARP   
Há dois cenários possíveis:
- Destino na mesma rede: A busca é feita diretamente pelo IPv4 do host de destino.
- Destino remoto: A busca é feita pelo IPv4 do gateway padrão, já que o roteador é o próximo salto.

Se o IPv4 procurado existir na tabela ARP, o MAC correspondente é usado imediatamente. Se não existir, o dispositivo precisa realizar uma requisição ARP.

📢 Como a Requisição ARP Funciona   
Uma requisição ARP é enviada quando o endereço MAC do IPv4 desejado ainda não é conhecido.

Características dessa mensagem:
- Encapsulamento direto em um quadro Ethernet (sem cabeçalho IP).
- MAC de destino: broadcast → FF-FF-FF-FF-FF-FF (todos os dispositivos da LAN recebem).
- MAC de origem: MAC do dispositivo que está fazendo a requisição.
- Tipo: 0x806 indicando que o conteúdo é uma mensagem ARP.

Todos os hosts da LAN recebem a requisição, mas apenas o host que possui o IPv4 solicitado responde.

📨 Resposta ARP   
A resposta ARP é enviada como unicast diretamente para quem fez a solicitação. O quadro contém:
- MAC de destino: MAC do dispositivo que iniciou a requisição.
- MAC de origem: MAC do dispositivo que está respondendo.
- Tipo: novamente 0x806.

Após receber a resposta, o endereço IP e seu MAC correspondente são registrados na tabela ARP. Assim, o host passa a ter os dados necessários para montar novos quadros. Se ninguém responder, o pacote não pode ser enviado e é descartado.

🕒 Tempo de Vida da Tabela ARP   
As entradas no cache ARP expiram após um período. Esse tempo varia conforme o sistema operacional. No Windows, por exemplo, as entradas costumam permanecer entre 15 e 45 segundos. Também é possível limpar manualmente a tabela, removendo uma ou todas as entradas, o que força novas resoluções ARP na próxima comunicação.

🖥️ Como Visualizar a Tabela ARP   
- Em roteadores Cisco → comando: `show ip arp`
- Em Windows → comando: `arp -a`

🌐 Quando o Destino Está em Outra Rede   
Se o IPv4 de destino não está na mesma sub-rede que o host:
- O host identifica que o destino está em outra rede.
- O pacote deve ser enviado ao gateway padrão.
- O ARP é usado para descobrir o MAC do gateway, caso ele ainda não esteja no cache.
- O quadro é montado com:
  - MAC de destino: MAC da interface do roteador.
  - MAC de origem: MAC do host emissor.

⚠️ Problemas Relacionados ao ARP   
- Excesso de Broadcast:
  - Requisições ARP são broadcasts e, portanto, todos os dispositivos precisam processá-las. Em redes grandes, especialmente em momentos de pico (como quando muitos equipamentos ligam ao mesmo tempo), pode ocorrer um pequeno impacto no desempenho. Após o cache ser preenchido, esse impacto desaparece.
- Segurança: Falsificação ARP (ARP Spoofing)
  - Como o ARP não possui autenticação, um invasor pode enviar respostas ARP falsas, associando seu próprio MAC ao IP de outro dispositivo — geralmente o gateway. 
  Isso redireciona o tráfego da vítima para o atacante, que pode interceptar ou modificar os dados. 
  - Switches corporativos usam técnicas como Dynamic ARP Inspection (DAI) para mitigar esse tipo de ataque.

🔄 IPv6: Equivalente ao ARP   
No IPv6, a função do ARP é substituída pelo processo Neighbor Discovery (ND), realizado através de mensagens ICMPv6. O princípio é o mesmo: descobrir o endereço de enlace correspondente ao endereço IP.

<a name="item09.04"><h4>9.4 Descoberta de vizinhos de IPv6</h4></a>[Back to summary](#item09)

🌐 IPv6 Neighbor Discovery (ND)   
O IPv6 utiliza o Neighbor Discovery (ND) para relacionar endereços IPv6 com endereços MAC. Ele substitui o ARP do IPv4 e funciona com mensagens ICMPv6 responsáveis por descobrir vizinhos, identificar roteadores e auxiliar no encaminhamento local.

✉️ Mensagens do ND   
O ND utiliza cinco mensagens ICMPv6:
- Solicitação de Vizinho (Neighbor Solicitation);
- Anúncio de Vizinho (Neighbor Advertisement);
- Solicitação de Roteador (Router Solicitation);
- Anúncio de Roteador (Router Advertisement);
- Redirecionamento (Redirect).

As duas primeiras funcionam entre dispositivos; as duas seguintes, entre hosts e roteadores.

🔍 Resolução de Endereço IPv6   
A resolução de endereço em IPv6 segue uma lógica próxima ao ARP:
- O dispositivo envia uma Neighbor Solicitation para um endereço multicast gerado a partir do IPv6 alvo.
- O dispositivo de destino responde com uma Neighbor Advertisement contendo seu MAC.
- O emissor registra esse mapeamento no cache ND e passa a encapsular quadros Ethernet com o MAC correto.

🖧 Exemplo   
Se o PC1 precisa acessar o PC2 usando o IPv6 2001:db8:acad:11::2:
- O PC1 envia uma Solicitação de Vizinho para o multicast correspondente ao endereço do PC2.
- O PC2 responde com um Anúncio de Vizinho contendo seu endereço MAC.
- O PC1 grava essa informação no cache e já pode comunicar diretamente.

<a name="item09.05"><h4>9.5 Módulo Prático e Quiz</h4></a>[Back to summary](#item09)

🔗 Mapeamento IPv4/IPv6 para MAC na Rede Local   
Os endereços MAC da camada 2 são responsáveis por entregar quadros Ethernet entre as NICs dentro da mesma rede. Quando o destino está na mesma sub-rede, o MAC de destino é o próprio dispositivo final. Mas, se o destino estiver em outra rede, o quadro é enviado para o gateway padrão, usando o MAC da interface do roteador. Cada salto no caminho até o destino envolve um novo encapsulamento: o pacote IP segue o trajeto completo, mas cada link utiliza seu próprio quadro Ethernet com endereços MAC específicos daquele trecho. 

Para relacionar o endereço IP ao endereço MAC em cada enlace, cada protocolo usa um processo específico:
- IPv4 usa ARP
- IPv6 usa ICMPv6 ND

🔍 ARP no IPv4   
Em redes IPv4, cada host Ethernet possui um MAC único. Para enviar um quadro, o dispositivo informa o MAC de origem e precisa descobrir o MAC de destino. O ARP resolve exatamente isso: encontra o endereço MAC associado a um endereço IPv4 local. O ARP executa duas funções principais:
- Descobrir o MAC do dispositivo correspondente a um IP conhecido.
- Armazenar esses mapeamentos em uma tabela ARP.

A solicitação ARP é enviada como broadcast para toda a LAN, e somente o host que possui o IP solicitado responde. A resposta retorna diretamente ao solicitante, que então registra esse par IP–MAC na tabela ARP. Quando o IP de destino está em outra rede, o host não procura o MAC do destino remoto. Ele procura o MAC do gateway padrão, pois será o roteador que fará o encaminhamento.

Entradas ARP possuem um tempo de vida e são removidas quando ficam inativas por um período. Também podem ser apagadas manualmente. Como o ARP usa broadcast, ele pode gerar tráfego excessivo. Além disso, o processo pode ser explorado em ataques como ARP spoofing, que alteram a tabela ARP e desviam tráfego.

🧭 ND no IPv6   
O IPv6 não utiliza ARP. Em vez disso, usa o Neighbor Discovery (ND), que é baseado em mensagens ICMPv6. O ND trata da resolução de endereço MAC, descoberta de roteadores e redirecionamento de pacotes. Ele utiliza cinco tipos de mensagens ICMPv6:
- Solicitação de vizinho
- Anúncio de vizinho
- Solicitação de roteador
- Anúncio de roteador
- Redirecionamento

Assim como no IPv4 com o ARP, o ND permite que dispositivos IPv6 descubram o MAC correspondente a um endereço IPv6 conhecido, garantindo a comunicação correta dentro da rede.
# CCNA: Introduction to Networks - Módulo 12   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_001 (CCNA: Introduction to Networks)   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="25"></a>
### Module: 12. Endereçamento IPv6

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

### Course Module 12 Structure:
12. <a name="item12">Endereçamento IPv6</a><br>
  12.1 <a href="#item12.01">Introdução</a><br>
  12.2 <a href="#item12.02">Problemas do IPv4</a><br>
  12.3 <a href="#item12.03">Representação do Endereço IPv6</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;12.3.1 <a href="#item12.03.01">Verifique sua compreensão - Representação de endereço IPv6</a><br>
  12.4 <a href="#item12.04">Tipos de Endereço IPv6</a><br>
  12.5 <a href="#item12.05">Configuração Estática do GUA e do LLA</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;12.5.1 <a href="#item12.05.01">Verificador de Sintaxe - Configuração Estática GUA e LLA</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;12.5.2 <a href="../../../pkt/files/pkt_036/">Packet Tracer - Configuração Básica do Dispositivo</a><br>
  12.6 <a href="#item12.06">Endereçamento dinâmico para GUAs IPv6</a><br>
  12.7 <a href="#item12.07">Endereçamento Dinâmico para LLAs IPv6</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;12.7.1 <a href="#item12.07.01">Verificador de sintaxe - Verifique a configuração do endereço IPv6</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;12.7.2 <a href="../../../pkt/files/pkt_037/">Packet Tracer - Configurar Endereçamento IPv6</a><br>
  12.8 <a href="#item12.08">Endereços IPv6 Multicast</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;12.8.1 <a href="../../../labs/files/lab_051/">Laboratório - Identificando Endereços IPv6</a><br>
  12.9 <a href="#item12.09">Sub-rede de uma rede IPv6</a><br>
  12.10 <a href="#item12.10">Módulo Prático e Quiz</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;12.10.1 <a href="../../../pkt/files/pkt_038/">Packet Tracer - Implementando um Esquema de Endereçamento IPv6 com Sub-Redes</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;12.10.2 <a href="../../../pkt/files/pkt_039/">Packet Tracer - Configurar Endereços IPv6 em Dispositivos de Rede - Modo Físico</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item12.01"><h4>12.1 Introdução</h4></a>[Back to summary](#item12)

🌐 Endereçamento IPv6   
A adoção do IPv6 ocorre paralelamente ao uso contínuo do IPv4, exigindo que diversas redes operem em dual stack. O IPv6 foi criado para superar limitações estruturais do IPv4, oferecendo um espaço massivo de endereços, mais flexibilidade e novos mecanismos de autoconfiguração. Este módulo apresenta a estrutura dos endereços IPv6, seus principais tipos e as formas de configurá-los manualmente ou dinamicamente, além da segmentação em sub-redes.

🎯 Objetivo do módulo   
Implementar um esquema de endereçamento IPv6.

✅ Objetivos Específicos   
- Problemas do IPv4: Apresentação das limitações técnicas do IPv4 que levaram ao desenvolvimento do IPv6, incluindo exaustão de endereços e incapacidade de atender ao crescimento das redes.
- Representação do Endereço IPv6: Descrição da forma como os endereços IPv6 são escritos, abreviados e interpretados, considerando blocos hexadecimais e regras de compressão.
- Tipos de Endereço IPv6: Comparação entre os principais tipos de endereços IPv6, como unicast global, link-local, multicast e outros usados em operações de rede.
- Configuração Estática do GUA e do LLA: Explicação sobre como definir manualmente endereços unicast globais e endereços link-local diretamente nas interfaces.
- Endereçamento Dinâmico para GUAs IPv6: Apresentação dos métodos automáticos de obtenção de endereços unicast globais, incluindo DHCPv6 e SLAAC.
- Endereçamento Dinâmico para LLAs IPv6: Demonstração de como endereços link-local são gerados automaticamente a partir das propriedades da interface.
- Endereços Multicast IPv6: Identificação dos grupos multicast e suas finalidades dentro do funcionamento do protocolo IPv6.
- Sub-rede de uma Rede IPv6: Implementação de um conjunto organizado de sub-redes IPv6, utilizando prefixos e planejamento estruturado de endereçamento.

<a name="item12.02"><h4>12.2 Problemas do IPv4</h4></a>[Back to summary](#item12)

🌍 O porquê da transição para o IPv6   
O esgotamento do IPv4 não é mais uma previsão — é uma realidade. O IPv6 surgiu como substituto natural justamente para resolver esse limite. Ele trabalha com endereços de 128 bits, abrindo um espaço praticamente inesgotável. Esse novo protocolo não é apenas “mais IPs”; ele traz melhorias estruturais que corrigem limitações antigas do IPv4 e preparam a Internet para um cenário muito mais amplo.

🧰 Melhorias incorporadas ao IPv6   
A definição do IPv6 permitiu que a IETF revisasse pontos fracos do IPv4 e introduzisse avanços importantes. Um dos exemplos mais evidentes é o ICMPv6, que não apenas mantém funções básicas do ICMP tradicional, mas também incorpora recursos essenciais, como resolução de endereços e autoconfiguração — capacidades que não existiam no ICMPv4. Isso torna a operação em redes IPv6 mais autônoma e eficiente.

📉 O esgotamento do IPv4 pelo mundo   
Com a expansão da Internet para regiões que antes tinham pouca infraestrutura, a demanda por endereços cresceu rapidamente. A maioria dos RIRs já atingiu o limite de distribuição de endereços IPv4 há anos, mostrando que não há mais como sustentar o crescimento global apenas com esse protocolo. Enquanto isso, o IPv6 permanece praticamente ilimitado, oferecendo o caminho mais seguro para a evolução da Internet.

🛑 Limitações do IPv4 e o papel do NAT   
O IPv4 oferece pouco mais de 4 bilhões de endereços, número insuficiente para suportar o volume atual de usuários e dispositivos. O uso de endereços privados combinado ao NAT foi essencial para prolongar a vida útil do IPv4, mas isso trouxe impactos:
- cria complexidade adicional;
- pode causar lentidão;
- dificulta comunicações diretas entre dispositivos.

Para muitas aplicações modernas, especialmente as que dependem de conexões peer-to-peer, o NAT é um obstáculo significativo.

📱 A adoção crescente do IPv6   
Operadoras móveis foram pioneiras na migração porque precisam lidar com milhões de dispositivos que acessam a Internet diariamente. Em várias delas, mais de 90% do tráfego já utiliza IPv6. Grandes provedores de conteúdo e empresas globais também avançaram nesse caminho, migrando serviços externos e até redes internas para o novo protocolo. Esse movimento mostra que a adoção já está consolidada entre quem precisa de grande escala.

🔗 IPv6 em um mundo cheio de dispositivos   
A Internet mudou profundamente. Hoje, não se trata apenas de computadores e smartphones: sensores, eletrodomésticos, sistemas automotivos e equipamentos médicos também precisam se comunicar. Essa evolução, conhecida como Internet das Coisas, demanda um número de endereços muito maior do que o IPv4 pode fornecer. O IPv6 nasceu exatamente para suportar esse cenário massivo.

🚀 Por que a migração é inevitável   
Com mais usuários conectados, aumento de dispositivos inteligentes, insistência das grandes empresas no uso de IPv6 e esgotamento quase total do IPv4, a transição não é mais opcional — é questão de tempo. Não existe uma data limite, e o processo será gradual, com os dois protocolos convivendo por anos. Mesmo assim, caminhar para o IPv6 nativo é o objetivo final.

🧩 Métodos de transição para o IPv6   
A IETF definiu ferramentas e técnicas para permitir que redes façam a migração sem interrupções. Elas se dividem em três abordagens:
- Pilha dupla: Permite que os dispositivos utilizem IPv4 e IPv6 ao mesmo tempo. É a opção ideal quando há suporte total ao IPv6 pela rede e pelo provedor, permitindo acesso direto via IPv6.
- Tunelamento: Encapsula pacotes IPv6 dentro de pacotes IPv4 para atravessar redes que ainda não suportam o novo protocolo. Funciona como um “corredor temporário” durante a transição.
- Conversão: Usa mecanismos como NAT64 para permitir que hosts IPv6 e IPv4 se comuniquem. O tráfego é traduzido de um protocolo para o outro, garantindo compatibilidade durante o período de coexistência.

Essas duas últimas técnicas devem ser usadas apenas quando necessário. A meta sempre é alcançar comunicação nativa de ponta a ponta em IPv6.

<a name="item12.03"><h4>12.3 Representação do Endereço IPv6</h4></a>[Back to summary](#item12)

🧱 Estrutura básica de um endereço IPv6   
Para começar a trabalhar com IPv6, é essencial entender como os endereços são montados e escritos. Eles possuem 128 bits, bem maiores que os do IPv4, o que praticamente elimina o risco de esgotamento. Diferente da escrita decimal do IPv4, o IPv6 utiliza valores hexadecimais — cada grupo de 4 bits vira um dígito hex, resultando em 32 dígitos no total. A escrita aceita letras maiúsculas ou minúsculas, sem distinção.

🔢 Organização em hextetos   
Os 128 bits de um endereço são divididos em oito blocos de 16 bits. Cada bloco é formado por quatro dígitos hexadecimais, e a formatação tradicional coloca esses blocos separados por dois-pontos, no formato: `x:x:x:x:x:x:x:x`. Cada “x” representa um hexteto — termo usado informalmente para esses grupos de 16 bits. Essa é a forma completa do endereço, sem nenhuma abreviação, exibindo todos os 32 dígitos hexadecimais.

✂️ Regras para encurtar a escrita   
Como a forma completa pode ficar longa, o IPv6 permite duas reduções para simplificar a visualização. A primeira consiste em remover zeros iniciais dentro de um hexteto. Isso deixa a notação mais leve, sem alterar o valor real do endereço. A regra vale apenas para zeros à esquerda, pois remover zeros à direita mudaria o significado do hexteto.

Exemplos válidos:
- 01AB → 1AB
- 09f0 → 9f0
- 0a00 → a00

Zerar apenas o começo evita ambiguidades e mantém a interpretação correta do valor.

🚪 Uso do :: para substituir hextetos zerados   
A segunda técnica de redução utiliza o símbolo `::` para representar uma sequência contínua de hextetos formados apenas por zeros. Isso permite encurtar significativamente endereços que possuam longas áreas vazias. Esse recurso só pode aparecer uma única vez no endereço, justamente para evitar múltiplas interpretações.

Exemplo de compactação válida:
- Forma completa: `2001:db8:cafe:1:0:0:0:1`.
- Forma reduzida: `2001:db8:cafe:1::1`.
- Aqui, os três hextetos 0:0:0 viraram ::.

O erro mais comum é tentar usar `::` mais de uma vez no mesmo endereço. Quando isso acontece, surgem múltiplas expansões possíveis, e o endereço deixa de ser válido. Por exemplo: `2001:db8::abcd::1234`. Esse formato é inválido porque duas compressões aparecem ao mesmo tempo, e várias interpretações seriam possíveis ao expandir os zeros ocultos.

🧭 Boas práticas ao compactar   
Quando um endereço possui mais de uma sequência de hextetos zerados, a recomendação é usar `::` apenas na maior sequência. Caso duas sequências tenham o mesmo tamanho, aplica-se a compactação na primeira. Essa convenção mantém a escrita organizada e reduz a chance de interpretações dúbias, garantindo um padrão consistente entre diferentes administradores de rede.

<a name="item12.03.01"><h4>12.3.1 Verifique sua compreensão - Representação de endereço IPv6</h4></a>[Back to summary](#item12)

O objetivo desta atividade foi converter os endereços IPv6 em formatos curtos e compactos (omita os zeros à esquerda).
- IPv6: 2001:0000:0db8:1111:0000:0000:0000:0200
  - Remover zeros à esquerda: 2001:0:db8:1111:0:0:0:200
  - Formato Compacto: 2001:0:db8:1111::200

- IPv6: fe80:0000:0000:0000:0000:0000:0101:1111
  - Remover zeros à esquerda: fe80:0:0:0:0:0:101:1111
  - Formato Compacto: fe80::101:1111

- IPv6: 1031:1976:0001:0002:0003:0004:0000:0101
  - Remover zeros à esquerda: 1031:1976:1:2:3:4:0:101
  - Formato Compacto: 1031:1976:1:2:3:4::101

<a name="item12.04"><h4>12.4 Tipos de Endereço IPv6</h4></a>[Back to summary](#item12)

🌐 Tipos de Endereços IPv6   
Assim como no IPv4, o IPv6 possui diferentes categorias de endereços. Os três grupos principais são:
- Unicast: identifica uma única interface em um dispositivo.
- Multicast: permite enviar um pacote para vários destinos ao mesmo tempo.
- Anycast: é um endereço unicast atribuído a vários dispositivos; o tráfego vai para o mais próximo.

Diferente do IPv4, o IPv6 não possui broadcast. O papel é substituído pelo multicast para “todos os nós”.

🧩 Comprimento do Prefixo (/)   
No IPv4 existe o prefixo (ex.: /24) e também a máscara decimal. No IPv6, não existe máscara decimal com pontos, tudo é feito apenas com notação de barra.
- O comprimento pode variar de /0 a /128.
- Para LANs, o padrão recomendado é /64, pois o SLAAC usa 64 bits para o ID da interface.
- Usar /64 facilita planejamento, automação e criação de sub-redes.

🧭 Endereços Unicast   
Um endereço unicast identifica exclusivamente uma interface. O pacote chega somente naquele dispositivo. Os dispositivos IPv6 normalmente têm dois endereços unicast, não apenas um:
- Global Unicast Address (GUA): Equivalente ao IPv4 público. É roteável na Internet, globalmente único e pode ser configurado manualmente ou distribuído dinamicamente.
- Link-Local Address (LLA):
  - Necessário para qualquer dispositivo IPv6.
  - Funciona somente no link local (mesma sub-rede).
  - Não é roteável, e roteadores descartam pacotes cujo destino/origem seja LLA.
- Existe também o Unique Local Address (ULA), mas ainda pouco usado.

🏠 Unique Local Address (ULA)   
Intervalo fc00::/7 a fdff::/7. É parecido com o conceito de IPv4 privado (RFC 1918), mas com diferenças importantes:
- Serve para uso interno/local entre um ou poucos sites.
- Não deve ser roteado globalmente.
- Não depende de tradução de endereços.

Esses endereços podem, no futuro, ser usados para equipamentos internos (como impressoras ou servidores).

🌍 Global Unicast (GUA) em Detalhes   
O GUA é o endereço roteável na Internet IPv6. Ele equivale ao IPv4 público. O ICANN/IANA entrega faixas para os RIRs; atualmente os GUAs começam com 2000::/3 (endereços iniciados com 2 ou 3). O bloco 2001:db8::/32 é reservado para exemplos e documentação.

- Estrutura do GUA:
  - O endereço global unicast possui três partes:
    - Prefixo de roteamento global: geralmente fornecido pelo ISP; comum o uso de /48.
    - ID da sub-rede: parte usada pela organização para dividir sua rede.
    - ID da interface: equivalente à parte host no IPv4.
  - Com um prefixo típico /48, os 48 primeiros bits são a rede do ISP.
  - Usando o /64 recomendado, ficam 16 bits (1 hexteto) para identificar sub-redes internas.

Observação importante: Organizações que recebem um prefixo /32 podem ter até 4,3 bilhões de sub-redes /64, cada uma com 18 quintilhões de dispositivos.

🔌 ID da Interface   
No IPv6, o ID da interface equivale ao “host” no IPv4. Um /64 deixa 64 bits para o ID da interface — quantidade gigantesca de endereços. Diferente do IPv4, no IPv6 todos os 0s e todos os 1s podem ser usados como endereços válidos, já que o protocolo não usa broadcast. O uso de /64 é recomendado porque:
- Permite SLAAC criar ID de interface automaticamente.
- Simplifica o planejamento e o gerenciamento das sub-redes.

🔗 Link-Local (LLA)   
O LLA permite comunicação com outros dispositivos no mesmo link. Ele é obrigatório — mesmo que o dispositivo não tenha GUA. Intervalo: fe80::/10. Se não for configurado manualmente, o equipamento gera seu próprio LLA automaticamente, usando:
- Valores aleatórios;
- O método EUI-64 (gerado a partir do MAC).

Os LLAs são usados inclusive para o gateway padrão, já que o roteador costuma anunciar e utilizar seu endereço local.

Existem duas formas como um dispositivo obtém o LLA:
- Estático: configurado manualmente.
- Dinâmico: gerado automaticamente pelo próprio dispositivo, sem DHCP.

<a name="item12.05"><h4>12.5 Configuração Estática do GUA e do LLA</h4></a>[Back to summary](#item12)

🌐 GUA e LLA no IPv6   
As GUAs no IPv6 funcionam como os endereços públicos do IPv4: são únicas globalmente e roteáveis na Internet. Já os endereços LLA permitem comunicação apenas entre dispositivos no mesmo link (mesma sub-rede). É simples configurar GUAs e LLAs estaticamente em roteadores Cisco, e isso ajuda bastante na criação de uma rede IPv6 básica.

A maior parte dos comandos IPv6 no IOS é idêntica aos do IPv4, mudando apenas o prefixo `ipv6` no lugar de `ip`. No IPv4, um endereço é configurado com `ip address ip mask`. No IPv6, o equivalente é `ipv6 address endereço/prefixo`. Sem espaço entre o endereço e o comprimento do prefixo. 

O exemplo utiliza três sub-redes e aplica a configuração de GUA nas interfaces G0/0/0, G0/0/1 e Serial 0/1/0 do R1:
- `2001:db8:acad:1:/64`
- `2001:db8:acad:2:/64`
- `2001:db8:acad:3:/64`

🖥️ Configuração de GUA em Host Windows   
Configurar o IPv6 manualmente no Windows segue a mesma lógica do IPv4. No PC1, o gateway padrão foi configurado como 2001:db8:acad:1::1, que é o GUA da interface do R1 nessa rede. Também seria possível configurar o gateway usando o LLA do roteador, o que é até considerado prática recomendada. Ambos funcionam, mas o uso do LLA evita dependência de um endereço global.

Assim como no IPv4, configurar endereços manualmente em hosts não escala. Por isso, redes reais utilizam métodos automáticos. Existem duas formas de atribuição automática de GUAs: 
- SLAAC
- DHCPv6 com estado

Quando qualquer um desses métodos é usado, o gateway padrão já é configurado automaticamente como o LLA do roteador.

🔗 Configuração Manual de LLA   
Criar o LLA manualmente torna o endereço mais reconhecível, o que é útil em roteadores, já que seus LLAs servem como gateway padrão e são usados em mensagens de roteamento. O comando utilizado é `ipv6 address endereço link-local`. Qualquer endereço entre fe80 e febf é válido para LLA, mas é obrigatório usar o parâmetro link-local quando configurado manualmente.

No exemplo, o R1 usa um padrão fácil de identificar: todos os LLAs começam com `fe80::1:n`, onde o “1” indica o roteador R1, e “n” muda conforme a interface. Se existisse um R2 no diagrama, seguiria o mesmo padrão:
- `fe80::2:1`
- `fe80::2:2`
- `fe80::2:3`

O mesmo LLA poderia ser reutilizado em links diferentes, já que LLAs só precisam ser únicos dentro da própria sub-rede. Porém, a prática comum é usar um endereço diferente em cada interface para facilitar identificação.

<a name="item12.05.01"><h4>12.5.1 Verificador de Sintaxe - Configuração Estática GUA e LLA</h4></a>[Back to summary](#item12)

- Configure e ative o IPv6 na interface Gigabit Ethernet 0/0/0 com os seguintes endereços:
  - Use g0/0/0 como o nome da interface: `interface g0/0/0`.
  - LLA - fe80::1:1: `ipv6 address fe80::1:1 link-local`.
  - GUA - 2001:db8:acad:1::1/64: `ipv6 address 2001:db8:acad:1::1/64`.
  - Ative a interface: `no shutdown`
  - Saia do modo de configuração de interface: `exit`.
- Configure e ative o IPv6 na interface Gigabit Ethernet 0/0/1 com os seguintes endereços:
  - Use g0/0/1 como o nome da interface: `interface g0/0/1`.
  - LLA - fe80::2:1: `ipv6 address fe80::2:1 link-local`.
  - GUA - 2001:db8:acad:2::1/64: `ipv6 address 2001:db8:acad:2::1/64`.
  - Ative a interface: `no shutdown`.
  - Saia do modo de configuração de interface.: `exit`.
- Configure e ative o IPv6 na interface Gigabit Ethernet 0/1/0 com os seguintes endereços:
  - Use s0/1/0 como o nome da interface: `interface s0/1/0`.
  - LLA - fe80::3:1: `ipv6 address fe80::3:1 link-local`.
  - GUA - 2001:db8:acad:3::1/64: `ipv6 address 2001:db8:acad:3::1/64`.
  - Ative a interface: `no shutdown`.
  - Saia do modo de configuração de interface.: `exit`.

<a name="item12.06"><h4>12.6 Endereçamento dinâmico para GUAs IPv6</h4></a>[Back to summary](#item12)

🌐 Mensagens RA, RS e os métodos de obtenção dinâmica de endereços IPv6   
Quando não se deseja configurar manualmente os endereços unicast globais (GUAs) em cada dispositivo da rede, entra em cena o mecanismo nativo do IPv6 para atribuição automática. Essa atribuição dinâmica depende do uso de mensagens ICMPv6 — especificamente os anúncios de roteador (RA) e as solicitações de roteador (RS). Entender como esses dois tipos de mensagem funcionam é essencial para compreender como os dispositivos obtêm seus endereços e demais parâmetros de rede.

📡 Como o GUA é obtido dinamicamente   
Roteadores habilitados para IPv6 enviam periodicamente mensagens RA para todos os dispositivos do link. Essas mensagens incluem informações sobre a rede, como prefixo e endereço do gateway padrão. Se um host estiver recém-conectado e não quiser aguardar o próximo anúncio periódico, poderá enviar uma RS, solicitando que o roteador responda imediatamente com um novo RA.

🛠️ Pré-requisito: habilitar roteamento IPv6 no roteador   
Para que um roteador envie mensagens RA, ele precisa estar configurado para encaminhar pacotes IPv6. Isso é ativado no modo de configuração global com `ipv6 unicast-routing`. Sem esse comando, nenhum anúncio será enviado.

🧩 O que existe dentro de uma mensagem RA   
A mensagem RA dá ao host uma orientação de como obter seu endereço IPv6. Entre os dados fornecidos, estão:
- Prefixo da rede e o tamanho do prefixo.
- Gateway padrão, que é sempre o endereço link-local (LLA) da interface do roteador.
- Informações opcionais, como servidores DNS e nome de domínio (dependendo do método utilizado).

Apesar de o roteador sugerir o método, o sistema operacional do host decide como irá gerar o endereço.

🔀 Os três métodos possíveis de RA   
Existem três formas pelas quais o RA direciona o host a obter suas configurações:
- Somente SLAAC: O roteador fornece todas as informações necessárias para que o host crie o próprio GUA. Não há necessidade de DHCPv6. O host usa o prefixo fornecido pelo RA e cria o ID da interface.
- SLAAC + DHCPv6 Stateless: O host ainda cria o próprio GUA usando SLAAC, mas precisa consultar um servidor DHCPv6 para obter informações adicionais, como DNS e nome de domínio. Esse DHCPv6 não entrega endereços, apenas parâmetros extras.
- DHCPv6 Stateful (sem SLAAC): O roteador apenas envia o gateway padrão via RA e orienta o host a obter todo o restante com o DHCPv6 stateful. Nesse modo, o DHCPv6 mantém registro dos endereços alocados, assim como no IPv4. As informações fornecidas pelo DHCPv6 são as seguintes:
  - GUA;
  - Tamanho do prefixo;
  - DNS;
  - Nome de domínio.

🔧 SLAAC em detalhes   
O SLAAC permite que o host forme seu endereço sozinho. Nesse processo, o endereço é construído por duas partes:
- Prefixo recebido no RA.
- ID da interface, criado de duas maneiras possíveis:
  - EUI-64, baseado no MAC
  - Valor aleatório de 64 bits, dependendo do sistema operacional

Sistemas atuais tendem a preferir IDs aleatórios por questões de privacidade.

🆔 Como funciona o EUI-64   
O método EUI-64 transforma o MAC Ethernet de 48 bits em um identificador de 64 bits. Isso ocorre em três etapas principais:
- Separar o MAC entre OUI (metade esquerda) e identificador de dispositivo (metade direita).
- Inserir o valor fffe entre essas duas partes.
- Inverter o sétimo bit da primeira parte (bit U/L).

O resultado é um ID de interface determinístico, fácil de rastrear — motivo pelo qual muitos sistemas modernos preferem IDs aleatórios.

🔒 Por que IDs aleatórios existem?   
O uso de EUI-64 expõe o endereço MAC, o que permite rastrear um dispositivo ao longo de diferentes redes. Para evitar esse tipo de identificação, vários sistemas — como Windows desde o Vista — adotam um ID gerado aleatoriamente, mantendo a privacidade do usuário.

✔️ Garantindo que o endereço não esteja duplicado   
Depois que a interface cria seu identificador (seja via EUI-64 ou aleatório), o host realiza a Detecção de Endereço Duplicado (DAD). É uma verificação equivalente a perguntar na rede: “Alguém já está usando esse endereço?”. Se não houver resposta, o endereço é considerado seguro para uso.

<a name="item12.07"><h4>12.7 Endereçamento Dinâmico para LLAs IPv6</h4></a>[Back to summary](#item12)

💻 Endereço IPv6 de Link Local (LLA)   
Todos os dispositivos que usam o Protocolo de Internet versão 6 (IPv6) precisam de um Endereço de Link Local (LLA). O LLA tem um papel fundamental, permitindo a comunicação dentro do mesmo segmento de rede (ou "link"), mesmo que não haja um roteador ou um endereço global configurado.

🔄 Geração Dinâmica de LLAs   
Assim como os Endereços Unicast Globais (GUAs), os LLAs podem ser criados dinamicamente pelos próprios dispositivos. O LLA é sempre construído utilizando o prefixo FE80::/10 e uma ID de Interface de 64 bits. A parte da ID da Interface pode ser gerada de duas formas principais:
- Processo EUI-64: Utiliza o endereço MAC da interface (48 bits) e insere FFFE no meio, resultando em 64 bits.
- Geração Aleatória: Um número de 64 bits é gerado aleatoriamente para ser usado como a ID.

É comum que sistemas operacionais como o Windows utilizem o mesmo método de geração (aleatório ou EUI-64) tanto para o LLA atribuído dinamicamente quanto para um GUA criado por meio do SLAAC.

⚙️ LLAs em Roteadores Cisco   
Nos roteadores Cisco, a criação de LLAs é simplificada. O roteador gera automaticamente um LLA para uma interface sempre que um Endereço Unicast Global (GUA) é atribuído a ela. Por padrão, o Cisco IOS utiliza o processo EUI-64 para criar a ID da interface do LLA.

É importante notar uma particularidade nas interfaces seriais: como elas não possuem um endereço MAC nativo, o Cisco IOS normalmente utiliza o endereço MAC da primeira interface Ethernet disponível no roteador para gerar o LLA da interface serial. Isso é permitido porque os endereços de link local só precisam ser exclusivos dentro do seu link. No entanto, o uso da ID de interface longa gerada dinamicamente pelo EUI-64 pode dificultar a identificação e a lembrança dos endereços. Por isso, muitos administradores preferem configurar estaticamente os LLAs em roteadores para facilitar o gerenciamento.

🔍 Verificação de Endereçamento IPv6  
A verificação é uma etapa crucial para garantir que os endereços IPv6 estejam configurados e operando corretamente. O comando `show ipv6 interface brief` é a principal ferramenta para uma visão rápida. A saída desse comando exibe:
- O estado da interface (indicado por `[up/up]`).
- O GUA configurado.
- O LLA (o endereço que começa com FE80).
- O endereço MAC da interface (para interfaces Ethernet).

Note que cada interface terá pelo menos dois endereços: o LLA, que é adicionado automaticamente, e o GUA.

🗺️ Verificando a Tabela de Roteamento   
O comando `show ipv6 route` permite verificar quais redes e endereços IPv6 foram instalados na tabela de roteamento. Uma rota marcada com C (Connected) é adicionada quando uma interface está configurada com um GUA e está no estado operacional. Isso representa o prefixo da rede diretamente conectada.

Além disso, o endereço IPv6 Unicast Global configurado na interface também é instalado na tabela como uma rota local, marcada com L (Local) e um prefixo /128. As rotas locais são utilizadas pela tabela de roteamento para processar de forma eficiente pacotes destinados ao endereço da própria interface do roteador. É fundamental lembrar que os Endereços de Link Local (LLAs) não são incluídos na tabela de roteamento do roteador, pois eles não são endereços roteáveis.

🌐 Testando a Conectividade   
O comando `ping` em IPv6 é idêntico ao usado no IPv4 e serve para verificar a conectividade da Camada 3. Ao tentar realizar um `ping` de um roteador para um LLA de destino, o Cisco IOS solicitará que o usuário especifique a interface de saída. Esta exigência se deve ao fato de que o endereço de link local de destino pode estar em um ou mais links conectados ao roteador, e o dispositivo precisa saber exatamente para qual interface enviar o tráfego.

<a name="item12.07.01"><h4>12.7.1 Verificador de sintaxe - Verifique a configuração do endereço IPv6</h4></a>[Back to summary](#item12)

- Insira o comando show que exibirá um breve resumo do status das interfaces IPv6: `show ipv6 interface brief`.
- Verifique a conectividade de R1 para PC2 em 2001:db8:acad:1: :10: `show ipv6 route` e  `ping 2001:db8:acad:1::10`.

<a name="item12.08"><h4>12.8 Endereços IPv6 Multicast</h4></a>[Back to summary](#item12)

🌐 Multicast IPv6   
Depois de ver as categorias gerais de endereços IPv6, agora o foco é o funcionamento dos endereços multicast. Eles existem tanto no IPv4 quanto no IPv6, mas no IPv6 aparecem de forma mais estruturada e são identificados pelo prefixo ff00::/8. Importante lembrar: endereço multicast só pode ser usado como destino, nunca como origem.

📡 Endereços multicast comuns   
Há grupos multicast reservados para funções específicas da própria pilha IPv6. Esses grupos reúnem dispositivos que compartilham algum papel em comum. Entre os mais importantes:
- ff02::1 — Grupo de todos os nós: Todos os dispositivos IPv6 entram automaticamente nesse grupo. Qualquer pacote enviado para esse endereço é recebido por todos os hosts do link. Na prática, cumpre um papel parecido com o broadcast do IPv4. Mensagens RA costumam ser enviadas para esse grupo.
- ff02::2 — Grupo de todos os roteadores: Dispositivos só entram aqui quando operam como roteadores IPv6 (habilitados com `ipv6 unicast-routing`). Mensagens RS são destinadas a esse grupo, permitindo que hosts solicitem informações de configuração ao roteador do link.

🎯 Endereço multicast solicitado pelo nó   
Existe ainda um tipo especial chamado solicited-node multicast. Ele funciona como uma versão otimizada do grupo “todos os nós”. Cada dispositivo gera seu próprio endereço multicast solicitado a partir do seu IPv6, criando um grupo muito menor e específico. A vantagem é simples: a placa de rede pode verificar apenas o MAC associado a esse grupo multicast específico, evitando repassar pacotes desnecessários para a pilha IPv6. Isso reduz tráfego interno e melhora o desempenho do processo de verificação de destino.

<a name="item12.09"><h4>12.9 Sub-rede de uma rede IPv6</h4></a>[Back to summary](#item12)

📏 Introdução ao Sub-Redeamento em IPv6   
A criação de sub-redes (sub-redeamento) em IPv6 é, de fato, mais simples e planejada do que em IPv4. No IPv4, a sub-rede foi uma funcionalidade adicionada posteriormente, exigindo que os administradores "emprestassem" bits da porção de host para criar novas sub-redes. Em contraste, o IPv6 foi projetado desde o início com o sub-redeamento em mente, utilizando um campo dedicado para essa finalidade.

🆔 O Campo ID da Sub-Rede   
O Endereço Unicast Global (GUA) IPv6 possui um campo específico chamado ID da Sub-Rede.
- Localização: Este campo está posicionado entre o Prefixo de Roteamento Global (a parte da rede) e o ID da Interface (a parte do host).
- Vantagem do 128 Bits: Devido ao vasto espaço de endereçamento de 128 bits, não há preocupação com a conservação de endereços. O IPv6 oferece endereços de host e sub-redes mais do que suficientes para qualquer rede.

🔢 Capacidade de Sub-Redeamento   
Ao usar um prefixo de roteamento global comum, como /48, e mantendo 64 bits para o ID da Interface (o padrão para hosts), obtém-se um campo de ID da Sub-Rede de 16 bits. Este campo de 16 bits fornece uma capacidade imensa: 
- **Sub-redes**: Permite a criação de até 2^{16}, ou 65.536 sub-redes distintas.
- **Hosts por Sub-Rede**: Os 64 bits restantes do ID da Interface suportam até 2^{64}, o que equivale a 18 quintilhões de endereços de host por sub-rede.

> **Nota**: Embora seja tecnicamente possível realizar o sub-redeamento dentro dos 64 bits do ID da Interface (a porção de host), isso raramente é necessário devido ao grande número de sub-redes já disponíveis no campo ID da Sub-Rede.

➕ Implementação Simplificada  
A implementação do sub-redeamento em IPv6 é facilitada porque não exige conversões binárias complexas. Para identificar a próxima sub-rede disponível, o administrador simplesmente incrementa o valor do ID da Sub-Rede em ordem hexadecimal.

Exemplo de Sub-Redeamento: Suponha que uma organização receba o prefixo de roteamento global 2001:db8:acad::/48. Usando o ID da Sub-Rede de 16 bits, o administrador pode criar sub-redes simplesmente incrementando o hexteto correspondente:
- Sub-rede 1: 2001:db8:acad:0001::/64
- Sub-rede 2: 2001:db8:acad:0002::/64
- Sub-rede N: 2001:db8:acad:FFFF::/64

O prefixo de roteamento global (2001:db8:acad) permanece inalterado. Apenas o hexteto do ID da Sub-Rede é modificado.

🗺️ Design do Esquema de Endereçamento   
Com mais de 65.536 sub-redes disponíveis, a principal tarefa do administrador é projetar um esquema lógico para atribuir esses endereços à rede.
- Sub-Redes de Link Serial: Diferentemente do IPv4, no IPv6, a sub-rede utilizada para um link serial entre roteadores deve ter o mesmo comprimento de prefixo padrão das LANs (ou seja, /64). Embora isso pareça um "desperdício" de endereços para um link que só precisa de dois hosts, a conservação de endereços não é uma preocupação no IPv6.
- Alocação: Em uma topologia de exemplo que requer cinco sub-redes (quatro LANs e um link serial), sub-redes com o campo ID de sub-rede de 0001 a 0005 podem ser alocadas, sendo que cada sub-rede /64 fornecerá endereços mais do que suficientes.

A configuração final em cada roteador envolve atribuir endereços IPv6 a cada interface, garantindo que cada interface pertença a uma sub-rede IPv6 diferente.

<a name="item12.10"><h4>12.10 Módulo Prático e Quiz</h4></a>[Back to summary](#item12)

🧭 Transição do IPv4 para o IPv6   
O espaço IPv4 já não comporta a quantidade atual de dispositivos conectados. Para permitir a evolução da Internet, adotou-se o IPv6, que convive com o IPv4 durante a migração. A transição ocorre usando três métodos: pilha dupla, encapsulamento e tradução, permitindo que redes antigas e novas funcionem ao mesmo tempo.

🌐 Formato e simplificação dos endereços IPv6   
Um endereço IPv6 tem 128 bits representados em oito blocos hexadecimais. Para facilitar a escrita, zeros à esquerda podem ser removidos e sequências longas de zeros podem ser substituídas por `::`, mas apenas uma vez por endereço. Isso torna endereços extensos muito mais curtos e legíveis.

🎯 Tipos de endereços IPv6 e funções   
O IPv6 utiliza unicast, multicast e anycast. Todo dispositivo possui um link-local para comunicação dentro da mesma rede e pode ter um global unicast (GUA) para acesso externo. Endereços locais exclusivos (ULA) servem para uso interno sem roteamento na Internet.

🛠️ Configuração de IPv6 no Cisco IOS   
A configuração difere do IPv4: GUAs usam o comando `ipv6 address X/64`, e link-local pode ser definido manualmente. Como configurações manuais não escalam, redes IPv6 normalmente adotam métodos automáticos.

📨 Atribuição dinâmica: RA, SLAAC e DHCPv6   
Roteadores enviam Router Advertisements (RA) contendo prefixo, gateway e parâmetros adicionais. Dependendo das flags, o host pode:
- criar seu próprio endereço (SLAAC);
- usar SLAAC + DHCPv6 sem estado;
- receber tudo via DHCPv6 com estado.

A parte final do endereço pode ser criada via EUI-64 ou gerada aleatoriamente.

🔗 Link-local e verificação   
Todos os dispositivos IPv6 precisam de um endereço link-local. Roteadores Cisco o geram automaticamente quando um GUA é configurado. A verificação é feita com `show ipv6 interface brief`, `show ipv6 route` e `ping`.

📢 Multicast IPv6   
O IPv6 depende fortemente de multicast. Existem grupos bem conhecidos, como `ff02::1` (todos os nós) e `ff02::2` (todos os roteadores). Também existe o solicited-node multicast, usado para substituir ARP e otimizar buscas por vizinhos.

🏗️ Sub-redes em IPv6   
O IPv6 já foi projetado para ter sub-redes abundantes. Um prefixo /48, por exemplo, oferece 65 mil sub-redes, cada uma com 18 quintilhões de endereços de host. Assim, o foco do administrador deixa de ser economizar espaço e passa a ser criar um esquema lógico de endereçamento.
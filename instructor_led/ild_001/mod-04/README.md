# CCNA: Introduction to Networks - Módulo 4   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_001 (CCNA: Introduction to Networks)   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="25"></a>
### Module: 4. Camada física

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

### Course Module 4 Structure:
4. <a name="item04">Camada física</a><br>
  4.1 <a href="#item04.01">Introdução</a><br>
  4.2 <a href="#item04.02">Propósito da camada física</a><br>
  4.3 <a href="#item04.03">Características da camada física</a><br>
  4.4 <a href="#item04.04">Cabeamento de Cobre</a><br>
  4.5 <a href="#item04.05">Cabeamento UTP</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;4.5.1 <a href="#item04.05.01">Atividade - Pinagem de cabos</a><br>
  4.6 <a href="#item04.06">Cabeamento de Fibra Óptica</a><br>
  4.7 <a href="#item04.07">Meios Sem Fio</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;4.7.1 <a href="../../../pkt/files/pkt_014/">Packet Tracer - Conecte uma Rede cabeada e sem Fio</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;4.7.2 <a href="../../../labs/files/lab_013/">Laboratório - Exibir informações de Placas de Rede com fio e sem fio</a><br>
  4.8 <a href="#item04.08">Módulo Prático e Quiz</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;4.8.1 <a href="../../../pkt/files/pkt_016/">Packet Tracer - Exploração de Camada Física</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;4.8.2 <a href="../../../pkt/files/pkt_017/">Packet Tracer - Conecte a Camada Física</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item04.01"><h4>4.1 Introdução</h4></a>[Back to summary](#item04)

📘 Introdução   
Este módulo explora a base física que sustenta qualquer rede de computadores. É nessa camada que os bits realmente percorrem cabos, fibras ou sinais sem fio, permitindo que toda a comunicação digital aconteça. Ao compreender como os diferentes tipos de mídia funcionam e como os dispositivos se conectam, torna-se possível montar e identificar corretamente as estruturas que dão vida à rede. As práticas e simulações acompanharam essa parte do curso para reforçar a compreensão sobre como montar conexões reais.

🎯 Objetivo Geral   
Apresentar como a camada física, seus protocolos, meios de transmissão e serviços tornam possível o envio de dados entre dispositivos.

✅ Objetivos Específicos   
- Explicar a função e o propósito da camada física dentro de uma rede.
- Identificar as principais características que definem o funcionamento dessa camada.
- Reconhecer os elementos essenciais do cabeamento de cobre.
- Descrever como o cabo UTP é aplicado em redes Ethernet.
- Apresentar as propriedades da fibra óptica e suas vantagens em relação a outros meios de transmissão.
- Mostrar como dispositivos podem ser conectados utilizando mídias físicas ou conexões sem fio.

<a name="item04.02"><h4>4.2 Propósito da camada física</h4></a>[Back to summary](#item04)

🔌 Conexões Físicas em Redes   
Antes de qualquer comunicação ocorrer, é necessário estabelecer uma conexão física com a rede local. Essa conexão pode ser realizada por meio de cabos ou por sinais sem fio, dependendo do tipo de rede e da infraestrutura disponível.

🧷 Conexões com Fio   
Em redes corporativas, computadores de mesa e laptops costumam ser conectados fisicamente a um switch compartilhado. Os dados trafegam por um cabo físico, caracterizando uma rede conectada de forma tradicional.

📡 Conexões Sem Fio   
Além das conexões cabeadas, redes corporativas e residenciais utilizam conectividade sem fio para notebooks, tablets e smartphones. A transmissão é feita por ondas de rádio, e os dispositivos se conectam a um ponto de acesso sem fio (AP) ou a um roteador sem fio.

🛠️ Componentes de um Ponto de Acesso   
Um ponto de acesso sem fio costuma incluir:
- Antenas sem fio internas ou externas;
- Portas de comutação Ethernet;
- Porta dedicada de acesso à internet.

🏠 Conectividade em Ambientes Residenciais   
Assim como nos ambientes corporativos, residências utilizam conexões com fio e sem fio. Roteadores domésticos fornecem acesso à LAN por meio de portas Ethernet e redes Wi-Fi.

💽 Placas de Interface de Rede (NICs)   
As NICs conectam dispositivos à rede:
- NIC Ethernet: usada para conexões com fio.
- NIC WLAN: usada para conexões sem fio.

Dispositivos podem ter uma ou ambas. Exemplos:
- Impressoras de rede podem ter apenas NIC Ethernet.
- Tablets e smartphones geralmente possuem apenas NIC WLAN.

⚡ Diferentes Níveis de Desempenho   
As conexões físicas variam em desempenho dependendo da tecnologia utilizada. Cabos, padrões Wi-Fi e meios físicos diferentes resultam em capacidades distintas de velocidade e estabilidade.

📶 Função da Camada Física   
A camada física do modelo OSI fornece os meios para transportar os bits que compõem um quadro da camada de enlace.

- Funções principais:
  - Receber um quadro da camada de enlace;
  - Codificar os bits como sinais elétricos, ópticos ou de rádio;
  - Transmitir esses sinais pelo meio físico;
  - No destino, recuperar os sinais e reconstruir os bits;
  - Entregar o quadro completo à camada de enlace de dados.

🔁 Processo de Encapsulamento na Camada Física   
Durante a transmissão:
- Os bits do quadro são convertidos em sinais adequados à mídia;
- Os sinais são enviados um a um;
- O dispositivo destino decodifica esses sinais;
- Os bits são recombinados para formar o quadro original;
- O quadro é entregue à camada de enlace para processamento.

<a name="item04.03"><h4>4.3 Características da camada física</h4></a>[Back to summary](#item04)

🧱 Papel da Camada Física   
Este tópico detalha os elementos que compõem a camada física: componentes, mídia, codificação e padrões que viabilizam o funcionamento correto da rede.

🏛️ Padrões e Organizações   
Os protocolos das camadas superiores são definidos pela IETF, mas a camada física depende de organizações de engenharia que padronizam cabos, conectores e sinais. A camada física é padronizada por diversas entidades:
- ISO;
- TIA/EIA;
- ITU;
- ANSI;
- IEEE;
- FCC;
- ETSI;
- Grupos regionais como CSA, CENELEC, JSA/JIS.

🧩 Áreas Funcionais da Camada Física   
A camada física define três funções principais:
- Componentes físicos;
- Codificação;
- Sinalização.

🔧 Componentes Físicos   
Incluem todos os elementos eletrônicos e de mídia que transportam bits:
- NICs;
- Interfaces e conectores;
- Materiais e padrões de cabos;
- Portas e interfaces de roteadores, como as do Cisco 1941.

🧾 Codificação (Line Encoding)   
A codificação converte o fluxo de bits em padrões reconhecíveis por emissores e receptores. Funciona como um “alfabeto” digital — semelhante ao código Morse. Exemplos:
- Manchester:
  - 0 = alta → baixa voltagem.
  - 1 = baixa → alta voltagem.
  - Usado em Ethernet 10BASE-T.
- 4B/5B: usado em 100BASE-TX
- 8B/10B: usado em 1000BASE-T

📶 Sinalização   
Define como os bits serão representados fisicamente. Um “1” e um “0” podem ser representados por:
- Pulsos elétricos;
- Pulsos de luz;
- Sinais de rádio.

Exemplos:
- Cobre: voltagem x tempo.
- Fibra óptica: pulsos de luz x tempo.
- Sem fio: micro-ondas x tempo.

📡 Mídia
Cada tipo de mídia possui características próprias que influenciam como os bits são transportados. A qualidade do meio (cobre, fibra, rádio) afeta diretamente velocidade, estabilidade e distância alcançada.

📶 Largura de Banda   
Largura de banda é a capacidade máxima que um meio físico pode enviar de dados por segundo. É o limite teórico da transmissão.

- Unidades:
  - bps;
  - Kbps = 10³ bps;
  - Mbps = 10⁶ bps;
  - Gbps = 10⁹ bps;
  - Tbps = 10¹² bps.

- O que Determina a Largura de Banda:   
Dois fatores principais definem a capacidade prática da rede:
  - Propriedades do meio físico.
  - Tecnologia usada para sinalização e detecção de sinais.

🕒 Latência   
Latência é o tempo que os dados levam para ir de um ponto a outro. Um único segmento lento pode se tornar o gargalo de toda a comunicação.

📤 Taxa de Transferência (Throughput)   
É a quantidade real de bits transmitidos por segundo. Geralmente é menor que a largura de banda por fatores como:
- Quantidade de tráfego;
- Tipo de tráfego;
- Número de dispositivos intermediários.

📦 Dados Úteis (Goodput)   
Goodput mede apenas os dados realmente utilizáveis, descontando:
- Overhead de sessões;
- Acks;
- Encapsulamento;
- Retransmissões;

Goodput < Throughput < Largura de banda

<a name="item04.04"><h4>4.4 Cabeamento de Cobre</h4></a>[Back to summary](#item04)

🧵 Cabeamento de Cobre   
O cabeamento de cobre é o tipo mais comum nas redes. Existem três tipos principais, usados conforme a necessidade do ambiente. É barato, fácil de instalar e tem baixa resistência elétrica, mas sofre limitações de distância e interferência.

⚡ Atenuação do Sinal   
Os dados viajam como pulsos elétricos. Quanto maior a distância percorrida, mais o sinal se deteriora — isso é a atenuação. Por isso os cabos de cobre possuem limites de distância definidos em padrões técnicos.

📡 Fontes de Interferência   
A temporização e voltagem dos sinais podem ser afetadas por:
- EMI/RFI (interferência eletromagnética e de radiofrequência):
  - Causada por motores, lâmpadas fluorescentes, equipamentos de rádio, etc.
  - Pode distorcer e corromper o sinal.
- Diafonia (Crosstalk):
  - Um fio interfere em outro fio adjacente.
  - O campo magnético gerado em um cabo pode ser captado pelo cabo ao lado.

🛡️ Métodos de Proteção   
Para reduzir interferências, utiliza-se:
- Blindagem metálica e aterramento adequado.
- Pares de fios trançados em direções opostas para reduzir crosstalk.
- Seleção correta da categoria do cabo.
- Projeto físico que evita fontes de interferência.
- Técnicas de instalação adequadas.

🪢 Tipos de Mídias de Cobre   
Três tipos principais são usados em redes:
- UTP (Unshielded Twisted Pair);
- STP (Shielded Twisted Pair);
- Coaxial;

🔌 Cabo UTP   
O tipo mais comum nas LANs. Usa conector RJ-45 e interliga hosts, switches e roteadores.

Características:
- 4 pares trançados codificados por cor.
- Capa externa para proteção física.
- Trançamento reduz interferência.
- Isolamento plástico com código de cores identifica cada par.

🛡️ Cabo STP   
Oferece proteção maior contra ruídos que o UTP. É mais caro e mais difícil de instalar. Também usa RJ-45, mas exige conectores blindados especiais.

Características:
- Blindagens individuais por par.
- Revestimento metálico externo.
- Redução de EMI, RFI e crosstalk.
- Necessita de aterramento correto — caso contrário age como antena.

📯 Cabo Coaxial   
Possui dois condutores no mesmo eixo. Composto por:
- Condutor interno de cobre.
- Isolamento plástico.
- Malha trançada ou folha metálica (blindagem).
- Revestimento externo.

Conectores comuns: BNC, N e F.

Usos atuais:
- Antenas e equipamentos sem fio (transporte de RF).
- Instalações de internet a cabo dentro das casas.

Características principais identificadas:
- Revestimento externo;
- Blindagem trançada;
- Isolante plástico;
- Condutor de cobre.

<a name="item04.05"><h4>4.5 Cabeamento UTP</h4></a>[Back to summary](#item04)

🧵 Visão Geral do Cabo UTP   
O UTP é o padrão mais utilizado em LANs. Ele contém quatro pares trançados, codificados por cor, dentro de uma capa plástica flexível. O tamanho reduzido facilita a instalação.

⚠️ Limitações e Soluções no UTP   
O UTP não possui blindagem, portanto depende de técnicas próprias para reduzir interferências.

- Cancelamento (Self-Shielding): O cancelamento ocorre porque os dois fios de um par têm campos magnéticos opostos, que se anulam. Isso reduz EMI, RFI e crosstalk.
- Variação de Torções por Par: Cada par possui um número diferente de torções por metro. Isso aumenta o efeito de cancelamento. Exemplo:
  - Par laranja ≠ par azul em quantidade de torções.
  - Essa padronização é obrigatória e definida por normas técnicas.

🛡️ Autoblindagem   
O UTP depende exclusivamente do trançamento e do cancelamento para manter a qualidade do sinal. Não há blindagem metálica.

📐 Padrões TIA/EIA   
O cabeamento UTP segue o TIA/EIA-568, que define:
- Tipos de cabo;
- Comprimentos máximos;
- Conectores;
- Métodos de terminação;
- Testes de cabo.

🔌 Classificação IEEE por Categoria   
O IEEE classifica os cabos UTP conforme o desempenho e a largura de banda suportada.

Categorias principais:
- Cat 3: originalmente voz; depois dados.
- Cat 5: 100 Mbps.
- Cat 5e: 1000 Mbps.
- Cat 6: separador interno; até 10 Gbps.
- Cat 7: até 10 Gbps.
- Cat 8: até 40 Gbps.
- Cat 5e é o mínimo atual; Cat 6 é recomendado para novas instalações.

🔗 Conector RJ-45   
O UTP normalmente usa o conector RJ-45, seguindo o padrão de pinagem TIA/EIA-568.
- RJ-45: plug macho prensado no cabo.
- Tomada / porta: conector fêmea no dispositivo, parede ou patch panel.

Uma terminação incorreta degrada o desempenho da camada física. Exemplos de Terminação
- Má terminação: fios expostos, pares destorcidos, capa curta.
- Boa terminação: pares mantidos torcidos até quase o conector, sem fios expostos.

🔃 Tipos de Cabo (Direto, Cruzado e Rollover)   
- Ethernet Direto (Straight-Through):
  - Ambas as pontas T568A ou T568B;
  - Usado para conectar: host → switch; switch → roteador.
- Ethernet Cruzado (Crossover):
  - Uma ponta T568A, outra T568B;
  - Usado para conectar dispositivos semelhantes: switch ↔ switch; host ↔ host; roteador ↔ roteador.
  - Hoje é legado porque NICs modernas usam Auto-MDIX (detectam automaticamente).
- Rollover:
  - Cabo proprietário Cisco;
  - Usado para conectar um PC à porta console de um roteador/switch.

❗ Uso Incorreto   
Usar cabo direto quando deveria ser cruzado (ou vice-versa) não danifica o equipamento, mas impede a conexão. É a primeira coisa a verificar ao solucionar problemas.

🧵 Padrões T568A e T568B   
Os padrões T568A e T568B definem a ordem dos fios dentro do conector RJ-45. A diferença entre eles está apenas na disposição dos pares e nas cores utilizadas.

Resumo prático:
- Direto: T568A em ambas as extremidades (A–A) ou T568B em ambas as extremidades (B–B);
- Cruzado: Uma ponta T568A e a outra T568B (A–B);
- Rollover: Padrão proprietário da Cisco usado para conexão via porta console.

<a name="item04.05.01"><h4>4.5.1 Atividade - Pinagem de cabos</h4></a>[Back to summary](#item04)

Para esta atividade, foi ordenado corretamente as cores do fio para uma pinagem de cabo TIA/EIA. 

Pinagem T568A:
- Verde com Branco;
- Verde;
- Laranja com Branco;
- Azul;
- Azul com Branco;
- Laranja;
- Marrom com Branco;
- Marrom.

Pinagem T568B:
- Laranja com Branco;
- Laranja;
- Verde com Branco;
- Azul;
- Azul com Branco;
- Verde;
- Marrom com Branco;
- Marrom.

<a name="item04.06"><h4>4.6 Cabeamento de Fibra Óptica</h4></a>[Back to summary](#item04)

📘 Cabeamento de Fibra Óptica   
O cabeamento de fibra óptica é a segunda grande categoria de meios físicos utilizados em redes, ao lado dos cabos de cobre. Apesar de ter um custo mais elevado, ele oferece benefícios que tornam sua utilização essencial em diversos cenários — especialmente quando o objetivo é transmitir dados a longas distâncias, com alta velocidade e praticamente sem interferências.

✨ Por que a fibra óptica é tão especial?   
A fibra óptica transporta informações usando pulsos de luz, em vez de sinais elétricos. Isso permite:
- Alcances muito maiores sem perda significativa de sinal.
- Larguras de banda extremamente altas, superiores a qualquer meio metálico.
- Imunidade total à interferência eletromagnética e de rádio, já que não conduz eletricidade.

Em outras palavras: quando a rede exige desempenho, estabilidade e longas distâncias, a fibra domina.

🔬 Como a fibra transmite dados   
A fibra é composta por um fio extremamente fino de vidro transparente. A luz viaja em seu interior “preso” por reflexões contínuas, como se a fibra fosse um túnel espelhado que guia a luz até o destino. Os bits são enviados como pulsos luminosos, interpretados no outro extremo como 0s e 1s.

Uma forma simples de imaginar: pense em um canudo longo por onde um ponto de laser percorre sem escapar pelas bordas. A fibra faz exatamente isso, só que com material muito mais refinado e em escalas microscópicas.

🧬 Tipos de fibra óptica   
Existem dois tipos principais, definidos pelo tamanho do núcleo e pela forma como a luz se propaga.

- Fibra Monomodo (SMF): 
  - O feixe segue praticamente em linha reta, o que reduz a dispersão e mantém a qualidade do sinal por longos percursos.
  - Envia apenas um único feixe de luz.
  - Usa lasers como fonte luminosa.
  - Ideal para grandes distâncias, chegando a quilômetros sem regeneração de sinal.
  - Aplicações típicas:
    - telecomunicações de longa distância;
    - provedores de internet;
    - interconexão entre cidades ou países.
  - Composição típica:
    - Núcleo: ~9 µm;
    - Revestimento: ~125 µm
- Fibra Multimodo (MMF):
  - Como existem vários “modos” de luz percorrendo a fibra, ocorre mais dispersão — limitando seu alcance a algumas centenas de metros.
  - Permite vários feixes de luz viajando simultaneamente por caminhos diferentes.
  - Utiliza LEDs como fonte de luz.
  - Usada principalmente em redes locais (LAN) e distâncias curtas.
  - Suporta até 10 Gb/s a certos comprimentos.
  - Composição típica:
    - Núcleo: 50 ou 62,5 µm;
    - Revestimento: ~125 µm;

🌀 Dispersão: o que limita a distância   
Dispersão é o fenômeno em que o pulso de luz se espalha ao longo do tempo. Quanto maior a dispersão, mais rapidamente o sinal se deteriora.
- MMF: dispersão maior → alcance menor.
- SMF: dispersão mínima → grandes distâncias.

É por isso que fibras multimodo raramente ultrapassam 500–600 metros em links de alta velocidade.

🏙 Onde a fibra óptica é usada?   
A tecnologia aparece em quatro grandes segmentos:
- Redes Corporativas: Backbone, links de alta capacidade, interligação de andares ou prédios.
- FTTH (Fiber to the Home): Entrega de banda larga direta para residências e pequenos negócios.
- Redes de Longo Alcance: Conexões entre cidades, regiões e países feitas por operadoras.
- Cabos Submarinos: Rotas oceânicas de altíssima capacidade que interligam continentes.

🔌 Conectores de Fibra Óptica   
As fibras precisam de conectores específicos para serem encaixadas em switches, roteadores ou transceptores SFP. Cada padrão varia em tamanho, formato e mecanismo de fixação.
- ST (Straight Tip):
  - Um dos primeiros padrões.
  - Fixação tipo baioneta (gira para travar).
- SC (Subscriber Connector):
  - Visual quadrado.
  - Muito popular em LAN/WAN.
  - Mecanismo push-pull (entra e trava ao pressionar).
- LC Simplex:
  - Versão reduzida do SC.
  - Muito usado em equipamentos modernos devido ao tamanho compacto.
- LC Duplex:
  - Variante com duas fibras lado a lado (transmissão e recepção).
  - Comum em multimodo.
- Observação: Diversos equipamentos oferecem portas de fibra usando transceptores SFP, que permitem trocar o tipo de mídia de forma modular.

🎨 Identificação visual das fibras   
A cor externa do cabo ajuda a identificar o tipo:
- Amarelo → fibras monomodo;
- Laranja → fibras multimodo.

Alguns exemplos comuns:
- SC–SC (SMF);
- LC–LC (SMF);
- ST–LC (MMF);
- SC–ST (SMF).

Lembre-se: conectores e extremidades da fibra devem ficar protegidos com tampas quando não estão em uso.

⚖️ Comparação: Cobre vs Fibra Óptica   
- Cobre (UTP):
  - Suporta entre 10 Mb/s e 10 Gb/s.
  - Alcance típico de até 100 metros.
  - Baixa imunidade contra EMI/RFI.
  - Conduz eletricidade, podendo apresentar riscos.
  - Custo baixo.
  - Instalação simples e rápida.
  - Segurança básica e mais fácil de interceptar.
- Fibra Óptica:
  - Suporta entre 10 Mb/s e 100 Gb/s.
  - Pode alcançar dezenas ou até centenas de quilômetros.
  - Totalmente imune a EMI/RFI.
  - Não conduz eletricidade, sendo mais segura.
  - Custo mais elevado.
  - Instalação mais complexa, exige habilidade especializada.
  - Segurança alta, muito difícil de interceptar.

🏢 Como a fibra é usada atualmente nas empresas   
Na maioria dos ambientes corporativos, a fibra serve como:
- Backbone interno que liga switches centrais.
- Conexões entre prédios em um campus corporativo.
- Links de alto tráfego entre data centers, salas de telecom e racks.

Por não conduzir eletricidade e sofrer pouca atenuação, ela é perfeita para percursos longos e ambientes sujeitos a interferência.

<a name="item04.07"><h4>4.7 Meios Sem Fio</h4></a>[Back to summary](#item04)

📡 O Que é a Mídia Sem Fio   
A mídia sem fio permite transmitir dados usando ondas eletromagnéticas, como rádio e micro-ondas. É graças a ela que dispositivos como tablets, notebooks e smartphones conseguem acessar redes sem depender de cabos.

🚶‍♂️ Mobilidade e Popularidade   
É a mídia com maior mobilidade entre todas. O número de dispositivos sem fio cresce a cada ano. Hoje, é o método principal de acesso em redes domésticas e muitas redes corporativas.

⚠️ Limitações do Meio Sem Fio   
- Área de Cobertura:
  - Funciona melhor em espaços abertos.
  - Paredes, estruturas metálicas e relevo podem reduzir o alcance.
- Interferência:
  - Suscetível a fontes como:
    - telefones sem fio;
    - lâmpadas fluorescentes;
    - micro-ondas;
    - outros sinais sem fio.
- Segurança:
  - Como o sinal se espalha pelo ar, qualquer dispositivo próximo pode tentar captar.
  - Por isso, redes sem fio exigem segurança rigorosa.
- Compartilhamento do Meio:
  - A mídia é compartilhada entre todos os usuários.
  - Muitos dispositivos conectados = menos largura de banda por usuário.
  - A comunicação costuma operar em half-duplex (um envia ou recebe por vez).

🧱 Onde o Sem Fio Não Substitui os Cabos   
Apesar da popularidade, cobre e fibra ainda são preferidos para:
- switches;
- roteadores;
- links de backbone;
- interconexões de alta capacidade.

📐 Padrões e Regulações   
Os padrões sem fio definem aspectos importantes, como:
- codificação dos dados no sinal;
- frequência usada;
- potência de transmissão;
- recepção e decodificação;
- características das antenas.

📶 Principais Tecnologias Sem Fio   
- Wi-Fi (IEEE 802.11):
  - Tecnologia de LAN sem fio.
  - Usa CSMA/CA, onde o dispositivo escuta antes de transmitir.
  - É o padrão mais comum em casas, empresas e hotspots.
- Bluetooth (IEEE 802.15):
  - Padrão para redes pessoais (WPAN).
  - Ideal para curtas distâncias: 1 a 100 metros.
  - Exige emparelhamento.
- WiMAX (IEEE 802.16):
  - Tecnologia ponto-multiponto para fornecer banda larga sem fio.
  - Menos comum hoje, mas projetada para longas distâncias.
- Zigbee (IEEE 802.15.4):
  - Baixa energia, baixa taxa de dados, longo tempo de bateria.
  - Muito usado em IoT, automação residencial e sensores.
- Outras Tecnologias:
  - Redes celulares (4G/5G);
  - Comunicação via satélite.

📡 Componentes de uma WLAN   
- Ponto de Acesso (AP):
  - Concentra conexões Wi-Fi.
  - Liga os dispositivos sem fio à rede cabeada.
  - Em residências, normalmente o AP já vem embutido no roteador.
- Adaptador de Rede Sem Fio (NIC Wi-Fi):
  - Permite que computadores e outros dispositivos se conectem por rádio.
  - Pode ser interno (notebooks) ou USB.

🔧 Compatibilidade de Equipamentos   
Ao adquirir dispositivos Wi-Fi, verifique:
  - suporte ao mesmo padrão (ex.: 802.11ac, 802.11ax);
  - compatibilidade de bandas (2.4 GHz / 5 GHz);
  - interoperabilidade entre marcas.

🛡️ Segurança: Prioridade Máxima   
Redes sem fio são convenientes, mas exigem cuidados:
- políticas de acesso;
- senhas fortes;
- criptografia adequada (WPA2 ou WPA3);
- monitoramento ativo.

Administradores devem tratar segurança em WLAN como um ponto crítico, já que o sinal pode ser captado além da área do prédio.

<a name="item04.08"><h4>4.8 Módulo Prático e Quiz</h4></a>[Back to summary](#item04)

📡 Conexão física e camada física   
Antes de qualquer comunicação de rede ocorrer, é necessário estabelecer uma conexão física — com fio (cabos) ou sem fio (ondas de rádio). As NICs conectam dispositivos à rede: NICs Ethernet para conexões com fio e NICs WLAN para conexões sem fio. A camada física do modelo OSI transporta os bits que formam os quadros da camada de enlace, convertendo-os em sinais adequados ao meio. Os dispositivos finais e intermediários recebem esses bits já codificados.

🔧 Funções e características da camada física   
A camada física reúne circuitos eletrônicos, meios e conectores definidos em padrões que tratam de três áreas: componentes físicos, codificação e sinalização.  
- **Largura de banda:** capacidade máxima do meio.  
- **Taxa de transferência:** quantidade real de bits transmitidos.  
- **Latência:** tempo total de viagem dos dados.  
- **Goodput:** apenas os dados realmente úteis transmitidos.

Cada mídia representa os bits de forma diferente:  
- **Cobre:** pulsos elétricos;
- **Fibra óptica:** pulsos de luz;
- **Wireless:** ondas de micro-ondas.

🧵 Mídia de cobre   
Muito usada por ser barata, fácil de instalar e apresenta baixa resistência elétrica, mas limitada por distância e interferência. Problemas comuns vêm de EMI e diafonia. Os principais tipos incluem:
- **UTP:** sem blindagem, usa torção dos pares para reduzir interferências.  
- **STP:** pares blindados individualmente e blindagem geral.  
- **Coaxial:** dois condutores no mesmo eixo; usado em antenas e provedores de TV a cabo.

O UTP segue padrões TIA/EIA e especificações elétricas IEEE, geralmente usando conectores RJ-45. Os principais padrões de fiação são:  
- **Straight-through**  
- **Crossover**  
- **Rollover (Cisco)** para acesso ao console.

💡 Fibra óptica   
Transmite dados a longas distâncias e com alta largura de banda, com baixa atenuação e total imunidade a EMI e RFI. É um filamento de vidro extremamente puro que codifica bits como luz. Usada em redes corporativas, FTTH, backbones de longa distância e cabos submarinos.  
- Conectores comuns: ST, SC, LC e LC multimodo duplex.  
- Cabos de patch típicos: SC-SC, LC-LC, ST-LC e SC-ST.  

Em empresas, a fibra é geralmente usada para backbone e interligação entre prédios.

🌐 Mídia sem fio   
Transporta sinais eletromagnéticos que representam bits via frequências de rádio ou micro-ondas. Suas limitações incluem: cobertura, interferência, segurança e compartilhamento do meio. Os padrões principais conteplam:
- **Wi-Fi (802.11)**  
- **Bluetooth (802.15)**  
- **WiMAX (802.16)**  
- **Zigbee (802.15.4)**  

Uma WLAN exige um ponto de acesso (AP) e NICs sem fio nos dispositivos.
# CyberOps Associate - Módulo 6   <img src="../0-aux/logo_course.png" alt="ild_002" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="../">ild_002 (CyberOps Associate)   <img src="../0-aux/logo_course.png" alt="ild_002" width="auto" height="25"></a>
### Module: 6. Ethernet e IP

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

### Course Module 6 Structure:

6. <a name="item06">Ethernet e IP</a><br>
  6.1 <a href="#item06.01">Introdução</a><br>
  6.2 <a href="#item06.02">Ethernet</a><br>
  6.3 <a href="#item06.03">IPv4</a><br>
  6.4 <a href="#item06.04">Noções básicas de endereçamento IP</a><br>
  6.5 <a href="#item06.05">Tipos de endereços IPv4</a><br>
  6.6 <a href="#item06.06">O gateway padrão</a><br>
  6.7 <a href="#item06.07">IPv6</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;6.7.1 <a href="#item06.06.01">Verifique sua compreensão - Representação de endereço IPv6</a><br>
  6.8 <a href="#item06.08">Resumo de protocolo Ethernet e IP</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item06.01"><h4>6.1 Introdução</h4></a>[Back to summary](#item06)

🔹 Endereçamento de Rede e Protocolos de Transmissão   
A identificação precisa de origem e destino é o pilar que sustenta o fluxo de dados tanto em redes locais quanto na rede mundial de computadores. Para profissionais de defesa cibernética, a análise de registros de eventos depende diretamente do entendimento de como as informações de endereçamento são estruturadas. Este estudo detalha as tecnologias de enlace e os protocolos de camada de rede, fundamentais para rastrear conexões e monitorar tentativas de acesso em infraestruturas organizacionais.

🎯 Objetivo Geral   
- Analisar o papel das tecnologias Ethernet e dos protocolos de endereçamento IP na viabilização da comunicação digital.

✅ Objetivos Específicos   
- Ethernet: Descrever o funcionamento da subcamada MAC e a estrutura dos quadros que organizam o tráfego em redes locais.
- IPv4: Explicar as características e a operação do protocolo de quarta geração no transporte de pacotes de dados.
- Noções básicas de endereçamento IP: Demonstrar como os identificadores lógicos permitem a localização e a troca de informações entre diferentes sistemas.
- Tipos de endereços IPv4: Classificar as diferentes categorias de endereçamento que organizam a distribuição de conectividade.
- O gateway padrão: Definir a função do ponto de saída que permite a comunicação entre dispositivos de redes distintas.
- IPv6: Apresentar a estrutura e as vantagens do protocolo de endereçamento de última geração para a escalabilidade da rede.

<a name="item06.02"><h4>6.2 Ethernet</h4></a>[Back to summary](#item06)

📦 A Anatomia do Quadro Ethernet   
Para que os dados viajem com segurança, a Ethernet os organiza em uma estrutura chamada quadro (frame). Existem limites rígidos para o tamanho desses quadros: eles devem ter entre 64 e 1518 bytes.
- Quadros muito pequenos (<64 bytes): Conhecidos como "fragmentos de colisão", são descartados por serem considerados inválidos ou incompletos.
- Quadros muito grandes (>1500 bytes de dados): Chamados de "Jumbo frames", podem ser aceitos por switches de alto desempenho, mas normalmente são descartados em redes comuns.

Campos Principais do Quadro:
- Sincronização (Preâmbulo e SFD): Os primeiros 8 bytes servem para "acordar" a placa de rede receptora e sincronizar o tempo da transmissão.
- Endereçamento MAC: Contém o endereço de quem envia e de quem deve receber. O destino pode ser um dispositivo específico (unicast), um grupo (multicast) ou todos na rede (broadcast).
- Tipo/Comprimento (EtherType): Indica qual protocolo de camada superior está escondido ali dentro (ex: 0x800 para IPv4, 0x86DD para IPv6 ou 0x806 para ARP).
- Dados (Payload): O conteúdo real da mensagem. Se o dado for pequeno demais, o sistema adiciona "enchimentos" (pads) para atingir o mínimo de 64 bytes.
- Verificação de Erros (FCS): Um campo de 4 bytes que usa um cálculo matemático (CRC) para conferir se os dados foram corrompidos no trajeto. Se o cálculo não bater, o quadro é jogado fora.

🆔 Endereço MAC: A Identidade Física   
O endereço MAC é um valor binário de 48 bits, mas para facilitar nossa vida, ele é representado por 12 dígitos hexadecimais (0-9 e A-F). É a "impressão digital" da placa de rede (NIC). Dependendo do sistema (Windows, Linux, Cisco), esse endereço será encontrado escrito de formas diferentes, embora o valor seja o mesmo:
- Com traços: 00-60-2F-3A-07-BC
- Com dois pontos: 00:60:2F:3A:07:BC
- Com pontos: 0060.2F3A.07BC

<a name="item06.03"><h4>6.3 IPv4</h4></a>[Back to summary](#item06)

🛠️ As 4 Operações de "Trânsito" da Camada 3   
Para que um dado saia de um host e chegue a outro, a Camada de Rede executa um ciclo de quatro etapas essenciais:
- Endereçamento: Cada dispositivo final precisa de uma identidade única (Endereço IP) para ser localizado no mapa global.
- Encapsulamento: O host de origem pega o dado da camada superior e o coloca dentro de um "envelope" digital, adicionando o cabeçalho IP com os endereços de quem envia e de quem recebe.
- Roteamento: É o papel do GPS. Os roteadores analisam o endereço de destino e decidem o melhor caminho. Cada roteador no trajeto é chamado de salto (hop).
- Desencapsulamento: No destino, o host abre o pacote, verifica se o IP é realmente dele e, se estiver tudo certo, remove o cabeçalho IP para entregar o conteúdo à Camada de Transporte.

🚀 O Pacote IP: Um Entregador Indiferente   
O protocolo IP (seja o IPv4 de 32 bits ou o moderno IPv6 de 128 bits) é focado na estrutura do transporte, não no conteúdo. Ele não se importa se está carregando um pedaço de um vídeo do YouTube ou um comando crítico de banco de dados; seu único trabalho é garantir que o pacote tenha o cabeçalho correto para ser roteado.

Um ponto crucial é que o cabeçalho IP permanece praticamente inalterado durante toda a viagem (do primeiro ao último roteador), a menos que passe por um processo de tradução de endereços (NAT). Isso garante a integridade do endereçamento de ponta a ponta.

⚖️ As Três Características Básicas do IP   
O IP foi projetado para ser leve e rápido, o que o torna eficiente, mas também "desapegado". Ele possui três pilares fundamentais:
- Sem Conexão (Connectionless): O IP não liga antes para saber se o destinatário está pronto ou se o computador está ligado. Ele simplesmente envia o pacote. É como mandar uma carta pelo correio: o remetente a deposita na caixa e espera que chegue.
- Melhor Esforço (Best Effort): O IP não garante a entrega. Ele não tem mecanismos para recuperar pacotes perdidos ou corrompidos. Se algo der errado, o pacote é descartado. A responsabilidade de garantir que tudo chegou em ordem fica para as camadas superiores (como o TCP).
- Independente da Mídia: O pacote IP não muda sua estrutura se estiver viajando por um cabo de cobre, uma fibra óptica ou por ondas de rádio (Wi-Fi). Ele flui de forma transparente sobre qualquer tecnologia física.

📬 Comunicação Sem Conexão (Connectionless)   
O IP opera sob uma lógica de "enviar e esquecer". Diferente de uma chamada telefônica, onde você espera a pessoa atender para começar a falar, o IP não estabelece uma conexão prévia com o destinatário.
- Baixa Sobrecarga: Como não há troca de mensagens iniciais para "combinar" a conversa, o cabeçalho do pacote permanece leve.
- Incerteza do Remetente: A desvantagem é que a origem não tem como saber se o destino está ligado, se o endereço existe ou se a mensagem foi lida. O pacote é simplesmente lançado na rede.

⚖️ O Modelo de "Melhor Esforço" (Best Effort)   
Dizer que o IP é não confiável não significa que ele funciona mal, mas sim que ele não possui mecanismos próprios de recuperação. Ele faz o seu "melhor esforço" para entregar o pacote, mas não assume compromissos:
- Sem Garantias: Se um pacote for corrompido por um ruído no cabo ou se perder em um roteador congestionado, o IP não tentará retransmiti-lo. Ele apenas descarta o dado.
- Indiferença à Ordem: Pacotes de uma mesma mensagem podem chegar fora de sequência ou nem chegar.
- Divisão de Tarefas: Essa "irresponsabilidade" do IP é proposital. Ao deixar a correção de erros para as camadas superiores (especialmente o TCP na Camada 4), o IP consegue processar bilhões de pacotes por segundo com uma eficiência altíssima.

🔌 Independência de Meio e o Desafio da MTU   
O protocolo IP é "cego" em relação ao hardware. Ele não se importa se os bits estão viajando como eletricidade no cobre, pulsos de luz na fibra óptica ou ondas de rádio no Wi-Fi. No entanto, ele precisa respeitar um limite físico fundamental: a MTU (Unidade Máxima de Transmissão).
- O que é a MTU: É o tamanho máximo que um quadro físico consegue carregar. A camada de enlace informa esse valor para a camada de rede, que ajusta o tamanho do pacote IP.
- Fragmentação (IPv4): Se um pacote IPv4 precisar passar de uma rede com MTU grande para uma rede com MTU menor, um roteador intermediário terá que "fatiar" esse pacote em pedaços menores. Isso gera latência e consome recursos do roteador.
- A Mudança no IPv6: Para aumentar a performance global, os roteadores não fragmentam pacotes IPv6. Se o pacote for grande demais para o próximo link, ele é descartado e o remetente é avisado para reenviá-lo em um tamanho menor.

🏗️ Estrutura e Identificação do Pacote   
Cada campo no cabeçalho tem uma função técnica específica, lida pelos dispositivos de Camada 3 da esquerda para a direita.
- Versão: Um campo de 4 bits que, no caso do IPv4, é sempre 0100. Ele avisa ao hardware que as regras a serem seguidas são as deste protocolo específico.
- IHL (Internet Header Length): Informa o tamanho exato do cabeçalho. Isso é crucial para o receptor saber onde terminam as instruções e onde começam os dados reais.
- Serviços Diferenciados (DiffServ): Antigamente chamado de ToS, este campo de 8 bits gerencia a prioridade. Ele usa o DSCP para marcar tráfegos sensíveis (como voz sobre IP) e o ECN para avisar sobre congestionamentos na rede antes que pacotes comecem a ser descartados.
- Tamanho Total: Define o comprimento somado do cabeçalho e dos dados. Ajuda o dispositivo a saber o volume total que está sendo processado.
- Gerenciamento de Fragmentação (Identificação, Flags e Deslocamento): Quando um pacote é grande demais para um link, ele é dividido. Esses três campos funcionam como "etiquetas de montagem", permitindo que o destino saiba a qual "original" aquele pedaço pertence e qual a ordem correta para reconstruí-lo.
- Tempo de Vida (TTL): Um contador de "saltos". Cada roteador que o pacote atravessa subtrai 1 desse valor. Se chegar a zero, o pacote morre para não ficar circulando infinitamente em loops de rede, e o emissor recebe um aviso via ICMP.
- Protocolo: É o "apontador" da próxima camada. Um valor binário de 8 bits indica se o conteúdo deve ser entregue ao ICMP (1), TCP (6) ou UDP (17).
- Checksum do Cabeçalho: Uma ferramenta de verificação rápida. Se os bits do cabeçalho sofrerem qualquer alteração no caminho (corrupção), o checksum não baterá e o pacote será descartado para garantir a integridade.
- Endereço IPv4 de Origem: Os 32 bits que identificam o remetente. É sempre um endereço individual (unicast).
- Endereço IPv4 de Destino: Os 32 bits que dizem para onde a mensagem vai. Pode ser para um único host, um grupo (multicast) ou para toda a vizinhança (broadcast).
- Opções e Preenchimento: Campos raramente utilizados na prática diária, servindo para extensões do protocolo ou para garantir que o cabeçalho tenha um tamanho múltiplo de 32 bits.

<a name="item06.04"><h4>6.4 Noções básicas de endereçamento IP</h4></a>[Back to summary](#item06)

🏷️ A Estrutura Hierárquica do IPv4   
Um endereço IPv4 possui 32 bits. Para que a comunicação ocorra, todos os aparelhos de uma mesma rede precisam compartilhar a mesma "parte de rede". Já a "parte de host" deve ser exclusiva de cada dispositivo naquela vizinhança digital.

Para configurar um host corretamente, além do endereço IP único, são necessários outros três elementos:
- Máscara de Sub-rede: O "tradutor" que separa o que é rede do que é host.
- Gateway Padrão: A porta de saída para acessar outras redes (geralmente o roteador).
- Servidor DNS: O catálogo que transforma nomes (como www.google.com) em números IP.

🎭 Máscara de Sub-rede e Notação de Prefixo   
O endereço IPv4 é uma identidade de 32 bits dividida em duas partes: a identificação da Rede e a identificação do Host (dispositivo). A máscara de sub-rede é o que define onde termina uma e começa a outra.
- Bit 1 na máscara: Indica que aquela posição do IP pertence à rede.
- Bit 0 na máscara: Indica que aquela posição do IP pertence ao host.

Para facilitar a escrita, é usado o Comprimento do Prefixo (notação CIDR), que nada mais é do que contar quantos bits "1" a máscara possui e colocar esse número após uma barra (/). Exemplos de conversão rápida:
- 255.0.0.0 vira /8
- 255.255.0.0 vira /16
- 255.255.255.0 vira /24
- 255.255.255.240 vira /28

🔢 Lógica Booleana: A Operação AND   
Os computadores não "leem" o IP como nós; eles usam uma operação matemática chamada AND para descobrir o endereço da rede. É uma comparação bit a bit onde o resultado só será "1" se ambos os bits comparados forem "1". A regra do AND é simples:
- 1 AND 1 = 1
- 1 AND 0 = 0
- 0 AND 1 = 0
- 0 AND 0 = 0

Ao aplicar esse cálculo entre o IP do dispositivo e sua máscara de sub-rede, o resultado final é o Endereço de Rede.

🚀 Como o Host decide para onde enviar o dado?   
O dispositivo realiza o cálculo AND para saber qual é a sua própria rede. Quando ele precisa enviar um pacote, ele faz o mesmo cálculo com o IP de destino:
- Se o Endereço de Rede do destino for igual ao dele, o host entrega o pacote diretamente na rede local.
- Se o Endereço de Rede for diferente, o host entende que o alvo está em outra rede e envia o pacote para o Gateway Padrão (o roteador).

✂️ Sub-redes: Dividindo para Conquistar   
Redes muito grandes podem se tornar "barulhentas". Quando um host envia um Broadcast (mensagem para todos), cada dispositivo na rede precisa parar o que está fazendo para processar aquele pacote. Se houver milhares de usuários, a rede fica lenta. A solução é o Subnetting (divisão em sub-redes). Esse processo consiste em "pegar emprestado" bits da parte de host para criar redes menores.

Benefícios:
- Performance: Redução do tráfego de broadcast e domínios de colisão.
- Segurança: Permite isolar departamentos (ex: Financeiro não acessa o Wi-Fi de Visitantes).
- Organização: Facilita a gestão de endereços por localização física ou função.

<a name="item06.05"><h4>6.5 Tipos de endereços IPv4</h4></a>[Back to summary](#item06)

🏷️ Categorias de Endereçamento: O Legado Classful   
Antigamente, a internet dividia o bolo de endereços IPv4 em fatias fixas chamadas classes. Embora esse modelo seja considerado ineficiente hoje em dia e tenha sido substituído pelo sistema sem classe (classless), ele ainda é a base de muita documentação e configurações de rede.
- Classe A (0.0.0.0/8 a 127.0.0.0/8): Criada para organizações gigantescas. Utiliza apenas o primeiro bloco (octeto) para identificar a rede, o que permite criar poucas redes, mas com mais de 16 milhões de dispositivos em cada uma.
- Classe B (128.0.0.0/16 a 191.255.0.0/16): Voltada para empresas de médio e grande porte. Divide o endereço ao meio (16 bits para rede e 16 para hosts), suportando cerca de 65 mil aparelhos por rede.
- Classe C (192.0.0.0/24 a 223.255.255.0/24): O padrão para redes pequenas. Usa os três primeiros blocos para a rede, limitando-se a apenas 254 endereços para dispositivos.
- Classes D e E: A Classe D é reservada exclusivamente para tráfego Multicast (envio para grupos), enquanto a Classe E é mantida para fins de testes e pesquisas experimentais.

📉 O Desperdício e a Evolução   
O grande problema das classes era a rigidez. Se uma empresa precisasse de 300 endereços, ela não cabia na Classe C e recebia uma Classe B inteira, "jogando fora" milhares de IPs que ninguém usaria. Por isso, nos anos 90, o modelo de classes foi abandonado em favor de métodos mais flexíveis e da criação dos endereços privados.

🔒 Endereços Públicos vs. Privados (RFC 1918)   
Os endereços Públicos são como números de telefone internacionais: únicos no mundo e visíveis em toda a internet. Já os endereços Privados são usados apenas dentro de casas e empresas. Eles não podem navegar na internet aberta; se um roteador de um provedor (ISP) recebe um pacote vindo de um IP privado, ele o descarta na hora. Existem três faixas de IPs reservadas para uso interno:
- 10.0.0.0 a 10.255.255.255 (Bloco /8)
- 172.16.0.0 a 172.31.255.255 (Bloco /12)
- 192.168.0.0 a 192.168.255.255 (Bloco /16) — O mais comum em roteadores domésticos.

🔄 NAT: O Tradutor de Redes   
Como os dispositivos internos usam IPs privados e a internet só aceita IPs públicos, precisamos de um intermediário. O NAT (Tradução de Endereços de Rede) é o serviço que roda no roteador e faz essa ponte. 
- Como funciona: O NAT pega o pedido (vindo de um IP privado como 192.168.1.10) e o envia para a internet usando o endereço público que o provedor deu. Quando a resposta volta, o NAT sabe exatamente para qual dispositivo interno deve entregar a informação.
- Importância: Sem o NAT e os IPs privados, os endereços IPv4 do mundo teriam acabado décadas atrás.

<a name="item06.06"><h4>6.6 O gateway padrão</h4></a>[Back to summary](#item06)

🗺️ Para onde o pacote pode ir?   
Sempre que um host gera um tráfego, ele avalia o destino em três categorias:
- Ele mesmo (Loopback): O host envia um pacote para testar sua própria capacidade de comunicação. No IPv4 usa-se o IP 127.0.0.1 e no IPv6 o ::1. Isso serve para validar se o software de rede (pilha TCP/IP) está funcionando corretamente no próprio aparelho.
- Host Local: O destino está na mesma vizinhança. O remetente e o destinatário compartilham o mesmo endereço de rede. Nesse caso, o dado é entregue diretamente através de um switch ou ponto de acesso sem fio.
- Host Remoto: O destino está fora da rede local (em outra empresa, outra casa ou na Internet). Aqui, o host sabe que não consegue entregar o pacote sozinho e precisa de ajuda externa.

🔍 Como o host decide se o destino é local ou remoto?   
A lógica de descoberta muda conforme a versão do protocolo:
- No IPv4: O host realiza um cálculo matemático binário usando sua própria máscara de sub-rede contra o IP de destino. Se o resultado do endereço de rede for igual ao dele, o destino é local.
- No IPv6: O processo é mais automatizado. O roteador da rede anuncia periodicamente o "prefixo" (endereço da rede) para todos os dispositivos, que já sabem de antemão quem faz parte da vizinhança.

🚪 O Gateway Padrão (A Porta de Saída)   
Se o host percebe que o destino é remoto, ele envia o pacote para o Gateway Padrão. Imagine o gateway como a porta de uma sala: se uma pessoa quer falar com alguém dentro da sala, ela fala diretamente; se quer ir para a rua ou outra sala, ela precisa passar pela porta.

Características do Gateway:
- Ele é um roteador ou switch de Camada 3 conectado à rede local.
- Possui um endereço IP na mesma faixa que os outros dispositivos da rede.
- Sua função é receber o tráfego interno e roteá-lo para caminhos externos.
- Sem um gateway configurado (ou se ele estiver inativo), o computador fica "preso" na rede local, sem acesso à Internet ou outras filiais.

📋 A Tabela de Roteamento do Host   
Cada computador mantém uma lista interna de direções chamada tabela de roteamento. É nela que fica gravada a "rota padrão" (o caminho para o gateway). No Windows, é possível visualizar esse "GPS interno" usando os comandos: `route print` e `netstat -r`. Ao executar esses comandos, o sistema exibe três informações principais:
- Lista de Interfaces: Mostra todas as placas de rede (Ethernet, Wi-Fi, Bluetooth) e seus endereços físicos (MAC).
- Tabela IPv4: Todas as rotas conhecidas para endereços de 32 bits.
- Tabela IPv6: Todas as rotas conhecidas para endereços de 128 bits.

Com essas informações, o analista de segurança consegue entender por onde o tráfego de um dispositivo está saindo e se existem rotas estáticas suspeitas configuradas no sistema.

<a name="item06.07"><h4>6.7 IPv6</h4></a>[Back to summary](#item06)

🚀 Por que migrar para o IPv6?   
O principal motor da mudança é o esgotamento dos endereços IPv4. Quase todos os registros regionais (RIRs) ao redor do globo já declararam que seus estoques acabaram. 
- Fim do "Quebra-galho" (NAT): O NAT (Tradução de Endereços) ajudou a adiar o fim do IPv4, mas ele traz problemas: gera latência, dificulta conexões diretas entre dispositivos (P2P) e quebra o funcionamento de diversos aplicativos modernos.
- Internet das Coisas (IoT): Hoje, não são apenas computadores e celulares que precisam de IP. Carros, geladeiras, sensores médicos e cidades inteligentes exigem bilhões de novas conexões, algo que só o IPv6 consegue entregar.
- Adoção em Massa: Provedores de telefonia móvel e gigantes como Netflix, Facebook e YouTube já operam majoritariamente em IPv6. Algumas empresas estão até abandonando o IPv4 em suas redes internas.

🔢 A Estrutura do Endereço IPv6   
Enquanto o IPv4 tem 32 bits, o IPv6 saltou para 128 bits. Isso resulta em aproximadamente 340 undecilhões de endereços únicos — um número tão vasto que é praticamente impossível esgotar.

Características do Formato:
- Escrita Hexadecimal: Ao contrário do decimal (0-9) do IPv4, o IPv6 usa hexadecimal (0-9 e A-F).
- Os Hextetos: O endereço é dividido em 8 segmentos de 16 bits cada. O termo técnico para esses segmentos é "hexteto".
- Separadores: Em vez de pontos, os hextetos são separados por dois-pontos (:).
- Flexibilidade: O endereço não diferencia maiúsculas de minúsculas.

✍️ O Formato Preferencial   
O chamado "formato preferencial" é a escrita completa do endereço, utilizando todos os 32 dígitos hexadecimais. Exemplo de estrutura: `xxxx:xxxx:xxxx:xxxx:xxxx:xxxx:xxxx:xxxx`. Cada x representa quatro valores hexadecimais. Escrever tudo isso pode ser cansativo, por isso existem regras de compressão (como omitir zeros à esquerda ou usar dois-pontos duplos) para encurtar a representação, mas a base estrutural é sempre essa sequência de 8 hextetos.

✂️ Regra 1: Omitir Zeros à Esquerda   
A primeira forma de encurtar um endereço é eliminar os zeros que aparecem no início de cada hexteto (segmento de 16 bits). Pense nisso como os números decimais: o número "050" é apenas "50". Exemplos:
- 01AB vira 1AB
- 09f0 vira 9f0
- 00ab vira ab
- 0000 vira apenas 0

Atenção: Essa regra vale apenas para zeros à esquerda. Zeros à direita nunca devem ser removidos, pois alterariam completamente o valor do hexteto (transformariam abc0 em abc, o que é um erro grave).

🔗 Regra 2: O Uso do Duplo Dois-Pontos (::)   
Essa é a regra mais "poderosa". É possível substituir uma sequência contínua de hextetos compostos apenas por zeros por um símbolo de dois-pontos duplo (::).
- Exemplo: 2001:db8:cafe:1:0:0:0:1 compactado vira 2001:db8:cafe:1::1.
- Restrições Importantes:
  - Use apenas uma vez: só pode ser utilizado uma única vez no endereço todo. Se for usado duas vezes, o computador não saberá quantos zeros existem em cada lacuna, tornando o endereço ambíguo.
  - Melhor prática: Se houver duas sequências de zeros em partes diferentes do endereço, use o :: na sequência mais longa. Se forem de tamanhos iguais, use na primeira que aparecer.

🗺️ Comprimento do Prefixo e o Padrão /64   
Diferente do IPv4, que aceita máscaras decimais (como 255.255.255.0), o IPv6 utiliza exclusivamente a notação de barra (ex: /64). No IPv6, isso é chamado de Comprimento do Prefixo. Esse valor indica quantos bits do endereço pertencem à rede. O padrão recomendado para quase todas as redes locais (LANs) é o /64.
- Prefix (Rede): Os primeiros 64 bits.
- Interface ID (Host): Os últimos 64 bits.

Por que usar sempre /64?   
O uso de 64 bits para a interface facilita a criação de sub-redes e é um requisito obrigatório para o funcionamento do SLAAC (Configuração Automática de Endereço Sem Estado), que permite que os dispositivos se auto-configurem sem precisar de um servidor DHCP.

<a name="item06.07.01"><h4>6.7.1 Verifique sua compreensão - Representação de endereço IPv6</h4></a>[Back to summary](#item07)

Converta os endereços IPv6 em formatos curtos e compactos (omita os zeros à esquerda). Insira letras em minúsculas. Clique em Avançar para avançar a atividade para o próximo endereço.

- Formato preferencial: 2001:0db8:2233:4455:6677:0000:0000:0101
  - Zeros à esquerda omitidos: 2001:db8:2233:4455:6677:0:0:101
  - Formato compactado: 2001:db8:2233:4455:6677::101

- Formato preferencial: bb2b:ef12:bff3:9125:1111:0101:1111:0101
  - Zeros à esquerda omitidos: bb2b:ef12:bff3:9125:1111:101:1111:101
  - Formato compactado: bb2b:ef12:bff3:9125:1111:101:1111:101

- Formato preferencial: 2001:0db8:0000:1234:5678:9101:1112:1113
  - Zeros à esquerda omitidos: 2001:db8:0:1234:5678:9101:1112:1113
  - Formato compactado: 2001:db8::1234:5678:9101:1112:1113

<a name="item06.08"><h4>6.8 Resumo de protocolo Ethernet e IP</h4></a>[Back to summary](#item06)

🌐 Padrões de Conexão Local   
A Ethernet e as redes sem fio representam as tecnologias de maior uso para conectar dispositivos em curtas distâncias, operando nas bases físicas e de enlace do sistema de comunicação. Enquanto a Ethernet suporta velocidades variadas, sua identificação depende do endereço MAC, uma etiqueta única de 48 bits representada em formato hexadecimal que garante que os dados cheguem ao hardware correto dentro da rede local.

📡 Protocolos de Interconexão   
Para que a informação atravesse diferentes redes e alcance a internet, utilizam-se os protocolos IP em suas versões 4 e 6, responsáveis pelo endereçamento e pelo roteamento dos pacotes. O processo consiste em envolver os dados em um cabeçalho específico que permite aos roteadores identificar o destino final, funcionando de forma independente do meio físico utilizado para a transmissão.

🔢 Estrutura do IPv4   
Um endereço IPv4 possui 32 bits e é dividido hierarquicamente em uma porção que identifica a rede e outra que identifica o dispositivo específico. Através da máscara de sub-rede e do cálculo binário AND, o sistema diferencia essas partes, permitindo a criação de divisões menores que reduzem o congestionamento de tráfego, melhoram o desempenho e facilitam o controle de segurança por departamento ou local.

🌍 Endereçamento Público e Privado   
Antigamente, a distribuição de IPs seguia um sistema rígido de classes que levava ao desperdício de endereços, sendo substituído por modelos mais flexíveis e sem classes. Atualmente, existem blocos de endereços privados destinados ao uso interno das organizações, que não circulam na internet aberta, ajudando a preservar o estoque limitado de endereços públicos disponíveis globalmente.

🚪 Portão de Saída e Rotas   
Para decidir se um dado deve ser entregue localmente ou enviado para fora, o dispositivo consulta seu gateway padrão, que atua como a porta de saída da rede local. No Windows, é possível visualizar o mapa de caminhos que o computador utiliza para alcançar destinos remotos através de comandos de rede, identificando a rota padrão que o tráfego deve seguir para sair da vizinhança imediata.

🚀 Expansão com IPv6   
Com um espaço de 128 bits, o IPv6 soluciona a escassez de endereços ao oferecer uma quantidade quase infinita de identificadores públicos. Além da capacidade ampliada, esta versão traz melhorias automáticas na configuração e resolução de endereços, simplificando a comunicação entre dispositivos sem a necessidade de intervenções manuais complexas que eram comuns no protocolo anterior.

📝 Compactação de Endereços IPv6   
Devido à extensão dos endereços hexadecimais, existem regras para simplificar sua escrita, como a eliminação de zeros à esquerda e o uso de dois-pontos duplos para substituir sequências nulas contínuas. Na organização dessas redes, utiliza-se a notação de barra para definir o prefixo, sendo o padrão de 64 bits o mais recomendado para facilitar a gestão e a criação automática de IDs para cada interface de rede.
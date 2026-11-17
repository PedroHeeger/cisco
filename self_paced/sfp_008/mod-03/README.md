# Networking Devices and Initial Configuration - Módulo 3   <img src="../0-aux/logo_course.png" alt="sfp_008" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">sfp_008 (Networking Devices and Initial Configuration)   <img src="../0-aux/logo_course.png" alt="sfp_008" width="auto" height="25"></a>
### Module: 3. Sistemas numéricos

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

### Course Module 3 Structure:
3. <a name="item03">Sistemas numéricos</a><br>
  3.1 <a href="#item03.01">Introdução</a><br>
  3.2 <a href="#item03.02">Sistema de numeração binário</a><br>
  3.3 <a href="#item03.03">Sistema de numeração hexadecimal</a><br>
  3.4 <a href="#item03.04">Resumo dos sistemas numéricos</a><br>
  3.5 Exame de ponto de verificação: características do projeto de rede<br>
  
---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item03.01"><h4>3.1 Introdução</h4></a>[Back to summary](#item03)

🔢 Sistemas de Numeração e Conversão de Dados   
O processamento e o endereçamento em redes de computadores baseiam-se em diferentes sistemas numéricos para a representação interna de dados e a leitura de identificadores. Enquanto as arquiteturas de hardware operam de forma nativa por meio do sistema binário, as notações lógicas e físicas utilizam representações decimais e hexadecimais para simplificar a administração de protocolos como IPv4, IPv6 e endereços MAC. A habilidade de transição entre essas bases é fundamental para a análise técnica de sub-redes e tráfego de dados.

🎯 Objetivo do módulo:   
- Converter valores numéricos entre as bases decimais, binárias e hexadecimais utilizadas em redes de computadores.

📘 Tópicos do módulo:   
- Sistema de numeração binário: Métodos matemáticos para a conversão de valores entre a base decimal e a base secundária de dois dígitos.
- Sistema de numeração hexadecimal: Procedimentos técnicos para a alternância de valores entre o sistema decimal e a base dezesseis de caracteres alfanuméricos.

<a name="item03.02"><h4>3.2 Sistema de numeração binário</h4></a>[Back to summary](#item03)

🔢 A Dualidade do Endereçamento IPv4: Binário vs. Decimal   
As máquinas e ativos de rede processam dados exclusivamente em formato binário (composto por bits 0 e 1). No entanto, gerenciar sequências extensas de caminhos lógicos nesse formato é inviável para seres humanos. Por essa razão, adota-se a notação decimal pontilhada, que traduz o fluxo binário bruto em números de base 10 separados por pontos, facilitando a administração das redes.

🧬 A Anatomia de um Endereço IP   
A estrutura interna de um endereço IPv4 é composta por um conjunto linear de 32 bits. Para fins de organização e leitura, esse bloco é fragmentado uniformemente:
- Divisão por Octetos: Os 32 bits são separados em 4 seções de 8 bits (cada seção equivale a 1 octeto ou 1 byte).
- Mapeamento de Dispositivos: Enquanto o computador armazena e processa a informação como um único fluxo contínuo de 32 bits, o administrador configura e visualiza interfaces (como o IP de um host ou do gateway padrão) em formato decimal.

🧮 O Mecanismo de Conversão por Posição   
A conversão de um número decimal para binário dentro de um octeto baseia-se em oito posições fixas. Cada uma dessas posições possui um peso específico baseado em potências de 2, lidos sempre da esquerda para a direita:
- 1ª posição (mais significativa): vale 128
- 2ª posição: vale 64
- 3ª posição: vale 32
- 4ª posição: vale 16
- 5ª posição: vale 8
- 6ª posição: vale 4
- 7ª posição: vale 2
- 8ª posição (menos significativa): vale 1

O processo funciona como um teste lógico simples para cada posição:
- Se o valor for maior ou igual ao peso daquela posição, coloca-se o bit 1, subtrai o valor do peso e passa o que sobrou para a próxima posição.
- Se o valor for menor que o peso da posição, coloca-se o bit 0 e passa para a próxima posição sem fazer nenhuma subtração.

📝 Passo a Passo Prático: Convertendo o IP 192.168.10.11   
Vamos aplicar essa regra simples para cada um dos quatro octetos do endereço de exemplo:
- 1º Octeto: 192:
  - 192 é maior ou igual a 128? Sim. Colocamos o bit 1 e guardamos o resto (192 menos 128 resulta em 64).
  - 64 é maior ou igual a 64? Sim. Colocamos o bit 1 e o resto agora é zero (64 menos 64 resulta em 0).
  - Como o resto chegou a zero, todas as posições seguintes (32, 16, 8, 4, 2 e 1) recebem automaticamente o bit 0.
  - Resultado do octeto: 11000000
- 2º Octeto: 168:
  - 168 é maior ou igual a 128? Sim. Colocamos o bit 1 e guardamos o resto (168 menos 128 resulta em 40).
  - 40 é maior ou igual a 64? Não. Colocamos o bit 0 e mantemos o valor 40.
  - 40 é maior ou igual a 32? Sim. Colocamos o bit 1 e guardamos o resto (40 menos 32 resulta em 8).
  - 8 é maior ou igual a 16? Não. Colocamos o bit 0 e mantemos o valor 8.
  - 8 é maior ou igual a 8? Sim. Colocamos o bit 1 e o resto zera (8 menos 8 resulta em 0).
  - As posições restantes (4, 2 e 1) recebem o bit 0.
  - Resultado do octeto: 10101000
- 3º Octeto: 10 (Análise por Soma Direta): Para valores menores, podemos apenas identificar quais pesos somados atingem o número desejado. Para formar o número 10, precisamos ativar os pesos 8 e 2 (já que 8 mais 2 é igual a 10).
  - Os pesos maiores (128, 64, 32 e 16) ficam zerados: 0000
  - O peso 8 fica ativo: 1
  - O peso 4 fica zerado: 0
  - O peso 2 fica ativo: 1
  - O peso 1 fica zerado: 0
  - Resultado do octeto: 00001010
- 4º Octeto: 11 (Análise por Soma Direta): Seguindo o mesmo raciocínio de soma direta, para obter o número 11, precisamos combinar os pesos 8, 2 e 1 (pois 8 mais 2 mais 1 é igual a 11).
  - Os pesos superiores (128, 64, 32 e 16) ficam desligados: 0000
  - O peso 8 fica ligado: 1
  - O peso 4 fica desligado: 0
  - Os pesos 2 e 1 ficam ligados: 11
  - Resultado do octeto: 00001011

Ao juntar as quatro partes processadas, o endereço decimal configurado pelo usuário é interpretado pelo roteador ou computador como a seguinte sequência de bits. O endereço decimal 192.168.10.11 equivale ao binário 11000000.10101000.00001010.00001011.

<a name="item03.03"><h4>3.3 Sistema de numeração hexadecimal</h4></a>[Back to summary](#item03)

🔢 O Sistema Hexadecimal na Infraestrutura de Rede   
Além do domínio sobre os formatos binário e decimal fundamentais para o IPv4, a compreensão do protocolo IPv6 exige a familiaridade com o sistema de numeração hexadecimal. Essa base numérica desempenha um papel crucial na simplificação e gerenciamento de dados em rede, sendo amplamente empregada para a representação de:
- Endereços IP versão 6 (IPv6).
- Endereços físicos de controle de acesso ao meio (Endereço MAC Ethernet).

A utilização do formato hexadecimal justifica-se pela eficiência de compactação, visto que um único caractere hexadecimal consegue condensar e expressar visualmente um conjunto exato de quatro bits binários.

🧬 Estrutura e Características do Endereço IPv6   
O dimensionamento do IPv6 apresenta especificações estruturais robustas para atender à demanda de conectividade global, diferenciando-se significativamente dos padrões adotados no IPv4:
- Extensão Total: Cada endereço possui um comprimento exato de 128 bits.
- Composição Hexadecimal: O bloco total de bits é convertido e representado por uma sequência de 32 dígitos hexadecimais.
- Insensibilidade a Caixa (Case Insensitivity): O protocolo aceita caracteres tanto em formato maiúsculo quanto minúsculo de maneira intercambiável (por exemplo, o registro FA2B possui o mesmo valor operacional que fa2b).

📂 Formatação e Terminologia: O Hexteto   
A exibição padrão para a escrita de um endereço IPv6 baseia-se na separação de blocos por meio de dois-pontos, seguindo a estrutura: x:x:x:x:x:x:x:x. Nessa representação, cada caractere x equivale a um agrupamento de quatro dígitos hexadecimais. Enquanto o ecossistema IPv4 adota o termo octeto para se referir aos blocos de 8 bits, a arquitetura IPv6 introduz uma nova nomenclatura de segmentação:
- Definição de Hexteto: Termo técnico utilizado para identificar cada um dos oito segmentos individuais de 16 bits (ou quatro caracteres hexadecimais) que integram o endereço.

Essa divisão em oito hextetos bem definidos permite que os dispositivos de encaminhamento processem as tabelas de roteamento com maior eficiência e velocidade.

<a name="item03.04"><h4>3.4 Resumo dos sistemas numéricos</h4></a>[Back to summary](#item03)

🔢 Sistemas de Numeração em TI   
O sistema binário baseia-se exclusivamente nos dígitos zero e um, conhecidos como bits, e constitui a linguagem nativa pela qual computadores, roteadores e servidores processam dados e endereços lógicos. Para tornar a gestão humana mais simples, os endereços IPv4, que são puramente binários por baixo dos panos, são convertidos e exibidos para nós no formato decimal separado por pontos.

🧮 Estrutura da Base Decimal   
A matemática do cotidiano utiliza a base 10, onde o valor de cada algarismo em um número depende diretamente da sua posição. Em uma análise estrutural de um número como 2.146, cada dígito ocupa uma casa específica correspondente às potências de dez, dividindo-se ordenadamente em unidades de milhar, centenas, dezenas e unidades para compor o valor total.

🔌 Lógica e Notação Binária   
Funcionando em base 2, a matemática computacional define que cada posição de um número pode assumir apenas duas opções lógicas de estado. Para organizar e converter esses valores, os profissionais utilizam tabelas posicionais padronizadas com oito divisões, já que o agrupamento de 8 bits forma um byte, a unidade fundamental de armazenamento de rede.

📐 O Sistema Hexadecimal   
Utilizado para simplificar anotações complexas de infraestrutura, como o endereçamento físico MAC e o lógico IPv6, o sistema de base 16 incorpora os numerais de 0 a 9 e as letras de A a F. Esse modelo funciona perfeitamente com a computação porque um único caractere hexadecimal consegue resumir perfeitamente o valor de um conjunto de quatro bits binários.

🌍 Composição do Endereço IPv6   
Os identificadores de nova geração possuem uma extensão total de 128 bits, mapeados em grupos onde cada bloco de 4 bits se transforma em um caractere da base dezesseis, resultando em uma linha de 32 dígitos. Essa estrutura confere flexibilidade na escrita dos endereços, permitindo que letras maiúsculas e minúsculas sejam interpretadas exatamente da mesma forma pelos dispositivos de rede.
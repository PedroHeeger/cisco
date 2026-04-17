# CCNA: Introduction to Networks - Módulo 5   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_001 (CCNA: Introduction to Networks)   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="25"></a>
### Module: 5. Sistemas de números

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

### Course Module 5 Structure:
5. <a name="item05">Sistemas de números</a><br>
  5.1 <a href="#item05.01">Introdução</a><br>
  5.2 <a href="#item05.02">Sistema de numeração binária</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;5.2.1 <a href="#item05.02.01">Atividade - Conversões binárias para decimais</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;5.2.2 <a href="#item05.02.02">Atividade - Conversões decimais para binárias</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;5.2.3 <a href="#item05.02.03">Atividade - Jogo Binário</a><br>
  5.3 <a href="#item05.03">Sistema de numeração hexadecimal</a><br>
  5.4 <a href="#item05.04">Módulo Prático e Quiz</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item05.01"><h4>5.1 Introdução</h4></a>[Back to summary](#item05)

📘 Introdução   
Este módulo aborda os sistemas numéricos aplicados ao funcionamento das redes de computadores. Endereços como IPv4 e IPv6 fazem uso de diferentes representações — binária, decimal e hexadecimal — essenciais para diversas atividades de configuração e análise. Embora essas conversões pareçam complexas à primeira vista, elas tornam-se mais simples quando se compreende o princípio de cada sistema. As práticas do módulo auxiliam no desenvolvimento da familiaridade com essas transformações.

🎯 Objetivo Geral   
Apresentar os fundamentos dos sistemas decimal, binário e hexadecimal, destacando como realizar conversões entre eles no contexto de endereçamento de redes.

✅ Objetivos Específicos   
- Converter valores entre decimal e binário.
- Converter valores entre decimal e hexadecimal.
- Reconhecer o uso dos sistemas numéricos em endereços IPv4 e IPv6.

<a name="item05.02"><h4>5.2 Sistema de numeração binária</h4></a>[Back to summary](#item05)

🧩 Visão Geral do Endereçamento IPv4   
Os endereços IPv4 começam como uma sequência de bits, compostos apenas por 0 e 1. Como é difícil para os humanos trabalharem com longas sequências binárias, os administradores de rede convertem esses endereços para decimal, em uma forma conhecida como notação decimal pontilhada. Mesmo assim, o binário é essencial, pois todos os dispositivos de rede interpretam e armazenam os endereços dessa forma. Um endereço IPv4 possui 32 bits, divididos em quatro octetos de 8 bits, separados por pontos.

🔢 Entendendo Binário e Decimal   
O sistema decimal utiliza 10 dígitos (0 a 9) e funciona com notação posicional: o valor de um dígito depende da posição que ocupa no número. Já o sistema binário utiliza apenas 2 dígitos (0 e 1), mas segue a mesma lógica. Cada posição de um octeto representa uma potência de 2, começando com 2⁷ (128) na esquerda até 2⁰ (1) na direita. Somando os valores correspondentes aos bits ativos (1), é possível converter um número binário para decimal. Por exemplo, o octeto binário 11000000 possui bits ativos em 128 e 64, então 128 + 64 = 192 em decimal.

🧮 Conversão de Binário para Decimal   
Para converter um endereço IPv4 completo, divide-se os 32 bits em quatro octetos e aplica-se a soma dos valores posicionais para cada octeto.
- Primeiro octeto: 11000000 → 128 + 64 = 192.
- Segundo octeto: 10101000 → 128 + 32 + 8 = 168.
- Terceiro octeto: 00001011 → 8 + 2 + 1 = 11.
- Quarto octeto: 00001010 → 8 + 2 = 10.

O endereço binário 11000000.10101000.00001011.00001010 se torna, portanto, 192.168.11.10 em decimal pontilhado.

🔄 Conversão de Decimal para Binário   
O processo inverso utiliza uma tabela de valores posicionais binários (128, 64, 32, 16, 8, 4, 2, 1). Para cada octeto, verifica-se quais valores somados chegam ao número desejado, marcando 1 para valores usados e 0 para os restantes. Por exemplo:
- Decimal 192 → Binário 11000000
- Decimal 168 → Binário 10101000
- Decimal 11 → Binário 00001011
- Decimal 10 → Binário 00001010

💡 Importância da Conversão   
Compreender ambos os sistemas é fundamental porque humanos trabalham com decimal, mas dispositivos de rede entendem binário. Saber converter permite interpretar endereços IP, calcular sub-redes e configurar equipamentos corretamente. Além disso, esse conhecimento é essencial para qualquer prática avançada de rede, como roteamento, segmentação e troubleshooting.

<a name="item05.02.01"><h4>5.2.1 Atividade - Conversões binárias para decimais</h4></a>[Back to summary](#item05)

Nesta atividade os seguintes números binários abaixo foram convertidos para decimais:
- 00000010: 0 + 0 + 0 + 0 + 0 + 0 + 2 + 0 = 2;
- 11111100: 128 + 64 + 32 + 16 + 8 + 4 + 0 + 0 = 252;
- 11101100: 128 + 64 + 32 + 0 + 8 + 4 + 0 + 0 = 236;
- 11100110: 128 + 64 + 32 + 0 + 0 + 4 + 2 + 0 = 230;
- 10111010: 128 + 0 + 32 + 16 + 8 + 0 + 2 + 0 = 186;

<a name="item05.02.02"><h4>5.2.2 Atividade - Conversões decimais para binárias</h4></a>[Back to summary](#item05)

Nesta atividade os seguintes números decimais abaixo foram convertidos para binários:
- 168: 1 + 0 + 1 + 0 + 1 + 0 + 0 + 0 = 10101000;
- 227: 1 + 1 + 1 + 0 + 0 + 0 + 1 + 1 = 11100011;
- 159: 1 + 0 + 0 + 1 + 1 + 1 + 1 + 1 = 10011111;
- 169: 1 + 0 + 1 + 0 + 1 + 0 + 0 + 1 = 10101001;
- 97: 0 + 1 + 1 + 0 + 0 + 0 + 0 + 1 = 01100001;

<a name="item05.02.03"><h4>5.2.3 Atividade - Jogo Binário</h4></a>[Back to summary](#item05)

Nesta aula foi apresentado o site [Binary Game](https://learningcontent.cisco.com/games/binary/index.html) que um jogo online educativo desenvolvido pela Cisco para praticar a conversão de números binários para decimais e decimais para binários.

<a name="item05.03"><h4>5.3 Sistema de numeração hexadecimal</h4></a>[Back to summary](#item05)

🧩 Endereçamento IPv6 e Hexadecimal   
Assim como é importante entender binário e decimal para trabalhar com endereços IPv4, é necessário compreender hexadecimal para lidar com endereços IPv6 e endereços MAC Ethernet. O sistema hexadecimal é de base 16, usando os dígitos de 0 a 9 e as letras A a F, representando valores de 0 a 15. Ele se conecta bem ao binário porque quatro bits binários podem ser representados por um único dígito hexadecimal, tornando mais simples a leitura de grandes números binários.

🔢 Estrutura dos Endereços IPv6   
Os endereços IPv6 possuem 128 bits. Cada quatro bits formam um dígito hexadecimal, resultando em 32 dígitos hexadecimais no total. O formato padrão de escrita é X:X:X:X:X:X:X:X, em que cada "X" representa um hextet. Um hextet é composto por 16 bits ou quatro dígitos hexadecimais. Diferente do IPv4, que usa octetos de 8 bits, o IPv6 organiza os endereços em hextets, facilitando o agrupamento e a leitura dos dados. Letras maiúsculas ou minúsculas podem ser usadas sem diferença no valor.

🧮 Conversão Decimal → Hexadecimal   
Para converter um número decimal em hexadecimal, o processo envolve três etapas:
- Transformar o número decimal em uma string binária de 8 bits.
- Dividir a sequência binária em grupos de quatro bits, da direita para a esquerda.
- Converter cada grupo de quatro bits no dígito hexadecimal equivalente.

Por exemplo, para converter o decimal 168:
- 168 em binário → 10101000
- Agrupamento em quatro bits → 1010 e 1000
- Conversão para hexadecimal → 1010 = A, 1000 = 8
- Resultado final → 168 = A8 em hexadecimal

🧮 Conversão Hexadecimal → Decimal   
O processo inverso, de hexadecimal para decimal, também segue três etapas:
- Converter cada dígito hexadecimal em 4 bits binários.
- Agrupar os bits em blocos de 8 bits, da direita para a esquerda.
- Converter cada bloco de 8 bits para seu valor decimal correspondente.

Exemplo: converter D2 em decimal:
- D2 em binário → D = 1101, 2 = 0010 → agrupamento → 11010010
- Converter para decimal → 11010010 = 210
- Resultado final → D2 = 210 em decimal

💡 Importância da Conversão   
Compreender hexadecimal e a conversão entre binário e decimal é essencial para interpretar endereços IPv6 e endereços MAC. Essa habilidade permite analisar, configurar e solucionar problemas de redes modernas, garantindo precisão ao lidar com grandes volumes de endereços e mantendo compatibilidade entre dispositivos.

<a name="item05.04"><h4>5.4 Módulo Prático e Quiz</h4></a>[Back to summary](#item05)

💾 Sistemas numéricos em redes   
O sistema binário utiliza apenas dois dígitos — 0 e 1 — chamados bits. Já o sistema decimal usa dez dígitos, de 0 a 9. A compreensão do binário é essencial porque hosts, servidores e dispositivos de rede trabalham com endereçamento binário, especialmente nas representações IPv4. Por isso, é importante saber converter endereços IPv4 entre decimal pontilhado e binário.

Além disso, existe o sistema hexadecimal, que é de base 16 e utiliza os números de 0 a 9 e as letras de A a F. Ele é amplamente usado para representar endereços IPv6 e endereços MAC. Um endereço IPv6 possui 128 bits, e cada grupo de 4 bits corresponde a um dígito hexadecimal, totalizando 32 caracteres hexadecimais.

Para conversões:
- Hexadecimal → Decimal: primeiro converte-se para binário e, em seguida, de binário para decimal.
- Decimal → Hexadecimal: também passa primeiro pela conversão para binário antes de chegar ao valor hexadecimal.
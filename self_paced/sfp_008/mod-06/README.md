# Networking Devices and Initial Configuration - Módulo 6   <img src="../0-aux/logo_course.png" alt="sfp_008" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">sfp_008 (Networking Devices and Initial Configuration)   <img src="../0-aux/logo_course.png" alt="sfp_008" width="auto" height="25"></a>
### Module: 6. Estrutura do endereço IPv4

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

### Course Module 6 Structure:
6. <a name="item06">Estrutura do endereço IPv4</a><br>
  6.1 <a href="#item06.01">Introdução</a><br>
  6.2 <a href="#item06.02">Estrutura do endereço IPv4</a><br>
  6.3 <a href="#item06.03">Resumo do Estrutura do endereço IPv4</a><br>
  6.4 Exame de ponto de verificação: endereçamento de rede<br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item06.01"><h4>6.1 Introdução</h4></a>[Back to summary](#item06)

🗺️ Estrutura e Segmentação do Endereçamento IPv4   
O planejamento eficiente de uma infraestrutura de rede exige a correta divisão do espaço de endereçamento lógico para otimizar o tráfego e garantir a segurança dos departamentos. A arquitetura de um endereço IPv4 é baseada em uma composição hierárquica que diferencia a identificação da rede da identificação dos hosts locais. A correta interpretação dessa estrutura permite realizar a segmentação lógica por meio de sub-redes, garantindo que a nova topologia cresça de forma organizada e escalável.

🎯 Objetivo do módulo:   
- Calcular esquemas de sub-redes IPv4 para realizar a segmentação eficiente de uma infraestrutura de rede.

📘 Tópicos do módulo:   
- Estrutura do endereço IPv4: Descrição dos componentes fundamentais do endereço de 32 bits, detalhando a porção de rede, a porção de host e a função da máscara de sub-rede.

<a name="item06.02"><h4>6.2 Estrutura do endereço IPv4</h4></a>[Back to summary](#item06)

🌐 Estrutura Binária do Endereço IPv4   
O endereço IPv4 é composto por uma cadeia hierárquica de 32 bits, estruturada rigidamente em duas seções distintas: a porção de rede e a porção de host.
- Porção de Rede: Os bits deste segmento devem ser perfeitamente idênticos em todas as estações e interfaces contidas em um mesmo limite de rede local.
- Porção de Host: Os bits deste segmento devem ser totalmente exclusivos, garantindo a identificação individual de um dispositivo específico dentro daquele domínio.

Para que um host obtenha conectividade plena, a parametrização do sistema operacional exige a definição de um conjunto de valores lógicos: o endereço IPv4 do dispositivo, a respectiva máscara de sub-rede, o gateway padrão (essencial para o roteamento de dados além das fronteiras locais) e os endereços de servidores DNS (responsáveis por traduzir nomes de domínio em sequências numéricas IP).

🎛️ A Máscara de Sub-rede e o Comprimento do Prefixo   
A diferenciação exata de onde termina a identificação de rede e onde começa a identificação de host é determinada pela máscara de sub-rede. Tecnicamente, a máscara consiste em uma sequência contínua de bits em nível lógico alto (1), seguida por uma sequência contínua de bits em nível lógico baixo (0). O alinhamento desses bits indica ao hardware a fronteira exata da rede.

Para simplificar a leitura e evitar a complexidade da escrita decimal pontilhada tradicional, utiliza-se a metodologia do comprimento do prefixo, também conhecida como notação de barra ou CIDR. Esse formato baseia-se na contagem direta de quantos bits estão configurados como 1 na máscara. Abaixo constam os exemplos de correlação entre as máscaras decimais, as sequências binárias e os respectivos prefixos:
- A máscara 255.0.0.0 possui a sequência binária 11111111.00000000.00000000.00000000, correspondendo ao prefixo /8.
- A máscara 255.255.0.0 possui a sequência binária 11111111.11111111.00000000.00000000, correspondendo ao prefixo /16.
- A máscara 255.255.255.0 possui a sequência binária 11111111.11111111.11111111.00000000, correspondendo ao prefixo /24.
- A máscara 255.255.255.128 possui a sequência binária 11111111.11111111.11111111.10000000, correspondendo ao prefixo /25.
- A máscara 255.255.255.192 possui a sequência binária 11111111.11111111.11111111.11000000, correspondendo ao prefixo /26.
- A máscara 255.255.255.224 possui a sequência binária 11111111.11111111.11111111.11100000, correspondendo ao prefixo /27.
- A máscara 255.255.255.240 possui a sequência binária 11111111.11111111.11111111.11110000, correspondendo ao prefixo /28.
- A máscara 255.255.255.248 possui a sequência binária 11111111.11111111.11111111.11111000, correspondendo ao prefixo /29.
- A máscara 255.255.255.252 possui a sequência binária 11111111.11111111.11111111.11111100, correspondendo ao prefixo /30.

Na documentação de infraestrutura, a junção do endereço com o prefixo elimina espaços, sendo grafada diretamente na forma: 192.168.10.10/24.

🧮 Determinação de Rede via Operação Lógica AND   
O cálculo matemático realizado pelas interfaces de rede para descobrir o endereço de rede baseia-se na aplicação da álgebra booleana através do operador AND lógico. Na lógica digital, o bit 1 representa um estado verdadeiro e o bit 0 representa um estado falso.

A regra booleana determina que o resultado da comparação será verdadeiro (1) apenas se as duas entradas analisadas forem simultaneamente verdadeiras. Qualquer outra combinação resulta em falso (0):
- 1 AND 1 resulta em 1
- 0 AND 1 resulta em 0
- 1 AND 0 resulta em 0
- 0 AND 0 resulta em 0

Para extrair o endereço de rede, o dispositivo executa essa validação bit a bit, cruzando o endereço IP do host com a máscara de sub-rede configurada.

📝 Demonstração Prática com o IP 192.168.10.10/24   
Ao realizar o alinhamento e a comparação booleana dos 32 bits, observa-se o seguinte comportamento:
- Análise dos Três Primeiros Octetos: Como a máscara de sub-rede /24 possui os primeiros 24 bits configurados como 1 (equivalente a 255.255.255.0), qualquer bit do endereço do host comparado com o bit 1 da máscara preservará exatamente o seu valor original. Dessa forma, os valores decimais 192.168.10 permanecem intactos.
- Análise do Quarto Octeto: O valor decimal do host é 10 (binário 00001010) e o valor correspondente na máscara é 0 (binário 00000000). A aplicação do operador AND entre qualquer bit do host e o bit 0 da máscara resulta obrigatoriamente em zero.

Dessa forma, o cruzamento lógico zera por completo a porção de host, isolando apenas a identidade da infraestrutura:
- Endereço do Host em binário: 11000000.10101000.00001010.00001010 (equivalente a 192.168.10.10)
- Máscara de Sub-rede em binário: 11111111.11111111.11111111.00000000 (equivalente a 255.255.255.0)
- Endereço de Rede Resultante em binário: 11000000.10101000.00001010.00000000 (equivalente a 192.168.10.0/24)

Este endereço de rede sintetiza a localização lógica global do segmento, permitindo que a estação reconheça os limites de sua própria rede local e determine se um pacote precisa ou não ser despachado para o gateway padrão.

<a name="item06.03"><h4>6.3 Resumo do Estrutura do endereço IPv4</h4></a>[Back to summary](#item06)

🧱 Estrutura Hierárquica do IPv4   
O endereço IPv4 é uma sequência de 32 bits dividida logicamente em duas seções fundamentais: o identificador de rede e o identificador de host. Todos os equipamentos que pertencem ao mesmo segmento local precisam compartilhar exatamente a mesma combinação de bits na porção de rede, enquanto a porção de host deve carregar uma numeração exclusiva para diferenciar cada aparelho individualmente naquele grupo.

🎭 Papel da Máscara de Sub-rede   
A máscara de sub-rede funciona como um filtro que revela onde termina a identificação da rede e onde começa a do host dentro dos 32 bits do endereço IP. Quando aplicada a uma interface, ela permite que o dispositivo calcule o endereço de rede correspondente, que funciona como o identificador coletivo de todos os computadores daquela vizinhança digital.

✒️ Notação de Comprimento de Prefixo   
Uma forma simplificada e muito comum de representar a máscara de sub-rede é através do comprimento do prefixo, também conhecido como notação CIDR ou de barra. Esse método consiste em contar a quantidade de bits seguidos que estão configurados com o valor um na máscara, adicionando uma barra comum (/) seguida por esse número ao final do endereço IP, como transformar a máscara 255.255.255.0 em um simples /24.

⚡ A Lógica da Operação AND   
O cálculo matemático que os dispositivos realizam por baixo dos panos baseia-se na operação lógica booleana AND (E). Esse operador compara dois bits por vez e estabelece uma regra binária muito rígida: o resultado só será igual a um se ambos os bits comparados forem iguais a um; qualquer outra combinação envolvendo o dígito zero resultará obrigatoriamente em zero.

🔀 Cálculo do Endereço de Rede   
Para descobrir a qual rede pertence, o sistema operacional realiza a operação AND bit a bit, cruzando o endereço IPv4 do host com a sua respectiva máscara de sub-rede convertida em binário. Como os bits correspondentes à rede na máscara são sempre representados por uns, o processo preserva a identidade da rede original e zera completamente os bits do host, isolando o endereço de rede exato.
# Laboratório - Criar um fluxograma de processo   <img src="./0-aux/logo_course.png" alt="lab_010" width="auto" height="45">

### Cisco: <a href="../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../self_paced/">self-paced</a>
### Software/Subject: programming_logic   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/programming_logic.jpg" alt="programming_logic" width="auto" height="25"></a>
### Course: <a href="./">lab_010 (Laboratório - Criar um fluxograma de processo)   <img src="./0-aux/logo_course.png" alt="lab_010" width="auto" height="25"></a>

---

### Theme:
- Programming Logic

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

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">Parte 1: Liste as etapas lógicas para resolver um problema</a><br>
2. <a href="#item02">Parte 2: Desenhe o Fluxograma</a><br>
  2.1 <a href="#item02.01">Parte 1: Liste as etapas lógicas para resolver um problema</a><br>
  2.2 <a href="#item02.02">Etapa 2: Desenhe o fluxograma completo.</a><br>
3. <a href="#item03">Reflexão</a><br>

---

### Objective:
Criar um fluxograma com base na construção de um processo de identificação de um número em um intervalo específico.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: Liste as etapas lógicas para resolver um problema</h4></a>[Back to summary](#item00)

O problema é desenvolver um processo para encontrar um número predeterminado. O processo pode ser programado como um jogo de computador simples. É solicitado que um jogador pense em um número inteiro entre 0 e 128. O programa usará o método de bissecção para encontrar o número.

- a. Liste as etapas lógicas para resolver um problema:
  - Pergunte o que o jogador pensa sobre um número inteiro entre 0 e 128.
  - Defina a como a extremidade inferior b como a extremidade superior e t como a hora do cálculo.
  - Defina os valores iniciais, a = 0, b = 128, t = 0.
  - Calcule o número médio entre a e b. Defina-o como M.
  - Defina t = t + 1
  - Pergunte ao jogador se M é o número correto. Se sim, imprima “O número que você pensou é M e eu adivinhei em t tentativas”. Finalize o processo.
  - Caso M não seja o número correto, pergunte ao jogador se o número pensado é maior ou menor que M.
  - Se o número for maior que M, atualize a extremidade inferior definindo a = M.
  - Se o número for menor que M, atualize a extremidade superior definindo b = M.
  - Retorne ao cálculo do número médio entre a e b e repita o processo até que o número seja encontrado.
- b. O processo pode detectar se o número que o jogador escolheu é 0 ou 128? Explique.
  - Não. Da forma como o processo está descrito, não há garantia de que os valores 0 ou 128 sejam detectados. Isso ocorre porque o método da bissecção baseia-se no cálculo do valor médio entre os limites inferior (a) e superior (b). Como 0 e 128 são valores extremos do intervalo, eles não serão obtidos como valor médio. Se o algoritmo não verificar explicitamente esses limites, o processo pode continuar indefinidamente sem encontrar o número escolhido.
- c. Se 0 ou 128 não puder ser detectado, o que deve ser feito para corrigir isso?
  - O processo deve ser ajustado para testar explicitamente os limites do intervalo. Em cada iteração, deve-se verificar se o número pensado pelo jogador é igual ao valor de a ou b. Caso seja, o processo deve ser finalizado, garantindo que os valores extremos também possam ser corretamente detectados.

<a name="item02"><h4>2. Parte 2: Desenhe o Fluxograma</h4></a>[Back to summary](#item00)

<a name="item02.01"><h4>2.1 Etapa 1: Use símbolos de fluxograma apropriados para cada função.</h4></a>[Back to summary](#item00)

Como a lista de etapas do processo é identificada, podemos usar símbolos de fluxograma para representar cada etapa.

- a. Use um símbolo oval como Iniciar e um símbolo de exibição para perguntas. Use uma linha para vinculá-los.
- b. Use um símbolo de preparação para fazer a atribuição inicial de valores.
- c. Use um símbolo de processo predefinido para definir uma função ou rotina de processo.
- d. Use um símbolo de decisão para representar um teste de condição.
- e. Use um símbolo de processo para representar uma operação.

<a name="item02.02"><h4>2.2 Etapa 2: Desenhe o fluxograma completo.</h4></a>[Back to summary](#item00)

Agora podemos usar símbolos para desenhar um fluxograma completo. Usaremos o Conector fora da página e Conector para estender o fluxograma para a próxima página.

A imagem 01 exibe o fluxograma construído.

<div align="center"><figure>
    <img src="./0-aux/img01.png" alt="img01"><br>
    <figcaption>Imagem 01.</figcaption>
</figure></div><br>

<a name="item03"><h4>3 Reflexão</h4></a>[Back to summary](#item00)

- a. Qual é o significado de teste se t = 6?
  - O teste t = 6 indica que o número máximo de tentativas permitidas foi atingido. Como o intervalo inicial vai de 0 a 128, o método da bissecção necessita, no máximo, 7 comparações para encontrar qualquer número nesse intervalo. Assim, quando t = 6, o processo está verificando se o limite esperado de tentativas foi alcançado, evitando que o algoritmo entre em um loop infinito.
- b. Onde o teste para os números 0 e 128 deve ser colocado?
  - O teste para os números 0 e 128 deve ser colocado no início do processo ou imediatamente após a definição dos valores iniciais de a e b. Dessa forma, o algoritmo pode verificar se o número pensado pelo jogador corresponde a um dos limites do intervalo antes de iniciar o cálculo do valor médio, garantindo que os valores extremos sejam corretamente detectados.
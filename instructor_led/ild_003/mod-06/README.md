# Fundamentos de Redes - Módulo 6   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_003 (Fundamentos de Redes)   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="25"></a>
### Module: 6. Mídia de rede

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
6. <a name="item06">Mídia de rede</a><br>
  6.1 <a href="#item06.01">Introdução</a><br>
  6.2 <a href="#item06.02">Tipos de Mídia de Rede</a><br>
  6.3 <a href="#item06.03">Resumo - Mídia de rede</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item06.01"><h4>6.1 Introdução</h4></a>[Back to summary](#item06)

🔌 Meios de Transmissão e Camada Física   
A transmissão de sinais em redes de computadores depende de meios físicos que servem como canais para o deslocamento da informação entre a origem e o destino. A seleção da mídia adequada baseia-se em critérios como a distância necessária, a taxa de transferência de dados e o nível de resistência a interferências eletromagnéticas, garantindo que os fluxos de comunicação ocorram de maneira estável tanto em conexões fixas quanto móveis.

🎯 Objetivo do módulo:   
- Descrever os principais meios de transmissão utilizados na infraestrutura de redes de dados.

📘 Tópicos do módulo:   
- Tipos de Mídia de Rede: Análise técnica das propriedades e aplicações das mídias metálicas, ópticas e sem fio.
- Cabeamento de Rede: Descrição das características físicas e padrões de desempenho dos condutores comuns em sistemas de redes locais e de longa distância.

<a name="item06.02"><h4>6.2 Tipos de Mídia de Rede</h4></a>[Back to summary](#item06)

🔌 Meios de Transmissão e Cabeamento de Rede   
A propagação de dados em infraestruturas de rede ocorre por meio de canais que ligam o ponto de origem ao destino final. Nota-se que o método de codificação da informação é intrínseco ao tipo de mídia utilizado:
- Condutores metálicos: Os dados são convertidos em impulsos elétricos que percorrem o interior dos cabos.
- Fibras de vidro ou plástico: A informação é transportada através de pulsos de luz.
- Transmissões sem fio: A comunicação é viabilizada pela modulação de frequências em ondas eletromagnéticas.

🎯 Critérios para Seleção de Mídia   
A definição da tecnologia de conexão mais adequada para uma rede baseia-se na avaliação de quatro requisitos fundamentais:
- Alcance do sinal: A distância máxima que o meio físico suporta sem perda da integridade dos dados.
- Ambiente de instalação: As condições físicas e a presença de interferências no local de implementação.
- Capacidade e velocidade: O volume de tráfego necessário e a taxa de transferência exigida.
- Viabilidade econômica: O custo total envolvendo a aquisição dos materiais e a execução da instalação.

🧶 Cabeamento de Par Trançado   
O cabo de par trançado constitui a base das redes locais modernas, sendo o componente essencial para a tecnologia Ethernet. Sua estrutura interna agrupa fios em pares entrelaçados, técnica aplicada para minimizar interferências externas. A organização dos filamentos segue um padrão de cores, combinando condutores de cor sólida com parceiros listrados em fundo branco, o que facilita a identificação e a terminação correta em ambas as extremidades da conexão.

📟 Cabo Coaxial   
Caracterizado por um núcleo central de cobre rígido, o cabo coaxial foi uma das primeiras soluções desenvolvidas para o tráfego de dados. O condutor principal é envolvido por camadas sobrepostas de isolamento, blindagem metálica trançada e um revestimento externo protetor. Essa configuração permite o transporte eficiente de sinais de alta frequência e banda larga, sendo o padrão utilizado em sistemas de televisão por assinatura e interconexões de comunicação via satélite.

🔬 Cabo de Fibra Óptica   
Composto por filamentos de vidro ou plástico da espessura de um fio de cabelo, este meio de transmissão suporta o tráfego de dados digitais em velocidades extremas por longas extensões geográficas. Pelo fato de utilizar a luz como portadora da informação, o sinal é imune a interferências eletromagnéticas. Além de sua aplicação em telecomunicações, a fibra óptica é empregada em áreas técnicas como inspeções de engenharia e procedimentos de imagem na medicina.

<a name="item06.03"><h4>6.3 Resumo - Mídia de rede</h4></a>[Back to summary](#item06)

🌐 Tipos de Meios de Transmissão   
O canal físico que conecta a origem ao destino é fundamental para o transporte da mensagem. Nas infraestruturas atuais, a comunicação ocorre através de três caminhos principais: cabos metálicos que utilizam eletricidade, filamentos de fibra óptica que conduzem luz e conexões aéreas que se baseiam em ondas eletromagnéticas para propagar dados sem a necessidade de suportes físicos.

📏 Critérios de Seleção da Mídia   
A escolha do cabeamento ou da tecnologia sem fio não é aleatória e depende de uma análise técnica rigorosa. É necessário avaliar a distância que o sinal consegue percorrer sem se degradar, as condições ambientais do local da instalação, a demanda de largura de banda necessária para a operação e, finalmente, o equilíbrio entre o desempenho técnico e o orçamento disponível para o projeto.

🔌 Cabos de Cobre e Coaxiais   
O par trançado é o padrão mais difundido em redes locais Ethernet devido à sua flexibilidade e custo-benefício. Já o cabo coaxial, conhecido por sua blindagem robusta, desempenha um papel crucial na distribuição de sinais de TV e internet via cabo, além de ser um componente essencial na conexão de sistemas de recepção via satélite, suportando frequências específicas de rádio.

✨ Características da Fibra Óptica   
A fibra óptica representa o ápice da velocidade e eficiência, utilizando filamentos extremamente finos para guiar pulsos de luz em trajetos de longa distância. Por não utilizar eletricidade como portadora, essa mídia é imune a interferências eletromagnéticas externas, o que permite transmissões extremamente estáveis e rápidas que superam as limitações físicas dos condutores metálicos tradicionais.
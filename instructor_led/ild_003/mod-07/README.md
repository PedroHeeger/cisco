# Fundamentos de Redes - Módulo 7   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_003 (Fundamentos de Redes)   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="25"></a>
### Module: 7. A Camada de Acesso

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

### Course Module 7 Structure:
7. <a name="item07">A Camada de Acesso</a><br>
  7.1 <a href="#item07.01">Introdução</a><br>
  7.2 <a href="#item07.02">Encapsulamento e o quadro Ethernet</a><br>
  7.3 A Camada de Acesso<br>
  7.4 <a href="#item07.04">Resumo: Camada de Acesso</a><br>
  7.5 Exame de ponto de verificação: acesso à rede<br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item07.01"><h4>7.1 Introdução</h4></a>[Back to summary](#item07)

⛓️ Comunicação em Redes Ethernet   
A operação de redes locais baseia-se no padrão Ethernet para a estruturação e a entrega de pacotes de dados entre dispositivos interconectados. Esse processo exige a formatação da informação em unidades específicas denominadas quadros, que contêm metadados de endereçamento e controle necessários para a navegação no meio físico. Embora o conteúdo da mensagem permaneça constante, a estrutura de encapsulamento adapta-se às exigências técnicas de cada tecnologia de rede para assegurar a integridade da transmissão.

🎯 Objetivo do módulo:   
- Explicar os mecanismos de funcionamento e os processos de troca de dados em infraestruturas baseadas no padrão Ethernet.

📘 Tópicos do módulo:   
- Encapsulamento e o quadro Ethernet: Detalhamento do processo de preparação dos dados e da organização dos campos que constituem o quadro na camada de enlace.
- A Camada de Acesso: Análise de métodos e tecnologias aplicadas para otimizar a eficiência da comunicação no ponto de entrada da rede.

<a name="item07.02"><h4>7.2 Encapsulamento e o quadro Ethernet</h4></a>[Back to summary](#item07)

🏗️ Tecnologia Ethernet e Identificação de Dispositivos   
A Ethernet consolida-se como a arquitetura predominante para a estruturação de redes locais. O acesso a esse meio ocorre por meio da Placa de Interface de Rede (NIC), componente que possui um identificador exclusivo e permanente denominado endereço MAC (Media Access Control). No tráfego de dados, as informações de origem e destino baseadas nesses endereços são integradas aos campos fundamentais do quadro Ethernet.

✉️ Encapsulamento e Formatação de Dados   
O tráfego de informações em sistemas computacionais exige a adoção de estruturas padronizadas para assegurar que a entrega e o processamento ocorram de forma correta. O procedimento de integrar uma mensagem a um formato de transporte específico é definido como encapsulamento. Inversamente, a extração dos dados originais pelo receptor, ao receber o pacote, caracteriza o desencapsulamento.

📦 O Quadro como Unidade de Transmissão   
Antes da transmissão física pela rede, cada conjunto de dados é inserido em um "quadro", que funciona como um invólucro técnico para a mensagem. Este componente contém os endereçamentos necessários do emissor e do receptor, sendo que sua configuração interna e conteúdo variam conforme a natureza da informação e as características do canal de comunicação. Nota-se que falhas na formatação impossibilitam a entrega e o processamento dos dados no host de destino.

🌐 O Protocolo IP e o Endereçamento Lógico   
O protocolo IP (Internet Protocol) desempenha uma função organizacional essencial para a entrega de pacotes através das infraestruturas de rede. Através de especificações como as presentes no IPv6, este protocolo define campos técnicos para identificar rigorosamente os pontos de origem e destino final da comunicação. O IP é o responsável por coordenar o trânsito da informação entre uma ou mais redes, garantindo que o fluxo alcance o destinatário pretendido de maneira metódica.

<a name="item07.04"><h4>7.4 Resumo: Camada de Acesso</h4></a>[Back to summary](#item07)

📦 Conceito de Encapsulamento   
O tráfego de dados funciona de forma análoga ao sistema postal, onde uma informação é inserida dentro de estruturas de controle para ser transportada. Esse processo de "empacotamento", conhecido como encapsulamento, adiciona as etiquetas necessárias para o envio, enquanto o destinatário realiza o desencapsulamento ao remover essas camadas para acessar o conteúdo original da mensagem.

🖼️ Estrutura do Quadro Ethernet   
Os padrões Ethernet estabelecem regras rígidas para a montagem dos quadros de dados, definindo onde informações cruciais como os endereços MAC de origem e destino devem ser posicionadas. Além dos endereços, o quadro inclui mecanismos de sincronização, delimitadores de início e códigos de verificação que permitem identificar se houve algum erro ou corrupção durante o trajeto físico.

🔌 Evolução da Camada de Acesso   
A camada de acesso é o ponto de entrada onde os dispositivos finais se conectam à rede para trocar arquivos e acessar recursos. Antigamente, essa função era exercida por hubs, que operavam de forma limitada permitindo apenas uma transmissão por vez; no entanto, devido à frequência de colisões de dados e lentidão, eles foram substituídos por switches, que gerenciam o tráfego de forma muito mais inteligente.

🧠 Inteligência do Switch Ethernet   
Operando na camada 2, o switch atua como um diretor de tráfego que analisa o endereço físico (MAC) de cada mensagem recebida. Ao contrário do hub, ele estabelece um circuito temporário dedicado entre a origem e o destino, permitindo que múltiplos dispositivos enviem e recebam informações simultaneamente sem interferências, o que otimiza drasticamente o desempenho da rede.

📑 Tabela de Endereços MAC   
Para saber exatamente para onde enviar cada quadro, o switch constrói e mantém uma base de dados dinâmica chamada tabela de endereços MAC. Ele aprende de forma automática, observando o endereço de origem de cada mensagem que passa por suas portas e registrando em qual interface o dispositivo está conectado, garantindo que a rede se autoconfigure conforme novos aparelhos são ligados.
# Packet Tracer - Interpretar a saída do comando show   <img src="./0-aux/logo_course.png" alt="pkt_047" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../pkt/">pkt</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">pkt_047 (Packet Tracer - Interpretar a saída do comando show)   <img src="./0-aux/logo_course.png" alt="pkt_047" width="auto" height="25"></a>

---

### Theme:
- Network

### Used Tools:
- Operating System (OS): 
  - Cisco Internetwork Operating System (Cisco IOS)   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/cisco_ios.jpg" alt="cisco_ios" width="auto" height="25">
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
- Network:
  - Cisco Packet Tracer <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/cisco_packet_tracer.webp" alt="cisco_packet_tracer" width="auto" height="25">

---

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">Parte 1: analisar as saídas de dados do comando show</a><br>
2. <a href="#item02">Parte 2: Perguntas para reflexão</a><br>

---

### Objective:
O objetivo desta atividade foi analisar as saídas de diferentes variações do comando show no **Cisco IOS**, visando identificar as informações específicas fornecidas por cada comando para o monitoramento e gerenciamento de dispositivos de rede.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: analisar as saídas de dados do comando show</h4></a>[Back to summary](#item00)

A imagem 01 mostra a topologia inicial.

<div align="center"><figure>
    <img src="./0-aux/img01.png" alt="img01"><br>
    <figcaption>Imagem 01.</figcaption>
</figure></div><br>

- a. Para conectar-se ao ISPRouter, clique em ISP PC, em seguida na guia Desktop, seguido por Terminal.
- b. Entre no modo EXEC privilegiado.
  - `enable`.
- c. Use os seguintes comandos show para responder às perguntas de reflexão na parte 2. Observação: Se um comando pausar com o prompt -—more—, certifique-se de que aperta a barra de espaços até que o  prompt IsProuter# apareça para obter toda a saída do comando. 
  - `show arp` -> `show flash:` -> `show ip route` -> `show interface` -> `show ip interface brief` -> `show protocols` -> `show users` -> `show version`.

<a name="item02"><h4>2. Parte 2: Perguntas para reflexão</h4></a>[Back to summary](#item00)

- a. Quais comandos você pode usar para determinar o endereço IP e o prefixo de rede das interfaces?
  - Resumidos: `show ip interface brief` e `show protocols`. Completos: `show ip interface`, `show interfaces` e `show running-config`.
- b. Qual comando fornece o endereço IP e a atribuição da interface, mas não o prefixo da rede?
  - `show ip interface brief`.
- c. Quais comandos você usaria para determinar se uma interface está ativa?
  - Resumidos: `show ip interface brief` e `show protocols`. Completos: `show ip interface`, `show interfaces` e `show running-config`.
- d. Você precisa determinar a versão do IOS que está sendo executada em um roteador. Que comando lhe dará essa informação?
  - `show version`.
- e. Quais comandos mostram informações sobre os endereços de interface do roteador?
  - Resumidos: `show ip interface brief` e `show protocols`. Completos: `show ip interface`, `show interfaces` e `show running-config`.
- f. Você está considerando uma atualização do IOS e precisa determinar se o flash do roteador pode conter o novo IOS. Quais comandos fornecem informações sobre a quantidade de memória Flash disponível?
  - `show flash:`, `dir flash:` e `show file systems`.
- g. Você precisa ajustar uma configuração do roteador, mas suspeita que um colega também esteja trabalhando no roteador de outro local. Qual comando fornece informações sobre as linhas que estão sendo usadas para configuração ou monitoramento de dispositivo?
  - `show users`.
- h. Você foi solicitado a verificar o desempenho de uma interface de dispositivo. Qual comando fornece estatísticas de tráfego para interfaces de roteador?
  - `show ip interface` e `show interfaces`.
- i. Os clientes reclamam que não conseguem alcançar um servidor que usam para armazenamento de arquivos. Você suspeita que a rede pode ter se tornado inacessível devido a uma atualização recente. Qual comando fornece informações sobre os caminhos disponíveis para o tráfego de rede?
  - `show ip route`.
- j. Quais interfaces estão atualmente ativas no roteador ISP?
  - Resumidos: `show ip interface brief` e `show protocols`. Completos: `show ip interface` e `show interfaces`.

A imagem 02 exibe alguns comandos usados.

<div align="center"><figure>
    <img src="./0-aux/img02.png" alt="img02"><br>
    <figcaption>Imagem 02.</figcaption>
</figure></div><br>
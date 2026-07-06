# Packet Tracer - A interação do cliente   <img src="./0-aux/logo_course.png" alt="pkt_063" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../pkt/">pkt</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">pkt_063 (Packet Tracer - A interação do cliente)   <img src="./0-aux/logo_course.png" alt="pkt_063" width="auto" height="25"></a>

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
- Network:
  - Cisco Packet Tracer   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/cisco_packet_tracer.webp" alt="cisco_packet_tracer" width="auto" height="25">

---

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">Parte 1: Entre no modo de simulação.</a><br>
2. <a href="#item02">Parte 2: Defina os Filtros da Lista de Eventos.</a><br>
3. <a href="#item03">Parte 3: Solicite uma página Web em um PC.</a><br>
4. <a href="#item04">Parte 4: Execute a simulação.</a><br>
5. <a href="#item05">Parte 5: Acesse uma PDU específica.</a><br>
6. <a href="#item06">Parte 6: Examine o conteúdo da janela de Informações da PDU.</a><br>

---

### Objective:
O objetivo desta atividade foi analisar o fluxo de tráfego gerado durante a comunicação entre um computador cliente e os servidor DNS e HTTP, observando todas as etapas do processo, desde a resolução de nomes (DNS) até o estabelecimento da comunicação e a troca de dados com o servidor web (HTTP).

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: Entre no modo de simulação.</h4></a>[Back to summary](#item00)

A imagem 01 mostra a topologia inicial.

<div align="center"><figure>
    <img src="./0-aux/img01.png" alt="img01"><br>
    <figcaption>Imagem 01.</figcaption>
</figure></div><br>

- a. Quando o Packet Tracer inicia, ele apresenta uma visão lógica da rede em modo de tempo real. Clique em Simulation Mode para entrar no modo de simulação. O ícone simulation mode está localizado no canto inferior direito do logical workplace.

<a name="item02"><h4>2. Parte 2: Defina os Filtros da Lista de Eventos.</h4></a>[Back to summary](#item00)

No simulation mode, o padrão é capturar todos os eventos. Você usará os filtros somente para capturar os eventos de DNS e HTTP.
- a. Na seção Event List Filters, clique em Show All/None para desmarcar todas as seleções.
- b. Clique em Edit Filters. Na guia IPv4, selecione DNS. Na guia Misc, selecione HTTP. Feche a janela quando terminar. Os Event List Filters mostram o DNS e o HTTP como os únicos eventos visíveis.

<a name="item03"><h4>3. Parte 3: Solicite uma página Web em um PC.</h4></a>[Back to summary](#item00)

Você abrirá um navegador da Web simulado no PC e solicitará uma página Web do servidor.
- a. Clique em PC. Clique na guia Desktop e no Web Browser.
- b. Um navegador da Web simulado será aberto. Digite www.example.com na caixa da URL e clique no botão Go à direita. Minimize a janela do PC.
  - `www.example.com`.

<a name="item04"><h4>4. Parte 4: Execute a simulação.</h4></a>[Back to summary](#item00)

- a. Na seção Play Controls do Simulation Panel, clique Play. A troca entre o PC e o servidor é animada e os eventos são adicionados na Event List. Esses eventos representam a solicitação do PC pela resolução da URL para um endereço IP, o fornecimento do endereço IP pelo servidor, a solicitação do PC pela a página Web, o servidor enviando a página Web em dois segmentos e o reconhecimento do PC sobre a página Web.
- b. Clique em View Previous Event (Visualizar Evento Anterior) para continuar quando o buffer estiver completo.

<a name="item05"><h4>5. Parte 5: Acesse uma PDU específica.</h4></a>[Back to summary](#item00)

- a. Restaure a janela simulada do PC. Observe que há uma página Web em exibição no Navegador da Web. Minimize a janela simulada do navegador.
- b. Na seção Simulation Panel Event List, a última coluna contém uma caixa colorida que fornece acesso a informações detalhadas sobre um evento. Clique na caixa colorida na primeira linha para o primeiro evento. A janela PDU Information (janela de Informações da PDU) será aberta.

A imagem 02 exibe a simulação do tráfego entre o cliente e servidor realizada com sucesso, obtendo acesso ao site.

<div align="center"><figure>
    <img src="./0-aux/img02.png" alt="img02"><br>
    <figcaption>Imagem 02.</figcaption>
</figure></div><br>

<a name="item06"><h4>6. Parte 6: Examine o conteúdo da janela de Informações da PDU.</h4></a>[Back to summary](#item00)

- a. A primeira guia na janela de informações da PDU contém informações sobre a PDU de entrada e/ou de saída com base no modelo OSI. Clique em Next Layer >> repetidamente para percorrer as camadas de inbound e outbound e leia a descrição na caixa abaixo das camadas para obter uma visão geral de como a troca funciona.
- b. Examine as informações da PDU quanto aos outros eventos para ter um resumo de todo o processo de troca.
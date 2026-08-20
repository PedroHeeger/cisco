# Packet Tracer - Identificar Fluxo   <img src="./0-aux/logo_course.png" alt="pkt_082" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../pkt/">pkt</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">pkt_082 (Packet Tracer - Identificar Fluxo)   <img src="./0-aux/logo_course.png" alt="pkt_082" width="auto" height="25"></a>

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
  - ping   <img src="" alt="iputils" width="auto" height="25">
  - Trace Route (tracert)   <img src="" alt="tracert" width="auto" height="25">

---

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">Parte 1: Verificação de Conectividade</a><br>
2. <a href="#item02">Parte 2: Topologia de rede remota de LAN</a><br>
3. <a href="#item03">Parte 3: Topologia de rede WAN</a><br>
  3.1 <a href="#item03.01">Etapa 1: PC0 para sites.</a><br>
  3.2 <a href="#item03.02">Etapa 2: PC1 para sites.</a><br>

---

### Objective:
O objetivo desta atividade foi analisar o fluxo de pacotes em diferentes topologias de rede (LAN e WAN) e observar como alterações na topologia podem modificar o caminho percorrido pelo tráfego.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: Verificação de Conectividade</h4></a>[Back to summary](#item00)

A imagem 01 mostra a topologia inicial.

<div align="center"><figure>
    <img src="./0-aux/img01.png" alt="img01"><br>
    <figcaption>Imagem 01.</figcaption>
</figure></div><br>

Nesta parte, você verificará se pode acessar as outras redes a partir de dispositivos na Rede Doméstica.

- a. Clique no PC0. Selecione a guia Desktop e abra o navegador da web. 
- b. No campo URL, digite www.cisco.pka e pressione Ir. Certifique-se de usar o domínio.pka, não o domínio.com. Ele deve ser bem-sucedido. Você pode clicar em Avanço rápido Time para acelerar o processo. 
  - `www.cisco.pka`.
- c. Repita isso para www.web.pka. Ele deve ser bem-sucedido. 
  - `www.web.pka`.
- d. Saia do navegador da Web quando terminar.

A imagem 02 comprova o acesso do PC0 aos servidores web.

<div align="center"><figure>
    <img src="./0-aux/img02.png" alt="img02"><br>
    <figcaption>Imagem 02.</figcaption>
</figure></div><br>

<a name="item02"><h4>2. Parte 2: Topologia de rede remota de LAN</h4></a>[Back to summary](#item00)

Nesta parte, você usará o modo de simulação no Packet Tracer para observar como os pacotes fluem através de uma rede LAN remota. 

- a. Mude para o modo Simulação (Shift + S). Clique em Mostrar tudo / nenhum para limpar todos os filtros da lista de eventos selecionados. 
- b. Clique em Editar Filtros. Selecione DNS na guia IPv4 e HTTP na guia Diversos. 
- c. Abra um navegador da web no PC0. Digite www.web.pka e pressione Go.
  - `www.web.pka`.
- c. Preveja o caminho do pacote para resolver www.web.pka para um endereço IP. Grave sua previsão.
  - O caminho previsto para a resolução do nome de domínio www.web.pka em um endereço IP foi: PC0 → Wireless Router0 → Cable Modem0 → Cloud0 → Router5 → East → Switch0 → Switch1 → Public DNS.
- d. Clique em Capturar/Encaminhar até que a página da Web seja exibida no PC0 para exibir o fluxo de pacotes. Clique em Exibir eventos anteriores quando solicitado pela caixa de diálogo Buffer Completo. Depois que o endereço IP foi resolvido, qual caminho os pacotes HTTP viajaram para exibir a página da Web? Registre suas observações.
  - Após a resolução do endereço IP, observou-se que os pacotes HTTP percorreram o seguinte caminho para exibir a página web: PC0 → Wireless Router0 → Cable Modem0 → Cloud0 → Router5 → East → Switch0 → Switch1 → Switch2 → servidor web.pka.
- e. Mude para o modo em tempo real (Shift + R). Clique no ícone X no painel de ferramentas direito para selecionar a ferramenta Excluir. Remova o link entre o Switch0 e o Switch 1 da Rede Pública para simular um link quebrado. Após 30 segundos, a rede aprenderá sobre o link quebrado. Você pode clicar em Avanço rápido para acelerar o processo. 
- f. Selecione a ferramenta Seta acima da ferramenta Excluir para desmarcar Excluir.
- g. Mude para o modo Simulação (Shift + S). Abra um navegador da Web no Tablet0 e navegue até www.web.pka. Você pode clicar em Captura/Reprodução Automática para que o Rastreador de Pacotes encaminhe os pacotes sem sua interação. Você também pode mover o controle deslizante de 
reprodução para a direita para acelerar o encaminhamento de pacotes. Com um link quebrado na LAN, como o caminho mudou? Grave sua observação. 
  - Esta LAN (Public Network) possuía um caminho alternativo entre o Switch0 e o Switch2, que permaneceu em espera até a interrupção do enlace entre o Switch0 e o Switch1. Após a falha, o tráfego foi redirecionado automaticamente pelo caminho redundante. Dessa forma, o novo percurso para a resolução de nomes foi: Tablet0 → Wireless Router0 → Cable Modem0 → Cloud0 → Router5 → East → Switch0 → Switch2 → Switch1 → Public DNS.

As imagens 03 e 04 mostram o fluxo do tráfego nos dois momentos analisados.

<div align="center"><figure>
    <img src="./0-aux/img03.png" alt="img03"><br>
    <figcaption>Imagem 03.</figcaption>
</figure></div><br>

<div align="center"><figure>
    <img src="./0-aux/img04.png" alt="img04"><br>
    <figcaption>Imagem 04.</figcaption>
</figure></div><br>

<a name="item03"><h4>3. Parte 3: Topologia de rede WAN</h4></a>[Back to summary](#item00)

<a name="item03.01"><h4>3.1 Etapa 1: PC0 para sites.</h4></a>[Back to summary](#item00)

- a. Permanecendo no modo Simulação, abra um navegador da Web no PC0. Digite www.cisco.pka e pressione Go.
  - `www.cisco.pka`.
- a. Preveja o caminho do pacote para resolver www.cisco.pka para um endereço IP. Record your prediction.
  - O caminho previsto para a resolução do nome www.cisco.pka foi: PC0 → Wireless Router0 → Cable Modem0 → Cloud0 → Router5 → East → Switch0 → Switch2 → Switch1 → Public DNS, pois o servidor DNS estava localizado na rede pública.
- b. Clique em Capturar / Encaminhar até que a página da web seja exibida no PC0 para visualizar o fluxo do pacote. Clique em Exibir eventos anteriores quando solicitado pela caixa de diálogo Buffer cheio. 
- b. Depois que o endereço IP foi resolvido, qual caminho os pacotes HTTP viajaram para exibir a página da web? Registre suas observações.
  - Após a resolução do nome, os pacotes HTTP seguiram o caminho: PC0 → Wireless Router0 → Cable Modem0 → Cloud0 → Router5 → Router2 → Router4 → West → Switch → Servidor Web (cisco.pka).
- c. Mude para o modo de tempo real (Shift + R). Remova o link entre o Roteador 4 e o Roteador 2 da topologia para simular um caminho inacessível. Os roteadores estão usando o EIGRP (Enhanced Interior Gateway Routing Protocol) para ajustar dinamicamente as tabelas de roteamento para contabilizar o link excluído.
- d. Mude para o modo Simulação (Shift + S). Abra um navegador da Web no Tablet0 e navegue até www.cisco.pka.
  - `www.cisco.pka`.
- d. Com um link quebrado na WAN, como o caminho mudaria? Grave sua observação.
  - O caminho até o servidor DNS permaneceu o mesmo, pois ele estava localizado na rede pública. Já o caminho até o servidor Web foi alterado para: Tablet0 → Wireless Router0 → Cable Modem0 → Cloud0 → Router5 → Router2 → Router3 → Router4 → West → Switch → Servidor Web (cisco.pka).
- e. Mude para o modo de tempo real (Shift + R).

As imagens 05 e 06 mostram o fluxo do tráfego nos dois momentos analisados.

<div align="center"><figure>
    <img src="./0-aux/img05.png" alt="img05"><br>
    <figcaption>Imagem 05.</figcaption>
</figure></div><br>

<div align="center"><figure>
    <img src="./0-aux/img06.png" alt="img06"><br>
    <figcaption>Imagem 06.</figcaption>
</figure></div><br>

<a name="item03.02"><h4>3.2 Etapa 2: PC1 para sites.</h4></a>[Back to summary](#item00)

- a. Clique em PC1 > Desktop e abra um prompt de comando.
- b. Digite tracert www.web.pka no comando.
  - `tracert www.web.pka`.
- c. Corresponda os endereços IP nos resultados do tracert aos dispositivos na topologia. Passe o mouse sobre os roteadores na topologia para exibir os endereços IP das interfaces nos roteadores.

<div align="center">

#### Tabela 1 — Fluxo do Tráfego

| Salto | Dispositivo     | Interface    | Endereço IP                         |
|:-----:|:---------------:|:------------:|:-----------------------------------:|
|   1   | West            | G0/1         | 192.168.0.1                         |
|   2   | Router4         | S0/1/1       | 209.165.200.225                     |
|   3   | Router3         | S0/0/0       | 192.0.2.2                           |
|   4   | Router2         | S0/0/1       | 192.0.2.18                          |
|   5   | Router5         | S0/1/1       | 192.0.2.26                          |
|   6   | East            | G0/1 (NAT)   | 209.165.202.132 / 192.168.2.1       |
|   7   | www.web.pka     | G0 (NAT)     | 209.165.202.132 / 192.168.2.254     |

</div>

- c. Se o pop-up não permanecer ativo o tempo suficiente, você poderá acessar os endereços IP do roteador da seguinte maneira: Clique no roteador > CLI > pressione Enter. Agora digite o comando show ip interface brief para obter uma listagem das interfaces e endereços IP.
  - `show ip interface brief`.
- c. A conversão de endereço de rede (NAT) é usada para traduzir o endereço IP www.web.pka privado de 192.168.2.254 para um endereço IPv4 roteável de 209.165.202.132. No resultado tracert, a primeira linha de endereço IPv4 de 209.165.202.132 é para a interface G0/1 do Leste. A segunda linha do endereço IPv4 de 209.165.202.132 exibe o endereço IPv4 público do servidor Web.
- d. Mude para o modo Simulação (Shift + S). Abra o navegador da Web no PC1 e digite www.web.pka como o URL. Clique em Go.
  - `www.web.pka`.
- e. Clique em Capturar/ Encaminhar para carregar a página da Web. Compare os resultados do tracert com os resultados da simulação dos pacotes HTTP. Registre suas observações.
  - Os saltos observados foram os mesmos. No modo Simulação, primeiro ocorre a resolução do nome para obter o endereço IP e, em seguida, os pacotes HTTP são encaminhados até o servidor Web. No tracert, a resolução do nome ocorre antes do rastreamento da rota até o endereço IP de destino.

A imagem 07 mostra o rastreamento da rota realizado no modo Simulação e com a ferramenta tracert.

<div align="center"><figure>
    <img src="./0-aux/img07.png" alt="img07"><br>
    <figcaption>Imagem 07.</figcaption>
</figure></div><br>
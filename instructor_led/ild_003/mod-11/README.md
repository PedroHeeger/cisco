# Fundamentos de Redes - Módulo 11   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_003 (Fundamentos de Redes)   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="25"></a>
### Module: 11. Endereçamento dinâmico com DHCP

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

### Course Module 11 Structure:
11. <a name="item11">Endereçamento dinâmico com DHCP</a><br>
  11.1 <a href="#item11.01">Introdução</a><br>
  11.2 <a href="#item11.02">Endereçamento estático e dinâmico</a><br>
  11.3 Configuração do DHCPv4<br>
&nbsp;&nbsp;&nbsp;&nbsp;11.3.1 <a href="../../../pkt/files/pkt_??/">Packet Tracer – Conexão com um servidor da Web</a><br>
  11.4 <a href="#item11.04">Resumo Endereçamento Dinâmico com DHCP</a><br>
  11.5 Exame de ponto de verificação: o protocolo da Internet<br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item11.01"><h4>11.1 Introdução</h4></a>[Back to summary](#item11)

⚡ Atribuição Dinâmica de Endereçamento com DHCP   
A gestão de endereços IP em redes de larga escala exige métodos eficientes para evitar conflitos e erros de configuração manual. O protocolo DHCP (Dynamic Host Configuration Protocol) automatiza a distribuição de parâmetros de rede, como endereços IPv4, máscaras de sub-rede e gateways padrão, para os dispositivos finais. Essa abordagem reduz a carga administrativa e minimiza interrupções de conectividade causadas por falhas na inserção estática de dados nos terminais.

🎯 Objetivo do módulo:   
- Configurar um servidor DHCPv4 para gerenciar e automatizar a distribuição de endereços em uma rede de dados.

📘 Tópicos do módulo:   
- Endereçamento estático e dinâmico: Comparação técnica entre a inserção manual de parâmetros de rede e a atribuição automática via protocolo.
- Configuração do DHCPv4: Implementação e ajuste de servidores DHCPv4 para o fornecimento dinâmico de identificadores aos hosts da rede.

<a name="item11.02"><h4>11.2 Endereçamento estático e dinâmico</h4></a>[Back to summary](#item11)

🛠️ Atribuição Estática: Precisão e Controle Manual   
Na configuração estática, o administrador de rede assume a responsabilidade de inserir manualmente os parâmetros fundamentais em cada dispositivo. Para que a comunicação ocorra, é necessário configurar o "trio essencial":
- Endereço IP: A identidade exclusiva do host na rede.
- Máscara de Sub-rede: O delimitador que define onde termina a rede e começa o host.
- Gateway Padrão: O ponto de saída (roteador) que permite ao host alcançar a internet ou outras redes externas.

Este método é ideal para infraestruturas fixas que não podem mudar de endereço, como servidores e impressoras, garantindo que os clientes sempre saibam onde encontrá-los. Contudo, em larga escala, torna-se uma tarefa exaustiva e altamente suscetível a erros de digitação (typos), o que pode causar conflitos de IP. Além disso, exige um controle rigoroso em planilhas para evitar a duplicidade de endereços.

⚡ Atribuição Dinâmica (DHCP): Eficiência em Escala   
Para lidar com a alta rotatividade de dispositivos — como notebooks e smartphones em aeroportos ou escritórios — utiliza-se o DHCP (Dynamic Host Configuration Protocol). Em vez de intervenção manual, um servidor distribui automaticamente as configurações de rede para os clientes.

O Conceito de "Aluguel" (Lease): No DHCP, o endereço IP não pertence permanentemente ao host; ele é "emprestado" por um tempo determinado. Se o dispositivo se desconecta ou é desligado, o endereço retorna para um pool comum e fica disponível para outro usuário. Isso otimiza o uso dos endereços disponíveis e elimina o erro humano na configuração.

🏠 O Papel do Roteador Doméstico como "Agente Duplo"   
Em ambientes de pequenas empresas ou residências, o roteador sem fio desempenha um papel duplo crucial:
- Como Cliente DHCP: Ele se conecta ao provedor de internet (ISP) para receber um endereço IP público.
- Como Servidor DHCP: Ele cria uma rede local interna e distribui endereços IPs privados para todos os dispositivos da casa (celulares, TVs, PCs).

Nota: Em redes corporativas maiores, essa função geralmente é centralizada em servidores dedicados (Windows ou Linux) para garantir maior capacidade de gerenciamento e logs detalhados de quem está usando cada IP.

<a name="item11.04"><h4>11.4 Resumo Endereçamento Dinâmico com DHCP</h4></a>[Back to summary](#item11)

✍️ Atribuição Estática de IPs   
Neste modelo, o administrador de rede insere manualmente os dados de conexão em cada dispositivo, definindo o endereço IP, a máscara de sub-rede e o gateway. Embora ofereça um controle rigoroso sobre a rede, essa prática torna-se exaustiva em ambientes grandes e exige uma documentação impecável para evitar conflitos, sendo mais comum em servidores ou equipamentos de infraestrutura que não podem mudar de endereço.

🤖 Automação via DHCP   
O protocolo DHCP é a solução padrão para redes dinâmicas, pois automatiza a entrega de endereços e reduz drasticamente as falhas de configuração manual. Em vez de uma atribuição fixa, o sistema trabalha com o conceito de "aluguel", onde o dispositivo utiliza o IP por um tempo determinado e, ao se desconectar, libera o identificador para que outro aparelho possa utilizá-lo.

📡 DHCP no Cotidiano   
Sempre que um dispositivo se conecta a uma rede Wi-Fi, ele inicia automaticamente uma comunicação com o servidor local para obter suas credenciais de rede. Em residências, essa função é geralmente centralizada no roteador sem fio, que atua como uma ponte: ele recebe um IP externo da operadora (como cliente) e distribui IPs internos para os celulares e computadores da casa (como servidor).

🔄 O Processo de Descoberta (DORA)   
A obtenção de um IP automático segue um rito de quatro etapas: primeiro, o cliente envia um pedido de descoberta em broadcast para toda a rede; o servidor responde com uma oferta de endereço; o cliente solicita formalmente o uso desse IP e, por fim, o servidor envia uma confirmação final. Esse diálogo garante que o dispositivo receba todas as informações necessárias para navegar sem conflitar com outros usuários.

⚙️ Configuração no Roteador   
A maioria dos roteadores domésticos já vem com o serviço DHCP ativo de fábrica, utilizando endereços padrão como o 192.168.0.1 para sua própria identificação. Através da interface web do aparelho, o usuário pode gerenciar o intervalo de endereços disponíveis no "pool" e visualizar quais dispositivos estão conectados, utilizando o próprio IP do roteador como o gateway padrão da rede local.
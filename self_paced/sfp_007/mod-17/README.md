# Networking Basics - Módulo 17   <img src="../0-aux/logo_course.png" alt="sfp_007" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">sfp_007 (Networking Basics)   <img src="../0-aux/logo_course.png" alt="sfp_007" width="auto" height="25"></a>
### Module: 17. Utilitários de teste de rede

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

### Course Module 17 Structure:
17. <a name="item17">Utilitários de teste de rede</a><br>
  17.1 <a href="#item17.01">Introdução</a><br>
  17.2 <a href="#item17.02">Comandos para solução de problemas</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;17.2.1 <a href="../../../pkt/files/pkt_067/">Packet Tracer - Use o comando ipconfig</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;17.2.2 <a href="../../../pkt/files/pkt_068/">Packet Tracer – Uso do comando ping</a><br>
  17.3 <a href="#item17.03">Resumo das Network Testing Utilities</a><br>
  17.4 Exame de ponto de verificação: protocolos para tarefas específicas<br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item17.01"><h4>17.1 Introdução</h4></a>[Back to summary](#item17)

🛠️ Diagnóstico e Resolução de Problemas de Rede   
A manutenção da conectividade em ambientes corporativos exige o uso de ferramentas de diagnóstico para identificar a origem de falhas técnicas. O processo de solução de problemas (troubleshooting) baseia-se em uma abordagem sistemática, utilizando utilitários de linha de comando para testar a comunicação entre o host local, o gateway padrão e destinos externos. A interpretação correta dos resultados desses comandos permite isolar se a interrupção ocorre na infraestrutura interna, no hardware terminal ou no fornecimento de serviços do provedor de internet (ISP).

🎯 Objetivo do módulo:   
- Utilizar utilitários de rede para testar a conectividade e solucionar falhas de comunicação em diferentes camadas.

📘 Tópicos do módulo:   
- Comandos para solução de problemas: Aplicação prática de ferramentas de diagnóstico para verificação de endereçamento, latência e integridade do caminho de rede.

<a name="item17.02"><h4>17.2 Comandos para solução de problemas</h4></a>[Back to summary](#item17)

🩺 Diagnóstico de Rede: Metodologia e Ferramentas de Linha de Comando   
As falhas de conectividade exigem uma abordagem metódica para a identificação da origem do problema. A maioria dos sistemas operacionais disponibiliza utilitários via interface de linha de comando (CLI) que permitem inspecionar desde a configuração lógica local até a integridade dos caminhos remotos.

🛠️ Principais Utilitários de Diagnóstico   
Abaixo, encontram-se as ferramentas fundamentais para a análise de tráfego e conectividade:
- ipconfig: Detalhamento das configurações de rede do host.
- ping: Teste de acessibilidade entre nós da rede IP.
- netstat: Monitoramento das conexões ativas e portas em uso.
- tracert: Rastreamento do caminho físico e lógico percorrido pelos pacotes até o destino.
- nslookup: Consulta direta a servidores de nomes para verificação de domínios.

🔍 Inspeção Lógica com o comando ipconfig   
A ausência ou incorreção de parâmetros de IP impede qualquer comunicação externa ou local. No ambiente Windows, o comando ipconfig atua como o primeiro nível de diagnóstico.
- ipconfig (Básico): Apresenta o endereço IP, a máscara de sub-rede e o gateway padrão.
- ipconfig /all: Fornece uma visão profunda, incluindo o endereço físico (MAC), servidores DNS e detalhes da concessão do servidor DHCP. Esta opção é vital para confirmar se o host consegue resolver nomes ou se possui uma identidade física válida.
- ipconfig /release e /renew: Utilizados em endereçamentos dinâmicos para descartar a configuração atual e solicitar novos dados ao servidor DHCP. Este procedimento resolve falhas causadas por informações obsoletas ou conflitos de endereçamento.

Ponto de Verificação: Caso o comando de renovação falhe, recomenda-se a inspeção física da placa de rede (NIC). A ausência de luzes de atividade (link light) sugere problemas no cabeamento ou na porta do switch, enquanto a presença de sinal físico sem resposta lógica aponta para falhas no servidor DHCP.

📡 Verificação de Conectividade com o ping   
O ping é a ferramenta de teste de alcance mais difundida. O funcionamento baseia-se no envio de um pacote de solicitação de eco (Echo Request) via protocolo ICMP. Se o destino estiver ativo e o caminho desimpedido, ocorre o retorno de uma resposta de eco (Echo Reply).
- Lógica de Diagnóstico via Ping:
  - Teste por IP vs. Nome: Ao realizar o teste para um endereço IP com sucesso, mas falhar ao utilizar o nome do host (ex: www.google.com), identifica-se uma falha específica no serviço de DNS.
- Escopo da Falha:
  - Sucesso no Gateway: O problema reside fora da rede local (na infraestrutura do provedor ou no destino).
  - Falha no Gateway: O problema é interno, possivelmente na configuração do host ou no ativo de rede local.
- Barreiras de Segurança: É possível que o teste falhe mesmo com a rede funcional, caso existam firewalls ou regras de segurança em roteadores configurados para bloquear mensagens ICMP.

📉 Análise de Resultados   
Mensagens como "Tempo de solicitação esgotado" (Request Timed Out) indicam que o pacote foi enviado, mas não houve resposta dentro do prazo esperado. Se o teste de conectividade for positivo para o endereço e para o nome, mas a aplicação continuar inacessível, a causa provável reside em falhas na própria camada de aplicação do servidor de destino, e não na infraestrutura de transporte da rede.

<a name="item17.03"><h4>17.3 Resumo das Network Testing Utilities</h4></a>[Back to summary](#item17)

🛠️ Utilitários de Diagnóstico CLI   
A maioria dos sistemas operacionais oferece ferramentas de linha de comando fundamentais para identificar e solucionar falhas de conectividade. Entre as principais, destacam-se comandos para visualizar configurações de interface, testar a presença de outros hosts, monitorar conexões ativas, rastrear o caminho físico dos dados e consultar bases de dados de nomes de domínio.

💻 Visualização com ipconfig   
O comando ipconfig é a ferramenta primária para verificar a identidade lógica de um host na rede. Ao ser executado, ele fornece um resumo rápido contendo o endereço IPv4 atual, a máscara de sub-rede que define o tamanho da rede local e o gateway padrão, que é a porta de saída obrigatória para o tráfego que se destina à internet.

🔍 Detalhamento e Endereço Físico   
Ao utilizar a variação `ipconfig /all`, o sistema entrega um relatório técnico completo sobre as interfaces de rede. Além dos dados básicos, essa opção revela o endereço físico (MAC) da placa, os servidores DNS configurados e detalhes específicos do DHCP, como o endereço do servidor que forneceu o IP e o tempo de validade do aluguel daquela conexão.

🔄 Gestão de Endereçamento Dinâmico   
Para resolver problemas causados por configurações de rede obsoletas ou corrompidas, utilizam-se os comandos de liberação e renovação. O `ipconfig /release` descarta o endereço IP atual, enquanto o `ipconfig /renew` força o dispositivo a entrar em contato com o servidor DHCP para solicitar novos dados de rede, sendo um passo essencial para restaurar conectividade em redes dinâmicas.

📡 Teste de Alcance com Ping   
O ping é o utilitário mais comum para validar se um dispositivo remoto está ativo e acessível através do protocolo IP. Ele funciona através do envio de um pacote de "solicitação de eco"; se o destino estiver operacional, ele devolve uma "resposta de eco" para a origem. Receber essa resposta confirma não apenas que o host está ligado, mas que todo o caminho de rede entre os dois pontos está funcional.
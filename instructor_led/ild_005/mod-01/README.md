# CCNA: Switching, Routing, and Wireless Essentials - Módulo 1   <img src="../0-aux/logo_course.png" alt="ild_005" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_005 (CCNA: Switching, Routing, and Wireless Essentials)   <img src="../0-aux/logo_course.png" alt="ild_005" width="auto" height="25"></a>
### Module: 1. Configuração básica de dispositivos

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

### Course Module 1 Structure:
1. <a name="item01">Configuração básica de dispositivos</a><br>
  1.1 <a href="item01.01">Introdução</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;1.1.1 <a href="../../../pkt/files/pkt_053/">Packet Tracer - Exploração dos modos lógico e físico</a><br>
  1.2 <a href="item01.02">Configurar um switch com definições iniciais</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;1.2.1 <a href="../../../pkt/files/pkt_087/">Packet Tracer - Configuração Básica do Switch - Modo Físico</a><br>
  1.3 <a href="item01.03">Configurar portas de switch</a><br>
  1.4 <a href="item01.04">Acesso remoto seguro</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;1.4.1 <a href="../../../pkt/files/pkt_070/">Packet Tracer - Configuração do SSH</a><br>
  1.5 <a href="item01.05">Configuração básica do roteador</a><br>
  1.6 <a href="item01.06">Verificar redes conectadas diretamente</a><br>
  1.7 <a href="item01.07">Módulo Prática e Quiz</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;1.7.1 <a href="../../../pkt/files/pkt_090/">Packet Tracer - Implementar uma rede pequena</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;1.7.2 <a href="../../../pkt/files/pkt_091/">Packet Tracer - Configurações Básicas do Roteador - Modo Físico</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01.01"><h4>1.1 Introdução</h4></a>[Back to summary](#item01)

⚙️ Configuração Inicial e Gerenciamento de Dispositivos de Rede   
O controle operacional de uma infraestrutura de comunicação exige a parametrização precisa de switches e roteadores, superando as definições de fábrica para atender aos requisitos específicos de topologia, desempenho e segurança. A aplicação de rotinas de configuração inicial em ativos de rede permite o estabelecimento de conectividade fim a fim entre redes distintas, a implementação de acesso remoto protegido para administração e a validação contínua da funcionalidade física e lógica dos segmentos interconectados.

🎯 Objetivo do módulo:   
Explicar e aplicar as configurações iniciais de segurança, conectividade e simulação em ativos de rede.

📘 Tópicos do módulo:   
- Parametrização de Switches: Definição das configurações iniciais e operacionais no ambiente IOS da Cisco.
- Configuração de Portas: Adequação das interfaces físicas e lógicas aos requisitos da infraestrutura.
- Gerenciamento Remoto Seguro: Implementação de protocolos de acesso protegido para administração dos dispositivos.
- Roteamento Básico via CLI: Parametrização de roteadores para viabilizar a comunicação entre redes diretamente conectadas.
- Validação de Conectividade: Verificação e diagnóstico do tráfego de dados entre segmentos de rede contíguos.

<a name="item01.02"><h4>1.2 Configurar um switch com definições iniciais</h4></a>[Back to summary](#item01)

🔄 Processo de Inicialização do Switch   
A inicialização de um switch Cisco ocorre em cinco etapas sequenciais a partir do momento em que o equipamento é ligado:
- Autoteste de Inicialização (POST): Execução de um programa armazenado na ROM para testar o subsistema da CPU, a memória DRAM e a porção do dispositivo flash que constitui o sistema de arquivos.
- Carga do Boot Loader: Carregamento de um pequeno programa residente na ROM, executado imediatamente após o sucesso do POST.
- Inicialização de Baixo Nível da CPU: O boot loader configura os registradores da CPU, mapeando a memória física, definindo sua quantidade e velocidade de operação.
- Inicialização do Sistema de Arquivos: O boot loader disponibiliza o sistema de arquivos da memória flash integrada.
- Carga do Sistema Operacional (IOS): Localização e carregamento da imagem do IOS na RAM, transferindo o controle do equipamento para o sistema operacional.

A localização do arquivo de imagem do IOS é determinada pela variável de ambiente BOOT. Caso essa variável esteja ausente, o dispositivo busca e executa o primeiro arquivo executável presente na memória flash. Após o carregamento do IOS, as interfaces são configuradas com base nos comandos gravados no arquivo de configuração inicial (config.text na flash).

A definição manual do caminho de boot é feita no modo de configuração global: `S1(config)# boot system flash:/c2960-lanbasek9-mz.150-2.SE/c2960-lanbasek9-mz.150-2.SE.bin`.

💡 Indicadores Luminosos (LEDs) e Painel Frontal   
O painel frontal dos switches Cisco Catalyst dispõe do botão Mode, utilizado para alternar a exibição de informações de estado nas portas físicas, e de LEDs indicadores do sistema:
- SYST (Sistema): Indica o estado de alimentação e funcionamento do equipamento. A cor verde sinaliza operação normal; a cor âmbar indica que a alimentação foi recebida, mas há falha funcional; a ausência de iluminação indica falta de energia.
- RPS (Fonte Redundante): Indica o estado da fonte de alimentação auxiliar. Verde continuo indica prontidão; verde piscante significa fornecimento ativo de energia para outro dispositivo; âmbar fixo aponta modo de espera ou falha; âmbar piscante sinaliza falha na fonte interna do switch, com o RPS assumindo a operação.
- STAT (Status da Porta): Exibe o estado operacional das portas quando selecionado (modo padrão). Verde indica link estabelecido; verde piscante sinaliza tráfego de dados; alternância verde/âmbar indica falha no link; âmbar fixo ou piscante aponta bloqueio da porta para prevenção de loops de camada 2.
- DUPLX (Duplex da Porta): Exibe a configuração duplex. LEDs de porta apagados indicam operação em half-duplex; LEDs na cor verde indicam full-duplex.
- SPEED (Velocidade da Porta): Sinaliza a velocidade do link. LED apagado indica 10 Mbps; verde indica 100 Mbps; verde piscante indica 1000 Mbps (1 Gbps).
- PoE (Power over Ethernet): Presente em modelos com suporte a fornecimento de energia. Apagado indica ausência do modo selecionado ou portas operando sem falhas; verde indica o modo PoE selecionado com portas alimentadas; alternância verde/âmbar indica solicitação de energia acima do limite do switch; âmbar fixo ou piscante aponta negação de energia ou falha no sistema PoE.

🛠️ Recuperação e Linha de Comando do Boot Loader   
Quando o IOS falha ou está ausente, o boot loader provê uma interface de linha de comando (prompt switch:) acessível via conexão de console para manutenção do sistema, alteração de variáveis e recuperação de senhas.

O procedimento de interrupção da inicialização para acesso ao boot loader consiste em:
- Conectar o terminal à porta de console e desconectar a alimentação do switch.
- Reconectar o cabo de força e, dentro de 15 segundos, manter pressionado o botão Mode enquanto o LED SYST piscar em verde.
- Soltar o botão Mode quando o LED SYST alternar brevemente para âmbar e fixar em verde.

Após a exibição do prompt switch:, os comandos de preparação e carga manual do sistema incluem: `flash_init`, `dir flash:`, `BOOT=flash:c2960-lanbasek9-mz.150-2.SE.bin`, `set` e `boot`.

🌐 Configuração do Acesso de Gerenciamento Remoto   
O gerenciamento remoto do switch exige a atribuição de um endereço IP e máscara de sub-rede a uma Interface Virtual do Switch (SVI). Por razões de segurança, recomenda-se a criação de uma VLAN de gerenciamento dedicada, evitando o uso da VLAN 1 nativa.

Antes de definir endereçamentos em pilha dupla no modelo Catalyst 2960 com IOS 15.0, é necessário ajustar a alocação de memória do modelo de banco de dados do sistema (SDM) e reiniciar o equipamento: `sdm prefer dual-ipv4-and-ipv6 default` e `reload`.

🌐 Configuração do Acesso de Gerenciamento Remoto
O gerenciamento remoto do switch exige a atribuição de um endereço IP e máscara de sub-rede a uma Interface Virtual do Switch (SVI). Por razões de segurança, recomenda-se a criação de uma VLAN de gerenciamento dedicada, evitando o uso da VLAN 1 nativa. A SVI permanece em estado operacional inativo até que a VLAN correspondente seja criada e exista ao menos uma porta física ativa associada a ela.

As etapas para estruturação e validação do acesso remoto compreendem:
- Ajuste de Pilha Dupla (SDM): Em modelos Catalyst 2960 com IOS 15.0, ativa-se o suporte simultâneo a IPv4 e IPv6 ajustando o banco de dados do sistema com `sdm prefer dual-ipv4-and-ipv6 default` no modo de configuração global e reiniciando o equipamento com `reload`.
- Endereçamento da Interface Virtual: O acesso à SVI é feito com interface vlan 99, aplicando o endereço IPv4 via `ip address 172.17.99.11 255.255.255.0` e o IPv6 via `ipv6 address 2001:db8:acad:99::1/64`. A interface é habilitada com `no shutdown`, encerra-se o modo de configuração com `end` e salva-se a alteração com `copy running-config startup-config`.
- Definição do Gateway Padrão: Para permitir a comunicação com sub-redes remotas, configura-se o gateway IPv4 no modo global via `ip default-gateway 172.17.99.1`. O protocolo IPv6 não exige essa etapa manual, pois descobre o roteador de saída automaticamente por mensagens de anúncio de roteador (RA).
- Verificação das Interfaces: A confirmação do estado operacional e dos endereços configurados é realizada no modo EXEC privilegiado através dos comandos `show ip interface brief` e `show ipv6 interface brief`.

O endereçamento aplicado à SVI destina-se exclusivamente ao acesso administrativo do switch, não habilitando o roteamento de pacotes na Camada 3 entre VLANs.

<a name="item01.03"><h4>1.3 Configurar portas de switch</h4></a>[Back to summary](#item01)

⚡ Modos de Transmissão Duplex e Velocidade   
As portas de um switch operam em modos de comunicação bidirecional (full-duplex) ou unidirecional (half-duplex). A operação em full-duplex desativa os circuitos de detecção de colisão da interface e permite a transmissão e recepção simultânea de dados, dobrando a taxa teórica de transferência e eliminando o domínio de colisão. Esse modo é obrigatório para o funcionamento de interfaces Gigabit e 10 Gb Ethernet. Por outro lado, o modo half-duplex limita o fluxo a um sentido por vez, sendo comum em dispositivos legados como hubs e sujeito a quedas de desempenho por colisões.

As configurações de velocidade e modo duplex podem ser ajustadas manualmente ou tratadas via negociação automática:
- Definição Manual: Recomendada para conexões estratégicas com servidores e dispositivos de infraestrutura. No modo de configuração de interface, aplicam-se os comandos `duplex full` e `speed 100`.
- Negociação Automática: Padrão em equipamentos Catalyst, permitindo que a interface ajuste seus parâmetros conforme o dispositivo conectado. Portas de fibra óptica operam exclusivamente com velocidade predefinida e modo full-duplex.

Em conexões manuais, a divergência de parâmetros entre as pontas do enlace gera falhas diretas de conectividade.

🔀 Funcionalidade Auto-MDIX   
A tecnologia Auto-MDIX detecta o tipo de cabo conectado (direto ou cruzado) e ajusta os pinos da interface para estabelecer o enlace. O uso desse recurso elimina a necessidade de cabos específicos para interconectar switches, roteadores ou servidores.

Para o funcionamento correto do Auto-MDIX, a interface deve estar configurada para negociar velocidade e duplex de forma automática. Nos modelos Catalyst 2960 e 3560, o recurso vem habilitado por padrão e pode ser gerenciado no modo de interface com o comando `mdix auto`. A verificação do estado operacional dessa função é realizada através do comando `show controllers ethernet-controller phy | include Auto-MDIX`.

🔍 Comandos de Verificação e Diagnóstico   
A verificação das configurações ativas e do estado operacional do switch utiliza comandos executados no modo EXEC privilegiado:
- `show interfaces [interface-id]`: Exibe o estado físico do link, protocolo de camada de enlace, velocidade, duplex e contadores de erros.
- `show running-config`: Apresenta a configuração em execução, incluindo atribuição de VLANs, endereçamento IP de gerenciamento e gateway padrão.
- `show startup-config`: Exibe a configuração salva na memória não volátil.
- `show version`: Detalha informações de hardware, versão do IOS e licenças ativos.
- `show mac address-table`: Mapeia os endereços físicos associados a cada porta.
- `show flash` e `show history`: Exibem o conteúdo do sistema de arquivos e o histórico recente de comandos executados.

Ao analisar a saída de `show interfaces`, o status up/up indica funcionamento correto. Um estado up/down aponta incompatibilidade de encapsulamento ou falhas de camada de enlace. O status down/down indica cabo desconectado ou equipamento oposto desligado, enquanto administratively down sinaliza que a interface foi desativada manualmente com o comando `shutdown`.

⚠️ Monitoramento de Erros de Mídia   
Estatísticas de falhas acumuladas nas estatísticas da interface ajudam a diagnosticar degradações de desempenho no cabeamento e na sinalização:
- Erros de Entrada (Input Errors): Somatório das falhas na recepção de quadros, abrangendo descartes por tamanho, integridade ou estouro de buffer.
- Runts: Quadros recebidos com tamanho inferior ao limite mínimo de 64 bytes, originados por colisão ou defeitos na placa de rede.
- Giants: Quadros que ultrapassam o tamanho máximo de 1.518 bytes.
- Erros de CRC: Incompatibilidade no código de verificação de redundância cíclica, indicando interferência eletromagnética, conectores danificados ou cabeamento com ruído excessivo.
- Erros de Saída (Output Errors): Falhas associadas ao envio de dados a partir da interface.
- Colisões Tardias (Late Collisions): Colisões registradas após a transmissão dos primeiros 512 bits do quadro. Ocorrem devido ao comprimento excessivo do cabo ou divergência no modo duplex (uma ponta configurada em half-duplex e a outra em full-duplex).

🛠️ Metodologia de Solução de Problemas em Enlaces   
A resolução de falhas de conectividade física ou lógica entre dispositivos segue um fluxo estruturado de análise:
- Interface em Estado Inativo (Down): Verificar a integridade dos cabos, conectores e especificações do meio físico. Se o cabeamento estiver normal, checar divergências na velocidade. Definir manualmente a mesma velocidade em ambas as extremidades caso a negociação automática falhe.
- Interface Ativa (Up), mas com Perda de Pacotes: Avaliar a presença de ruído elétrico e contadores de erros de entrada como runts e CRC. Eliminar fontes de interferência, validar se a extensão do cabo respeita os limites do padrão Ethernet e substituir cabos danificados.
- Ocorrência de Colisões Excessivas ou Tardias: Validar se as configurações de duplex nas pontas do enlace estão idênticas. Caso persista a falha de negociação, fixar o modo como duplex full em ambos os lados da conexão.

<a name="item01.04"><h4>1.4 Acesso remoto seguro</h4></a>[Back to summary](#item01)

🔒 Acesso Remoto Seguro com SSH   
O gerenciamento remoto de dispositivos de rede exige a proteção dos dados transmitidos contra interceptação. O protocolo Telnet utiliza a porta TCP 23 e envia credenciais e comandos em texto puro, permitindo que analisadores de tráfego capturem informações sensíveis como nomes de usuário e senhas.

Para garantir a confidencialidade e a integridade da conexão, deve-se utilizar o protocolo SSH (Secure Shell), que opera na porta TCP 22. O SSH estabelece um canal de comunicação criptografado que protege o processo de autenticação e todo o tráfego de dados transmitido entre o administrador e o equipamento.

🛠️ Requisitos e Etapas de Configuração do SSH   
A implementação do SSH em switches Cisco Catalyst exige que o sistema operacional possua suporte a recursos criptográficos. Essa capacidade é identificada pela presença da sigla k9 no nome do arquivo do IOS, verificável no modo EXEC privilegiado através do comando `show version`.

O procedimento para habilitar o SSH versão 2 no switch compreende os seguintes passos:
- Validação do Suporte ao Protocolo: Executar `show ip ssh` para confirmar se o sistema operacional instalado reconhece os comandos do SSH.
- Configuração do Domínio IP: Definir um nome de domínio para a rede no modo de configuração global utilizando o comando `ip domain-name cisco.com`. O domínio é parte integrante da identificação da chave de criptografia.
- Geração das Chaves RSA: Criar o par de chaves de criptografia com o comando `crypto key generate rsa`. Deve-se especificar um tamanho de módulo seguro, como 1024 bits ou superior. A geração dessas chaves ativa automaticamente o serviço SSH no switch. Caso seja necessário desativar o serviço e remover as chaves, utiliza-se o comando `crypto key zeroize rsa`.
- Criação de Credenciais Locais: Definir uma conta de usuário no banco de dados local do equipamento via `username admin secret ccna` para autenticação de acesso.
- Restrição das Linhas VTY: Acessar o intervalo de linhas virtuais com `line vty 0 15`, aplicar a obrigatoriedade da autenticação local com `login local` e restringir o protocolo de entrada exclusivamente ao SSH com `transport input ssh`. Essa ação impede tentativas de conexão não criptografadas via Telnet.
- Fixação do SSH Versão 2: Habilitar estritamente a versão 2 do protocolo com o comando de configuração global `ip ssh version 2`, eliminando vulnerabilidades conhecidas da versão 1.

💻 Conexão Cliente e Verificação de Estado   
O acesso remoto ao switch a partir de uma estação de trabalho é realizado através de programas clientes SSH, como o PuTTY, direcionando a conexão para a porta TCP 22 e informando o endereço IP da interface virtual de gerenciamento (SVI).

Após a solicitação de conexão, o terminal requisita o nome de usuário e a senha configurados no banco de dados local. Após a validação bem-sucedida das credenciais, a sessão criptografada é estabelecida e o acesso à CLI do switch é liberado.

A validação das configurações ativas do servidor SSH, a verificação da versão em execução e a checagem dos parâmetros globais do protocolo são realizadas no equipamento com o comando `show ip ssh`.

<a name="item01.05"><h4>1.5 Configuração básica do roteador</h4></a>[Back to summary](#item01)

🌐 Configuração Básica e Inicial de Rroteadores   
Roteadores e switches Cisco compartilham o mesmo sistema operacional (IOS), estrutura modal e comandos fundamentais de inicialização. As etapas de configuração básica visam estabelecer a identidade do equipamento, restringir o acesso administrativo, definir avisos legais e armazenar as parâmetros na memória permanente.

A sequência de comandos para a parametrização inicial do roteador abrange:
- Identificação do Equipamento: Definição do nome do dispositivo com `hostname R1` no modo de configuração global.
- Proteção de Acessos Privilegiados: Aplicação de senha criptografada para o modo EXEC privilegiado via `enable secret class`.
- Segurança das Linhas Físicas e Virtuais: Proteção da porta de console com `line console 0`, definição da senha com `password cisco` e solicitação de autenticação com `login`. O mesmo procedimento aplica-se às sessões remotas via `line vty 0 4`.
- Criptografia Geral de Senhas: Proteção de senhas exibidas em texto claro nos arquivos de configuração com o comando `service password-encryption`.
- Notificação Legal: Exibição de mensagem de aviso contra acessos não autorizados por meio de `banner motd #Authorized Access Only!#`.
- Salvamento da Configuração: Persistência dos dados da memória RAM para a memória não volátil NVRAM via `copy running-config startup-config`.

🔌 Configuração de Interfaces LAN e WAN   
Diferente dos switches de Camada 2 — focados prioritariamente em conexões LAN —, os roteadores interconectam redes distintas e suportam uma diversidade maior de interfaces físicas (Gigabit Ethernet, seriais e módulos de alta velocidade).

Para que uma interface de roteador passe ao estado operacional ativo, são exigidas as seguintes condições:
- Atribuição de Endereçamento: Definição do endereço IPv4 via `ip address [endereço] [máscara]` e do IPv6 via `ipv6 address [endereço]/[prefixo]`.
- Habilitação Administrativa: As interfaces do roteador permanecem desligadas por padrão e exigem o comando `no shutdown` para inicialização da sinalização elétrica.
- Conectividade Física: Presença de cabo conectado a um equipamento funcional oposto para estabelecer o link da Camada 1.
- Documentação Descritiva: Adição opcional de um texto explicativo de até 240 caracteres com `description [texto]`, facilitando o diagnóstico de falhas e a identificação de enlaces em ambientes de produção.

A definição dos parâmetros em uma interface Gigabit Ethernet é feita acessando `interface gigabitethernet 0/0/0`, configurando o IPv4 com `ip address 192.168.10.1 255.255.255.0`, o IPv6 com `ipv6 address 2001:db8:acad:1::1/64`, a descrição com `description Link to LAN 1` e ativando a porta com `no shutdown`. Em interfaces seriais, utiliza-se a mesma lógica acessando `interface serial 0/0/0`, atribuindo o IPv4 via `ip address 2009.165.200.225 255.255.255.252`, o IPv6 com `ipv6 address 2001:db8:acad:3::225/64`, a descrição com description `Link to R2` e ativando o meio com `no shutdown`.

🔄 Interfaces Virtuais Loopback   
A interface de loopback é uma interface lógica interna do roteador, sem vínculo a portas físicas e permanentemente no estado up/up enquanto o equipamento estiver energizado.

As utilidades e características dessa interface lógica incluem:
- Garantia de Acessibilidade: Prover um endereço IP estável para o gerenciamento administrativo e identificação do roteador, imune a falhas em links físicos individuais.
- Testes e Emulação de Redes: Simulação de sub-redes e links externos (como conexões de Internet) em ambientes de laboratório e validação de protocolos de roteamento interno sem necessidade de hardware adicional.
- Unicidade do Endereçamento: Cada interface loopback requer um endereço IP exclusivo dentro do dispositivo.

A criação e endereçamento da interface lógica é realizada diretamente na CLI entrando no modo de interface lógica com `interface loopback 0`, atribuindo o endereço IPv4 por meio de `ip address 10.0.0.1 255.255.255.0` e retornando ao nível anterior com `exit`.

<a name="item01.06"><h4>1.6 Verificar redes conectadas diretamente</h4></a>[Back to summary](#item01)

🔍 Comandos de Verificação e Validação de Interfaces   
A verificação das configurações de rede e do status operacional no roteador é realizada por meio de comandos show no modo EXEC privilegiado, garantindo a validação da conectividade e do endereçamento:
- Resumo de Interfaces: Os comandos `show ip interface brief` e `show ipv6 interface brief` exibem uma lista simplificada das portas físicas e lógicas, seus endereços IP e o estado das camadas física (Status) e de enlace (Protocol). O resultado up/up indica funcionamento correto.
- Endereçamento IPv6 nas Interfaces: A visualização em `show ipv6 interface brief` revela dois endereços por interface ativa: o endereço Unicast Global (GUA) configurado manualmente e o endereço Link-Local (iniciado pelo prefixo FE80), gerado automaticamente para comunicação no mesmo segmento.
- Detalhamento de Interfaces: O comando `show ip interface [interface-id]` ou `show ipv6 interface [interface-id]` detalha parâmetros de camada 3, incluindo os grupos multicast associados (prefixo FF02 no IPv6). Para consultar estritamente os comandos aplicados na CLI para uma porta, utiliza-se `show running-config interface [interface-id]`.
- Diagnóstico Abrangente: O comando `show interfaces` fornece estatísticas detalhadas de tráfego e contadores de fluxo para todas as portas do dispositivo.

🛣️ Análise da Tabela de Roteamento e Conectividade   
A verificação do encaminhamento de pacotes e das redes ativas é feita consultando a tabela de roteamento residente na RAM através dos comandos `show ip route` e `show ipv6 route`:
- Redes Conectadas (Código C): Indicam as sub-redes diretamente vinculadas às interfaces ativas do roteador em estado up/up.
- Rotas Locais (Código L): Representam o endereço IP específico atribuído à interface do próprio dispositivo. Possuem máscara /32 no IPv4 e /128 no IPv6, permitindo que o roteador processe pacotes endereçados a si próprio de forma otimizada.
- Teste de Conectividade: O comando `ping [endereço-IP]` valida a acessibilidade na Camada 3 tanto para IPv4 quanto para IPv6, confirmando a troca de pacotes entre o roteador e outros dispositivos da rede.

⚙️ Recursos de Produtividade na Linha de Comando (CLI)   
O IOS dispõe de funcionalidades para otimizar a navegação, exibição e filtragem de dados no terminal de gerenciamento:
- Controle de Paginação: O comando `terminal length 0` desativa a pausa automática --More-- exibida a cada 24 linhas, permitindo a visualização contínua de saídas extensas.
- Filtragem de Saída com Pipe: A inclusão do caractere | após qualquer comando show permite refinar o resultado retornado. Usa-se section para exibir o bloco completo de uma configuração, include para listar apenas linhas correspondentes a um termo, exclude para omitir linhas específicas e begin para mostrar o texto a partir de uma palavra-chave.
- Histórico de Comandos: O buffer armazena por padrão os últimos 10 comandos executados, navegáveis pelas teclas de seta para cima e para baixo (ou Ctrl+P e Ctrl+N). A exibição do histórico é feita com `show history`, e o limite de retenção da sessão pode ser expandido com `terminal history size 200`.

<a name="item01.07"><h4>1.7 Módulo Prática e Quiz</h4></a>[Back to summary](#item01)

⚡ Boot e Monitoramento do Switch   
A inicialização de um switch Cisco ocorre em cinco fases subsequentes, utilizando a variável global BOOT para apontar o caminho do arquivo do IOS na memória flash. Na ausência de um sistema operacional válido, a linha de comando do carregador de inicialização permite recuperar o acesso aos arquivos armazenados. Para fins de diagnóstico contínuo, os LEDs frontais do painel indicam o estado de funcionamento de recursos como PoE, estatísticas de portas e duplex.

🌐 Configuração de Gerenciamento do Switch   
A gestão remota de um switch exige a definição de um endereço IP, máscara de sub-rede e gateway padrão associados à interface virtual do sistema. A preparação da SVI estabelece o ponto de acesso administrativo necessário para viabilizar conexões originadas de sub-redes distintas.

🔌 Modos de Operação das Interfaces de Rede   
O envio e o recebimento concomitante de quadros ocorrem em conexões full-duplex, maximizando a taxa de transferência disponível, enquanto o modo half-duplex limita a navegação a um único sentido por vez. O ajuste dessas taxas pode ser estático ou gerenciado por negociação automática, complementado pelo recurso auto-MDIX para identificação automática de cabos diretos ou cruzados.

📊 Diagnóstico e Erros na Camada de Acesso   
A validação de portas é realizada com a checagem das definições ativas e do estado dos protocolos de enlace. A identificação de quadros fora do padrão, como runts e gigantes, somada ao registro de erros de verificação de redundância e colisões no tráfego, aponta problemas de conectividade ou desalinhamento de configurações físicas.

🔒 Protocolos de Acesso Remoto   
O gerenciamento remoto legado via porta TCP 23 transmite credenciais e informações em texto limpo, gerando vulnerabilidades de segurança. A adoção da porta TCP 22 via SSH contorna essa fragilidade ao aplicar criptografia forte no processo de autenticação e na troca de pacotes entre as extremidades.

🗝️ Requisitos e Implementação do SSH   
A presença do termo "k9" na imagem do sistema operacional confirma o suporte a algoritmos criptográficos necessários para a execução do SSH versão 2. O processo de ativação envolve a definição do domínio da rede, a geração de chaves RSA, a configuração de contas de usuários locais e a restrição de acesso nas linhas de navegação virtual.

📝 Ajustes Iniciais de Dispositivos   
A preparação básica de um ativo de rede inclui a atribuição de uma identificação única no sistema, o estabelecimento de senhas administrativas para controle de acesso, a exibição de avisos legais na entrada e a gravação permanente das alterações no arquivo de inicialização.

🔀 Características de Interfaces de Rede   
A diferenciação entre equipamentos reside na capacidade e diversidade de conexões suportadas, variando entre portas locais fixas de alta velocidade em switches e conectores modulares para redes amplas em roteadores. Ambientes de pilha dupla integram o endereçamento IPv4 e IPv6 simultaneamente nessas interfaces.

🛰️ Tipos de Conexão em Roteadores   
Os roteadores utilizam portas físicas integradas e expansões para placas de comunicação WAN, cobrindo cenários com linhas seriais, DSL ou cabo. Para testes e funções internas, o sistema operacional dispõe de interfaces lógicas que dispensam associação com portas físicas e permanecem ativas sem conexões externas.

🔎 Comandos para Verificação de Interfaces   
O acompanhamento do status operacional e dos endereços atribuídos às interfaces é feito por comandos que mostram um resumo compacto da camada de rede. Comandos adicionais permitem inspecionar as instruções aplicadas a uma porta específica ou consultar o estado do encaminhamento de pacotes na memória principal.

🏷️ Detalhamento de Endereçamento em Interfaces   
A inspeção aprofundada de uma interface de rede revela o estado do link físico, os endereços de alcance local e global, além dos grupos multicast aos quais a porta pertence. Essa verificação garante o correto alinhamento dos parâmetros de camada três no roteador.

🛠️ Auditoria e Filtros de Linha de Comando   
As consultas ao sistema podem ter sua saída filtrada por meio do caractere de canalização, permitindo buscar termos específicos ou delimitar o início da exibição. O sistema mantém um histórico automático das últimas instruções digitadas no modo privilegiado para facilitar a auditoria e reutilização de comandos.
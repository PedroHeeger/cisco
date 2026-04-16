# CCNA: Introduction to Networks - Módulo 2   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_001 (CCNA: Introduction to Networks)   <img src="../0-aux/logo_course.png" alt="ild_001" width="auto" height="25"></a>
### Module: 2. Switch básico e configuração de dispositivo final

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

### Course Module 2 Structure:
2. <a name="item02">Switch básico e configuração de dispositivo final</a><br>
  2.1 <a href="#item02.01">Introdução</a><br>
  2.2 <a href="#item02.02">Acesso ao Cisco IOS</a><br>
  2.3 <a href="#item02.03">Navegação IOS</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.3.1 <a href="#item02.03.01">Verificador de Sintaxe - Navegar entre modos IOS</a><br>
  2.4 <a href="#item02.04">A Estrutura de Comandos</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.4.1 <a href="../../../pkt/files/pkt_002/">Packet Tracer - Navegue no IOS</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.4.2 <a href="../../../pkt/files/pkt_003/">Packet Tracer - Navegue pelo IOS usando Tera Term para conectividade de console</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.4.3 <a href="../../../pkt/files/pkt_003/">Laboratório - Navegue pelo IOS usando Tera Term para conectividade de console</a><br>
  2.5 <a href="#item02.05">Configuração básica de dispositivos</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.5.1 <a href="#item02.05.01">Verificador de Sintaxe - Configuração básica do dispositivo</a><br>
  2.6 <a href="#item02.06">Salvar configurações</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.6.1 <a href="../../../pkt/files/pkt_007/">Packet Tracer - Definir configurações iniciais do switch</a><br>
  2.7 <a href="#item02.07">Portas e Endereços</a><br>
  2.8 <a href="#item02.08">Configurar Endereços IP</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.8.1 <a href="#item02.08.01">Verificador de sintaxe - Verifique a configuração de IP do PC do Windows</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.8.2 <a href="#item02.08.02">Verificador de sintaxe - Configurar uma interface virtual do switch</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.8.3 <a href="../../../pkt/files/pkt_008/">Packet Tracer - Implementação da conectividade básica</a><br>
  2.9 <a href="#item02.09">Verificar a conectividade</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.9.1 <a href="../../../pkt/files/pkt_009/">Vídeo Activity - Testar a atribuição de interface</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.9.2 <a href="../../../pkt/files/pkt_010/">Vídeo Activity - Teste a conectividade de ponta a ponta</a><br>
  2.10 <a href="#item02.10">Módulo Prático e Quiz</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.10.1 <a href="../../../pkt/files/pkt_011/">Packet Tracer - Configuração básica do switch e do dispositivo final</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;2.10.2 <a href="../../../pkt/files/pkt_012/">Packet Tracer - Configuração básica do switch e do dispositivo final - Modo Físico</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item02.01"><h4>2.1 Introdução</h4></a>[Back to summary](#item02)

📘 Introdução   
O módulo aborda a configuração básica de switches e dispositivos finais em uma rede. Embora esses dispositivos já possuam configurações padrão, cada rede exige ajustes específicos de endereçamento IP, senhas e parâmetros de gateway. Também são apresentadas as operações essenciais do Cisco IOS, incluindo comandos básicos de configuração, acesso aos dispositivos e verificação da conectividade entre hosts com endereços IP.

🎯 Objetivo Geral   
Antes de avançar na administração de rede, é fundamental configurar switches e dispositivos finais corretamente. Isso inclui definir senhas, endereçamento IP e parâmetros de gateway padrão, garantindo que todos os dispositivos estejam prontos para funcionar.

✅ Objetivos Específicos   
- Explicar como acessar um dispositivo Cisco IOS para configuração.
- Navegar no Cisco IOS para configurar os dispositivos de rede.
- Compreender a estrutura de comandos do Cisco IOS.
- Configurar um dispositivo Cisco IOS usando CLI.
- Salvar a configuração atual usando comandos IOS.
- Entender como os dispositivos se comunicam pelo meio físico da rede.
- Configurar um dispositivo final com endereço IP.
- Verificar a conectividade entre dois dispositivos finais.

<a name="item02.02"><h4>2.2 Acesso ao Cisco IOS</h4></a>[Back to summary](#item02)

💻 Sistemas Operacionais de Dispositivos   
Todos os dispositivos finais e de rede operam a partir de um sistema operacional (SO). O kernel do SO gerencia a comunicação entre hardware e software, enquanto o shell fornece a interface para interações com aplicações e usuários. Essa interação pode ocorrer por meio de uma interface de linha de comando (CLI) ou uma interface gráfica (GUI).

📟 CLI vs GUI   
A CLI permite inserir comandos em um ambiente baseado em texto, oferecendo controle detalhado sobre o sistema com baixo consumo de recursos. Já a GUI utiliza ícones, janelas e menus, facilitando o uso, mas consumindo mais recursos e oferecendo menos controle avançado. Em dispositivos de rede, a CLI é preferida devido à sua estabilidade e eficiência.

🖧 Cisco IOS e Sistemas de Rede   
Dispositivos Cisco utilizam o Cisco Internetwork Operating System (IOS), disponível em versões como IOS, IOS XE, IOS XR e NX-OS. Cada versão atende diferentes tipos de dispositivos e necessidades de recursos. Roteadores domésticos costumam usar firmware, geralmente configurado via GUI. Atualizações de IOS permitem expandir funcionalidades dos dispositivos.

🔌 Portas de Acesso e Conexões   
- Console: Porta física para acesso fora de banda, útil durante a configuração inicial do dispositivo, independente de serviços de rede ativos.
- SSH: Conexão segura em banda para acessar remotamente a CLI, exigindo interfaces de rede ativas.
- Telnet: Conexão em banda não criptografada, recomendada apenas para laboratórios.
- Porta AUX: Conexão fora de banda para sessões CLI via modem, semelhante ao console.

🖥 Programas de Emulação de Terminal   
Programas de emulação permitem conectar-se a dispositivos via console, SSH ou Telnet, oferecendo ajustes de janela, fonte e cores, otimizando a produtividade durante a administração da rede. Exemplos incluem PuTTY, Tera Term, SecureCRT, entre outros.

🔒 Configuração Inicial de Switches   
Switches novos podem encaminhar tráfego imediatamente, mas precisam ser configurados e protegidos para operação segura. Isso inclui definir endereços IP, senhas e políticas de acesso, garantindo controle e gerenciamento eficiente da rede.

<a name="item02.03"><h4>2.3 Navegação IOS</h4></a>[Back to summary](#item02)

🖥️ Modos de Acesso no Cisco IOS   
O Cisco IOS organiza o acesso à CLI em diferentes modos de comando, garantindo segurança e controle sobre o dispositivo.
- Modo EXEC de usuário: Permite apenas comandos básicos de monitoramento. Prompt padrão termina com >. É considerado modo “view-only”.
- Modo EXEC privilegiado: Permite acesso completo a comandos de monitoramento, configuração e gerenciamento. Prompt termina com #. É necessário para acessar modos de configuração avançados.

⚙️ Modo de Configuração Global   
Usado para alterar configurações que afetam o dispositivo como um todo. Prompt termina com (config)#. A partir desse modo, é possível acessar modos de subconfiguração específicos, como:
- Modo de configuração de linha: Ajustes de console, SSH, Telnet ou porta AUX. Prompt: (config-line)#.
- Modo de configuração de interface: Configuração de portas de switch ou interfaces de roteador. Prompt: (config-if)#.

🔄 Navegando entre modos   
- Para acessar o modo EXEC privilegiado: `enable`.
- Retornar ao modo EXEC de usuário: `disable`.
- Entrar no modo de configuração global: `configure terminal`.
- Retornar ao modo EXEC privilegiado: `exit`.
- Sair de modos de subconfiguração: `exit` ou `end` / `Ctrl+Z`.
- Alternar entre modos de subconfiguração diretamente ajusta o prompt conforme o modo selecionado.

🛠️ Prática em Ambiente Seguro   
Testes de configuração devem ser feitos em ambientes de simulação antes de aplicar em dispositivos reais. Ferramentas como:
- Verificador de Sintaxe: Exige comandos completos e corretos para avançar.
- Packet Tracer: Permite comandos abreviados, simulando mais de perto o comportamento em equipamentos reais.

<a name="item02.03.01"><h4>2.3.1 Verificador de Sintaxe - Navegar entre modos IOS</h4></a>[Back to summary](#item02)

- Entre no modo EXEC privilegiado: `enable`.
- Retorne ao modo EXEC do usuário: `disable`.
- Digite novamente o modo EXEC privilegiado: `enable`.
- Entre no modo de configuração global: `configure terminal`.
- Saia do modo de configuração global e retorne ao modo EXEC privilegiado: `exit`.
- Digite novamente o modo de configuração global: `configure terminal`.
- Digite o modo de subconfiguração de linha para a porta do console: `line console 0`.
- Retorne ao modo de configuração global: `exit`.
- Digite o modo de subconfiguração de linha VTY: `line vty 0 15`.
- Retorne ao modo de configuração global: `exit`.
- Entre no modo de subconfiguração de interface VLAN 1: `interface vlan 1`.
- No modo de configuração da interface, alterne para o modo de subconfiguração do console de linha: `line console 0`.
- Retorne ao modo EXEC privilegiado: `end`.

<a name="item02.04"><h4>2.4 A Estrutura de Comandos</h4></a>[Back to summary](#item02)

📚 Estrutura dos Comandos no Cisco IOS   
O Cisco IOS utiliza uma sintaxe padronizada para garantir que cada comando seja interpretado corretamente. Cada instrução é composta pelo comando base, seguido de palavras-chave e, quando necessário, argumentos definidos pelo administrador. Tanto o comando quanto os elementos adicionais só funcionam no modo apropriado da CLI.

🔤 Palavras-Chave e Argumentos   
As palavras-chave representam termos fixos reconhecidos pelo IOS, enquanto os argumentos são valores inseridos pelo usuário. Após digitar a sintaxe completa, o comando é enviado ao interpretador ao pressionar Enter. Quando um comando exige múltiplos argumentos, a ordem e o formato devem seguir exatamente o padrão descrito na sintaxe oficial.

🧩 Como Ler a Sintaxe dos Comandos   
A documentação do IOS utiliza convenções visuais para indicar como um comando deve ser usado:
- **Negrito**: elementos obrigatórios digitados exatamente como mostrados.
- **Itálico**: valores fornecidos pelo usuário.
- **[ ]**: elementos opcionais.
- **{ }**: elementos obrigatórios.
- **{x | y}**: escolha entre opções.
- **[x {y | z}]**: escolha dentro de algo opcional.

Essas regras definem como interpretar a sintaxe e identificar o que deve ou não ser digitado.

📝 Exemplos de Sintaxe   
Comando description utiliza uma estrutura simples em que o argumento é um texto livre. Exemplo: `description Connects to the main headquarter office switch`. Outros comandos seguem o mesmo padrão: `ping ip-address` e `traceroute ip-address`. O termo fixo é o comando; o endereço IP é o argumento inserido pelo usuário.

❓ Ajuda Sensível ao Contexto   
O IOS oferece mecanismos internos para auxiliar na composição correta dos comandos. O caractere ? revela:
- comandos permitidos no modo atual;
- palavras-chave possíveis para o comando iniciado;
- argumentos esperados conforme a posição do cursor.

Outro mecanismo é a verificação automática de sintaxe. Caso algo esteja incorreto, o IOS gera mensagens específicas indicando o erro.

⌨️ Edição e Atalhos na Linha de Comando   
A CLI disponibiliza combinações de teclas que agilizam a edição:
- Tab: completa automaticamente o comando.
- Backspace / Ctrl+D: apagam caracteres.
- Ctrl+K / Esc D: removem do cursor até o fim da linha ou palavra.
- Ctrl+U / Ctrl+X / Ctrl+W: apagam trechos maiores.
- Ctrl+A / Ctrl+E: movem o cursor para o início ou fim.
- Setas, Ctrl+B, Ctrl+F, Esc B, Esc F: movem o cursor por caracteres ou palavras.
- Setas para cima e para baixo, Ctrl+P, Ctrl+N: percorrem o histórico.
- Ctrl+R, Ctrl+I, Ctrl+L: redesenham a linha após mensagens do console.
- A tecla Delete não possui suporte funcional no IOS.

📄 Exibição de Saída – Prompt “More”   
Quando a saída ocupa mais linhas do que a tela suporta, o IOS pausa com o indicador “--More--”.
- Enter exibe a próxima linha.
- Barra de espaço avança uma página.
- Qualquer outra tecla encerra a exibição.

🛑 Saída de Comandos e Interrupções   
Algumas combinações permitem interromper ações ou sair de modos mais rapidamente:
- Ctrl+C: encerra operações e retorna ao modo EXEC privilegiado.
- Ctrl+Z: sai do modo de configuração.
- Ctrl+Shift+6: interrompe processos como ping, traceroute ou consultas DNS.

<a name="item02.05"><h4>2.5 Configuração básica de dispositivos</h4></a>[Back to summary](#item02)

📌 Nomeação de dispositivos
O primeiro passo na configuração é atribuir um nome único e descritivo ao equipamento. Nomes padronizados de fábrica dificultam identificação e documentação. Uma convenção clara (local, função, andar, etc.) facilita gerenciamento e suporte. Recomenda-se usar apenas letras, números e traços, começar com letra, evitar espaços e manter menos de 64 caracteres.

🔐 Senhas e boas práticas   
Senhas fracas são uma das maiores causas de comprometimento. Aplicar senhas fortes, únicas por dispositivo e com mais de oito caracteres (maiúsculas, minúsculas, números e símbolos) reduz riscos. Em ambientes de produção, evitar palavras comuns e reciclagem de senhas. Ferramentas geradoras de senhas ajudam a criar credenciais seguras.

🎛️ Proteção dos acessos administrativos   
O acesso ao console físico deve exigir senha para impedir acesso não autorizado. O modo privilegiado (que concede controle total do equipamento) também precisa de senha protegida. Linhas de gerenciamento remoto (VTY) devem ser protegidas para controlar Telnet/SSH e limitar acessos externos. A aplicação consistente de senhas em todos os pontos de acesso é fundamental.

🔏 Criptografia no arquivo de configuração   
Configurações em execução e de inicialização podem revelar senhas em texto claro. Aplicar a criptografia disponível no sistema impede a visualização direta das credenciais nesses arquivos, reduzindo o risco caso alguém consiga acesso à configuração armazenada. Importante lembrar: essa criptografia protege a exibição no arquivo, não o tráfego de rede.

📢 Mensagem de aviso (banner)   
Adicionar um banner de aviso (MOTD) deixa explícito que somente pessoal autorizado deve acessar o equipamento e pode ter implicações legais em casos de invasão. Utilizar um delimitador para inserir a mensagem e manter a linguagem institucional apropriada.

<a name="item02.05.01"><h4>2.5.1 Verificador de Sintaxe - Configuração básica do dispositivo</h4></a>[Back to summary](#item02)

- Entre no modo de configuração global: `configure terminal`.
- Nomeie o switch "Sw-Floor-1": `hostname Sw-Floor-1`.
- Proteja o acesso no modo EXEC do usuário inserindo line console 0, atribuindo a senha cisco, habilitando o login e retornando ao modo de configuração global usando exit:
  - `line console 0`.
  - `password cisco`.
  - `login`.
  - `exit`.
- Proteja o acesso ao modo EXEC privilegiado usando a senha class: `enable secret class`.
- Proteja as linhas VTY 0 a 15, atribua a senha cisco, habilite o login e volte ao modo de configuração global usando exit:
  - `line vty 0 15`.
  - `password cisco`.
  - `login`.
  - `exit`.
- Criptografe todas as senhas em texto simples: `service password-encryption`.
- Crie uma mensagem de banner usando o símbolo "#" como delimitador. O banner deve exibir exatamente "Apenas acesso autorizado": `banner motd # Apenas acesso autorizado #`.

<a name="item02.06"><h4>2.6 Salvar configurações</h4></a>[Back to summary](#item02)

💾 Arquivos de configuração   
O dispositivo trabalha com dois arquivos principais. O arquivo de inicialização fica na NVRAM e guarda a configuração que será usada após ligar ou reiniciar. O arquivo em execução fica na RAM e representa a configuração ativa no momento, sendo perdido sempre que o equipamento reinicia.

👁️ Visualização das configurações   
A configuração ativa pode ser visualizada pelo comando apropriado no modo privilegiado, exibindo tudo o que está carregado na RAM. A configuração de inicialização também pode ser listada para verificar o que será aplicado após uma reinicialização.

📥 Salvando alterações   
Alterações feitas na configuração ativa não são permanentes até serem gravadas na configuração de inicialização. Se a energia cair, tudo que não foi salvo é perdido. Para evitar isso, sempre salvar as mudanças após concluir ajustes no equipamento.

♻️ Restaurando configurações   
Caso ajustes feitos na configuração ativa não funcionem como esperado e ainda não tenham sido salvos, existe a opção de voltar ao estado anterior reiniciando o dispositivo. Essa ação remove apenas o conteúdo ativo e restaura aquilo que está salvo. O ponto negativo é o tempo de indisponibilidade durante o processo.

🧹 Limpando configurações   
Quando alterações indesejadas já foram salvas, pode ser necessário apagar completamente a configuração de inicialização. Após limpar esse arquivo, o próximo reinício fará o switch carregar a configuração padrão de fábrica. Esse procedimento remove tanto a configuração salva quanto a ativa.

📁 Arquivando configurações em arquivo   
É possível registrar a configuração do equipamento em um arquivo de texto usando o software de terminal. O log captura toda a saída exibida na tela, incluindo a configuração listada. Esse arquivo serve como histórico, documentação ou base para recuperar a configuração no futuro.

🔄 Restaurando a partir de arquivo   
Para restaurar uma configuração arquivada, basta entrar no modo de configuração global e colar o conteúdo do arquivo na janela do terminal. Cada linha será aplicada automaticamente, recriando a configuração ativa no dispositivo.

<a name="item02.07"><h4>2.7 Portas e Endereços</h4></a>[Back to summary](#item02)

🌐 Endereçamento dos dispositivos finais   
Para que dispositivos finais consigam trocar dados entre si, cada um precisa de um endereço IP válido e de uma conexão física adequada. O endereço IP permite que cada equipamento seja localizado dentro da rede e estabeleça comunicação ponto a ponto. Exemplos de dispositivos finais incluem computadores, impressoras, telefones VoIP, câmeras, smartphones e equipamentos móveis.

🔢 Estrutura do IPv4   
O endereço IPv4 utiliza quatro valores decimais separados por ponto, indo de 0 a 255. Cada dispositivo recebe um endereço próprio dentro da rede. Além do endereço, é necessário informar a máscara de sub-rede, que identifica qual parte do endereço representa a rede e qual representa o host. Também pode existir um gateway padrão, que é o endereço do roteador usado para alcançar redes externas.

🆕 Endereços IPv6   
O IPv6 utiliza 128 bits e é representado por valores hexadecimais separados por dois pontos. Um conjunto de quatro bits forma um dígito hexadecimal, resultando em um total de 32 dígitos. As letras podem aparecer em maiúsculas ou minúsculas sem diferença funcional.

🔌 Interfaces e meios físicos   
A comunicação depende das interfaces presentes nos dispositivos e dos cabos utilizados. Cada interface segue padrões específicos, e o cabo precisa ser compatível com esses padrões. Os principais tipos de mídia incluem cabos de cobre de par trançado, fibra óptica, cabo coaxial e conexões sem fio.

📏 Diferenças entre os tipos de mídia   
Cada tipo de meio físico possui características próprias, como a distância que suporta, o ambiente de instalação adequado, a taxa e velocidade de transmissão e o custo de material e instalação. Essas diferenças determinam qual meio é mais adequado para cada situação.

🏠 Tecnologias de rede e portas   
Internet e redes locais utilizam diferentes tecnologias. Ethernet é a tecnologia predominante nas LANs e está presente na maioria das portas de dispositivos finais, switches e equipamentos de rede que usam cabos para conexão física.

🖧 Portas e interfaces em switches   
Switches de Camada 2 possuem portas físicas usadas para conexões Ethernet, mas essas portas não aceitam endereços IP porque não operam na Camada 3. Para permitir gerenciamento remoto, o switch conta com interfaces virtuais criadas via software chamadas SVIs. A interface VLAN1 é a SVI padrão presente na configuração inicial.

🔑 Função da SVI   
A SVI fornece um endereço IP para gerenciamento remoto do equipamento utilizando IPv4 ou IPv6. Mesmo assim, o switch continua operando normalmente sem depender desse endereço, já que ele não é necessário para o funcionamento das funções de comutação.

<a name="item02.08"><h4>2.8 Configurar Endereços IP</h4></a>[Back to summary](#item02)

📡 Necessidade de endereços IP   
Dispositivos de uma rede precisam de endereços IP para trocar informações entre si. O endereço identifica cada equipamento e permite que a comunicação ocorra de forma organizada e direcionada.

📝 Configuração manual de IPv4   
O endereço IPv4 pode ser inserido manualmente em um dispositivo final. Em sistemas Windows, a definição de endereço, máscara de sub-rede e gateway padrão é feita na área de propriedades do adaptador de rede. As configurações de IPv6 seguem uma lógica semelhante à do IPv4.

🌐 Função do DNS   
Servidores DNS utilizam endereços IPv4 ou IPv6 para traduzir nomes de domínio em endereços IP. Essa conversão permite acessar serviços utilizando nomes legíveis em vez de números.

⚙️ Configuração automática com DHCP   
A maior parte das redes usa DHCP para atribuir endereços IPv4 automaticamente. O protocolo distribui endereço IP, máscara, gateway e DNS sem necessidade de configuração manual. Isso reduz erros, evita duplicidades e elimina o trabalho de configurar cada equipamento individualmente.

🔄 DHCP em dispositivos Windows   
Quando a opção de obtenção automática de endereço é ativada, o dispositivo procura um servidor DHCP e recebe as informações necessárias para participar da rede. No caso do IPv6, a atribuição dinâmica utiliza DHCPv6 ou SLAAC.

🖧 Endereçamento em switches   
Para permitir acesso remoto a um switch, é necessário configurar um endereço IP em sua interface virtual. A SVI, associada à VLAN 1 por padrão, recebe o endereço IP e a máscara de sub-rede. Após atribuir o endereço, a interface virtual precisa ser ativada para que o switch possa ser alcançado via rede.

<a name="item02.08.01"><h4>2.8.1 Verificador de sintaxe - Verifique a configuração de IP do PC do Windows</h4></a>[Back to summary](#item02)

- Insira o comando para exibir a configuração IP em um PC com Windows: `ipconfig`.

<a name="item02.08.02"><h4>2.8.2 Verificador de sintaxe - Verifique a configuração de IP do PC do Windows</h4></a>[Back to summary](#item02)

- Entre no modo de configuração de interface de VLAN 1: `interface vlan 1`.
- Configure o endereço IPv4 como 192.168.1.20 e a máscara de sub-rede como 255.255.255.0: `ip address 192.168.1.20 255.255.255.0`.
- Habilite a interface: `no shutdown`.

<a name="item02.09"><h4>2.9 Verificar a conectividade</h4></a>[Back to summary](#item02)

Neste módulo só houveram duas atividades do Packet Tracer (PTTA), listadas abaixo.

- <a href="#item02.09.01">Atividade de vídeo - Testar a atribuição de interface</a><br>
- <a href="#item02.09.02">Atividade em vídeo - Teste a conectividade de ponta a ponta</a><br>

<a name="item02.10"><h4>2.10 Módulo Prático e Quiz</h4></a>[Back to summary](#item02)

🖥️ Sistemas operacionais nos dispositivos   
Todos os dispositivos de rede precisam de um sistema operacional. O usuário pode interagir com o sistema usando uma CLI, digitando comandos e visualizando a saída no monitor.

🔐 Modos de acesso no Cisco IOS   
O Cisco IOS separa o gerenciamento em dois modos: EXEC de Usuário (acesso básico) e EXEC Privilegiado (acesso avançado). O gerenciamento completo ocorre a partir do modo privilegiado.

⚙️ Modos de configuração   
O modo de configuração global permite acessar modos específicos, como configuração de linha e configuração de interface. O comando `configure terminal` entra no modo global; o comando `exit` retorna ao modo EXEC privilegiado.

⌨️ Sintaxe e ajuda dos comandos   
Cada comando tem uma sintaxe correta e só funciona no modo apropriado. O IOS oferece ajuda sensível ao contexto e verificação de sintaxe para auxiliar o usuário durante a configuração.

🏷️ Nome do dispositivo e senhas   
O primeiro passo na configuração é definir um nome exclusivo ao dispositivo. Senhas devem ser configuradas e criptografadas para garantir segurança. Também é possível exibir um banner avisando que somente pessoas autorizadas devem acessar o equipamento.

💾 Arquivos de configuração   
O Cisco IOS trabalha com dois arquivos: *running-config* (configuração atual) e *startup-config* (configuração salva). Se as alterações na configuração atual não forem salvas, elas serão perdidas ao reiniciar o dispositivo.

🌐 Endereçamento IPv4   
Cada dispositivo de rede precisa de um endereço IP para se comunicar. Um endereço IPv4 segue a notação decimal com ponto, composta por quatro números entre 0 e 255.

⚡ DHCP e configuração automática   
Os endereços podem ser configurados manualmente ou atribuídos automaticamente usando DHCP, que distribui endereços IP para todos os dispositivos habilitados na rede.

🖧 Configuração de SVI no switch   
Para acessar um switch remotamente, é necessário configurar um endereço IP na interface virtual VLAN 1 (SVI), já que ela representa uma interface lógica, não física.

🔍 Verificação de conectividade e interfaces   
Comandos como `show ip interface brief` mostram o estado das interfaces do switch. O comando `ping` permite testar a comunicação com outros dispositivos ou até com sites da Internet.
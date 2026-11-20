# Networking Devices and Initial Configuration - Módulo 10   <img src="../0-aux/logo_course.png" alt="sfp_008" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">sfp_008 (Networking Devices and Initial Configuration)   <img src="../0-aux/logo_course.png" alt="sfp_008" width="auto" height="25"></a>
### Module: 10. A linha de comando do Cisco IOS

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

### Course Module 10 Structure:
10. <a name="item10">A linha de comando do Cisco IOS</a><br>
  10.1 <a href="#item10.01">Introdução</a><br>
  10.2 <a href="#item10.02">Navegação IOS</a><br>
  10.3 <a href="#item10.03">A estrutura de comandos</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;10.3.1 <a href="../../../pkt/files/pkt_002/">Packet Tracer - Navegue no IOS</a><br>
  10.4 <a href="#item10.04">Exibir Informações do dispositivo</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;10.4.1 <a href="../../../pkt/files/pkt_069/">Packet Tracer - Usando comandos Show do Cisco IOS</a><br>
  10.5 <a href="#item10.05">Resumo Linha de Comando do Cisco IOS</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item10.01"><h4>10.1 Introdução</h4></a>[Back to summary](#item10)

🛠️ Navegação e Operação do Sistema Operacional Cisco IOS   
A administração de ativos de rede baseados na tecnologia Cisco exige o domínio de seu sistema operacional embarcado, o Cisco IOS. O gerenciamento e a personalização desses equipamentos ocorrem por meio de uma interface de linha de comando estruturada em níveis de privilégio distintos. A correta operação dessa interface envolve a compreensão de sua sintaxe e o uso de comandos específicos para configurar parâmetros, validar alterações e acompanhar o estado operacional dos dispositivos de interconexão.

🎯 Objetivo do módulo:   
- Operar o sistema operacional Cisco IOS para realizar configurações e monitorar o status de dispositivos de rede.

📘 Tópicos do módulo:   
- Navegação IOS: Utilização prática de comandos específicos para alternar de forma estruturada entre os modos de operação e de configuração do sistema.
- A estrutura de comandos: Análise da sintaxe, dos parâmetros e das regras de validação necessárias para a inserção correta de diretivas nos equipamentos.
- Exibir Informações do dispositivo: Aplicação de comandos de verificação para inspecionar parâmetros operacionais, tabelas internas e o status das interfaces do hardware.

<a name="item10.02"><h4>10.2 Navegação IOS</h4></a>[Back to summary](#item10)

💻 A Interface de Linha de Comando (CLI) no Cisco IOS   
A CLI (Command Line Interface) do Cisco IOS consiste em um ambiente operacional baseado estritamente em texto, projetado para a inserção e execução de diretivas que permitem parametrizar, monitorar e gerenciar os ativos de rede da Cisco. O acesso a essa interface pode ser estabelecido por meio de estratégias de gerenciamento fora de banda (utilizando uma conexão física dedicada à porta de console) ou em banda (através de conexões de rede seguras como o SSH).

A estrutura de comandos é consistente em quase todo o portfólio de hardware da fabricante. Essa padronização permite que analistas de infraestrutura utilizem a mesma base de comandos e a mesma lógica de navegação tanto para gerenciar switches quanto roteadores. Assim que o hardware conclui o seu processo de inicialização (boot), o sistema exibe o prompt inicial, indicando que a interface está pronta para receber instruções.

Em comparação com as interfaces gráficas (GUIs), a linha de comando confere ao administrador maior flexibilidade, velocidade de execução e precisão no controle dos processos internos do sistema operacional. Além disso, o ambiente conta com um sistema de ajuda integrado para auxiliar na sintaxe das instruções.

🔒 Níveis de Acesso e Modos de Operação   
Como diretriz de segurança e controle de privilégios, o Cisco IOS fragmenta o ambiente de gerenciamento em diferentes níveis de operação. O acesso inicial é dividido em dois modos de comando principais:

🔎 1. Modo EXEC do Usuário (User EXEC Mode)   
Trata-se do nível de entrada no dispositivo, caracterizado operacionalmente como um modo de "somente visualização".
- Capacidades: Apresenta recursos restritos, permitindo a execução de apenas um conjunto limitado de comandos básicos de monitoramento e diagnóstico de conectividade.
- Restrições: O usuário não possui autorização para realizar qualquer modificação nas configurações globais ou locais do hardware, protegendo o ativo contra alterações acidentais.
- Identificação do Prompt: Este modo é facilmente reconhecido na CLI porque o nome do dispositivo é sucedido pelo caractere maior que, exibido nos formatos Switch> ou Router>.

🔑 2. Modo EXEC Privilegiado (Privileged EXEC Mode)   
Este nível confere autoridade total sobre o sistema operacional do ativo, sendo o ponto de partida para a administração avançada.
- Capacidades: Permite o uso de todas as diretivas de monitoramento, ferramentas de auditoria e comandos de gerenciamento do sistema. É a partir deste modo que o técnico ganha permissão para ingressar nos níveis superiores de parametrização, como o modo de configuração global.
- Restrições: O acesso a este modo deve ser protegido por senhas complexas, pois comandos executados aqui podem alterar o comportamento operacional do dispositivo ou interromper o tráfego da rede.
- Identificação do Prompt: Este modo é reconhecido na CLI porque o nome do dispositivo passa a ser sucedido pelo caractere cerquilha, exibido nos formatos Switch# ou Router#.

<a name="item10.03"><h4>10.3 A estrutura de comandos</h4></a>[Back to summary](#item10)

💻 Estrutura de Sintaxe e Convenções do Cisco IOS   
Para operar a interface de linha de comando com precisão, é necessário compreender a anatomia de uma instrução no Cisco IOS. Cada comando possui uma estrutura padronizada e linear, constituída pelo prompt do modo atual, o comando em si, e elementos adicionais separados obrigatoriamente por espaços. Esses componentes adicionais dividem-se em duas categorias:
- Palavras-chave: Parâmetros fixos e predefinidos no código do sistema operacional. Eles funcionam como diretivas específicas que determinam a ação do comando (por exemplo, o termo protocols ip).
- Argumentos: Valores variáveis fornecidos pelo próprio administrador para contextualizar a instrução. Não são predefinidos pelo sistema (por exemplo, o endereço 192.168.10.5).

Após a digitação completa do comando com seus respectivos parâmetros, o envio das informações para o interpretador do sistema ocorre ao pressionar a tecla Enter. 

Na documentação técnica e nas referências oficiais da Cisco, adota-se um conjunto de convenções tipográficas para descrever como os comandos complexos devem ser estruturados:
- Texto em Negrito: Indica os comandos e as palavras-chave que o operador deve digitar textualmente na linha de comando.
- Texto em Itálico: Representa as variáveis e argumentos onde o usuário deve fornecer um valor real de configuração.
- Colchetes [ x ]: Delimitam componentes de caráter puramente opcional dentro da estrutura da instrução.
- Chaves { x }: Sinalizam a obrigatoriedade de preenchimento daquele elemento ou argumento específico.
- Construções combinadas [ x { y | z } ]: Linhas verticais dentro de chaves e colchetes indicam que o usuário deve fazer uma escolha obrigatória entre duas ou mais opções fornecidas, mas toda essa escolha reside dentro de um bloco que é opcional na instrução global.

Como exemplo de aplicação prática, o comando utilizado para inserir comentários de identificação em uma interface segue o formato description string, onde o termo string é o argumento textual criado pelo técnico. Em diagnósticos lógicos, o comando de teste básico adota a sintaxe ping ip-address (como em ping 10.10.10.5) e a verificação de rotas segue o modelo traceroute ip-address (como em traceroute 192.168.254.254). A fonte definitiva para sanar dúvidas sobre estes formatos é a Referência de Comandos do Cisco IOS.

🏎️ Atalhos de Produtividade e Edição de Linha de Comando   
O interpretador de comandos dispõe de recursos que aceleram a digitação e facilitam as rotinas de configuração e diagnóstico. Comandos e palavras-chave podem ser abreviados para a menor quantidade de caracteres que mantenha o termo exclusivo no sistema. O comando configure, por exemplo, aceita a abreviação conf, pois nenhuma outra instrução compartilha essa raiz; contudo, a redução para con gerará um erro por ambiguidade.

Para otimizar o fluxo de trabalho, os seguintes recursos e atalhos de teclado são implementados na CLI:
- Mecanismos de Digitação e Navegação do Cursor:
  - Tecla Tab: Completa de forma automática o nome de um comando ou palavra-chave que foi digitado parcialmente.
  - Tecla Seta para a Esquerda ou Ctrl+B: Desloca o cursor um caractere para trás sem apagar o texto.
  - Tecla Seta para a Direita ou Ctrl+F: Avança o cursor um caractere para a frente.
  - Combinação Esc B: Recua o cursor uma palavra inteira para a esquerda.
  - Combinação Esc F: Avança o cursor uma palavra inteira para a direita.
  - Ctrl+A: Posiciona o cursor de forma imediata no início da linha de comando atual.
  - Ctrl+E: Posiciona o cursor de forma imediata no término da linha de comando.
- Recursos de Exclusão e Limpeza de Linha:
  - Tecla Backspace: Remove o caractere localizado imediatamente à esquerda do cursor.
  - Ctrl+D: Elimina o caractere que está posicionado exatamente sob o cursor. (Nota: A tecla física Delete não é reconhecida pela estrutura do Cisco IOS).
  - Ctrl+W: Apaga a palavra inteira situada à esquerda do cursor.
  - Combinação Esc D: Elimina todos os caracteres a partir da posição do cursor até o final da palavra atual.
  - Ctrl+K: Remove todo o conteúdo da linha a partir da posição atual do cursor até o final da frase.
  - Ctrl+U ou Ctrl+X: Limpa instantaneamente todos os caracteres digitados do cursor até o início da linha.
- Histórico de Comandos e Atualização do Prompt:
  - Tecla Seta para Cima ou Ctrl+P: Varre o buffer de histórico recuperando os comandos executados anteriormente, dos mais recentes para os mais antigos.
  - Tecla Seta para Baixo ou Ctrl+N: Avança para a próxima instrução armazenada no histórico de comandos.
  - Ctrl+R (ou Ctrl+I / Ctrl+L): Força a reexibição do prompt e da linha de comando atual, o que é útil quando mensagens de sistema (syslogs) surgem no console e quebram a visualização do texto que estava sendo editado.

🛑 Gerenciamento de Saídas e Interrupção de Processos   
Sempre que a resposta a uma consulta gera um volume de texto superior à capacidade vertical da janela do terminal, o Cisco IOS pausa a rolagem automática e exibe o prompt indicador --More-- na base da tela. O avanço dessas informações deve ser controlado por meio das seguintes teclas:
- Tecla Enter: Avança a exibição do relatório em uma linha adicional por vez.
- Tecla Espaço (ou a tecla "y"): Avança a paginação exibindo uma tela inteira de conteúdo de cada vez.
- Qualquer outra tecla: Interrompe imediatamente a rolagem do relatório e devolve o controle ao prompt de comando do modo atual.

Para abortar operações ativas ou sair dos níveis de configuração do dispositivo, utilizam-se as seguintes combinações de controle:
- Ctrl+C: Interrompe qualquer nível de parametrização de forma imediata e retorna o console para o modo EXEC privilegiado. Se utilizado durante o assistente de inicialização (setup mode), retorna o usuário ao prompt inicial.
- Ctrl+Z: Desativa os modos de configuração globais ou de subinterfaces e devolve o controle do prompt para o nível EXEC privilegiado.
- Ctrl+Shift+6: Funciona como uma sequência de quebra universal de processos. Este atalho é utilizado para forçar o cancelamento imediato de buscas DNS demoradas, execuções de comandos traceroute, sequências de ping ou qualquer outra rotina interna travada no Cisco IOS.

<a name="item10.04"><h4>10.4 Exibir Informações do dispositivo</h4></a>[Back to summary](#item10)

🛠️ Comandos de Verificação Operacional (Comandos show) no Cisco IOS   
O sistema operacional Cisco IOS disponibiliza uma série de diretivas de diagnóstico estruturadas sob o comando show. Essas instruções funcionam como ferramentas de auditoria essenciais para técnicos e analistas de infraestrutura, permitindo inspecionar arquivos de parametrização, monitorar o status de interfaces físicas e validar o comportamento operacional de quase todos os processos e funções ativos em roteadores e switches.

Abaixo encontram-se os comandos de verificação mais utilizados na rotina de suporte e quando cada um deles deve ser aplicado:
- show running-config: Utilizado para inspecionar e auditar os parâmetros e configurações que estão em execução ativa na memória RAM do hardware no momento atual.
- show interfaces: Empregado para checar o status físico e lógico de todas as interfaces do ativo, permitindo o acompanhamento de contadores de tráfego, taxas de utilização e a identificação de mensagens de erro ou descarte de quadros.
- show ip interface: Focado na auditoria de parâmetros da Camada 3 (Rede), servindo para validar o endereçamento IPv4 associado às interfaces, além de exibir o estado de recursos como filtros de pacotes e diretrizes de mascaramento.
- show arp: Destinado à consulta da tabela de cache ARP local do dispositivo, listando os mapeamentos ativos entre os endereços lógicos IPv4 e os respectivos endereços físicos MAC das estações localizadas nas redes locais conectadas.
- show ip route: Comando fundamental para a verificação da tabela de roteamento de Camada 3, permitindo ao administrador conferir as redes conhecidas pelo dispositivo, as rotas estáticas configuradas, as rotas aprendidas via protocolos dinâmicos e as interfaces de saída para o encaminhamento de pacotes.
- show protocols: Aplicado para realizar uma varredura global e identificar quais protocolos de rede e de roteamento estão ativos e operacionais no sistema.
- show version: Fornece um relatório detalhado sobre o hardware e o software do ativo. Exibe o tempo de atividade (uptime), a versão do firmware em uso, a quantidade de memória instalada, o inventário de interfaces físicas disponíveis e o status das licenças de recursos ativas.

<a name="item10.05"><h4>10.5 Resumo Linha de Comando do Cisco IOS</h4></a>[Back to summary](#item10)

⌨️ Interface de Linha de Comando Cisco IOS   
O Cisco IOS CLI funciona como um ambiente textual dedicado à inserção e execução de instruções técnicas para ajustar, acompanhar e gerenciar o estado operacional de ativos da marca. Os administradores podem interagir com essa interface de duas formas principais: de maneira local e isolada, conhecida como gerência fora da banda, ou remotamente através da própria rede de dados, chamada de gerência em banda.

🚦 Modos de Operação e Segurança   
Com o objetivo de restringir privilégios e blindar a infraestrutura contra alterações acidentais, o sistema operacional da Cisco segmenta seus níveis de acesso em estágios bem definidos. Após concluir o processo de inicialização do hardware, a CLI se apresenta em uma estrutura de camadas lógicas, onde cada nível determina o poder de execução do operador técnico sobre as funções internas do equipamento.

👤 Modo EXEC do Usuário   
O ponto de entrada inicial na CLI é o nível básico de visualização, projetado exclusivamente para tarefas simples de monitoramento e diagnósticos de rotina que não oferecem riscos à estabilidade do sistema. Esse estágio impede qualquer modificação nos arquivos operacionais do aparelho e pode ser facilmente reconhecido na linha de comando pelo uso do caractere maior que no prompt.

🔓 Modo EXEC Privilegiado   
Para obter acesso completo aos recursos de modificação e auditoria profunda do hardware, o profissional precisa elevar seus privilégios para o nível avançado. Identificado visualmente pelo símbolo de cerquilha no prompt, este estágio atua como o único trampolim de segurança a partir do qual é possível invocar os níveis superiores de parametrização do equipamento, como o ambiente de ajuste global.

🌍 Configuração Global e Submodos   
O estágio de parametrização global, sinalizado na CLI pela nomenclatura entre parênteses acompanhada da cerquilha, é o local onde comandos que impactam o funcionamento de todo o chassi são aplicados. A partir dele, o administrador consegue filtrar ainda mais o foco da CLI para realizar ajustes em componentes específicos, abrindo submodos direcionados para portas físicas, terminais virtuais ou canais de gerenciamento local.

🧭 Comandos de Navegação Interna   
A movimentação entre as diferentes esferas de controle do sistema ocorre por meio de palavras-chave padronizadas que abrem ou fecham os níveis de privilégio. Instruções específicas permitem subir um degrau na hierarquia de permissões ou recuar para estágios anteriores, enquanto atalhos de teclado e termos de encerramento conseguem interromper o submodo atual de forma abrupta, devolvendo o operador diretamente para a raiz do nível de controle avançado.

📐 Regras de Sintaxe e Parâmetros   
Toda instrução digitada no sistema deve respeitar uma ordem gramatical estrita para ser interpretada corretamente pelo hardware, consistindo no comando principal acompanhado de suas respectivas diretrizes adicionais. O sistema operacional diferencia esses complementos entre palavras-chave, que são termos fixos e nativos do próprio software, e argumentos, que representam as variáveis numéricas ou textuais definidas pelo próprio usuário.

📋 Convenções de Documentação Técnica   
Os manuais técnicos de redes utilizam uma padronização visual específica para instruir os profissionais sobre como preencher a sintaxe de cada comando sem gerar erros de digitação. Palavras que devem ser copiadas exatamente iguais aparecem destacadas, enquanto as variáveis editáveis ficam inclinadas; além disso, elementos que possuem uso facultativo aparecem envolvidos por colchetes, e as opções de preenchimento obrigatório são delimitadas por chaves.
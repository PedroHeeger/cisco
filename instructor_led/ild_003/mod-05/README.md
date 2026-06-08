# Fundamentos de Redes - Módulo 5   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_003 (Fundamentos de Redes)   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="25"></a>
### Module: 5. Princípios de comunicação

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

### Course Module 5 Structure:
5. <a name="item05">Princípios de comunicação</a><br>
  5.1 <a href="#item05.01">Introdução</a><br>
  5.2 <a href="#item05.02">Protocolos de comunicação</a><br>
  5.3 <a href="#item05.03">Padrões de comunicação</a><br>
  5.4 <a href="#item05.04">Modelos de comunicação de rede</a><br>
  5.5 <a href="#item05.05">Resumo dos Princípios de comunicação</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item05.01"><h4>5.1 Introdução</h4></a>[Back to summary](#item05)

📑 Protocolos e Modelos de Referência em Redes   
A comunicação eficiente em sistemas computacionais exige a adoção de regras predefinidas que governam a troca de informações entre entidades distintas. Assim como na interação humana, onde a escolha de um idioma comum e a confirmação de recebimento são fundamentais, as redes de dados operam sob protocolos e padrões técnicos que asseguram a interoperabilidade, a integridade e a entrega correta das mensagens em ambientes heterogêneos.

🎯 Objetivo do módulo:   
- Explicar a relevância dos padrões técnicos e dos protocolos para a viabilização das comunicações em redes de dados.

📘 Tópicos do módulo:   
- Protocolos de comunicação: Descrição do conjunto de regras que gerenciam o empacotamento, endereçamento e transporte de dados.
- Padrões de comunicação: Análise das normas estabelecidas por organizações internacionais para garantir a compatibilidade entre diferentes fabricantes.
- Modelos de comunicação de rede: Estudo comparativo entre as arquiteturas em camadas dos modelos de referência OSI e TCP/IP.

<a name="item05.02"><h4>5.2 Protocolos de comunicação</h4></a>[Back to summary](#item05)

💬 Fundamentos da Comunicação e Protocolos   
A interação comunicativa, seja no cotidiano humano ou entre sistemas computacionais, exige a definição prévia de regras e acordos que garantam a compreensão mútua. Esses conjuntos de normas são denominados protocolos e estabelecem parâmetros críticos como o método de transmissão, o idioma utilizado e a necessidade de confirmação de recebimento. A eficácia do processo depende de que o emissor e o receptor estejam devidamente identificados e operem sob uma gramática e ritmo comuns.

🌐 Protocolos de Rede e Interconectividade   
No contexto das redes de computadores, os protocolos são essenciais para que os dispositivos interconectados em uma rede local consigam trocar informações. Sem a adoção de um protocolo comum, a comunicação entre hosts torna-se impossível, de forma análoga a uma conversa entre pessoas que não compartilham o mesmo idioma. Esses regulamentos técnicos padronizam a forma como os dados são preparados, enviados e interpretados.

⚙️ Parâmetros Operacionais dos Protocolos   
A arquitetura de comunicação em rede é regida por diretrizes específicas que controlam cada etapa do tráfego de dados:
- Formato da Mensagem: Define a estrutura e a organização dos dados, que variam conforme a natureza da mensagem e o canal de entrega utilizado.
- Tamanho da Mensagem: Estabelece limites para os pacotes transmitidos. Mensagens extensas são fragmentadas em partes menores para assegurar que o transporte através do meio físico ocorra de maneira estável e confiável.
- Temporização: Controla a velocidade de transmissão dos bits e regula os momentos em que um host pode iniciar o envio de informações, além de gerenciar a quantidade de dados permitida em cada transmissão.
- Codificação: Consiste na conversão da informação em padrões de bits, que são traduzidos em sinais elétricos, ondas luminosas ou impulsos de rádio, dependendo do meio físico. No destino, o processo inverso de decodificação permite a reconstrução da mensagem original.
- Encapsulamento: Processo de inserção de cabeçalhos nos dados, contendo informações de endereçamento da origem e do destino. Este mecanismo garante que a mensagem seja encaminhada corretamente até a aplicação correspondente no receptor.
- Padrão da Mensagem: Define o comportamento da comunicação, podendo exigir uma confirmação de recebimento antes do envio da próxima sequência (modelo de solicitação/resposta) ou permitindo o fluxo contínuo de dados sem rastreamento de entrega.

<a name="item05.03"><h4>5.3 Padrões de comunicação</h4></a>[Back to summary](#item05)

🌐 Padronização e Interoperabilidade Global   
O gerenciamento das constantes inovações tecnológicas e a oferta de serviços estáveis, como o correio eletrônico, baseiam-se na aplicação de padrões da internet. Um padrão é definido como um conjunto normativo que orienta a implementação uniforme de protocolos em diferentes equipamentos. Essa conformidade garante que dispositivos de naturezas distintas, como computadores pessoais e smartphones, consigam trocar informações de maneira transparente, seguindo estruturas idênticas para a formatação e o encaminhamento de dados.

📝 Desenvolvimento e Documentação Técnica   
A consolidação de um padrão ocorre após ciclos rigorosos de debate, resolução de falhas e validação técnica. Diversas organizações internacionais são responsáveis pelo desenvolvimento e pela manutenção dessas diretrizes, assegurando a evolução coordenada da rede global.

O processo de criação de normas é documentado e monitorado através de mecanismos específicos:
- RFC (Request for Comments): Consistem em documentos numerados que registram cada etapa do desenvolvimento de um protocolo, desde a proposta inicial até a aprovação final, permitindo o acompanhamento de sua evolução.
- IETF (Internet Engineering Task Force): Atua como a principal entidade encarregada da publicação e do gerenciamento das RFCs, servindo como o fórum técnico central para a evolução dos padrões da internet.
- Entidades de Normatização: Diversas organizações colaboram na sustentação da infraestrutura lógica da rede, garantindo que as regras de comunicação permaneçam universais e independentes de fabricantes específicos.

<a name="item05.04"><h4>5.4 Modelos de comunicação de rede</h4></a>[Back to summary](#item05)

📚 Fundamentos dos Modelos em Camadas   
A utilização de modelos em camadas permite a visualização do funcionamento integrado de diversos protocolos em uma rede. Esse método de organização descreve as operações internas de cada nível e a forma como ocorre a interação com as camadas adjacentes.

Nota-se que essa estrutura oferece vantagens significativas, como a facilitação no design de novos protocolos e o estímulo à concorrência, permitindo que produtos de diferentes fabricantes operem de forma conjunta. Além disso, o modelo possibilita que evoluções tecnológicas em um nível específico não impactem os demais, estabelecendo uma linguagem técnica padronizada para os profissionais da área.

🌐 O Modelo TCP/IP   
Desenvolvido no início da década de 1970, o modelo de Internet, conhecido como TCP/IP, é classificado como um modelo de protocolo. Isso ocorre porque sua estrutura corresponde fielmente às funções executadas pela suíte de protocolos que sustenta a internet global.

O modelo TCP/IP é organizado em quatro categorias funcionais:
- Aplicação: Gerencia a representação dos dados para o usuário, incluindo a codificação e o controle de diálogo.
- Transporte: Viabiliza a comunicação entre diversos dispositivos localizados em redes distintas.
- Internet: Responsável por determinar a melhor rota para o tráfego das informações.
- Acesso à Rede: Controla os componentes de hardware e os meios físicos que constituem a infraestrutura de rede.

🏗️ O Modelo de Referência OSI   
Diferente de um modelo de protocolo, um modelo de referência serve para descrever as funções necessárias em cada estágio da comunicação sem especificar a implementação técnica. O modelo OSI é composto por sete camadas distintas:
- 7-Aplicação: Contém protocolos destinados à comunicação entre processos.
- 6-Apresentação: Provê uma representação comum para os dados transferidos.
- 5-Sessão: Organiza o diálogo e gerencia a troca de informações entre serviços.
- 4-Transporte: Define serviços para segmentar, transferir e reagrupar dados entre dispositivos finais.
- 3-Rede: Garante a troca de informações entre dispositivos identificados em diferentes redes.
- 2-Enlace de Dados: Estabelece métodos para a troca de quadros em um meio físico compartilhado.
- 1-Física: Descreve os requisitos elétricos e mecânicos para a transmissão de bits pelo meio físico.

🔄 Comparativo e Mapeamento entre Modelos   
Embora o TCP/IP seja a suíte utilizada na prática, o modelo OSI é fundamental para compreender funções gerais de rede. O modelo TCP/IP não detalha os procedimentos de acesso à mídia ou as especificações físicas de transmissão, funções estas que são minuciosamente descritas nas camadas 1 e 2 do modelo OSI.

Nota-se que existe uma correspondência direta entre as camadas de Transporte de ambos os modelos. Da mesma forma, a camada de Internet do TCP/IP equivale à camada de Rede do modelo OSI. Contudo, as funções que o modelo TCP/IP agrupa na camada de Aplicação são desmembradas nas camadas 5, 6 e 7 do OSI, permitindo uma análise mais granular para desenvolvedores e fornecedores de software. Atualmente, o modelo OSI é amplamente utilizado como referência para descrever as camadas inferiores da comunicação de dados.

<a name="item05.05"><h4>5.5 Resumo dos Princípios de comunicação</h4></a>[Back to summary](#item05)

📜 Fundamentos dos Protocolos   
Para que a comunicação digital ocorra sem erros, os dispositivos utilizam protocolos que definem regras rígidas para a troca de informações. Essas normas estabelecem desde a estrutura gramatical da mensagem até o seu tamanho máximo, garantindo que o receptor consiga interpretar exatamente o que foi enviado pelo emissor, independentemente do fabricante do hardware.

⏱️ Temporização e Codificação   
A eficiência de uma rede depende da sincronia entre os hosts, que define a velocidade de transmissão e o momento exato em que um dado pode ser enviado para evitar colisões. Antes de trafegar, a informação é convertida em bits e codificada conforme o meio físico, transformando dados digitais em pulsos elétricos, sinais luminosos ou ondas de rádio.

📦 Encapsulamento de Dados   
O processo de encapsulamento funciona como colocar uma carta dentro de vários envelopes sucessivos, onde cada camada adiciona um cabeçalho com informações essenciais de endereçamento. Isso permite que a mensagem identifique corretamente sua origem e seu destino, garantindo que os dispositivos intermediários saibam exatamente para onde encaminhar cada pacote de dados.

📢 Padrões de Mensagens   
Existem diferentes fluxos de comunicação dependendo da necessidade da aplicação: alguns protocolos exigem uma confirmação de recebimento antes de prosseguir, funcionando em um ciclo de solicitação e resposta. Outros protocolos priorizam a velocidade e transmitem os dados de forma contínua, sem interromper o fluxo para verificar se cada pequena parte chegou ao destino.

🌍 Importância da Padronização   
Os padrões de rede são conjuntos de regras universais que garantem a interoperabilidade entre equipamentos de marcas distintas em todo o mundo. O desenvolvimento desses padrões é um processo rigoroso e documentado através das RFCs (Request for Comments), gerenciadas por órgãos como o IETF, que registram toda a evolução e testes de uma nova tecnologia.

📚 Pilha de Protocolos e Camadas   
A comunicação em rede não é feita por um único protocolo, mas por um conjunto deles trabalhando de forma hierárquica, conhecido como pilha de protocolos. Essa estrutura em camadas permite que cada nível execute uma função específica e independente, onde os níveis superiores lidam com a interface do usuário e os inferiores tratam da transmissão física dos bits.

⚙️ O Modelo TCP/IP   
O modelo TCP/IP é a base da internet moderna e organiza as funções de rede em quatro camadas principais: Aplicação, Transporte, Internet e Acesso à Rede. Cada uma desempenha um papel crítico, desde a representação dos dados para o usuário até a determinação da melhor rota que a informação deve seguir para atravessar diversos nós globais.

🔍 O Modelo de Referência OSI   
Diferente do TCP/IP, o modelo OSI detalha a comunicação em sete camadas distintas para facilitar o entendimento e o suporte técnico. Ele descreve desde as características físicas dos cabos e conectores até os processos complexos de sessão e apresentação de dados, servindo como um mapa universal para profissionais de TI diagnosticarem e desenvolverem tecnologias de rede.
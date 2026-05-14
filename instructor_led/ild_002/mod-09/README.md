# CyberOps Associate - Módulo 9   <img src="../0-aux/logo_course.png" alt="ild_002" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="../">ild_002 (CyberOps Associate)   <img src="../0-aux/logo_course.png" alt="ild_002" width="auto" height="25"></a>
### Module: 9. A camada de transporte

---

### Theme:
- Cybersecurity

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

### Course Module 9 Structure:

9. <a name="item09">A camada de transporte</a><br>
  9.1 <a href="#item09.01">Introdução</a><br>
  9.2 <a href="#item09.02">Características da Camada de Transporte</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;9.2.1 <a href="#item09.02.01">Verifique sua compreensão - Compare as características TCP e UDP</a><br>
  9.3 <a href="#item09.03">Estabelecimento da Sessão da Camada de Transporte</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;9.3.1 <a href="../../../labs/lab_044/">Laboratório - Usando o Wireshark para Observar o Handshake TCP de 3 Vias</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;9.3.2 <a href="#item09.03.02">Verifique sua Compreensão - Conexão TCP e Processo de Rescisão</a><br>
  9.4 <a href="#item09.04">Confiabilidade da Camada de Transporte</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;9.4.1 <a href="../../../labs/lab_045/">Laboratório - Explorando o Nmap</a><br>
  9.5 <a href="#item09.05">O Resumo da Camada de Transporte</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item09.01"><h4>9.1 Introdução</h4></a>[Back to summary](#item09)

🔹 Mecanismos e Protocolos da Camada de Transporte   
A camada de transporte desempenha o papel fundamental de segmentar e encaminhar fluxos de dados entre dispositivos finais, garantindo que a comunicação chegue à aplicação correta. Através do uso de protocolos distintos, a rede pode priorizar a integridade absoluta da informação ou a velocidade de entrega, dependendo da necessidade do serviço. Este módulo detalha o funcionamento lógico por trás do tráfego de dados, explorando como as conexões são gerenciadas para sustentar a interatividade e a transferência de arquivos em redes digitais.

🎯 Objetivo Geral   
- Analisar como as regras da camada de transporte viabilizam e sustentam as funcionalidades de comunicação na rede.

✅ Objetivos Específicos   
- Características da Camada de Transporte: Descrever as responsabilidades e os métodos utilizados pelos protocolos para suportar o intercâmbio de dados entre hosts.
- Estabelecimento da Sessão da Camada de Transporte: Explicar os processos de abertura e manutenção de canais de comunicação para a troca ordenada de mensagens.
- Confiabilidade da Camada de Transporte: Demonstrar os mecanismos de controle de fluxo e confirmação que asseguram a entrega fidedigna das informações ao destino.

<a name="item09.02"><h4>9.2 Características da Camada de Transporte</h4></a>[Back to summary](#item09)

🏗️ Responsabilidades da Camada de Transporte   
Diferente da camada de rede, que se preocupa com o roteamento e endereçamento de pacotes, a camada de transporte gerencia como os dados são entregues. Suas funções principais incluem:
- Rastreamento de Conversas: Cada conjunto de dados entre uma origem e um destino é monitorado como uma conversa individual. Um único host pode manter múltiplas comunicações simultâneas.
- Segmentação e Remontagem: Devido às limitações de tamanho dos pacotes na rede, os dados da aplicação são divididos em blocos menores (segmentos para TCP ou datagramas para UDP). No destino, a camada de transporte reagrupa esses blocos para a aplicação correspondente.
- Identificação de Aplicações (Portas): Para garantir que os dados cheguem ao software correto, utiliza-se um identificador chamado número de porta. Cada processo de rede recebe uma porta exclusiva no host.
- Multiplexação: Técnica que permite intercalar diferentes conversas (ex: vídeo, e-mail, navegação web) no mesmo meio físico, otimizando o uso da largura de banda e facilitando a recuperação de erros.

🛡️ TCP: O Protocolo Orientado a Conexão   
O TCP (Transmission Control Protocol) é um protocolo robusto e confiável. Ele é considerado stateful, pois monitora o estado da sessão desde o estabelecimento até o encerramento. Suas operações básicas garantem a integridade da entrega através de:
- Numeração de Segmentos: Permite a remontagem na ordem correta, mesmo que os dados cheguem fora de sequência.
- Confirmação de Recebimento (ACK): O destino avisa o remetente sobre quais dados foram recebidos.
- Retransmissão: Caso um dado não seja confirmado em um período determinado, o remetente envia o segmento novamente.
- Controle de Fluxo: Ajusta a taxa de envio conforme a capacidade de processamento do receptor.

📑 Estrutura e Campos do Cabeçalho TCP   
A encapsulação TCP adiciona 20 bytes de informações de controle aos dados da aplicação. Os campos binários organizados no cabeçalho permitem a execução das funções de gerenciamento da sessão.
- Porta de Origem e Destino (16 bits cada): Identificam as aplicações envolvidas na comunicação em ambas as pontas.
- Número de Sequência (32 bits): Define a posição do segmento para garantir a ordem correta na remontagem final.
- Número de Confirmação (32 bits): Indica o recebimento dos dados e sinaliza qual é o próximo byte esperado.
- Comprimento do Cabeçalho (4 bits): Informa o tamanho do cabeçalho para que o receptor saiba onde iniciam os dados da aplicação.
- Bits de Controle (6 bits): Conjunto de sinalizadores (flags) que definem a finalidade do segmento, como sincronização (SYN), confirmação (ACK) ou finalização (FIN).
- Tamanho da Janela (16 bits): Estipula a quantidade de bytes que podem ser transmitidos antes da necessidade de uma nova confirmação.
- Checksum (16 bits): Realiza a verificação de integridade, detectando corrupções no cabeçalho ou nos dados durante o transporte.
- Urgente (16 bits): Indica se o conteúdo do segmento possui prioridade de processamento imediato.

⚡ Protocolo User Datagram (UDP)   
O UDP atua como uma alternativa de baixa sobrecarga ao TCP, priorizando a velocidade em detrimento da confiabilidade. Por não realizar o controle de fluxo ou garantir a entrega dos dados, o processamento dos datagramas ocorre de forma significativamente mais rápida. É o equivalente digital a enviar uma carta comum: o remetente a deposita no correio sem a garantia de que o destinatário a recebeu ou de que ela chegará íntegra.

🏎️ Características Operacionais   
Diferente do seu equivalente "burocrático" (TCP), o UDP opera sob princípios de extrema simplicidade:
- Sem Conexão (Connectionless): Não existe uma etapa inicial de estabelecimento de sessão. Os dados são enviados imediatamente para o destino.
- Sem Estado (Stateless): Nem o cliente nem o servidor monitoram o progresso da comunicação. Cada datagrama é tratado como uma unidade isolada.
- Melhor Esforço (Best Effort): Não há confirmações de recebimento (ACKs). Se um pacote for corrompido ou perdido no caminho, o protocolo não solicita a retransmissão.
- Tolerância a Perdas: Aplicações que exigem fluidez em tempo real, como VoIP (voz sobre IP) e streaming de vídeo ao vivo, utilizam o UDP por suportarem pequenas perdas de dados sem comprometer a experiência final.

📑 Estrutura do Cabeçalho UDP   
A simplicidade do UDP reflete-se em seu cabeçalho, que possui apenas 8 bytes (64 bits) de sobrecarga, distribuídos em quatro campos fixos:
- Porta de Origem (16 bits): Identifica a aplicação remetente no host de origem.
- Porta de Destino (16 bits): Identifica o serviço ou aplicação alvo no host de destino.
- Tamanho (16 bits): Indica o comprimento total do datagrama (cabeçalho + dados).
- Checksum (16 bits): Realiza uma verificação básica de integridade para detectar erros no cabeçalho ou na carga útil.

🔌 O Conceito de Sockets e Pares de Sockets   
Para que a camada de transporte direcione o tráfego corretamente, utiliza-se a estrutura de sockets. Um socket é a combinação única de um Endereço IP e um Número de Porta.
- Identificação Unívoca: Sockets permitem que um único host execute múltiplos serviços simultaneamente (como Web na porta 80 e FTP na porta 21) sem que os fluxos de dados se misturem.
- Par de Sockets: A comunicação completa entre dois dispositivos é definida pelo conjunto dos sockets de origem e destino. Por exemplo, uma conexão de um PC (192.168.1.5:1099) para um Servidor Web (192.168.1.7:80) forma o par que rastreia aquela conversa específica.
- Função do Número de Porta: Atua como um endereço de retorno. A camada de transporte monitora qual aplicação iniciou a requisição para que, no momento da resposta, os dados sejam entregues ao processo de software correto.

<a name="item09.02.01"><h4>9.2.1 Verifique sua compreensão - Compare as características TCP e UDP</h4></a>[Back to summary](#item09)

Selecione o método de entrega correspondente para cada característica:
- Menos Sobrecarga: UDP
- Requisitos de Transmissão Rápida: UDP
- Sem confirmação de recebimento: UDP
- Garantia de Entrega: TCP
- Entrega Ordenada: TCP
- Sem Conexão: UDP
- Segmentos de Mensagem Sequenciados: TCP
- Entrega Não Ordenada: UDP
- Controle de fluxo: TCP
- Estabelecimento de Sessão: TCP

<a name="item09.03"><h4>9.3 Estabelecimento da Sessão da Camada de Transporte</h4></a>[Back to summary](#item09)

🔌 Gerenciamento de Sessões e Portas no TCP   
O funcionamento do protocolo TCP baseia-se na utilização de números de porta para distinguir múltiplos processos de comunicação. Cada serviço em um servidor é vinculado a uma porta exclusiva, que deve estar no estado "aberto" para processar requisições. Dois serviços distintos não podem ocupar a mesma porta simultaneamente no mesmo protocolo de transporte.

🔄 Dinâmica de Portas entre Cliente e Servidor   
A comunicação estabelece um fluxo onde as portas de origem e destino se alternam conforme a direção do tráfego:
- Requisição do Cliente: O dispositivo de origem gera uma porta de origem dinâmica (geralmente de número alto) e endereça o pacote a uma porta de destino conhecida no servidor (como a porta 80 para HTTP ou 25 para SMTP).
- Resposta do Servidor: Ao retornar os dados, o servidor inverte os papéis. A porta que era o destino na requisição torna-se a origem na resposta, e a porta dinâmica do cliente torna-se o novo destino. Esse mecanismo permite que o host cliente direcione a resposta para a aplicação correta que iniciou a conversa.

🤝 Estabelecimento de Conexão: Handshake de Três Vias   
Para garantir a confiabilidade, o TCP realiza um processo de sincronização inicial antes de transmitir dados reais. Esse procedimento valida a presença do destino e a disponibilidade do serviço solicitado.
- SYN (Sincronizar): O cliente envia um segmento com o sinalizador SYN ativado para solicitar a abertura de uma sessão.
- SYN-ACK (Sincronizar e Confirmar): O servidor responde confirmando o recebimento da solicitação (ACK) e enviando sua própria solicitação de sincronização (SYN).
- ACK (Confirmar): O cliente envia uma confirmação final, estabelecendo a conexão bilateral.

🏁 Finalização de Sessão: Handshake de Quatro Etapas   
O encerramento de uma conexão TCP é um processo controlado, pois o protocolo é full-duplex (permite comunicação simultânea em ambas as direções). Cada via de comunicação deve ser encerrada individualmente.
- Etapa 1 (FIN): O host que deseja encerrar o envio de dados envia um segmento com o flag FIN.
- Etapa 2 (ACK): O receptor confirma o recebimento do pedido de encerramento.
- Etapa 3 (FIN): O receptor também envia seu sinalizador FIN para encerrar a via oposta.
- Etapa 4 (ACK): O host inicial confirma o encerramento final, e a sessão é oficialmente fechada.

🚩 Bits de Controle (Flags) do Cabeçalho TCP   
A gestão do status da conexão é realizada por seis sinalizadores (flags) binários presentes no cabeçalho do segmento. Cada bit indica uma função específica para o processamento dos dados:
- SYN: Sincroniza números de sequência para o início de conexões.
- ACK: Confirma o recebimento de segmentos e é obrigatório após o primeiro pacote.
- FIN: Sinaliza que o remetente concluiu o envio de dados e deseja encerrar a sessão.
- RST: Força a redefinição de uma conexão em caso de erros fatais ou tempos de espera excedidos.
- PSH (Push): Solicita que os dados sejam enviados imediatamente para a aplicação, sem aguardar o preenchimento total do buffer.
- URG: Indica que os dados contidos no segmento possuem prioridade de processamento.

<a name="item09.03.02"><h4>9.3.2 Verifique sua Compreensão - Conexão TCP e Processo de Rescisão</h4></a>[Back to summary](#item09)

Usando os menus suspensos, selecione a opção apropriada para ilustrar o handshake de 3 vias de uma sessão de estabelecimento TCP.
- Enviar SYN SYN recebido.
- Recebido: SYN.
- Envia: SYN, ACK.
- Recebido SYN, ACK.
- Envia: ACK.
- Recebido: ACK.

<a name="item09.04"><h4>9.4 Confiabilidade da Camada de Transporte</h4></a>[Back to summary](#item09)

🧩 Ordenação e Remontagem: O Papel dos Números de Sequência   
Na rede, os dados raramente chegam na mesma ordem em que foram enviados. Para resolver esse quebra-cabeça, o TCP utiliza Números de Sequência.
- Identificação por Byte: Cada byte de dados recebe um número. O número de sequência no cabeçalho representa o primeiro byte daquele segmento específico.
- ISN (Número de Sequência Inicial): A conversa não começa do zero ou do um. O ISN é um número aleatório gerado no início da sessão para evitar ataques de previsão de pacotes.
- Reordenação no Destino: O receptor armazena os segmentos em um buffer. Se o segmento 3 chegar antes do 2, ele fica guardado até que o "buraco" seja preenchido, garantindo que a aplicação receba a mensagem original perfeita.

🔄 Confiabilidade: Recuperação de Perdas e SACK   
Quando um pacote se perde, o TCP entra em ação para recuperá-lo usando os campos SEQ (Sequência) e ACK (Confirmação).
- Reconhecimento Positivo: O receptor envia um ACK indicando qual é o próximo byte que ele espera receber.
- Reconhecimento Seletivo (SACK): Antigamente, se fosse perdido o pacote 3 de uma sequência de 10, o remetente tinha que reenviar do 3 ao 10. Com o SACK, o receptor avisa: "Recebi o 1, 2 e do 5 ao 10; só me mande o 3 e o 4". Isso economiza muita banda e tempo.

🌊 Controle de Fluxo: Janelas Deslizantes   
O Tamanho da Janela é o que impede que um servidor rápido "atropele" um cliente lento. É um campo de 16 bits no cabeçalho que diz quantos bytes podem ser enviados antes que o remetente precise parar e esperar por um ACK.
- Janela Deslizante: À medida que o receptor processa os dados e envia ACKs, a "janela" de envio avança (desliza), permitindo o envio de novos dados.
- Ajuste Dinâmico: Se o dispositivo de destino ficar sobrecarregado, ele pode diminuir o tamanho da janela no próximo segmento enviado para avisar o remetente: "Ei, vá mais devagar, meu buffer está enchendo!".

📏 Tamanho Máximo do Segmento (MSS)   
O MSS define o maior bloco de dados que um dispositivo pode receber em um único segmento, sem contar os cabeçalhos. Ele é calculado com base na MTU (Unidade Máxima de Transmissão) da rede física. Em uma rede Ethernet padrão, o cálculo para IPv4 costuma ser:

```
MSS = MTU - (Cabeçalho IP + Cabeçalho TCP).
MSS = 1500 bytes - (20 bytes + 20 bytes) = 1460 bytes
```

🚦 Prevenção de Congestionamento   
O TCP também atua como um guarda de trânsito para a rede global. Quando ele percebe que muitos pacotes estão se perdendo (falta de ACKs), ele assume que há um congestionamento nos roteadores do caminho. Independentemente do que o destinatário diz sobre a janela dele, o remetente reduz proativamente a quantidade de dados que envia para ajudar a rede a se recuperar. Sem esse mecanismo, as retransmissões infinitas de pacotes perdidos criariam um efeito de bola de neve que poderia travar links inteiros da internet.

<a name="item09.05"><h4>9.5 O Resumo da Camada de Transporte</h4></a>[Back to summary](#item09)

🔗 Elo de Comunicação   
A camada de transporte atua como uma ponte entre os programas que o usuário utiliza e a infraestrutura física da rede. Sua função principal é garantir que as mensagens cheguem ao aplicativo correto no dispositivo de destino, sendo responsável por dividir as informações em partes menores, rastrear cada conversa individual e reunir tudo na ordem certa após a entrega.

⚖️ TCP vs UDP   
Existem dois caminhos principais para o transporte de dados: o TCP, que prioriza a segurança e a ordem, sendo ideal para e-mails e navegação web por confirmar o recebimento de cada pacote; e o UDP, focado em velocidade e baixa latência. O UDP é utilizado em serviços de voz e vídeo em tempo real, pois não perde tempo reenviando dados que ficaram para trás, processando as informações conforme elas chegam.

🔌 Portas e Soquetes   
Para gerenciar diversas conversas ao mesmo tempo, o sistema utiliza números de porta que variam de 0 a 65535, identificando o serviço solicitado e o aplicativo que deve responder. A união entre o endereço IP e o número da porta cria o que chamamos de soquete, uma combinação única que permite ao servidor saber exatamente para onde enviar os dados de volta.

🤝 O Aperto de Mão (Handshake)   
Antes de iniciar uma troca segura via TCP, os dispositivos realizam uma negociação em três etapas para confirmar se o destinatário está disponível e pronto para receber dados naquela porta específica. Durante esse processo e ao longo da conversa, são utilizados sinalizadores técnicos (flags) para controlar o início, a confirmação e o encerramento das sessões de comunicação.

🧩 Organização e Reenvio   
Para que a mensagem faça sentido, os segmentos recebidos são organizados através de números de sequência gravados em seus cabeçalhos. Caso ocorra perda de dados, o sistema utiliza mecanismos de confirmação para identificar o que falta; tecnologias modernas permitem até que o receptor avise exatamente quais partes chegaram, evitando que o emissor precise repetir o envio de informações que já foram entregues com sucesso.

🌊 Controle de Fluxo e Janelas   
O sistema ajusta automaticamente a velocidade do envio de dados para não sobrecarregar quem está recebendo, utilizando um campo chamado "tamanho da janela". Através das chamadas janelas deslizantes, a origem monitora as confirmações do destino e regula o volume de informações transmitidas, prevenindo congestionamentos na rede e garantindo que o fluxo de dados seja constante e eficiente.
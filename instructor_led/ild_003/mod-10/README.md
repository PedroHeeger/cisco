# Fundamentos de Redes - Módulo 10   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../instructor_led/">instructor-led</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">ild_003 (Fundamentos de Redes)   <img src="../0-aux/logo_course.png" alt="ild_003" width="auto" height="25"></a>
### Module: 10. Formatos e regras de endereçamento IPv6

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
10. <a name="item10">Formatos e regras de endereçamento IPv6</a><br>
  10.1 <a href="#item10.01">Introdução</a><br>
  10.2 <a href="#item10.02">Problemas do IPv4</a><br>
  10.3 <a href="#item10.03">Endereçamento IPv6</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;10.3.1 <a href="#item10.03.01">Atividade - Representações do Endereço IPv6</a><br>
  10.4 <a href="#item10.04">Resumo de Formatos e regras de endereçamento IPv6</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item10.01"><h4>10.1 Introdução</h4></a>[Back to summary](#item10)

🌐 Fundamentos e Estrutura do Endereçamento IPv6   
A evolução das redes de dados e o crescimento exponencial do número de dispositivos conectados globalmente tornaram escasso o sistema de endereçamento IPv4. Para solucionar as limitações de escalabilidade e garantir a continuidade da conectividade mundial, o protocolo IPv6 foi desenvolvido. Este novo padrão não apenas expande massivamente o espaço de endereçamento disponível, mas também introduz melhorias na eficiência do processamento de pacotes e na autoconfiguração de dispositivos.

🎯 Objetivo do módulo:   
- Explicar as características, a necessidade de transição e os métodos de representação do endereçamento IPv6.

📘 Tópicos do módulo:   
- Problemas de IPv4: Análise técnica sobre o esgotamento dos endereços de 32 bits e os desafios gerados pela crescente demanda por identificadores exclusivos.
- Endereçamento IPv6: Estudo da estrutura de 128 bits, regras de notação hexadecimal e técnicas de compressão para a representação simplificada de endereços.

<a name="item10.02"><h4>10.2 Problemas do IPv4</h4></a>[Back to summary](#item10)

🚀 A Transição para o IPv6: Além do Esgotamento do IPv4   
O esgotamento dos endereços IPv4 não é mais uma previsão para o futuro, mas uma realidade consolidada. Com um limite teórico de 4,3 bilhões de combinações, o antigo protocolo tornou-se insuficiente para a escala da internet moderna. Embora técnicas como o NAT (Tradução de Endereços de Rede) tenham adiado esse fim, elas trouxeram efeitos colaterais como latência e dificuldades em comunicações ponto a ponto.

🌐 A Magnitude do IPv6   
Projetado pela IETF para ser o sucessor definitivo, o IPv6 expande o espaço de endereçamento para 128 bits. Isso resulta em aproximadamente 340 undecilhões de endereços, uma quantidade virtualmente infinita que permite conectar desde grandes servidores até os menores sensores da Internet das Coisas (IoT).

Além do tamanho, o IPv6 trouxe melhorias estruturais:
- ICMPv6: Evolução do protocolo de controle que agora integra funções nativas de resolução e configuração automática de endereços (SLAAC).
- Eficiência: Eliminação da necessidade de NAT em comunicações nativas, restaurando o modelo de conectividade direta entre as pontas.

📈 O Cenário Global de Adoção   
Atualmente, quase todos os grandes Registros Regionais de Internet (RIRs) — como LACNIC e RIPE — já esgotaram suas reservas de IPv4. Esse movimento forçou grandes provedores de conteúdo (como Netflix e Google) e operadoras de telefonia móvel a liderarem a migração, com muitas redes operando majoritariamente em IPv6.

🛠️ Estratégias de Coexistência e Migração   
Como o desligamento do IPv4 não ocorrerá da noite para o dia, foram criadas técnicas para que ambos os protocolos operem simultaneamente durante a transição:
- Pilha Dupla (Dual Stack): É a implementação ideal, onde os dispositivos executam as duas pilhas de protocolos ao mesmo tempo no mesmo segmento de rede.
- Tunelamento: Utilizado para transportar pacotes IPv6 encapsulados dentro de pacotes IPv4, permitindo que ilhas IPv6 se comuniquem através de uma infraestrutura que ainda só entende o protocolo antigo.
- Tradução (NAT64): Permite a comunicação direta entre dispositivos que falam apenas IPv6 e dispositivos que falam apenas IPv4, realizando a conversão dos pacotes em tempo real.

O objetivo final de qualquer infraestrutura moderna deve ser a conectividade IPv6 nativa de ponta a ponta, simplificando a gerência e garantindo a escalabilidade necessária para o futuro tecnológico.

<a name="item10.03"><h4>10.3 Endereçamento IPv6</h4></a>[Back to summary](#item10)

🔢 Estrutura e Representação do Endereço IPv6   
Para compreender o IPv6, o primeiro passo é abandonar o sistema decimal e adotar o hexadecimal (base 16). Esse sistema utiliza os números de 0 a 9 e as letras de A a F para representar valores. No contexto das redes, essa escolha é fundamental para organizar os extensos endereços de 128 bits de forma mais legível.

🏛️ A Anatomia do Endereço: Hextetos   
Diferente do IPv4, que trabalha com octetos, o IPv6 é dividido em oito segmentos de 16 bits cada, conhecidos tecnicamente como hextetos.

Cada hexteto é composto por 4 dígitos hexadecimais.
- O formato completo (chamado de Formato Preferencial) é escrito como x:x:x:x:x:x:x:x.
- O endereço totaliza 32 dígitos hexadecimais.
- Curiosidade: O IPv6 não diferencia maiúsculas de minúsculas; ABCD é o mesmo que abcd.

✂️ Regras de Compressão (Simplificando a Escrita)   
Como escrever 32 dígitos pode ser exaustivo e propenso a erros, existem duas regras essenciais para compactar o endereço sem perder informações:
- Omissão de Zeros à Esquerda: Você pode remover os zeros que aparecem no início de qualquer hexteto.
  - Exemplo: 01AB torna-se 1AB.
  - Exemplo: 0005 torna-se apenas 5.
  - Atenção: Isso só vale para zeros à esquerda. Zeros à direita devem ser mantidos, caso contrário, o valor do segmento mudaria (ex: A000 não pode virar A).
- A Regra dos Dois Pontos Duplos (::): Qualquer sequência contínua de um ou mais hextetos compostos apenas por zeros pode ser substituída por dois pontos duplos (::).
  - Exemplo: 2001:db8:0:0:0:0:0:1 vira 2001:db8::1.
  - Regra de Ouro: Você só pode usar o :: uma única vez em cada endereço. Se usasse duas vezes, o computador não saberia quantos zeros foram omitidos em cada parte, tornando o endereço ambíguo.

💡 Prática Recomendada   
Se o seu endereço tiver mais de um grupo de zeros em locais diferentes, a melhor estratégia é usar o :: no maior grupo. Se os grupos tiverem o mesmo tamanho, utilize os dois pontos duplos na primeira ocorrência para manter o padrão de legibilidade. Ao aplicar essas duas regras juntas, um endereço longo e complexo é transformado no chamado Formato Compactado, muito mais fácil de gerenciar no dia a dia de um administrador de redes.

<a name="item10.03.01"><h4>10.3.1 Atividade - Representações do Endereço IPv6</h4></a>[Back to summary](#item10)

- Instruções: Converta os endereços IPv6 em formatos curtos e compactos (omita os zeros à esquerda). Insira letras em minúsculas. Clique em Avançar para seguir na atividade para o próximo endereço.
  - Formato Preferencial: 2001 : 0db8 : 2233 : 4455 : 6677 : 0000 : 0000 : 0101
  - Omitir zeros à esquerda: 2001 : db8 : 2233 : 4455 : 6677 : 0 : 0 : 101
  - Formato compactado: 2001 : db8 : 2233 : 4455 : 6677 :: 101

<a name="item10.04"><h4>10.4 Resumo de Formatos e regras de endereçamento IPv6</h4></a>[Back to summary](#item10)

🚀 Transição para o IPv6   
O esgotamento global dos endereços IPv4 impulsionou a criação do IPv6, que utiliza uma estrutura de 128 bits para oferecer uma quantidade virtualmente infinita de identificadores. Além da expansão do espaço de endereçamento, o novo protocolo introduziu melhorias significativas, como o ICMPv6, que automatiza funções de configuração e descoberta que antes exigiam processos manuais ou serviços externos no padrão antigo.

🛠️ Estratégias de Coexistência   
Como a substituição total do IPv4 não acontece instantaneamente, existem técnicas que permitem que ambos os protocolos operem juntos. A abordagem de pilha dupla permite que o hardware processe os dois tipos de pacotes simultaneamente, enquanto o tunelamento "esconde" dados IPv6 dentro de pacotes IPv4 para atravessar redes antigas. Já a tradução, como o NAT64, converte os protocolos entre si para permitir a comunicação entre dispositivos de gerações diferentes.

🔢 Estrutura e Escrita Hexadecimal   
Diferente da notação decimal do IPv4, o IPv6 utiliza o sistema hexadecimal, composto por 32 dígitos divididos em oito grupos de 16 bits chamados hextetos. Essa representação não diferencia letras maiúsculas de minúsculas e, em seu formato completo, exibe todos os caracteres. No entanto, para facilitar a leitura e reduzir o tamanho das anotações, existem regras específicas de simplificação.

⬅️ Omissão de Zeros à Esquerda   
A primeira regra de simplificação permite descartar qualquer zero que apareça no início de um hexteto. Por exemplo, um segmento grafado como 00AB pode ser reduzido apenas para AB, enquanto um bloco como 09F0 torna-se 9F0. É fundamental ressaltar que essa regra só se aplica aos zeros iniciais; os zeros que aparecem ao final de um segmento devem ser mantidos para não alterar o valor matemático do endereço.

↔️ Regra dos Dois-Pontos Duplos   
Para endereços que possuem longas sequências de zeros, utiliza-se a abreviação por dois-pontos duplos (::) para substituir um ou mais grupos nulos contíguos. Essa técnica só pode ser empregada uma única vez em cada endereço para evitar ambiguidades na reconstrução dos dados. Se houver múltiplas sequências de zeros, a recomendação técnica é aplicar a abreviação no trecho mais longo para obter a maior simplificação possível.
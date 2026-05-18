# CyberOps Associate - Módulo 14   <img src="../0-aux/logo_course.png" alt="ild_002" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../..//instructor_led/">instructor-led</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="../">ild_002 (CyberOps Associate)   <img src="../0-aux/logo_course.png" alt="ild_002" width="auto" height="25"></a>
### Module: 14. Ameaças e ataques comuns

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

### Course Module 14 Structure:

14. <a name="item14">Ameaças e ataques comuns</a><br>
  14.1 <a href="#item14.01">Introdução</a><br>
  14.2 <a href="#item14.02">Malware</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;14.2.1 <a href="../../../labs/lab_???/">Laboratório - Anatomia do Malware</a><br>
  14.3 <a href="#item14.03">Ataques de rede comuns - reconhecimento, acesso e engenharia social</a><br>
  14.4 <a href="#item14.04">Ataques de rede - negação de serviço, estouros de buffer e evasão</a><br>
  14.5 <a href="#item14.05">Uso de IA para Analisar Malware</a><br>
  14.6 <a href="#item14.06">Resumo de ameaças e ataques comuns</a><br>


1. <a name="item01">As redes de hoje</a><br>
  1.1 <a href="#item01.01">Introdução</a><br>
  1.2 <a href="#item01.02">Redes afetam nossas vidas</a><br>
  1.3 <a href="#item01.03">Componentes de rede</a><br>
  1.4 <a href="#item01.04">Representações e topologias de rede</a><br>
  1.5 <a href="#item01.05">Tipos comuns de redes</a><br>
  1.6 <a href="#item01.06">Conexões com a Internet</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;1.6.1 <a href="../../../pkt/pkt_001/">Packet Tracer - Representação da Rede</a><br>
  1.7 <a href="#item01.07">Redes confiáveis</a><br>
  1.8 <a href="#item01.08">Tendênciais das redes</a><br>
  1.9 <a href="#item01.09">Segurança de Redes</a><br>
  1.10 <a href="#item01.10">O profissional de TI</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;1.10.1 <a href="../../../labs/lab_001/">Laboratório - Pesquise oportunidades de trabalho em TI e redes</a><br>
  1.11 <a href="#item01.11">Módulo Prático e Quiz</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item14.01"><h4>14.1 Introdução</h4></a>[Back to summary](#item14)

🔹 Vetores de Malwares e Metodologias de Incursão   
A compreensão das motivações por trás das ofensivas digitais precede o estudo técnico das ameaças em si. Este módulo detalha as categorias de códigos maliciosos e as táticas de exploração que desafiam a integridade das infraestruturas modernas. Ao explorar desde técnicas de manipulação humana até falhas lógicas em sistemas e sobrecarga de serviços, o conteúdo capacita a identificação de comportamentos suspeitos e a antecipação de manobras adversárias no ambiente de rede.

🎯 Objetivo Geral:   
- Analisar as diversas categorias de softwares nocivos e as técnicas de exploração utilizadas em ataques cibernéticos.

✅ Objetivos Específicos:   
- Malware: Classificar as diferentes variedades de softwares mal-intencionados e seus respectivos modos de propagação e execução.
- Ataques de rede comuns - reconhecimento, acesso e engenharia social: Descrever os métodos de coleta de informações, técnicas de invasão e a exploração do fator humano para obter vantagens ilícitas.
- Ataques de rede - negação de serviço, estouros de buffer e evasão: Demonstrar o funcionamento de táticas voltadas à interrupção de sistemas, manipulação de memória e técnicas de ocultação para contornar dispositivos de segurança.

<a name="item14.02"><h4>14.2 Malware</h4></a>[Back to summary](#item14)

🛡️ Ameaças aos Dispositivos Finais: Malware   
Dispositivos como computadores e smartphones são os alvos preferenciais de softwares maliciosos, conhecidos genericamente como Malware. Esse termo engloba qualquer código criado para roubar dados, danificar sistemas ou interromper operações ilegitimamente. A evolução constante dessas ameaças torna a defesa um desafio, pois novos códigos surgem mais rápido do que a capacidade de atualização das ferramentas de proteção.

🦠 Vírus: O Invasor Dependente   
Um vírus é um código que se anexa a outros programas legítimos. Ele não opera sozinho; sua propagação depende da execução do arquivo hospedeiro e, quase sempre, de uma ação humana.
- Propagação: Ocorre via compartilhamento de arquivos em pendrives, e-mails ou redes. Ao executar um programa infectado, o vírus busca outros executáveis para contaminar.
- Comportamento: Pode permanecer latente por meses, ativando-se apenas em datas específicas.
- Impacto: Varia de ações inofensivas (exibir imagens) até a exclusão total de dados do disco rígido.

🐎 Cavalo de Tróia (Trojan)   
Inspirado no mito grego, o Trojan apresenta-se como um software útil ou atraente (como um jogo ou utilitário), mas esconde intenções maliciosas. Ao contrário do vírus, ele não infecta outros arquivos. O usuário é enganado para baixar e executar o programa. Enquanto a função legítima (o jogo) funciona, o código malicioso se instala em segundo plano.

Funcionalidades Comuns:
- Acesso Remoto: Cria backdoors para controle externo.
- Roubo de Dados: Captura senhas e informações bancárias através de keyloggers (registro de teclas).
- Proxy: Transforma o PC da vítima em uma base para lançar ataques a outros alvos.
- Destrutivo: Corrompe arquivos e desativa softwares de segurança, como antivírus e firewalls.

🪱 Worms: Os Replicadores Autônomos   
Os worms são considerados uma das ameaças mais devastadoras devido à sua capacidade de se propagar de forma independente, sem necessidade de intervenção humana ou de um programa hospedeiro.
- Autonomia: Eles exploram falhas de segurança diretamente na rede para saltar de um sistema para outro.
- Velocidade: Casos históricos como o SQL Slammer infectaram centenas de milhares de servidores em poucos minutos, dobrando de tamanho a cada poucos segundos.

Estrutura de um Worm:
- Vulnerabilidade Habilitadora: O ponto de entrada usado para se instalar (ex: falha em um serviço de rede).
- Mecanismo de Propagação: A lógica usada para localizar e infectar novos alvos automaticamente.
- Carga Útil (Payload): O código que executa a ação "ruim", como criar acessos remotos ou lançar ataques de Negação de Serviço (DoS).

Nota-se que muitos incidentes graves ocorrem por falta de atualização (patching) de sistemas, mesmo quando a solução para a vulnerabilidade já foi disponibilizada pelos fabricantes meses antes do ataque.

💰 Ransomware: O Sequestro Digital   
O ransomware atua bloqueando o acesso ao sistema ou criptografando os arquivos do usuário.
- Mecanismo: Utiliza algoritmos de criptografia avançados que tornam os dados ilegíveis. Sem a chave de descriptografia, que está em posse do criminoso, a recuperação dos arquivos é virtualmente impossível.
- Pagamento: Os criminosos exigem o resgate geralmente em Bitcoin, devido ao anonimato e à natureza descentralizada dessa moeda digital.
- Vetores de Ataque: Disseminado principalmente via e-mail (phishing), anúncios maliciosos (malvertising) e técnicas de engenharia social.

🎭 Variedades de Malware Contemporâneo   
Além do ransomware, outras formas de software malicioso operam com objetivos distintos, desde a espionagem até o controle total do hardware:
- Spyware: Coleta dados sobre o comportamento e informações do usuário sem consentimento, enviando-os para entidades externas. Inclui rastreadores de cookies e keyloggers.
- Adware: Focado em gerar receita para o autor através da exibição intrusiva de anúncios e pop-ups, muitas vezes baseados no histórico de navegação da vítima.
- Scareware: Usa táticas de choque ou ansiedade (como falsos avisos de vírus) para induzir o usuário a baixar softwares fraudulentos ou realizar ações que comprometam o sistema.
- Phishing: Técnica que utiliza comunicações fraudulentas (geralmente e-mail) para enganar o usuário e levá-lo a revelar dados confidenciais, como credenciais bancárias e números de documentos.
- Rootkits: Projetados para ocultar a presença de invasores e manter acesso privilegiado (nível de administrador) ao sistema comprometido de forma invisível para as ferramentas de segurança convencionais.

🔍 Sinais de Comprometimento (Indicadores)   
Embora o código do malware mude constantemente para evitar a detecção, a maioria das infecções produz sintomas característicos que podem ser monitorados:
- Desempenho: Lentidão extrema do sistema e do navegador, além de aumento súbito no consumo de CPU e memória RAM.
- Alterações de Sistema: Aparecimento de ícones estranhos, modificação ou exclusão não autorizada de arquivos e programas.
- Segurança: Desativação espontânea de antivírus ou alterações nas configurações do firewall.
- Conectividade: Problemas para acessar a rede, abertura de portas TCP/UDP desconhecidas ou conexões automáticas com hosts externos na Internet sem intervenção do usuário.
- Comportamento Instável: Congelamentos de tela, travamentos frequentes (crashes) e envio de e-mails para a lista de contatos sem o conhecimento do dono da conta.

É fundamental que o monitoramento de logs de rede seja constante, pois novos comportamentos maliciosos são desenvolvidos diariamente para contornar as defesas estabelecidas.

<a name="item14.02.01"><h4>14.2.1 Laboratório - Desenvolver Políticas e procedimentos de segurança cibernética</h4></a>[Back to summary](#item14)



<a name="item14.03"><h4>14.3 Ataques de rede comuns - reconhecimento, acesso e engenharia social</h4></a>[Back to summary](#item14)

  








<a name="item14.04"><h4>14.4 Ataques de rede - negação de serviço, estouros de buffer e evasão</h4></a>[Back to summary](#item14)







<a name="item14.05"><h4>14.5 Uso de IA para Analisar Malware</h4></a>[Back to summary](#item14)







<a name="item14.06"><h4>14.6 Resumo de ameaças e ataques comuns</h4></a>[Back to summary](#item14)









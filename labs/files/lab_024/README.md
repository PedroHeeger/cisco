# Atividade de Classe - Top Hacker nos Mostra Como é Feito   <img src="./0-aux/logo_course.png" alt="lab_024" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../labs/">labs</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="./">lab_024 (Atividade de Classe - Top Hacker nos Mostra Como é Feito)   <img src="./0-aux/logo_course.png" alt="lab_024" width="auto" height="25"></a>

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

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">Parte 1: Veja o vídeo TEDx “Top Hacker Mostra-nos como é feito; Pablos Holman em TEDxMidwests”</a><br>
2. <a href="#item02">Parte 2: Responda às perguntas a seguir.</a><br>

---

### Objective:
Analisar e investigar as vulnerabilidades exploradas em um dos ataques (hacks) demonstrados no vídeo.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Parte 1: Veja o vídeo TEDx “Top Hacker Mostra-nos como é feito; Pablos Holman em TEDxMidwests”</h4></a>[Back to summary](#item00)

- a. Localize o vídeo na internet e assista.
  - Título: Top hacker shows us how it's done | Pablos Holman | TEDxMidwest.
- b. Escolha um dos hacks discutidos pelo Sr. Holman no vídeo e use seu mecanismo de busca favorito para conduzir algumas pesquisas adicionais sobre o hack.
  - Sistemas de Hotéis e Conectividade:
    - Televisões de Hotel: Utilizando um transceptor de infravermelho conectado ao computador, Holman consegue enviar códigos para as TVs de hotéis para assistir filmes gratuitamente, jogar videogames ou até monitorar o que outros hóspedes estão fazendo (como transferências bancárias ou navegação na web).
    - Hackerbot: Um robô criado para circular por ambientes, identificar usuários de redes Wi-Fi e exibir as senhas desses usuários em uma tela.
    - Sniper Yagi: Uma versão em formato de "pistola" do Hackerbot, capaz de monitorar redes sem fio e capturar senhas a cerca de 1,6 km (uma milha) de distância.
    - Vigilância por Bluetooth: Holman utilizou computadores espalhados por uma conferência para registrar o tráfego Bluetooth, permitindo mapear onde as pessoas circulavam e com quem elas interagiam.
  - Comunicação e Redes Sociais:
    - Acesso a Correio de Voz: Ele demonstra como é possível invadir e acessar o menu de mensagens de voz de celulares de terceiros.
    - Worm do MySpace (Samy): Um código em Javascript que adicionava automaticamente o autor (Samy) como amigo de quem visitasse seu perfil e replicava esse comportamento nas páginas dos novos "amigos", gerando um milhão de conexões em menos de 24 horas.
    - Filtro de Spam para Encontros: O uso do código "Spam Assassin" (um filtro de spam de e-mails) treinado com perfis de mulheres para filtrar automaticamente candidatas a encontros no MySpace, baseando-se em preferências anteriores.
  - Acesso Físico e Dispositivos Pessoais:
    - Controles Remotos de Carros: A manipulação de códigos de chaves remotas para abrir qualquer veículo de um determinado fabricante.
    - Chaves de Impacto (Bump Keys): O uso de uma chave cortada de forma específica e um martelo para abrir fechaduras comuns de portas (como as da marca Schlage) em segundos.
    - Pendrives Espiões: Dispositivos USB que, ao serem conectados para uma tarefa simples (como imprimir um documento), fazem secretamente o backup de pastas pessoais, histórico do navegador, cookies e bancos de dados de senhas.
    - Cartões de Crédito RFID: O uso de um leitor para extrair sem fio o nome do titular, número do cartão e data de validade de cartões de crédito equipados com chips de proximidade "seguros".
  - Protocolos de Internet e Ciência:
    - Exploração de SSL: Holman descreve como hackers atacam protocolos de criptografia (como o SSL), enviando dados inesperados ou alterando o tempo de resposta para encontrar brechas no sistema.
    - Laser Anti-Mosquitos: Aplicando a mentalidade de "descobrir o que é possível fazer", ele e sua equipe criaram um sistema usando peças de eletrônicos de consumo (webcams, gravadores de Blu-ray e impressoras a laser) para identificar e abater em pleno voo mosquitos que transmitem malária.
- c. Para o hack escolhido na Etapa 1b, responda às perguntas abaixo. Esteja preparado para compartilhar seu trabalho em uma discussão em classe. 
  - Vigilância por Bluetooth.

<a name="item02"><h4>2. Parte 2: Responda às perguntas a seguir.</h4></a>[Back to summary](#item00)

- a. Qual é a vulnerabilidade que está sendo explorada?
  - A vulnerabilidade explorada é a emissão passiva de sinais Bluetooth por dispositivos móveis, como celulares e laptops. Esses aparelhos transmitem tráfego de dados sem fio que pode ser detectado e registrado (logado) por qualquer computador posicionado estrategicamente em um ambiente, sem a necessidade de uma conexão direta ou autorização do usuário. Holman chama isso de "vigilância passiva", pois o hacker apenas "escuta" o que os aparelhos já estão transmitindo naturalmente enquanto as pessoas se deslocam.
- b. Quais informações, dados ou controle podem ser obtidos por um hacker que explora esta vulnerabilidade?
  - Ao explorar essa vulnerabilidade, um hacker não assume o controle do aparelho, mas consegue extrair dados comportamentais valiosos através da correlação de logs:
    - Mapeamento de Movimentação: É possível criar um mapa detalhado de onde cada pessoa esteve e por quais salas ela passou.
    - Identificação de Relacionamentos: O sistema permite correlacionar os dados para mostrar com quem uma pessoa anda ou interage, baseando-se na proximidade dos sinais de Bluetooth ao longo do tempo.
    - Padrões de Comportamento: É possível identificar rotinas, como o momento exato em que alguém fica entediado e decide ir para o saguão (lobby) do hotel, por exemplo.
    - Rastreamento Individualizado: Holman demonstrou que pôde seguir os passos de indivíduos específicos (como o Arquiteto de Privacidade da Microsoft) sem que eles tivessem qualquer conhecimento disso.
- c. Como o hack é executado?
  - O hack de Vigilância por Bluetooth é executado através da coleta passiva de sinais em pontos estratégicos para rastrear o movimento de dispositivos em um ambiente físico. A execução segue este processo:
    - Instalação de Sensores: São posicionados computadores em diversos locais de um ambiente (como em cada sala de uma conferência em um hotel).
    - Captura de Tráfego: Esses computadores funcionam como receptores que registram (logam) todo o tráfego de Bluetooth emitido pelos celulares e laptops das pessoas que circulam pelo local.
    - Correlação de Dados: As informações coletadas por todos os computadores são reunidas e cruzadas.
    - Mapeamento e Análise: Através dessa correlação, é possível gerar um mapa que mostra por onde cada pessoa passou, em quais horários e com quem ela interagiu com base na proximidade dos sinais.
- d. Que tal esse hack em particular interessou você especificamente?
  - Vigilância Passiva: Diferente de outros hacks que exigem "invadir" um sistema, este é um exemplo de vigilância passiva. O hacker não precisa enviar nenhum comando ao seu celular; ele apenas "escuta" o que o aparelho já está transmitindo voluntariamente para o ar.
- e. Como você acha que esse hack específico poderia ser atenuado?
  - A mitigação desse hack específico de Vigilância por Bluetooth envolve reduzir a "exposição" de sinais que nossos aparelhos emitem. Embora o Sr. Holman foque na demonstração da vulnerabilidade, as seguintes estratégias de atenuação podem ser extraídas da lógica do ataque:
    - Desativar o Bluetooth quando não estiver em uso: O hack funciona porque os computadores do hacker registram (logam) o tráfego de Bluetooth de quem entra e sai dos ambientes. Se o rádio Bluetooth estiver desligado, o dispositivo não emite o sinal necessário para ser rastreado ou correlacionado em um mapa.
    - Conscientização sobre Dispositivos Móveis como PCs: Holman enfatiza que celulares e laptops são, essencialmente, computadores (PCs) e, por isso, herdam todos os problemas e riscos de segurança desses sistemas. A atenuação começa ao entender que qualquer dispositivo "inteligente" está constantemente transmitindo dados que podem ser capturados passivamente.
    - Uso de Barreiras Físicas (Bloqueio de Sinal): Assim como Holman sugere o uso de carteiras de aço inoxidável para proteger cartões de crédito contra a leitura indesejada de chips RFID, uma lógica semelhante de blindagem física poderia, em teoria, ser aplicada para impedir que sinais de rádio (como Bluetooth ou Wi-Fi) escapem de um dispositivo quando a privacidade total for necessária.

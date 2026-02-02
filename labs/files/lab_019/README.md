# Laboratório - Tipos de Dados   <img src="./0-aux/logo_course.png" alt="lab_019" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../labs/">labs</a>
### Software/Subject: iot   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/iot.jpg" alt="iot" width="auto" height="25"></a>
### Course: <a href="./">lab_019 (Laboratório - Tipos de Dados)   <img src="./0-aux/logo_course.png" alt="lab_019" width="auto" height="25"></a>

---

### Theme:
- Internet of Things (IoT)

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

1. <a href="#item01">Laboratório - Tipos de Dados</a><br>

---

### Objective:
O objetivo deste laboratório foi identificar cenários e objetos para a implementação de sensores, analisando a natureza dos dados coletados para classificá-los como confidenciais (sensíveis ou PII) ou não confidenciais, além de avaliar suas aplicações práticas e os respectivos impactos na privacidade.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Laboratório - Tipos de Dados</h4></a>[Back to summary](#item00)

- a. Selecione 3 ou 4 objetos ou locais que possam conter sensores. Liste os tipos de dados que poderiam ser coletados pelo sensores. Determine se algum dos dados coletados é confidencial. Registre sua descoberta na tabela abaixo.
  - Smartphone:
    - Sensores: GPS, acelerômetro, giroscópio, microfone, câmera, sensor de proximidade.
    - Dados coletados: localização, movimento, imagens, áudio, hábitos de uso.
    - Dados confidenciais: Sim (localização, fotos, áudios e padrões de uso).
    - Como os dados podem ser usados: Os dados de GPS, movimento, áudio e imagem podem ser usados para navegação, personalização de aplicativos e melhoria de serviços. No entanto, o histórico de localização e hábitos de uso pode revelar locais visitados com frequência, rotinas diárias e horários, permitindo que agentes mal-intencionados determinem a localização do usuário ou prevejam seus deslocamentos.
  - Câmera de segurança:
    - Sensores: sensor de imagem, sensor de movimento, sensor infravermelho.
    - Dados coletados: vídeos, imagens, horários de movimentação.
    - Dados confidenciais: Sim (imagens de pessoas e rotinas).
    - Como os dados podem ser usados: As imagens e vídeos coletados podem ser usados para monitoramento, prevenção de crimes e identificação de incidentes. Porém, se acessados indevidamente, esses dados podem expor rotinas, horários de ausência, número de pessoas no local e facilitar ações como vigilância não autorizada ou planejamento de invasões.
  - Relógio inteligente (smartwatch):
    - Sensores: batimentos cardíacos, oxigenação do sangue, acelerômetro, GPS.
    - Dados coletados: frequência cardíaca, atividade física, localização.
    - Dados confidenciais: Sim (dados de saúde e localização).
    - Como os dados podem ser usados: Os dados de saúde e atividade física podem ser usados para acompanhamento do bem-estar, exercícios e alertas médicos. Em mãos erradas, informações como localização, horários de treino e condições de saúde podem ser exploradas para rastreamento, discriminação ou exposição de informações sensíveis do usuário.
  - Semáforo inteligente (trânsito):
    - Sensores: sensores de presença, câmeras, laços indutivos no asfalto.
    - Dados coletados: fluxo de veículos, tempo de espera, volume de tráfego.
    - Dados confidenciais: Não, geralmente são dados agregados e anônimos.
    - Como os dados podem ser usados: Os dados de fluxo de veículos podem ser usados para otimizar o trânsito, reduzir congestionamentos e melhorar a segurança viária. Como normalmente são dados agregados e anônimos, o risco de uso mal-intencionado é baixo, pois não permitem identificar indivíduos específicos.
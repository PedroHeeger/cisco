# Network Support and Security - Módulo 3   <img src="../0-aux/logo_course.png" alt="sfp_010" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="../">sfp_010 (Network Support and Security)   <img src="../0-aux/logo_course.png" alt="sfp_010" width="auto" height="25"></a>
### Module: 3. Segurança de Rede

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

### Course Module 3 Structure:
3. <a name="item03">Segurança de Rede</a><br>
  3.1 <a href="#item03.01">Introdução</a><br>
  3.2 <a href="#item03.02">Fundamentos de Segurança</a><br>
  3.3 <a href="#item03.03">Controle de acesso</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.3.1 <a href="../../../pkt/files/pkt_076/">Packet Tracer - Configurar Controle de Acesso</a><br>
  3.4 <a href="#item03.04">Defesa de sistemas e dispositivos</a><br>
  3.5 <a href="#item03.05">Proteção Antimalware</a><br>
  3.6 <a href="#item03.06">Prevenção de Intrusão Baseada em Host e Firewalls</a><br>
  3.7 <a href="#item03.07">Acesso sem fio seguro</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;3.7.1 <a href="../../../pkt/files/pkt_077/">Packet Tracer - Configurando Segurança Básica em Redes sem Fios</a><br>
  3.8 <a href="#item03.08">Resumo de Segurança de Rede</a><br>

---

### Objective:
O objetivo do módulo é apresentado na introdução, que compõe o primeiro item do desenvolvimento.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item03.01"><h4>3.1 Introdução</h4></a>[Back to summary](#item03)

🛡️ Governança e Diretrizes para Proteção de Ativos e Perímetros   
A estruturação de uma política de segurança corporativa ou institucional estabelece as regras, diretrizes e mecanismos tecnológicos necessários para salvaguardar a infraestrutura digital contra incidentes e acessos indevidos. Esse arcabouço normativo orienta a administração de TI na manutenção dos três pilares fundamentais da segurança da informação: a confidencialidade, a integridade e a disponibilidade dos dados (Tríade CID). Através da combinação de controles de acesso rígidos, barreiras de filtragem de tráfego e defesas locais, cria-se uma estratégia de proteção em camadas capaz de neutralizar ameaças internas e externas.

🎯 Objetivo do módulo:   
- Configurar e gerenciar mecanismos de autenticação, controle de acesso e políticas de defesa para blindar terminais e perímetros de rede.

📘 Tópicos do módulo:   
- Fundamentos de Segurança: Estudo dos conceitos estruturais de proteção de ativos, com foco nas metas de confidencialidade, integridade e disponibilidade da informação.
- Controle de acesso: Técnicas e configurações voltadas à identificação, autenticação e autorização estrita de usuários autorizados a trafegar na rede.
- Defesa de sistemas e dispositivos: Processos, rotinas administrativas e procedimentos técnicos padronizados para mitigar riscos e blindar sistemas operacionais.
- Proteção Antimalware: Análise de ferramentas de detecção, isolamento e resposta contra códigos maliciosos e softwares invasores em pontos finais.
- Prevenção de Intrusão Baseada em Host e Firewalls: Funcionamento de regras de filtragem de pacotes, monitoramento de portas lógicas e aplicação de sistemas de proteção local (HIPS).
- Acesso sem fio seguro: Protocolos de criptografia e procedimentos para parametrização de segurança básica (padrões WPA/WPA2/WPA3) em ambientes com tecnologia wireless.

<a name="item03.02"><h4>3.2 O Fundamentos de Segurança</h4></a>[Back to summary](#item03)

🧊 Cubo de Segurança Digital   
O Cubo de Segurança Digital (ou Cubo de McCumber) serve como um modelo conceitual estruturado para gerenciar a proteção de dados e sistemas de informação através de três dimensões essenciais.

🎯 Princípios Fundamentais: A Tríade CIA   
Esta dimensão define os objetivos centrais para a proteção do ciberespaço, orientando a priorização de ações defensivas em redes e sistemas.
- Confidencialidade: Restrição do acesso a dados sensíveis apenas a indivíduos, processos ou entidades autorizadas. A mitigação de exposição pode ocorrer via algoritmos de criptografia simétrica (como o AES) ou por meio de tokenização, técnica que substitui dados originais por valores aleatórios sem relação matemática, preservando o formato para bancos de dados e sistemas de pagamento. O controle também é exercido pelo gerenciamento de direitos digitais, subdividido em DRM (focado na proteção de propriedade intelectual e mídias contra cópias não autorizadas) e IRM (voltado ao controle corporativo de e-mails e documentos internos).
- Integridade: Salvaguarda dos dados contra modificações, exclusões ou falsificações não autorizadas durante todo o ciclo de vida (captura, armazenamento, recuperação, atualização e transferência). É mantida através de funções de hash criptográfico (como o SHA), validações, verificações de consistência e controles de acesso estritos. A criticidade da integridade varia conforme o segmento de atuação:
  - Crítica (Saúde): Validação contínua devido ao risco de impacto direto à vida humana (ex: precisão de receitas médicas).
  - Alta (Finanças/Comércio Eletrônico): Verificações frequentes para assegurar a precisão de transações e saldos.
  - Média (Mecanismos de Busca): Coleta de dados públicos com baixa frequência de auditoria.
  - Baixa (Mídias Sociais): Plataformas baseadas em opiniões e interações abertas, onde o nível de confiabilidade do conteúdo é reduzido.
- Disponibilidade: Garantia de acesso contínuo e oportuno aos dados e sistemas por usuários legítimos. A resiliência contra ataques ou falhas de hardware baseia-se na implementação de infraestrutura redundante (links, gateways e servidores).

💾 Estados dos Dados   
A segurança eficaz exige a aplicação de controles simultâneos nos três estados possíveis da informação no ciberespaço:
- Dados em Trânsito: Informações que trafegam através de redes locais ou externas.
- Dados Inativos (Armazenamento): Informações gravadas em mídias físicas ou digitais persistentes.
- Dados em Processamento: Informações em uso ativo pelas memórias e unidades de processamento dos sistemas.

🛠️ Pilares de Proteção e Salvaguardas   
A terceira dimensão estabelece os mecanismos de defesa e práticas recomendadas para mitigar vulnerabilidades e responder a incidentes:
- Tecnologia: Emprego de ferramentas atualizadas, inspeção de portas, varreduras de vulnerabilidades e testes de penetração (pentests).
- Políticas e Práticas: Atualização constante de sistemas operacionais e aplicações via aplicação de patches, além do monitoramento contínuo de logs de eventos e alertas para detecção de anomalias em tempo real.
- Pessoas (Conscientização): Treinamento em planos de contingência, testes práticos de restauração de backups e simulações de cenários de desastre para garantir a continuidade operacional.

<a name="item03.03"><h4>3.3 Controle de acesso</h4></a>[Back to summary](#item03)

🔒 Controles de Acesso   
A segurança da informação baseia-se na implementação de barreiras e permissões divididas em três categorias principais: físicas, lógicas e administrativas.
- Controles Físicos: Barreiras tangíveis que impedem o contato direto com ativos e instalações. Exemplos incluem guardas, cercas, detectores de movimento, travas de segurança para hardware, portas trancadas, cartões de proximidade, cães de guarda, sistemas de CFTV, eclusas (mantraps) e alarmes de intrusão.
- Controles Lógicos: Soluções de hardware e software destinadas ao gerenciamento de recursos digitais. Abrangem criptografia, cartões inteligentes com microchips, senhas, biometria, Listas de Controle de Acesso (ACLs), protocolos de comunicação, firewalls, roteadores, Sistemas de Detecção de Intrusão (IDS) e níveis de corte para bloqueio por tentativas incorretas.
- Controles Administrativos: Diretrizes institucionais voltadas a práticas de pessoal e negócios. Compreendem políticas organizacionais, procedimentos operacionais, critérios de contratação, checagem de antecedentes (criminais e de crédito), classificação de dados por nível de sensibilidade, treinamentos de segurança e avaliações periódicas de desempenho.

🔑 A Estrutura AAA    
Os controles administrativos utilizam a estrutura AAA para mitigar acessos não autorizados em redes, computadores e bancos de dados.
- Autenticação: Processo de validação da identidade declarada por um usuário (geralmente informada por um identificador exclusivo ou username). A comprovação exige a apresentação de fatores baseados em três categorias:
  - Algo que se sabe: Senhas alfanuméricas, frases secretas (passphrases) ou PINs.
  - Algo que se tem: Cartões inteligentes ou dispositivos geradores de chaves (tokens ou key fobs).
  - Algo que se é: Identificadores biométricos físicos (impressão digital, geometria da face, leitura de retina/íris) ou comportamentais (ritmo de digitação, dinâmica de voz, padrões de escrita).
- Autorização: Determinação automatizada dos privilégios concedidos ao usuário autenticado, definindo permissões de leitura, escrita, execução, alteração ou exclusão de recursos. O controle pode ser baseado em horários permitidos ou estruturado por meio de políticas:
  - Associação baseada em grupo: Permissões atribuídas a um conjunto de usuários com funções similares (ex: acesso restrito de TI à sala de servidores).
  - Nível de autoridade: Restrições baseadas na hierarquia ou cargo ocupado na organização.
- Contabilidade (Accounting): Rastreamento e registro cronológico das atividades executadas pelos usuários e processos em tempo real. Coleta métricas operacionais para auditorias e investigações de segurança, registrando tentativas de login (sucedidas ou falhas), horários de conexão, dados modificados e recursos consumidos.

🌐 Gestão de Identidade Federada (FIM)   
A Federação de Identidades interliga sistemas de gerenciamento de identidades de diferentes organizações ou plataformas.
- Objetivo: Permitir que o usuário utilize um único conjunto de credenciais para acessar sistemas distribuídos entre múltiplos domínios empresariais (conceito de login unificado).
- Risco Associado: O comprometimento de uma credencial federada concede ao agente de ameaça acesso potencial a múltiplos ambientes integrados.
- Mecanismo de Proteção: Vinculação estrita da identidade federada a dispositivos previamente autorizados e validados (como estações de trabalho e dispositivos móveis corporativos) para mitigar o compartilhamento inadvertido de dados sensíveis.

🛡️ Melhores Práticas para Credenciais e Autenticação   
Para mitigar ataques de quebra de credenciais e roubo de identidade, recomendam-se diretrizes estruturadas de governança de acessos:
- Complexidade de Senhas: Utilização de cadeias com comprimento igual ou superior a 8 caracteres (preferencialmente mais de 10), combinando letras maiúsculas, minúsculas, numerais e caracteres especiais. O uso de frases secretas (passphrases) eleva a entropia da senha e facilita a memorização.
- Gerenciamento de Senhas: Adoção de cofres de senhas centrais para geração automatizada e armazenamento seguro de credenciais complexas e exclusivas para cada sistema, eliminando reutilizações.
- Autenticação Multifator (MFA / 2FA): Exigência de dois ou mais fatores independentes de categorias distintas (ex: senha + código temporário enviado ao dispositivo móvel ou validação biométrica). O método impede o acesso mesmo em cenários de vazamento de senhas, elevando o nível de segurança em transações críticas, a exemplo de saques em caixas eletrônicos (cartão físico + PIN).
- Ciclo de Vida de Senhas: Alteração periódica de credenciais para limitar a janela de oportunidade de agentes maliciosos e proibição estrita de anotações físicas expostas no ambiente de trabalho.

<a name="item03.04"><h4>3.4 Defesa de sistemas e dispositivos</h4></a>[Back to summary](#item03)

🛡️ Fortalecimento e Endurecimento do Sistema Operacional   
O processo de fortalecimento (hardening) de um sistema operacional consiste na eliminação de vetores potenciais de ataque e na aplicação de configurações estritas de proteção para mitigar riscos de segurança.

🔄 Gerenciamento Sistemático de Atualizações e Patches   
A aplicação de correções de código (patches) impede que vulnerabilidades conhecidas sejam exploradas por agentes de ameaças ou códigos maliciosos (worms e vírus). A governança de atualizações deve seguir uma abordagem metodológica documentada:
- Estabelecimento de Linha de Base (Baseline): Definição de parâmetros padrão de desempenho e segurança para identificar desvios operacionais ou novas vulnerabilidades.
- Monitoramento e Avaliação: Acompanhamento contínuo de alertas de segurança dos fabricantes para verificar a aplicabilidade das correções no ambiente corporativo.
- Ciclo de Homologação: Teste prévio das atualizações em ambiente controlado antes da distribuição massiva na infraestrutura.
- Serviços Automatizados de Patch (Servidores Locais): Centralização do download de atualizações diretamente do fabricante para um servidor interno. Esse mecanismo otimiza o consumo de banda da rede, gera relatórios de conformidade por ativo, impede que usuários finais desativem as atualizações e permite que administradores programem ou recusem pacotes específicos (service packs).
- Manutenção Preventiva de Terceiros: Extensão do gerenciamento proativo de correções para aplicações críticas de terceiros (como navegadores e leitores de PDF) para neutralizar portas de entrada de ransomware.

🦠 Vetores de Código Malicioso e Defesas Avançadas   
A proteção contra malwares exige a compreensão de ameaças complexas que fogem do escopo dos antivírus tradicionais:
- Antivírus Falsos (Rogue Antivirus): Engenharia social baseada em janelas pop-up que simulam alertas legítimos do sistema operacional para induzir o usuário a baixar cargas maliciosas.
- Malware Sem Arquivo (Fileless): Códigos que residem estritamente na memória volátil (RAM), utilizando binários legítimos do próprio sistema (como o Windows PowerShell) para executar ações. Não deixam vestígios estruturais em disco e sua execução é interrompida com o reinício do host.
- Ataques Baseados em Scripts: Uso de linguagens como Python, Bash ou macros VBA para automatizar ações danosas.
- Remoção de Software Não Homologado: Eliminação rigorosa de aplicações não autorizadas que, mesmo sem código malicioso intencional, violam políticas corporativas e abrem brechas de segurança.

🖥️ Proteção Avançada do Endpoint   
As soluções de segurança baseadas em host executam diretamente nos dispositivos finais com o objetivo de monitorar, analisar e interceptar atividades maliciosas em tempo real.
- Firewall Baseado em Host: Atua na filtragem de tráfego de rede local. O mecanismo bloqueia ou permite conexões de entrada e saída por meio de regras estritas aplicadas a portas e protocolos específicos.
- HIDS (Sistema de Detecção de Intrusão em Host): Realiza o monitoramento e a auditoria interna do dispositivo. A ferramenta analisa registros, chamadas de sistema e modificações no registro do sistema em busca de anomalias, salvando os arquivos de log localmente.
- HIPS (Sistema de Prevenção de Intrusão em Host): Focado na mitigação ativa de ameaças. O software analisa desvios de tráfego, assinaturas de pacotes e comportamentos dos protocolos. Ao identificar uma ação maliciosa, executa contramedidas automáticas, como o descarte de pacotes ou a redefinição da conexão.
- EDR (Detecção e Resposta de Endpoint): Provê monitoramento analítico contínuo através da coleta de telemetria do dispositivo. Diferente de softwares antivírus convencionais, o sistema rastreia, investiga e responde ativamente a ameaças complexas já instaladas no host.
- DLP (Prevenção de Perda de Dados): Fornece controle centralizado para assegurar que informações sensíveis não sofram exfiltração, uso indevido ou acesso por elementos não autorizados.
- NGFW (Firewall de Próxima Geração): Aparelho ou software de segurança que combina as capacidades de um firewall tradicional com funções avançadas, como a inspeção profunda de pacotes (DPI) integrada diretamente a sistemas de prevenção contra intrusão (IPS).

🔐 Criptografia de Armazenamento e Hardware de Segurança   
A confidencialidade dos dados em repouso é assegurada por mecanismos de criptografia estrutural:
- Criptografia de Arquivo (EFS): Proteção aplicada a arquivos ou pastas individuais.
- Criptografia de Disco Total (FDE): Criptografia integral da unidade de armazenamento, incluindo arquivos temporários e paginação de memória. O subsistema utiliza a tecnologia BitLocker integrada ao chip TPM (Trusted Platform Module) na placa-mãe, responsável por armazenar chaves criptográficas, certificados e chaves de integridade física.
- Dispositivos Removíveis: O recurso BitLocker To Go assegura mídias externas mediante autenticação por senha, operando sem a obrigatoriedade do chip TPM.
- Unidades de Autocriptografia (SEDs): Discos com criptografia nativa processada diretamente no hardware pelo fabricante, blindando os dados contra manipulações no sistema operacional.

🏗️ Integridade e Segurança do Processo de Inicialização   
A proteção do sistema deve ocorrer antes mesmo do carregamento completo do sistema operacional.
- Evolução do Firmware: Substituição do BIOS tradicional pelo padrão UEFI, que permite execução em modo de 64 bits e fornece uma interface padronizada entre hardware e software.
- Inicialização Segura (Secure Boot): Padrão de segurança onde o firmware UEFI valida a assinatura digital de cada componente de boot (drivers, aplicações e núcleo do sistema operacional). Caso a assinatura seja inválida ou modificada, o processo é interrompido.
- Inicialização Medida (Measured Boot): Processo complementar que analisa sequencialmente cada módulo carregado e armazena os registros criptográficos no chip TPM. Essa cadeia gera um log de integridade auditável remotamente, viabilizando o carregamento antecipado de ferramentas antimalware e bloqueando aplicações não confiáveis.

🍏 Arquitetura de Segurança da Plataforma macOS   
O ecossistema Apple adota soluções nativas acopladas ao hardware para a proteção do endpoint:
- Secure Enclave: Coprocessador de segurança isolado da CPU principal que gerencia a criptografia AES em nível de hardware, chaves de criptografia e processamento de dados biométricos, neutralizando o acesso direto do sistema operacional ou de malwares.
- FileVault e Data Protection: Criptografia de armazenamento em tempo real integrada ao motor AES do hardware, impedindo a exposição de chaves na memória principal do sistema.
- ROM de Inicialização: Proteção de baixo nível que impede a execução de códigos que não correspondam ao sistema operacional original e assinado pela Apple.
- Mecanismos de Defesa de Software:
  - Gatekeeper: Validação de assinaturas digitais que restringe a instalação de softwares apenas a desenvolvedores autenticados.
  - XProtect: Módulo antimalware baseado na identificação e bloqueio de assinaturas de códigos maliciosos conhecidos.
  - MRT (Malware Removal Tool): Ferramenta automatizada que atua na remoção de infecções ativas durante o login ou reinicialização do host.
  - Find My Mac: Recurso de localização geográfica com capacidade de bloqueio remoto e destruição lógica de dados em caso de perda ou roubo.

🏢 Controles de Segurança Física Aplicados à Infraestrutura   
A integridade digital depende diretamente do isolamento físico dos ativos de tecnologia:
- Proteção do Hardware: Uso de travas de cabo mecânicas para fixação de endpoints, manutenção de salas de servidores/telecomunicações estritamente trancadas e aplicação de blindagens eletromagnéticas (Gaiolas de Faraday) para mitigar a interceptação de sinais.
- Mecanismos de Controle de Acesso: Substituição de fechaduras cilíndricas comuns por fechaduras digitais cifradas (que permitem restrição por horários e geram trilhas de auditoria das aberturas).
- Sistemas de RFID: Implementação de etiquetas de Identificação por Radiofrequência passivas ou ativas conectadas a antenas para automatizar o inventário de ativos corporativos, rastreamento de hardware e liberação de acessos sem fio.

<a name="item03.05"><h4>3.5 Proteção Antimalware</h4></a>[Back to summary](#item03)

🌐 Expansão do Perímetro e Definição de Endpoints   
Endpoints são definidos como nós ou hosts em uma rede que possuem a capacidade de iniciar comunicações ou responder a acessos de outros hosts.
- Escopo de Dispositivos: Além de servidores, desktops e laptops tradicionais, a proliferação da Internet das Coisas (IoT) integrou elementos como câmeras de segurança, controladores industriais, eletrodomésticos e sistemas de iluminação inteligente a esta categoria.
- Vetor de Vulnerabilidade: Cada endpoint conectado atua como uma porta de entrada potencial para a execução de códigos maliciosos.
- Impacto da Computação em Nuvem: A adoção de ambientes em nuvem expandiu as fronteiras lógicas das redes corporativas para ativos hospedados na internet, fora do controle direto de infraestrutura da organização.

📈 Desafios de Segurança no Cenário Tecnológico   
Pesquisas com especialistas em segurança cibernética apontam que as principais preocupações operacionais estão diretamente ligadas a ameaças direcionadas a endpoints:
- Ransomware (53%): Vetor prioritário devido ao aumento expressivo de ataques de sequestro de dados.
- Trabalho Remoto (47%): Riscos decorrentes da descentralização dos acessos pós-pandemia.
- Visibilidade Limitada (41%): Dificuldade no monitoramento analítico de ameaças na infraestrutura.

⚔️ Vetores de Ataque: Externos vs. Internos   
A proteção de ativos exige estratégias distintas para conter ameaças de acordo com a sua origem.
- Ataques Externos e Proteção de Perímetro: As investidas originadas fora da rede visam a interrupção de serviços e a exfiltração de dados sensíveis. Exemplos comuns incluem ataques de Negação de Serviço (DoS), invasão de servidores web para desfiguração (defacement) e violação de repositórios de dados confidenciais. A defesa de perímetro utiliza um conjunto de dispositivos dedicados:
  - Roteadores endurecidos (hardened) com terminação de VPN.
  - Firewalls de Próxima Geração (NGFW).
  - Appliances de Sistemas de Prevenção de Intrusão (IPS).
  - Servidores de Autenticação, Autorização e Contabilidade (AAA).
- Ataques Internos e Segurança de LAN: A infiltração em um host interno permite que o atacante o utilize como pivô para movimentação lateral em direção a sistemas críticos. A segurança da rede local (LAN) subdivide-se em duas frentes de proteção:
  - Segurança de Endpoints: Proteção de dispositivos de usuários (laptops, telefones IP, impressoras) contra infecções por malware.
  - Segurança da Infraestrutura de Rede: Blindagem de ativos de interconexão (switches e roteadores) contra ataques estruturais da camada 2, como estouro de tabela de endereços MAC, falsificações (spoofing), ataques direcionados ao protocolo DHCP, tempestades de broadcast (LAN storms), manipulação do protocolo STP e saltos de VLAN.

🛡️ Soluções de Proteção Baseadas em Host   
A proteção de dispositivos móveis que acessam redes domésticas ou públicas não confiáveis requer a instalação de ferramentas locais de segurança.
- Software Antivírus / Antimalware: Ferramentas instaladas para detecção e mitigação de ameaças em tempo real. A análise é realizada por meio de três metodologias distintas:
  - Baseada em Assinaturas: Identificação de padrões e características específicas de arquivos maliciosos conhecidos.
  - Baseada em Heurística: Reconhecimento de traços gerais e estruturas compartilhadas por famílias de malwares.
  - Baseada em Comportamento: Monitoramento analítico de ações e execuções suspeitas no sistema.
- Modelos de Implantação de Antivírus:
  - Baseado em Agente: O software roda localmente consumindo memória e processamento de cada máquina protegida.
  - Sem Agente (Agentless): Centraliza as varreduras a partir de um servidor ou appliance virtual dedicado. Modelo amplamente adotado em ambientes virtualizados para evitar a degradação de desempenho provocada pela execução de múltiplos agentes em um mesmo hardware (ex: VMware vShield).
- Firewalls de Host: Softwares integrados ao sistema operacional (como o Windows Defender Firewall) ou soluções específicas (como iptables e TCP Wrappers no Linux). Têm a função de restringir tráfego de entrada e saída a conexões estritamente legítimas, mitigando o alastramento de pragas na rede local.
- Suítes de Segurança Integradas: Combinação de antivírus, anti-phishing, filtros de navegação segura, HIPS e firewall em um único pacote para estruturar uma defesa em camadas.
- Telemetria Centralizada: Capacidade de gerar registros detalhados (logs) de eventos locais e encaminhá-los a repositórios centrais para auditoria e análise por equipes de SOC. Avaliações independentes sobre a eficácia dessas ferramentas são fornecidas por institutos especializados, como o AV-TEST.

🕸️ Proteção de Endpoints Baseada em Rede   
Para cenários de redes sem fronteiras, as defesas locais são complementadas por mecanismos de varredura e inteligência compartilhada em nível de rede:
- Cisco Secure Endpoint: Plataforma centralizada para detecção, bloqueio e remediação de malwares diretamente nos dispositivos finais.
- Cisco Secure Email: Filtra e bloqueia mensagens de SPAM, tentativas de phishing e anexos maliciosos antes que o tráfego atinja o endpoint do usuário.
- Cisco Umbrella: Atua na camada de resolução de nomes (DNS), bloqueando o acesso de hosts internos a domínios maliciosos, aplicando políticas de uso aceitável e inspecionando conexões web contra malwares.
- Controle de Admissão de Rede (NAC): Sistema de governança que inspeciona o estado de conformidade e a autorização de um dispositivo, bloqueando o acesso à infraestrutura caso este não atenda aos requisitos mínimos de segurança estabelecidos.

<a name="item03.06"><h4>3.6 Prevenção de Intrusão Baseada em Host e Firewalls</h4></a>[Back to summary](#item03)

🧱 Operação e Fundamentos de Firewalls   
Um firewall atua como um sistema ou conjunto de sistemas configurado para aplicar políticas de controle de acesso entre diferentes zonas de rede, servindo como o mecanismo central de segurança perimetral.

⚙️ Propriedades, Benefícios e Limitações   
Propriedades Comuns   
- Resiliência Estrutural: Sistemas projetados com alta resistência a ataques diretos direcionados à rede.
- Choke Point (Ponto Único de Trânsito): Todo o tráfego entre a infraestrutura interna e as redes externas é forçado a transitar obrigatoriamente através do dispositivo.
- Imposição de Políticas: Aplicação rigorosa das diretrizes de controle de acesso definidas pela organização.

Benefícios Operacionais   
- Ocultação de hosts, aplicações e recursos sensíveis contra acessos de usuários externos não confiáveis.
- Saneamento de fluxos de comunicação, mitigando a exploração de vulnerabilidades e falhas nativas dos protocolos.
- Intercepção de cargas úteis maliciosas direcionadas a clientes ou servidores.
- Redução da complexidade de governança ao centralizar o controle de acessos da rede em pontos específicos.

Limitações Técnicas   
- Ponto Único de Falha (SpoF): Falhas de configuração podem indisponibilizar a rede ou criar brechas críticas.
- Incompatibilidade de Aplicações: Restrições nativas impedem o tráfego seguro de determinados tipos de dados.
- Evasão e Encapsulamento: Usuários internos podem burlar as regras criando túneis para tráfego bloqueado; agentes de ameaça podem ocultar tráfego malicioso dentro de protocolos permitidos (túneis legítimos).
- Degradação de Desempenho: A análise e filtragem de pacotes podem elevar a latência e reduzir o throughput da rede.

🗂️ Classificação e Tipos de Firewalls   
- Filtragem de Pacotes (Sem Estado / Stateless): Operam geralmente integrados ao hardware de roteadores, processando o tráfego com base estritamente em critérios das Camadas 3 e 4 do modelo OSI (endereços IP, portas e protocolos).
  - Mecanismo: Consulta simples a tabelas estáticas de ACL (Lista de Controle de Acesso). Por exemplo, realiza o bloqueio direto da porta TCP 25 (SMTP) em um host específico para conter a propagação de pragas via e-mail.
  - Vantagens: Baixo impacto no desempenho da rede, facilidade de implementação, suporte universal em roteadores e proteção básica de baixo custo.
  - Desvantagens: Vulnerável a ataques de falsificação de IP (IP Spoofing), ineficácia no tratamento de pacotes fragmentados (fragmentos subsequentes ao primeiro contornam o filtro de cabeçalho TCP), tabelas de regras complexas de manter e incapacidade de lidar com portas dinâmicas ou verificar o contexto da conexão.
- Inspeção de Estado (Stateful): Consiste na tecnologia mais difundida no mercado corporativo, atuando nas camadas de Rede, Transporte e Sessão (Camadas 3, 4 e 5 do modelo OSI).
  - Mecanismo: Monitora o contexto das conexões por meio de uma tabela de estado interna. Determina se os pacotes recebidos pertencem a uma sessão legítima em andamento ou se são de origem não autorizada.
  - Vantagens: Defesa nativa contra ataques de negação de serviço (DoS) e spoofing, filtragem mais rigorosa e desempenho superior em comparação a proxies.
  - Desvantagens: Ausência de inspeção na camada de aplicação (não analisa o conteúdo de requisições HTTP, por exemplo), suporte limitado a protocolos sem estado (como UDP e ICMP) e dificuldade em gerenciar aplicações com negociação dinâmica de portas sem abrir intervalos amplos de conexões.
- Gateway de Aplicação (Proxy Firewall): Interpõe-se diretamente na comunicação entre o cliente e o servidor remoto, operando até a camada de aplicação (Camada 7 do modelo OSI).
  - Mecanismo: O processamento ocorre via software. O cliente estabelece uma conexão com o proxy, e este inicia uma nova sessão com o destino em seu próprio nome, ocultando a identidade e a estrutura interna do cliente original.
- Firewall de Próxima Geração (NGFW): Evolução dos sistemas baseados em estado que agrega funções de segurança integradas em um único elemento de hardware ou software.
  - Recursos: Motores de Prevenção de Intrusão (IPS) integrados, controle e visibilidade profunda de aplicações (identificação de softwares específicos e comportamentos de risco), atualização dinâmica contra vetores de ameaças emergentes e feeds de inteligência de segurança cibernética.
- Transparente (Bridge Mode): Atua na filtragem de tráfego IP operando em modo de ponte entre interfaces de rede, sem alterar o roteamento.
- Híbrido: Integração de múltiplas arquiteturas, como a combinação de mecanismos stateful com gateways de aplicação.

💻 Firewalls Baseados em Host e Arquitetura Distribuída   
Softwares executados diretamente no sistema operacional do endpoint para gerenciar as regras de conectividade locais através de perfis e diretrizes específicas.
- Capacidades Operacionais: Permitem a criação de regras restritas por portas, protocolos e endereços IP, gerando alertas em tempo real sobre comportamentos suspeitos e registrando eventos (logs com data, hora, IPs de origem/destino e status da conexão).
- Firewalls Distribuídos: Modelo de governança onde agentes instalados nos hosts executam as regras localmente, mas recebem diretrizes, políticas e centralizam o envio de registros para um console de gerenciamento unificado.
- Principais Soluções de Mercado:
  - Windows Defender Firewall: Utiliza perfis automáticos de conectividade para ajustar o nível de restrição:
    - Domínio: Aplicado a redes corporativas confiáveis que possuem infraestrutura de segurança dedicada.
    - Privado: Destinado a redes isoladas da internet por roteadores ou firewalls perimetrais (redes domésticas).
    - Público: Perfil estrito para conexões em ambientes de alto risco (redes abertas ou wireless públicas).
  - Soluções do Ecossistema Linux:
    - iptables: Ferramenta clássica de espaço de usuário para configuração de tabelas de regras integradas aos módulos Netfilter do kernel.
    - nftables: Sucessor moderno do iptables, utiliza uma máquina virtual interna no kernel do Linux para otimizar a inspeção e o encaminhamento de pacotes.
    - TCP Wrappers: Sistema de controle de acesso e auditoria focado em filtrar chamadas de serviços de rede com base em endereços IP.

🛡️ Governança de Portas e Suítes de Endpoint   
A postura de segurança de um firewall orienta-se por duas filosofias principais de configuração:
- Política Restritiva: Todo o tráfego e portas são bloqueados por padrão, exceto aqueles explicitamente autorizados. É o padrão de fábrica adotado pela indústria para mitigar exposições causadas por negligência na configuração.
- Política Permissiva: Todo o tráfego é liberado, exceto as portas e serviços expressamente descritos na lista de bloqueio. Modelo considerado inseguro devido à ampla superfície de ataque exposta.

Ecossistema Antimalware de Endpoint   
As soluções baseadas em host combinam firewalls com ferramentas de proteção especializadas para mitigar ameaças estruturais (vírus, worms, cavalos de troia, keyloggers, spyware e adware):
  - Antivírus: Monitoramento contínuo da memória e disco com isolamento em quarentena ou eliminação de arquivos nocivos.
  - Anti-adware: Bloqueio de softwares focados em injeção de publicidade não autorizada.
  - Anti-phishing: Filtragem e interceptação de acessos a domínios e IPs catalogados como fraudes ou engenharia social.
  - Anti-spyware: Detecção de ferramentas de monitoramento oculto e registradores de digitação.
  - Validação de Fontes Confiáveis: Alertas proativos disparados antes da instalação de softwares não assinados ou acessos a páginas web com baixa reputação de segurança.

<a name="item03.07"><h4>3.7 Acesso sem fio seguro</h4></a>[Back to summary](#item03)

📶 Vetores de Vulnerabilidade em Redes Sem Fio (WLAN)   
O meio de propagação por radiofrequência torna as redes locais sem fio (WLANs) inerentemente expostas, permitindo que agentes de ameaças interceptem sinais sem a necessidade de acesso físico às instalações da organização.
- Interceptação de Dados: Captação de pacotes trafegados no espectro de rádio por meio de adaptadores de rede (NICs) em modo promíscuo. Exige a aplicação de criptografia robusta para impedir a leitura do tráfego.
- Intrusão de Usuários Não Autorizados: Tentativas de associação ilegítima à infraestrutura de rede, mitigadas apenas por mecanismos estritos de autenticação.
- Ataques de Negação de Serviço (DoS): Comprometimento da disponibilidade dos serviços da WLAN, divididos em três origens:
  - Falhas de Configuração: Erros administrativos ou alterações intencionais por agentes com privilégios elevados que desativam o ponto de acesso (AP).
  - Interferência Intencional (Jamming): Injeção maliciosa de ruído no espectro magnético para saturar o meio físico, impedindo a comunicação de clientes legítimos.
  - Interferência Acidental: Degradação do sinal provocada por barreiras físicas ou dispositivos que operam na mesma frequência (fornos de micro-ondas, telefones sem fio e babás eletrônicas). A faixa de 2,4 GHz apresenta maior suscetibilidade a esse tipo de atenuação em comparação à faixa de 5 GHz.

🛠️ Mitigação de Dispositivos Ilegais e Ataques no Caminho   
- Pontos de Acesso Não Autorizados (Rogue APs): Consistem em roteadores ou APs conectados à infraestrutura corporativa sem validação prévia da equipe de TI. Podem ser instalados por engenharia social, colaboradores sem intuito malicioso ou atacantes internos.
  - Riscos: Permitem a captura de endereços MAC, interceptação de pacotes e contornam os controles perimetrais de segurança. Incluem-se nesta categoria os hotspots pessoais ativados em estações de trabalho autorizadas.
  - Contramedida: Configuração de diretrizes específicas de detecção de Rogue APs em Controladores de LAN Sem Fio (WLCs) e monitoramento contínuo do espectro de rádio via software de gerência.
- Ataque de AP Gêmeo do Mal (Evil Twin): Variante de ataque Man-in-the-Middle (MITM) ou On-Path comum em ambientes com autenticação aberta (aeroportos e cafés).
  - Mecanismo: O atacante implanta um AP configurado com o mesmo Identificador de Conjunto de Serviços (SSID) da rede legítima. Dispositivos próximos ao AP malicioso associam-se a ele devido à maior intensidade de sinal.
  - Fluxo de Dados: O tráfego do cliente é capturado pelo AP do atacante, que o repassa ao AP legítimo. O fluxo de retorno segue o caminho inverso. Esse processo viabiliza o roubo de credenciais, exfiltração de dados pessoais e o comprometimento do sistema do endpoint.
  - Contramedida: Implementação de infraestruturas de WLAN que exijam autenticação mútua e monitoramento analítico de desvios de comportamento no tráfego de rede.

🔒 Mecanismos de Controle Legados e sua Ineficácia   
Historicamente, utilizavam-se duas técnicas para restringir o acesso à WLAN, embora ambas sejam consideradas insuficientes contra atacantes especializados:
- Ocultação do SSID: Desativação do envio dos quadros de sinalização (beacon) do AP, forçando a inserção manual do nome da rede no cliente. Limitação: O SSID permanece visível em texto claro em outros quadros de gerenciamento de associação, sendo facilmente capturado por farejadores de pacotes (sniffers).
- Filtragem de Endereços MAC: Criação de listas estáticas de permissão ou negação baseadas no endereço físico das NICs. Limitação: Endereços MAC legítimos podem ser clonados ou falsificados (MAC Spoofing) após a interceptação do tráfego aéreo.

🔐 Evolução dos Padrões de Autenticação e Criptografia   
O padrão IEEE 802.11 define dois modelos principais de controle de acesso à mídia:
- Autenticação de Sistema Aberto: Permite a associação de qualquer dispositivo sem validação de identidade. Indicado exclusivamente para redes públicas onde a segurança não é prioridade corporativa. Nestes cenários, a proteção dos dados deve ser gerenciada na camada de aplicação ou via túneis de Redes Virtuais Privadas (VPNs).
- Autenticação de Chave Compartilhada: Exige a inserção de credenciais comuns para autenticação e geração de chaves de criptografia. Divide-se em quatro padrões históricos e operacionais:
  - WEP (Wired Equivalent Privacy): Padrão legado baseado no algoritmo de cifra de fluxo RC4 com chaves estáticas. Devido a falhas estruturais na reutilização de vetores de inicialização, é considerado inseguro e seu uso é proibido.
  - WPA (Wi-Fi Protected Access): Implementação temporária que adota o protocolo TKIP (Temporal Key Integrity Protocol). O TKIP gera chaves dinâmicas exclusivas para cada pacote e adiciona uma verificação de integridade da mensagem (MIC), corrigindo as vulnerabilidades do WEP.
  - WPA2: Padrão consolidado de mercado baseado no algoritmo AES (Advanced Encryption Standard). Emprega o mecanismo CCMP (Modo de Cifra de Contador com Protocolo de Código de Autenticação de Mensagem em Cadeia de Blocos) para garantir confidencialidade e integridade estrutural, identificando alterações nos bits dos pacotes.
  - WPA3: Nova geração de segurança sem fio. Torna obrigatório o uso de Quadros de Gerenciamento Protegidos (PMF) e desativa retrocompatibilidades com protocolos inseguros.

🏢 Modelos de Implantação: Pessoal vs. Corporativo   
As arquiteturas WPA e WPA2 dividem-se em dois escopos de aplicação:
- Modo Pessoal (WPA-Personal / PSK): Projetado para ambientes domésticos ou pequenas filiais. Utiliza uma chave pré-compartilhada (PSK) única inserida diretamente no AP e nos clientes para autenticação, eliminando a necessidade de servidores dedicados.
- Modo Corporativo (WPA-Enterprise): Desenvolvido para infraestruturas empresariais que demandam gerenciamento centralizado através do padrão IEEE 802.1X.
  - Infraestrutura AAA: Exige a integração com um servidor de autenticação RADIUS. O AP atua como intermediário, autenticando-se com o RADIUS via chaves compartilhadas locais através das portas UDP oficiais 1812 (Autenticação) e 1813 (Contabilidade) — ou pelas portas legadas 1645 e 1646.
  - Mecanismo: O fluxo de autenticação do usuário final utiliza o protocolo EAP (Extensible Authentication Protocol), permitindo a negociação dinâmica e segura de chaves privadas de sessão (AES ou TKIP) sem a exposição de credenciais globais no meio físico.

🚀 Implementações Avançadas do Padrão WPA3   
O ecossistema WPA3 corrige falhas críticas de arquitetura encontradas nas revisões anteriores da Wi-Fi Alliance:
- WPA3-Personal e Proteção contra Força Bruta: No WPA2-Personal, atacantes podiam capturar o processo de handshake inicial e decifrar a senha offline via dicionários. O WPA3 mitiga essa vulnerabilidade ao substituir o método tradicional pelo mecanismo SAE (Simultaneous Authentication of Equals). O processo realiza uma troca de chaves baseada em criptografia assimétrica onde a senha nunca é exposta, impedindo ataques de força bruta.
- WPA3-Enterprise e Alta Criptografia: Restringe a operação ao conjunto de algoritmos de segurança nacional (CNSA), exigindo uma suíte criptográfica de 192 bits e eliminando a combinação de protocolos legados em ambientes de alta criticidade.
- Criptografia em Redes Abertas (OWE): Substitui o tráfego em texto claro de redes públicas sem autenticação pelo mecanismo OWE (Opportunistic Wireless Encryption), garantindo a criptografia individualizada dos dados de cada usuário conectado.
- Integração IoT via DPP (Device Provisioning Protocol): Substitui o padrão vulnerável WPS (Wi-Fi Protected Setup). O DPP facilita o provisionamento seguro de dispositivos IoT sem interface (headless). O firmware ou a embalagem do hardware traz um código QR contendo uma chave pública embutida. A leitura deste código por um administrador realiza a integração automatizada e criptografada do dispositivo à WLAN corporativa.

<a name="item03.08"><h4>3.8 Resumo de Segurança de Rede</h4></a>[Back to summary](#item03)

🏢 O Cubo de Segurança e a Tríade CIA   
O modelo tridimensional do cubo de segurança estrutura a proteção de dados sob três eixos centrais. O primeiro eixo define os objetivos essenciais conhecidos como a Tríade CIA:
- Confidencialidade: Garante o sigilo dos dados, impedindo o acesso de pessoas não autorizadas.
- Integridade: Assegura que as informações permaneçam exatas e confiáveis, utilizando funções de hashing, validações lógicas e travas de acesso para evitar alterações indevidas.
- Disponibilidade: Garante que os recursos permaneçam acessíveis aos usuários legítimos através de manutenção de hardware, redundâncias e cópias de segurança (backups).

Esses objetivos devem proteger a informação em seus três estados possíveis: em movimentação pela rede (trânsito), guardada em discos (repouso) ou sendo processada pela CPU, sustentados por três pilares defensivos: as pessoas, as tecnologias e os processos organizacionais.

🔑 Mecanismos de Controle e Governança (AAA)   
A restrição de acesso aos ambientes corporativos divide-se em três esferas de atuação. A primeira é o controle físico, focado em impedir a aproximação de pessoas não autorizadas aos equipamentos reais por meio de guardas, alarmes, cercas e biometria na portaria. A segunda esfera abrange os controles lógicos, que utilizam soluções digitais como firewalls, criptografia e regras de acesso em roteadores. Por fim, existem os controles administrativos, representados pelas políticas escritas da empresa, triagens de recursos humanos e normas internas.

A governança global de todas essas barreiras apoia-se em três pilares integrados:
- Autenticação: Valida e confirma quem é o usuário com base em credenciais de acesso, biometria de digitais ou códigos temporários enviados ao smartphone.
- Autorização: Define os privilégios exatos do indivíduo, estabelecendo os sistemas lógicos aos quais ele tem acesso e os horários permitidos de operação.
- Contabilidade e Auditoria: Registra todas as ações realizadas na infraestrutura em arquivos de log, documentando o que foi modificado e quando ocorreu o acesso para fins de auditoria.

Quando diferentes organizações decidem unificar esses parâmetros para que um único conjunto de credenciais dê acesso aos sistemas de todo o grupo comercial, adota-se a Gestão de Identidade Federada. Essa abordagem traz mais agilidade no dia a dia, mas centraliza o risco de invasão caso a base do provedor central sofra uma brecha de segurança.

💻 Proteção Avançada de Endpoints e Blindagem de Sistemas   
Para combater ameaças que não dependem da instalação de arquivos tradicionais no disco, como vírus sem arquivo que rodam instruções diretamente na memória RAM usando consoles como Python e Bash, as organizações precisam blindar seus computadores de forma automatizada. Essa manutenção exige a aplicação planejada de atualizações e correções de segurança nos sistemas operacionais para neutralizar brechas públicas antes que agentes maliciosos as descubram.

O ecossistema de defesa das estações de trabalho combina diferentes camadas de software especializado:
- A ferramenta de Detecção de Intrusão Baseada em Host atua vigiando os registros locais para gerar alertas sempre que o sistema operacional sofrer modificações não autorizadas. Para respostas imediatas, o mecanismo de Prevenção de Intrusão Baseada em Host vai além da vigilância e age bloqueando o ataque no momento em que ele tenta derrubar o sistema ou iniciar conexões suspeitas.
- Em um nível mais analítico, a tecnologia de Detecção e Resposta de Endpoint monitora continuamente o comportamento geral da máquina para coletar dados operacionais de segurança em tempo real. Complementando essa estrutura, os sistemas de Prevenção contra Perda de Dados impedem o vazamento de arquivos confidenciais da empresa por meio do bloqueio de uploads e transferências não autorizadas.
- A proteção da informação armazenada no computador baseia-se em recursos de criptografia de disco. No ambiente Windows, o sistema EFS codifica arquivos individuais, enquanto o BitLocker bloqueia a unidade inteira, exigindo a presença de um processador de segurança integrado na placa-mãe para validar a máquina. No ambiente Apple, essa integridade baseia-se em hardwares com motores de criptografia dedicados, chips que processam a biometria isolada do sistema operacional e sistemas nativos como o Gatekeeper, que impede a instalação de qualquer programa sem uma assinatura digital válida.

🚦 Arquitetura e Tipologias de Firewalls   
Os firewalls formam a barreira perimetral entre o ambiente interno confiável e a internet externa, filtrando fluxos de tráfego com base nas regras corporativas. Eles dividem-se em diferentes arquiteturas de funcionamento:
- Filtragem de Pacotes (Stateless): Analisa dados isolados das Camadas 3 e 4 (como IPs e portas). É veloz e consome poucos recursos, mas pode ser burlado por fragmentação de pacotes e falsificação de IP.
- Inspeção de Estado (Stateful): Monitora o contexto e o histórico de cada sessão das Camadas 4 e 5, sendo altamente eficaz no bloqueio de conexões não solicitadas externas.
- Gateway de Aplicação (Proxy): Intercepta e reconstrói o tráfego nas camadas superiores (até a Camada 7), inspecionando o conteúdo real da aplicação.
- Próxima Geração (NGFW): Combina as funções de filtragem tradicionais com inteligência profunda de pacotes, recursos de antivírus de rede e sistemas de prevenção a intrusões.
- Transparentes / Híbridos: Operam em modo bridge oculto na rede ou mesclam atributos de múltiplas categorias de firewall simultaneamente.

A aplicação dessas ferramentas pode ocorrer de forma centralizada ou distribuída na rede via agentes lógicos, enquanto firewalls pessoais (como o Windows Defender ou o iptables/nftables no Linux) protegem localmente os fluxos de entrada e saída das estações.

📻 Segurança e Criptografia em Redes Sem Fio   
As transmissões por ondas de rádio enfrentam ameaças severas de interceptação de dados, interferências geradas por ataques de negação de serviço e o risco de antenas clandestinas (Rogue APs / Evil Twin) projetadas para atrair clientes legítimos e capturar dados em ataques de Homem no Meio (MitM). Práticas básicas como ocultação de SSID e filtros de endereço MAC fornecem barreiras superficiais, exigindo protocolos de segurança robustos.

A evolução dos mecanismos de autenticação e proteção sem fio eliminou padrões obsoletos e vulneráveis, como o WEP e a primeira versão do WPA, estabelecendo novas diretrizes técnicas:
- WPA2: Utiliza algoritmos robustos como o AES para codificar as transmissões, sendo o requisito mínimo exigido nas redes atuais.
- WPA3: Representa o padrão ideal de segurança de rádio. Na modalidade corporativa, integra-se à autenticação 802.1X / EAP com servidores RADIUS dedicados. Em redes abertas ou públicas, adota a criptografia OWE para proteger o tráfego dos usuários mesmo sem uma senha de entrada, utilizando ainda o protocolo DPP para garantir a associação segura de dispositivos de Internet das Coisas (IoT).
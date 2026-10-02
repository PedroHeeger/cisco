# Digital Safety and Security Awareness - Módulo 2   <img src="../0-aux/logo_course.png" alt="sfp_006" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../self_paced/">self-paced</a>
### Software/Subject: cybersecurity   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/cybersecurity.jpg" alt="cybersecurity" width="auto" height="25"></a>
### Course: <a href="../">sfp_006 (Digital Safety and Security Awareness)   <img src="../0-aux/logo_course.png" alt="sfp_006" width="auto" height="25"></a>
### Module: 2. Proteja o que lhe é importante

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

### Course Module 2 Structure:
2. <a name="item02">Proteja o que lhe é importante</a><br>
2.1 <a href="#item02.01">Um guia abrangente para proteger a sua vida digital</a><br>
2.2 <a href="#item02.02">Fundamentos de Privacidade e Segurança Por Trás do Ecrã</a><br>
2.3 <a href="#item02.03">Gateway para uma rede segura: Estratégias-chave para manter a segurança e a eficiência</a><br>
2.4 <a href="#item02.04">Dicas para resolução de problemas</a><br>

---

### Objective:
O objetivo do módulo foi ensinar práticas essenciais de segurança digital e proteção de dispositivos, abordando a gestão de palavras-passe, autenticação de dois fatores, segurança em redes Wi-Fi, proteção contra a vigilância e os riscos associados à dark web e violações de dados.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, descrevendo todo conteúdo realizado neste módulo.
- [0-aux](../0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item02.01"><h4>2.1 Um guia abrangente para proteger a sua vida digital</h4></a>[Back to summary](#item02)

🛡️ Diretrizes Globais de Proteção e Gestão de Credenciais   
A segurança do ecossistema computacional baseia-se na implementação de controles defensivos nos ativos e na administração rigorosa de identidades.
- Hardening de Dispositivos: Instalação e execução contínua de soluções antivírus, antimalware e firewalls para mitigar a exploração de vulnerabilidades.
- Gestão de Atualizações (Patch Management): Aplicação sistemática de atualizações de sistemas operacionais e softwares para correção de falhas de segurança conhecidas.
- Política de Senhas e Cofres Virtuais: Adoção de credenciais únicas e complexas por serviço, utilizando gerenciadores de senhas para mitigar os riscos de comprometimento em cascata decorrentes do reuso de segredos.
- Autenticação Multi-fator (MFA): Exigência de segundo fator de validação (OTP, biometria ou tokens físicos) para barrar acessos indevidos resultantes de vazamentos de senhas.

💻 Arquitetura de Segurança: Desktops vs. Dispositivos Móveis   
Diferentes categorias de dispositivos exigem estratégias de proteção adaptadas às suas especificidades arquiteturais e modelos de ameaça:

🖥️ Computadores Desktop e Laptops   
- Mecanismos Principais: Varreduras ativas de softwares antivírus e controle de tráfego de rede via firewalls locais.
- Mitigação de Riscos: Atualização automatizada de softwares do sistema e restrição ao uso de contas com privilégios administrativos.

📱 Dispositivos Móveis (Smartphones e Tablets)   
- Mecanismos Principais: Controle de execução via sandboxing nativo do sistema operacional (iOS/Android) e verificação de integridade de aplicações nas lojas oficiais.
- Ameaças Específicas: Risco elevado de furto físico e sequestro de linha (SIM Swap), exigindo o uso de bloqueios biométricos, cifragem de armazenamento e capacidade de localização/limpeza remota (Remote Wipe).

⚙️ Procedimentos Operacionais no Windows Security   
Abaixo constam as sequências operacionais padronizadas para alteração de credenciais locais e varredura de integridade do sistema.

🔑 Alteração de Código PIN (Windows Hello)   
- Acessar o menu Configurações através do atalho ou do painel de navegação.
- Navegar até a seção Contas e selecionar Opções de Início de Sessão.
- Selecionar o item PIN (Windows Hello) e acionar a opção Alterar PIN.
- Inserir o código de verificação atual e especificar a nova combinação numérica.
- Confirmar a alteração clicando em OK.

🔍 Execução de Verificação Completa do Sistema   
- Abrir as Configurações do sistema e acessar Atualização e Segurança.
- Selecionar Segurança do Windows e entrar em Proteção contra vírus e ameaças.
- Clicar em Opções de verificação, selecionar a modalidade Verificação completa.
- Iniciar o procedimento acionando o botão Verificar agora.

🌐 Segurança em Redes Sem Fio e Ambientes Públicos   
A transmissão segura de dados exige a cifragem do canal de comunicação e a mitigação de interceptações em infraestruturas não confiáveis.
- Cifragem de Redes Sem Fio: Adoção obrigatória dos padrões WPA2 ou WPA3, descontinuando protocolos vulneráveis como WEP.
- Hardening de Roteadores Domésticos: Substituição das senhas padrão de fábrica, atualização frequente do firmware, desativação da gerência remota e segregação de tráfego de visitantes via Guest Network.
- Mitigação em Redes Públicas e Pontos de Acesso: Uso de Redes Virtuais Privadas (VPN) para criptografar todo o tráfego, além do bloqueio ao compartilhamento de arquivos e validação do protocolo HTTPS.
- Riscos em Terminais Públicos: Abstenção de autenticação em serviços críticos nesses equipamentos devido à presença potencial de keyloggers e softwares espiões.

<a name="item02.02"><h4>2.2 Fundamentos de Privacidade e Segurança Por Trás do Ecrã</h4></a>[Back to summary](#item02)

👁️ Vigilância Digital e Mecanismos de Privacidade   
A ampliação do monitoramento por entes estatais e corporativos transforma os rastros de navegação em ativos de controle e precificação, exigindo estratégias de ocultação e cifragem.

🏢 Monitoramento Corporativo vs. Estatal   
- Coleta Corporativa: Compilação continuada de histórico de buscas, geolocalização e padrões de consumo para criação de perfis comportamentais, direcionamento publicitário e comercialização com terceiros.
- Vigilância Estatal: Interceptação de fluxos de dados para segurança pública, prevenção de ilícitos e controle populacional, com risco potencial de repressão política e limitação do ativismo.

🛡️ Ferramentas de Mitigação de Rastreio   
- Comunicação Cifrada: Aplicação de criptografia de ponta a ponta (E2EE) para assegurar que apenas os interlocutores autorizados acessem o conteúdo transmitido.
- Redes Virtuais Privadas (VPN): Ocultação do endereço IP de origem e tunelamento criptografado do tráfego de rede para mitigar a análise de tráfego por provedores e terceiros.
- Efeito Inibidor (Chilling Effect): Redução do risco de autocensura e limitação da liberdade de expressão provocadas pela sensação de monitoramento ostensivo.

🕸️ Mitos, Riscos e dinâmicas da Dark Web   
Apesar da percepção de distanciamento, os mercados cibernéticos subterrâneos afetam diretamente usuários que não navegam nessas redes.
- Exposição por Vazamento de Dados: Dados exfiltrados de corporações em incidentes de segurança (credenciais, documentos, cartões de crédito) são comercializados em fóruns restritos da Dark Web, viabilizando roubo de identidade e fraudes financeiras.
- Vetores de Comprometimento via Pirataria: O consumo de conteúdo não licenciado e a interação com anúncios maliciosos (malvertising) servem de ponte para a execução de malwares e redirecionamentos não autorizados.

🔒 Ações Preventivas de Cidadania Digital   
A resposta às ameaças de vigilância e ao comércio ilícito de dados exige a adoção sistemática de hábitos de segurança defensiva:
- Gestão de Segredos: Implementação de credenciais exclusivas de alta complexidade com suporte de cofres de senhas.
- Autenticação de Dois Fatores (2FA): Inclusão de camada secundária de verificação para conter o uso de senhas expostas em vazamentos.
- Monitoramento de Contas e Crédito: Acompanhamento periódico de extratos e relatórios financeiros para identificação precoce de movimentações atípicas.
- Revisão de Permissões: Configuração restritiva de privacidade em plataformas online, limitando a exposição pública de dados identificáveis.

<a name="item02.03"><h4>2.3 Gateway para uma rede segura: Estratégias-chave para manter a segurança e a eficiência</h4></a>[Back to summary](#item02)

🌐 Atualização de Firmware em Roteadores Residenciais   
A manutenção do software embarcado (firmware) dos roteadores é fundamental para corrigir vulnerabilidades de segurança, otimizar a estabilidade do tráfego de rede e implementar novos recursos operacionais na infraestrutura doméstica.

📋 Procedimento Operacional Padrão de Atualização   
A execução do processo de atualização exige uma sequência estruturada para evitar a corrupção do dispositivo (brick):
- Acesso à Interface de Gerenciamento: Conectar ao painel do roteador via navegador digitando o endereço IP do gateway padrão (ex: 192.168.0.1 ou 192.168.1.1) e autenticar com as credenciais administrativas.
- Coleta de Informações do Ativo: Identificar o modelo exato do equipamento e a versão atual do firmware instalada na aba de menu corporativo (como Sistema, Administração ou Manutenção).
- Obtenção do Pacote de Atualização: Acessar o repositório oficial do fabricante, pesquisar pelo modelo do dispositivo e realizar o download da imagem de firmware mais recente, descompactando os arquivos se necessário.
- Instalação do Firmware: Carregar o arquivo de atualização no campo indicado na interface web do roteador e iniciar o processo de gravação na memória flash.
- Validação do Sistema: Aguardar a reinicialização automática do ativo — mantendo o fornecimento de energia ininterrupto durante todo o procedimento — e verificar a nova versão do sistema na interface de gestão.

<a name="item02.04"><h4>2.4 Dicas para resolução de problemas</h4></a>[Back to summary](#item02)

🛠️ Resolução de Incidentes e Mitigação de Riscos Operacionais   
A adoção de procedimentos preventivos e de resposta rápida reduz a exposição de dados sensíveis em cenários de risco iminente.

📱 Perda ou Furto de Dispositivo Móvel   
A perda de ativos com dados corporativos ou pessoais exige o uso imediato de ferramentas de localização e apaziguamento de danos via limpeza remota (Remote Wipe). Como medida preventiva, deve-se manter rotinas ativas de backup em nuvem e aplicar criptografia completa no armazenamento interno do dispositivo.

☕ Conexão em Redes Wi-Fi Públicas Não Confiáveis   
O acesso à internet em ambientes abertos demanda a inicialização obrigatoriamente intermediada por uma Rede Privada Virtual (VPN), garantindo a cifragem do tráfego de dados. Deve-se evitar a autenticação em serviços financeiros, sistemas corporativos ou manipulação de documentos confidenciais durante a conexão.

🔍 Gestão de Permissões de Aplicações   
O gerenciamento de riscos em softwares exige a revisão criteriosa das concessões de acesso requeridas por aplicativos (como contatos, câmera e geolocalização). Acesso a recursos não essenciais ao funcionamento da aplicação deve ser sumariamente recusado, avaliando-se a reputação do desenvolvedor antes da utilização.
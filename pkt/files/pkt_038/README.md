# Packet Tracer – Implementando um Esquema de Endereçamento IPv6 com Sub-Redes   <img src="./0-aux/logo_course.png" alt="pkt_038" width="auto" height="45">

### Cisco: <a href="../../../">cisco   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cisco.png" alt="cisco" width="auto" height="25"></a>
### Cisco Networking Academy: cna   <img src="https://github.com/PedroHeeger/my_tech_journey/blob/main/platforms/img/cna.png" alt="cna" width="auto" height="25"></a>
### Training Category: <a href="../../../pkt/">pkt</a>
### Software/Subject: network   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/content/network.jpg" alt="network" width="auto" height="25"></a>
### Course: <a href="./">pkt_038 (Packet Tracer – Implementando um Esquema de Endereçamento IPv6 com Sub-Redes)   <img src="./0-aux/logo_course.png" alt="pkt_038" width="auto" height="25"></a>

---

### Theme:
- Network

### Used Tools:
- Operating System (OS): 
  - Cisco Internetwork Operating System (Cisco IOS)   <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/cisco_ios.jpg" alt="cisco_ios" width="auto" height="25">
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
- Network:
  - Cisco Packet Tracer <img src="https://github.com/PedroHeeger/main/blob/main/0-aux/logos/software/cisco_packet_tracer.webp" alt="cisco_packet_tracer" width="auto" height="25">
  - ping   <img src="" alt="iputils" width="auto" height="25">

---

<h3><a name="item00">Course Strcuture:</a></h3>

1. <a href="#item01">Packet Tracer – Implementando um Esquema de Endereçamento IPv6 com Sub-Redes</a><br>
  1.1 <a href="#item01.01">Etapa 1: Determinar as Sub-Redes IPv6 e o Esquema de Endereçamento</a><br>
  1.2 <a href="#item01.02">Etapa 2: Configurar o endereçamento IPv6 em roteadores e PCs.</a><br>
  1.3 <a href="#item01.03">Etapa 3: Verificar a conectividade IPv6.</a><br>

---

### Objective:
O objetivo desta atividade consistiu no planejamento e implementação de um esquema de endereçamento IPv6 a partir de um prefixo determinado, visando a segmentação eficiente e a plena conectividade da infraestrutura de rede.

### Folder Structure:
- [README.md](./README.md): Este documento de README, escrito em **Markdown**, com o conteúdo do laboratório.
- [0-aux](./0-aux/): Pasta auxiliar com imagens utilizadas na construção dos arquivos de README desse curso.

### Development:

<a name="item01"><h4>1. Packet Tracer – Implementando um Esquema de Endereçamento IPv6 com Sub-Redes</h4></a>[Back to summary](#item00)

A imagem 01 mostra a topologia inicial.

<div align="center"><figure>
    <img src="./0-aux/img01.png" alt="img01"><br>
    <figcaption>Imagem 01.</figcaption>
</figure></div><br>

<a name="item01.01"><h4>1.1 Etapa 1: Determinar as Sub-Redes IPv6 e o Esquema de Endereçamento</h4></a>[Back to summary](#item00)

Você recebeu a sub-rede IPv6 2001:db8:acad:00c8::/64 como sub-rede inicial. Você precisará de mais quatro sub-redes para cada rede necessária. Incrementar os endereços de sub-rede consecutivamente por um para chegar às quatro sub-redes necessárias. Preencha a tabela abaixo.


<div align="center">

#### Tabela 1 — Planejamento das Sub-redes IPv6

| Nº Sub-rede | Nome da Sub-Rede | Endereço da Sub-Rede | Prefixo |
|:---:|:---:|:---:|:---:|
| 1 | R1 G0/0/ LAN | 2001:db8:acad:00c8:: | /64 |
| 2 | R1 G0/1 LAN | 2001:db8:acad:00c9:: | /64 |
| 3 | R2 G0/0 LAN | 2001:db8:acad:00ca:: | /64 |
| 4 | R2 G0/1 LAN | 2001:db8:acad:00cb:: | /64 |
| 5 | Link R1-R2 LAN | 2001:db8:acad:00cc:: | /64 |

</div>

<a name="item01.02"><h4>1.2 Etapa 2: Configure o endereçamento IPv6 em roteadores e PCs.</h4></a>[Back to summary](#item00)

Preencha a tabela de endereçamento acima para usar como guia para configurar os dispositivos.

- a. Atribua o primeiro endereço IP na sub-rede às interfaces LAN do roteador.
- b. Atribua os endereços de link local conforme designado na tabela de endereçamento.
- c. Para a conexão entre os roteadores, atribua o primeiro endereço na sub-rede a R1.
- d. Para a conexão entre os roteadores, atribua o segundo endereço na sub-rede ao R2.
- e. Defina todos os quatro hosts para configurar automaticamente com endereços IPv6.

<div align="center">

#### Tabela 2 — Planejamento de Endereçamento IPv6

| Dispositivo | Interface | Endereço IP | Endereço Link-Local |
|:---:|:---:|:---:|:---:|
| R1 | G0/0 | 2001:db8:acad:00c8::1/64 | FE80::1 |
| R1 | G0/1 | 2001:db8:acad:00c9::1/64 | FE80::1 |
| R1 | S0/0/0 | 2001:db8:acad:00cc::1/64 | FE80::1 |
| R2 | G0/0 | 2001:db8:acad:00ca::1/64 | FE80::2 |
| R2 | G0/1 | 2001:db8:acad:00cb::1/64 | FE80::2 |
| R2 | S0/0/0 | 2001:db8:acad:00cc::2/64 | FE80::2 |
| S1 | VLAN 1 | 2001:db8:acad:00c8::2/64 | FE80::1 |
| S2 | VLAN 1 | 2001:db8:acad:00c9::2/64 | FE80::1 |
| S3 | VLAN 1 | 2001:db8:acad:00ca::2/64 | FE80::2 |
| S4 | VLAN 1 | 2001:db8:acad:00cb::2/64 | FE80::2 |
| PC1 | NIC | Configuração Automática | FE80::1 |
| PC2 | NIC | Configuração Automática | FE80::1 |
| PC3 | NIC | Configuração Automática | FE80::2 |
| PC4 | NIC | Configuração Automática | FE80::2 |

</div>

- R1-G0/0: `enable` -> `configure terminal` -> `ipv6 unicast-routing` -> `interface g0/0` -> `ipv6 address 2001:db8:acad:00c8::1/64` -> `ipv6 address FE80::1 link-local` -> `no shutdown` -> `exit`.
- R1-G0/1: `interface g0/1` -> `ipv6 address 2001:db8:acad:00c9::1/64` -> `ipv6 address FE80::1 link-local` -> `no shutdown` -> `exit`.
- R1-S0/0/0: `interface s0/0/0` -> `ipv6 address 2001:db8:acad:00cc::1/64` -> `ipv6 address FE80::1 link-local` -> `no shutdown` -> `exit`.
- R2-G0/0: `enable` -> `configure terminal` -> `ipv6 unicast-routing` -> `interface g0/0` -> `ipv6 address 2001:db8:acad:00ca::1/64` -> `ipv6 address FE80::2 link-local` -> `no shutdown` -> `exit`.
- R2-G0/1: `interface g0/1` -> `ipv6 address 2001:db8:acad:00cb::1/64` -> `ipv6 address FE80::2 link-local` -> `no shutdown` -> `exit`.
- R2-S0/0/0: `interface s0/0/0` -> `ipv6 address 2001:db8:acad:00cc::2/64` -> `ipv6 address FE80::2 link-local` -> `no shutdown` -> `exit`.

A imagem 02 exibe as interfaces dos roteadores devidamente configuradas.

<div align="center"><figure>
    <img src="./0-aux/img02.png" alt="img02"><br>
    <figcaption>Imagem 02.</figcaption>
</figure></div><br>

<a name="item01.03"><h4>1.3 Etapa 3: Verificar a conectividade IPv6.</h4></a>[Back to summary](#item00)

Os PCs devem ser capazes de efetuar ping uns aos outros se o endereçamento tiver sido configurado corretamente.

- PC1-PC4: `ping 2001:db8:acad:00cb:02E0:A3FF:FE12:16CB`.
- PC3-PC2: `ping 2001:db8:acad:c9:201:C7FF:FE66:86E9`.
- PC4-R1: `ping 2001:db8:acad:00c8::1`.
- PC2-R2: `ping 2001:db8:acad:00cb::1`.

A imagem 03 evidencia a comunicação entre os dispositivos configurados.

<div align="center"><figure>
    <img src="./0-aux/img03.png" alt="img03"><br>
    <figcaption>Imagem 03.</figcaption>
</figure></div><br>
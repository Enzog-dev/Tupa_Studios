# 🛡️ Tupã Studios — Infraestrutura de TI, Redes e Segurança da Informação

> **Projeto Acadêmico** desenvolvido para as disciplinas de *Sistemas Computacionais e Segurança* e *Ambientes Computacionais e Conectividade* na Universidade São Judas Tadeu.

---

## 📌 Visão Geral

A **Tupã Studios** é um projeto de planejamento de infraestrutura computacional, redes e plano de segurança desenvolvido para um estúdio brasileiro fictício de desenvolvimento de jogos em fase de expansão. 

O trabalho simula o cenário de uma empresa com **210 colaboradores** distribuídos em 4 unidades geograficamente separadas (Matriz São Paulo, Filial SP II, Rio de Janeiro e Recife), exigindo uma solução de TI resiliente, escalável e de alta segurança para proteger ativos de propriedade intelectual (como código-fonte dos jogos).

---

## 🏗️ Arquitetura e Escopo Técnico

O projeto abrange a estruturação completa da tecnologia da informação da empresa:

* **Topologia de Rede Corporativa (WAN/LAN):** Arquitetura centralizada em modelo *Hub-and-Spoke* conectando as filiais à Matriz via VPNs criptografadas, garantindo que as políticas do firewall central sejam aplicadas a toda a organização.
* **Segmentação por VLANs & Endereçamento IP:** Criação de sub-redes lógicas (`10.x.x.x/16`) organizadas por departamento (Desenvolvimento, Servidores, Segurança, Corporativo e Wi-Fi Visitantes) para controle de acesso rigoroso e redução do tráfego de broadcast.
* **Plano de Segurança da Informação (PSI):** Mapeamento e Análise de Vulnerabilidades (Matriz de Riscos por setor), definição de Políticas de Boas Práticas (Autenticação MFA, Senhas, LGPD) e Plano de Contingência para resposta a incidentes.
* **Infraestrutura Cloud vs On-Premises:**
  * **On-Premises:** Dimensionamento de servidores locais (servidores de rede, repositórios de código GitLab, servidores de build/QA e backup).
  * **Cloud:** Estudo comparativo e análise financeira detalhada entre **AWS** e **Google Cloud Platform (GCP)** para hospedagem de servidores de jogos multiplayer e serviços de baixa latência, resultando na escolha estratégica do GCP.
* **Integração de Dispositivos IoT:** Aplicação de IoT para segurança física (controle de acesso inteligente NFC/RFID nas salas de servidores), sensores ambientais (temperatura e umidade) e no-breaks inteligentes (UPS).

---

## 🛠️ Tecnologias e Ferramentas Mapeadas

* **Redes & Segurança:** Fortinet FortiGate, Wireshark, Splunk, Bitdefender GravityZone, VPN, VLAN (Switch L2/L3), Roteamento Inter-VLAN.
* **Sistemas Operacionais & Servidores:** Linux Server (Ubuntu), Windows 10/11 Pro, Android (gestão predial).
* **Nuvem & Serviços:** Google Cloud Platform (Compute Engine, Cloud SQL, Cloud Storage, Cloud Load Balancing, Cloud CDN).
* **Desenvolvimento & Suporte:** GitLab, Jenkins, Docker, Python, Unreal Engine, Blender, Zendesk, SAP.

---

## 📄 Estrutura da Documentação

```text
├── docs/
│   └── Tupa_Studios_Documentacao_Completa.pdf   # Documentação acadêmica detalhada
└── README.md                                    # Apresentação do repositório

# 🛡️ Mini SOC com Wazuh – Laboratório Prático

## 📌 Sobre o projeto
Este projeto consiste na criação de um **Mini Security Operations Center (SOC)** em ambiente de laboratório, utilizando o **Wazuh** como ferramenta central de monitoramento, detecção e análise de eventos de segurança.

O objetivo é **aplicar na prática conceitos de Blue Team**, simular ataques controlados e analisar os alertas gerados, reproduzindo atividades comuns da rotina de um analista SOC.

---

## 🎯 Objetivos
- Compreender o funcionamento de um SOC na prática  
- Instalar e configurar o Wazuh Server e agentes  
- Monitorar sistemas Linux e Windows  
- Simular eventos de segurança e ataques controlados  
- Analisar alertas e dashboards  
- Documentar aprendizados e boas práticas  

---

## 🧱 Ambiente do laboratório
- Hypervisor: VMware  
- Wazuh Server (OVA oficial)  
- Linux (Ubuntu / Kali Linux) com agente Wazuh  
- Windows 10 com agente Wazuh  
- Ambiente totalmente isolado e controlado  

---

## 🛠️ Tecnologias e ferramentas
- Wazuh  
- Linux (Ubuntu / Kali Linux)  
- Windows 10  
- SSH  
- Hydra (para simulações controladas)  
- VMware  

---

## 📂 Estrutura do projeto

```text
01-ambiente
 └── vms.md

02-instalacao-wazuh
 ├── wazuh-server.md
 ├── agent-linux.md
 └── agent-windows.md

03-configuracoes
 ├── grupos-agentes.md
 └── politicas.md

04-simulacoes
 ├── brute-force-linux.md
 ├── autenticacao-windows.md
 └── comandos-utilizados.md

05-monitoramento
 ├── alertas.md
 └── dashboards.md

06-conclusao
 └── aprendizados.md

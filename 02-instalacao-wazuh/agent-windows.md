
---

## 📄 `docs/04-agente-windows.md`

```md
# 04 – Instalação do Agente Wazuh no Windows

## Visão Geral

Nesta etapa foi realizada a **instalação e configuração do agente do Wazuh em um sistema Windows**, possibilitando a coleta de eventos do Event Viewer e o monitoramento de atividades do sistema.

Este passo é essencial para simular o monitoramento de estações ou servidores Windows em um ambiente de SOC.

---

## Sistema Utilizado

- Sistema operacional: Windows 10 ou Windows Server
- Função: Host monitorado (agente)

---

## Download do Agente

O agente foi obtido através do instalador oficial do Wazuh em formato **MSI**.

---

## Instalação via PowerShell

A instalação foi realizada utilizando o **PowerShell com privilégios de administrador**, de forma silenciosa.

```powershell
msiexec.exe /i wazuh-agent-4.x.x-1.msi /q `
WAZUH_MANAGER="<IP_DO_WAZUH_SERVER>" `
WAZUH_REGISTRATION_SERVER="<IP_DO_WAZUH_SERVER>" `
WAZUH_AGENT_NAME="windows-agent"

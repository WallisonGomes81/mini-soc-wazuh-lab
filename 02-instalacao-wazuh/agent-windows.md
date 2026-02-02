# Instalação do Agente Wazuh no Windows

## Objetivo
Descrever o processo de instalação e configuração do **Wazuh Agent em ambiente Windows**, permitindo a coleta de logs de segurança e o monitoramento centralizado pelo Wazuh Server.

---

## Ambiente
- Sistema operacional: Windows 10  
- Wazuh Server: instalado via OVA oficial  
- Comunicação: agente → servidor Wazuh  
- Finalidade: laboratório educacional (Mini SOC)

---

## Pré-requisitos
- Windows atualizado
- Conectividade de rede entre o Windows e o Wazuh Server
- Endereço IP do Wazuh Manager
- Permissões administrativas no sistema

---

## Método de instalação
A instalação do agente foi realizada utilizando o **instalador oficial MSI do Wazuh**, executado via linha de comando para facilitar a configuração inicial.

---

## Procedimento de instalação

### 1. Download do agente
O instalador do Wazuh Agent para Windows foi obtido no site oficial do Wazuh.

---

### 2. Instalação via PowerShell
A instalação foi realizada utilizando o seguinte comando:

```powershell
msiexec.exe /i wazuh-agent.msi /q `
WAZUH_MANAGER="IP_DO_WAZUH_SERVER" `
WAZUH_REGISTRATION_SERVER="IP_DO_WAZUH_SERVER" `
WAZUH_AGENT_GROUP="windows" `
WAZUH_AGENT_NAME="windows-agent"

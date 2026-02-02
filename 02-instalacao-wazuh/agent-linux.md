# 03 – Instalação do Agente Wazuh no Linux

## Visão Geral

Nesta etapa foi realizada a **instalação e configuração do agente do Wazuh em um sistema Linux**, permitindo a coleta e o envio de logs para o Wazuh Server.

O objetivo é monitorar eventos do sistema operacional, autenticações e possíveis atividades suspeitas, simulando o funcionamento de um host Linux monitorado por um SOC.

---

## Sistema Utilizado

- Sistema operacional: Ubuntu Linux ou Kali Linux
- Função: Host monitorado (agente)

---

## Download e Instalação do Agente

O agente foi instalado utilizando o pacote oficial disponibilizado pelo Wazuh.

```bash
curl -sO https://packages.wazuh.com/4.x/wazuh-agent_4.x.x-1_amd64.deb
sudo WAZUH_MANAGER="<IP_DO_WAZUH_SERVER>" dpkg -i wazuh-agent_4.x.x-1_amd64.deb

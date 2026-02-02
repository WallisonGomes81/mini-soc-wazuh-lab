# Grupos de Agentes no Wazuh

## Objetivo
Organizar os agentes do Wazuh de acordo com o sistema operacional,
permitindo aplicar configurações e políticas específicas para cada tipo
de host monitorado.

## Grupos criados

### Grupo: linux
Utilizado para agrupar servidores e máquinas Linux monitoradas pelo Wazuh.

Exemplos de agentes:
- Ubuntu Server
- Kali Linux

Finalidade:
- Monitoramento de autenticação SSH
- Detecção de força bruta
- Coleta de logs do sistema (/var/log/auth.log)

---

### Grupo: windows
Utilizado para agrupar máquinas Windows monitoradas pelo Wazuh.

Exemplos de agentes:
- Windows 10

Finalidade:
- Monitoramento de eventos de logon
- Criação e alteração de usuários
- Eventos de segurança do Windows Event Log

## Benefícios da separação por grupos
- Aplicação de políticas específicas por sistema operacional
- Melhor organização do ambiente
- Facilidade de expansão do laboratório

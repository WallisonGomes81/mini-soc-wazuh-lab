# Políticas de Monitoramento e Segurança

## Objetivo
Definir políticas básicas de monitoramento e detecção de eventos de
segurança, simulando práticas utilizadas em um SOC.

## Políticas aplicadas

### Autenticação e acesso
- Monitoramento de falhas de autenticação
- Detecção de múltiplas tentativas de login inválidas
- Identificação de logins bem-sucedidos fora do padrão

Sistemas monitorados:
- Linux (SSH)
- Windows (Logon Events)

---

### Integridade de arquivos (FIM)
Monitoramento de alterações em arquivos sensíveis do sistema.

Exemplos:
- Arquivos de configuração do sistema
- Diretórios críticos

Finalidade:
- Identificar alterações não autorizadas
- Detectar possíveis comprometimentos

---

### Execução de comandos e processos
Monitoramento de comandos executados no sistema.

Finalidade:
- Identificar comportamentos suspeitos
- Analisar possíveis ações pós-exploração

---

### Níveis de severidade
Os alertas são classificados de acordo com o impacto do evento:

- Baixo: eventos informativos
- Médio: comportamentos suspeitos
- Alto: possíveis incidentes de segurança

## Observações
As políticas aplicadas seguem as configurações padrão do Wazuh,
com foco em aprendizado e simulação de um ambiente SOC.

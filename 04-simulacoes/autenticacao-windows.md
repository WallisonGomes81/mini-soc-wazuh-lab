# Simulação de Eventos de Autenticação no Windows

## Objetivo
Simular eventos de autenticação no Windows para validar a coleta e análise
de logs de segurança pelo Wazuh.

## Ambiente
- Máquina: Windows 10
- Agente Wazuh instalado e ativo
- Fonte de logs: Windows Event Log

## Procedimento

### 1. Tentativas de login inválidas
Foram realizadas múltiplas tentativas de login com usuário ou senha inválidos.

### 2. Login bem-sucedido
Realização de login válido para comparação de eventos.

### 3. Criação de usuário local
Criação de um novo usuário local para geração de eventos administrativos.

## Resultados observados no Wazuh
- Detecção de falhas de logon
- Identificação de eventos de criação de usuário
- Classificação adequada dos eventos de segurança

## Evidências
- Prints dos eventos no Windows
- Prints dos alertas no Wazuh Dashboard

## Conclusão
Os testes confirmaram que o Wazuh realiza a coleta e correlação de eventos
de autenticação no Windows, permitindo visibilidade sobre atividades
suspeitas ou administrativas.

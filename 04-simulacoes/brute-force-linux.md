# Simulação de Força Bruta SSH no Linux

## Objetivo
Simular um ataque de força bruta via SSH em uma máquina Linux monitorada
pelo Wazuh, com o objetivo de validar a detecção de múltiplas tentativas
de autenticação inválidas.

## Ambiente
- Máquina alvo: Ubuntu Server (agente Wazuh instalado)
- Máquina atacante: Kali Linux
- Serviço atacado: SSH (porta 22)

## Ferramenta utilizada
- hydra

## Procedimento

### 1. Validação do serviço SSH
Verificar se o serviço SSH está ativo na máquina alvo.

### 2. Execução do ataque de força bruta
O ataque foi realizado a partir da máquina Kali Linux utilizando o Hydra,
simulando tentativas repetidas de autenticação com credenciais inválidas.

### 3. Interrupção do ataque
O ataque foi interrompido manualmente após a geração de eventos suficientes
para análise.

## Resultados observados no Wazuh
- Geração de múltiplos alertas de falha de autenticação
- Identificação de possível ataque de força bruta
- Classificação dos alertas com severidade média/alta

## Evidências
- Prints do terminal com a execução do ataque
- Prints do dashboard do Wazuh exibindo os alertas

## Conclusão
A simulação demonstrou que o Wazuh é capaz de detectar tentativas de força
bruta em serviços SSH, auxiliando na identificação de possíveis ataques
de acesso não autorizado.

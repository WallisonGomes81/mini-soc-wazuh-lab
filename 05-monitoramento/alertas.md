# Análise de Alertas de Segurança

## Objetivo
Analisar os alertas gerados pelo Wazuh após as simulações de eventos
de segurança, avaliando severidade, contexto e impacto.

## Tipos de alertas observados

### Falhas de autenticação (Linux)
- Múltiplas tentativas de login SSH inválidas
- Identificação de possível ataque de força bruta
- Origem do evento: endereço IP externo

Severidade:
- Média a alta

---

### Falhas de autenticação (Windows)
- Eventos de logon inválido
- Tentativas repetidas com credenciais incorretas

Severidade:
- Média

---

### Atividades

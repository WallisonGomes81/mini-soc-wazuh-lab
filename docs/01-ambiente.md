01 – Ambiente do Laboratório (Mini SOC com Wazuh)

Visão Geral



Este laboratório foi criado com o objetivo de estudar e praticar o uso do Wazuh como SIEM, simulando um Mini SOC (Security Operations Center) em ambiente controlado.

O foco do projeto é aprendizado prático, documentação do processo e compreensão do fluxo de monitoramento, detecção e análise de eventos de segurança.



Todo o ambiente foi construído com ferramentas open source e máquinas virtuais, permitindo a reprodução do laboratório por outros estudantes.



Objetivo do Laboratório



Entender o funcionamento do Wazuh como SIEM



Simular um ambiente básico de SOC



Coletar e analisar logs de sistemas Linux e Windows



Gerar eventos de segurança para validação das detecções



Documentar o processo como parte de um portfólio de estudos em segurança da informação



Topologia do Ambiente



O laboratório é composto pelos seguintes elementos:



\[Kali Linux]  --->  \[Wazuh Server]  <---  \[Windows]

&nbsp;  (ataques)        (SIEM/SOC)           (agente)

&nbsp;                        ^

&nbsp;                        |

&nbsp;                   \[Ubuntu / Kali]

&nbsp;                     (agente)



Componentes do Ambiente

Wazuh Server



Função: Central de monitoramento e correlação de eventos



Componentes:



Wazuh Manager



OpenSearch



Wazuh Dashboard



Responsável por receber, processar e exibir os logs dos agentes



Agente Linux



Sistema operacional: Ubuntu ou Kali Linux



Função:



Envio de logs do sistema



Monitoramento de autenticação



Detecção de atividades suspeitas



Uso no laboratório:



Simulação de ataques de força bruta



Alterações em arquivos críticos



Eventos de login e erro



Agente Windows



Sistema operacional: Windows 10 ou Windows Server



Função:



Coleta de logs do Event Viewer



Monitoramento de autenticação e processos



Uso no laboratório:



Tentativas de login inválidas



Criação e remoção de usuários



Execução de processos suspeitos



Máquina Atacante



Sistema operacional: Kali Linux



Função:



Simular atividades maliciosas de forma controlada



Exemplos de testes:



Força bruta via SSH



Tentativas de login inválidas



Geração de eventos para análise no SOC



Ferramentas Utilizadas



Wazuh – SIEM / Plataforma de Segurança



Kali Linux – Simulação de ataques



Ubuntu Linux – Sistema monitorado



Windows – Sistema monitorado



VirtualBox ou VMware – Virtualização



Git \& GitHub – Versionamento e documentação



Escopo do Projeto



Este projeto não tem foco ofensivo, mas sim:



Monitoramento



Detecção



Análise



Documentação de eventos de segurança



Todas as atividades são realizadas em ambiente de laboratório, sem impacto em sistemas reais.



Observações



O ambiente pode ser adaptado conforme recursos disponíveis



As simulações são básicas, com foco didático



O projeto representa um Mini SOC, não um ambiente corporativo completo


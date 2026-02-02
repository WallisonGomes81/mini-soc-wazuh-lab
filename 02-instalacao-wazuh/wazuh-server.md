# 02 – Instalação do Wazuh Server (OVA – VMware)

## Visão Geral

Nesta etapa foi realizada a implantação do **Wazuh Server utilizando a imagem OVA oficial**, importada no **VMware**, com o objetivo de criar rapidamente um ambiente funcional para estudos.

O uso da OVA permite focar no aprendizado prático da ferramenta, na análise de eventos e na simulação de um Mini SOC, sem a necessidade de instalação manual de todos os componentes.

A imagem já inclui o **Wazuh Manager**, **OpenSearch** e **Wazuh Dashboard** em modo **all-in-one**.

---

## Método de Implantação

- Tipo de instalação: Imagem **OVA oficial do Wazuh**
- Hypervisor: **VMware**
- Arquitetura: **All-in-one**
- Finalidade: Laboratório e aprendizado

Este método é recomendado para ambientes de testes e estudos, pois reduz a complexidade inicial de configuração.

---

## Importação da OVA no VMware

A implantação foi realizada através da opção **Import Virtual Appliance** no VMware.

Etapas executadas:
1. Seleção do arquivo OVA do Wazuh
2. Definição do nome da máquina virtual
3. Ajuste de recursos (CPU, memória e disco)
4. Finalização da importação e inicialização da VM


---

## Inicialização do Wazuh Server

Após o boot da máquina virtual:
- O sistema operacional foi carregado corretamente
- Os serviços do Wazuh foram iniciados automaticamente

A imagem OVA já vem pré-configurada, não sendo necessária instalação manual dos serviços.


---

## Credenciais de Acesso

As credenciais padrão de acesso ao Wazuh Dashboard são fornecidas pela própria imagem OVA e podem ser visualizadas:
- No console da máquina virtual
- Ou na documentação oficial

⚠️ As credenciais foram armazenadas de forma segura e **não são expostas publicamente**.


---

## Acesso ao Wazuh Dashboard

O acesso ao Dashboard foi realizado via navegador utilizando o endereço:


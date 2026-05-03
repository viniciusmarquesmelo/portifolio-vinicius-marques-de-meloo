# 🔍 Projeto de Algoritmos Aplicados: Auditoria, Saúde e Automação Comercial

![Python](https://img.shields.io/badge/python-3.10+-blue.svg)
![Status](https://img.shields.io/badge/status-concluído-brightgreen.svg)

Este repositório contém o desenvolvimento de algoritmos lógicos aplicados a domínios críticos: **Auditoria de Dados Financeiros**, **Triagem de Risco Clínico** e **Sistemas de Automação de Caixa**. O projeto explora a automação de decisões baseada em parâmetros técnicos, tratamento de anomalias (*outliers*) e segurança da informação.

---

## 📊 1. Algoritmo de Auditoria de Dados (Python)
Módulo focado na verificação de integridade e detecção de erros em relatórios de vendas.

### 🧠 Conceitos Implementados
* **Outliers:** Identificação de valores que aumentam a média drasticamente por serem "pontos fora da curva" em relação ao padrão do conjunto.
* **Normalização:** Remoção de valores discrepantes para obter um resultado fiel da média, evitando que dados extremos mascarem a realidade.
* **Materialidade:** Definição do valor máximo de distorção que um auditor aceita sem comprometer a confiança da conclusão do trabalho.

### ⚙️ Lógica de Execução
O sistema calcula a média de transações e aplica uma regra de validação:
- Se uma venda for superior a **5x a média**, o sistema entra em estado de **REVISÃO MANUAL**.
- Se o auditor confirmar a legitimidade, o **Limite de Segurança** é atualizado dinamicamente.

---

## 🏥 2. Sistema de Triagem Clínica
Baseado em fluxogramas lógicos para priorização de atendimento médico com base em sinais vitais e sintomas.

### 🌡️ Critérios de Classificação
| Nível de Risco | Sinais Vitais / Sintomas | Conduta |
| :--- | :--- | :--- |
| **Emergência** | Temp > 39°C, FC > 120, Falta de ar ou Convulsão | Atendimento Imediato |
| **Urgência** | Temp >= 37.5°C, Vómitos ou Dores Fortes | Prioridade na Fila |
| **Comum** | Sinais estáveis e sintomas leves | Atendimento Padrão |

### 🛡️ Resiliência e Segurança
* **Desafio Logístico:** O maior obstáculo é transformar nuances clínicas subjetivas em regras rígidas de "Sim/Não".
* **Redundância (Fallback):** Caso um sensor falhe, o sistema deve acionar automaticamente um alerta de intervenção humana para garantir a segurança do paciente.

---

## 🛒 3. Automação de Caixa e Troco
Algoritmo para registro de produtos, cálculo de totais e decomposição eficiente de troco.

* **Módulo de Registro:** Loop interativo para entrada de nomes e preços de produtos.
* **Validação de Pagamento:** Verifica se o valor pago é suficiente antes de finalizar a compra.
* **Decomposição de Notas:** Calcula a quantidade mínima de cédulas físicas (R$ 100, 50, 20, 10, 5, 2 e 1) necessárias para o troco.

---

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Python 3.10
* **Ambiente:** Jupyter Notebook / Google Colab
* **Conceitos:** Lógica booleana, estruturas de repetição e tratamento de tipos de dados (`float`, `int`, `string`).

---

## 🔧 Como Utilizar
1. Clone o repositório.
2. Execute o ficheiro `Projeto-algoritmo-de-auditoria-de -dados.ipynb` para testar o sistema de auditoria.
3. Consulte os fluxogramas na documentação para visualizar as regras de negócio da triagem e automação de caixa.

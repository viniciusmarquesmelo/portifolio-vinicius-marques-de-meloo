# 🔍 Projeto: Algoritmos de Auditoria e Triagem Inteligente

![Python](https://img.shields.io/badge/python-3.10+-blue.svg)
![Status](https://img.shields.io/badge/status-concluído-brightgreen.svg)

Este repositório contém o desenvolvimento de algoritmos lógicos aplicados a dois domínios críticos: **Auditoria de Dados Financeiros** e **Triagem de Risco Clínico**. O foco do projeto é a identificação de anomalias (*outliers*) e a automação de tomada de decisão baseada em parâmetros técnicos e segurança de dados.

---

## 📊 1. Algoritmo de Auditoria de Dados

Este módulo automatiza a verificação de integridade em relatórios de vendas, utilizando conceitos estatísticos para identificar possíveis fraudes ou erros de lançamento.

### 🧠 Conceitos Implementados
* **Identificação de Outliers:** Deteção de valores que divergem drasticamente da média aritmética (pontos fora da curva), prevenindo distorções em relatórios financeiros.
* **Normalização:** Processo de ajustar os dados para refletir a realidade operacional, tratando discrepâncias que podem mascarar a performance real.
* **Limite de Materialidade:** Definição técnica da tolerância de erro aceitável antes de comprometer a confiança do auditor em todo o relatório.

### ⚙️ Lógica de Execução
O sistema calcula a média de transações e aplica uma regra de validação rigorosa:
- Se uma venda for superior a **5x a média calculada**, o sistema entra em estado de **REVISÃO MANUAL**.
- O auditor valida a legitimidade; se confirmada, o **Limite de Segurança** é atualizado dinamicamente pelo algoritmo.

---

## 🏥 2. Sistema de Triagem Clínica

Baseado em protocolos de classificação de risco, este módulo utiliza fluxogramas lógicos para priorizar atendimentos médicos com base em sinais vitais e sintomas.

### 🌡️ Critérios de Classificação
| Categoria | Sinais Vitais / Sintomas | Conduta |
| :--- | :--- | :--- |
| **Emergência** | Temp > 39°C, FC > 120, Falta de ar ou Convulsão | Atendimento Imediato |
| **Urgência** | Temp >= 37.5°C, Vómitos ou Dores Fortes | Prioridade na Fila |
| **Comum** | Sinais estáveis e sintomas leves | Atendimento Padrão |

*(Baseado na lógica de decisão clínica estruturada no fluxograma do projeto)*

---

## 🛡️ Segurança, Resiliência e Desafios
O projeto analisa pontos críticos de falha em sistemas automatizados:
1.  **Desafio Logístico:** A dificuldade em transformar nuances clínicas subjetivas em regras rígidas de "Sim/Não" (binário).
2.  **Validação de Dados:** Proteção contra dados corrompidos ou inserções inválidas que comprometam a média ou a triagem.
3.  **Redundância e Fallback (Plano B):** Protocolos para falhas em sensores clínicos ou erros humanos; o sistema deve acionar automaticamente alertas para intervenção humana imediata para garantir a segurança do paciente.
4.  **Integridade:** A falta de auditoria robusta pode levar a fraudes, inconsistências e falhas graves de segurança.

---

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Python 3.10
* **Ambiente:** Jupyter Notebook / Google Colab
* **Metodologia:** Análise estatística, lógica booleana e fluxogramas de decisão.

---

## 🔧 Como Utilizar
1. Clone o repositório.
2. Abra o ficheiro `Projeto-algoritmo-de-auditoria-de -dados.ipynb` no ambiente Jupyter ou Google Colab.
3. Execute as células sequencialmente para testar a lógica de auditoria através da consola de inputs.

---
*Este projeto foi desenvolvido como parte de um estudo prático sobre lógica de programação aplicada à auditoria e saúde.*

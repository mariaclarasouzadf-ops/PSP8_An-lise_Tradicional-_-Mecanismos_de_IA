# PSP8_An-lise_Tradicional-_-Mecanismos_de_IA
# Análise Comparativa: Estatística Tradicional vs. Modelos Inteligentes

Este projeto investiga empiricamente as diferenças de acurácia e capacidade analítica entre métodos descritivos convencionais e modelos de Machine Learning supervisionados.

## 1. Contexto e Dataset
* **Fonte:** Telco Customer Churn Dataset (Kaggle / IBM Public Dataset)
* **Amostra:** Mais de 7.000 registros com atributos contratuais, financeiros e comportamentais de clientes.
* **Objetivo de Previsão:** Identificar risco de cancelamento (Churn) e comparar com o baseline estático.

## 2. Metodologia do Experimento
O experimento foi organizado em pares comparativos:

* **Abordagem Tradicional:** Utilização de medidas de tendência central, correlações isoladas e segmentação univariada (ex.: churn isolado por tipo de contrato).
* **Mecanismo de Inteligência:** Treinamento de um classificador Random Forest multivariado com validação estratificada (75% treino / 25% teste).

## 3. Resultados Obtidos
A comparação por pares revelou os seguintes indicadores:

| Métrica Avaliada | Baseline Tradicional | Modelo de Inteligência (RF) | Variação |
| :--- | :--- | :--- | :--- |
| **Acurácia Geral** | ~73.4% (regra estática) | ~80.2% | +6.8 p.p. |
| **Poder de Discriminação** | Inexistente (global) | 0.842 (ROC-AUC) | Identificação individual de risco |
| **Visão de Drivers** | Fatores isolados | Importância multivariada | Pondera mensalidade, tempo de casa e contrato |

## 4. Conclusão
A abordagem tradicional oferece leitura adequada do panorama histórico, mas é insuficiente para antecipar comportamentos heterogêneos. O uso do mecanismo preditivo permitiu capturar padrões não-lineares, oferecendo diagnósticos individualizados superiores às análises descritivas usuais.

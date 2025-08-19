# Análise Preditiva de Evasão de Clientes - Telecom-X (Parte 2)

Este repositório documenta a segunda etapa do desafio de dados **"Telecom-X" da Alura**, com foco em **Análise Preditiva**. O objetivo principal foi utilizar a base de dados tratada na primeira fase para construir, avaliar e interpretar modelos de Machine Learning para prever a evasão de clientes (Churn).

## 🚀 **Visão Geral do Projeto**

A empresa fictícia Telecom-X enfrenta um problema de alta rotatividade de clientes. Para combater a evasão, o desafio consistiu em:

-   **Construir modelos preditivos:** Desenvolver modelos de Machine Learning para prever quais clientes têm maior probabilidade de evadir.
-   **Avaliar o desempenho:** Utilizar métricas como Acurácia, Precisão, Recall, F1-Score e Matriz de Confusão para comparar o desempenho dos modelos.
-   **Interpretar os resultados:** Identificar as variáveis mais relevantes que influenciam a decisão de evasão e propor estratégias de negócio baseadas nessas descobertas.

## 🛠️ **Metodologia**

O projeto foi desenvolvido em Python, utilizando bibliotecas como **pandas** para manipulação de dados e **scikit-learn** para a modelagem. A metodologia seguiu os seguintes passos:

1.  **Preparação dos Dados:** A base de dados, já limpa e tratada, foi dividida em conjuntos de treino e teste.

2.  **Criação dos Modelos:** Foram construídos dois modelos com diferentes abordagens:
    -   **Regressão Logística:** Um modelo linear que exige a normalização dos dados para uma performance ideal.
    -   **Árvore de Decisão:** Um modelo de árvore que não é afetado pela escala dos dados e, portanto, não requer normalização.

3.  **Avaliação dos Modelos:** Ambos os modelos foram avaliados no conjunto de teste, revelando que a **Regressão Logística** teve um desempenho superior e mais estável. A **Árvore de Decisão**, por sua vez, demonstrou sinais de **overfitting**.

4.  **Análise de Variáveis:** As variáveis mais importantes para a previsão de Churn foram identificadas através dos **coeficientes da Regressão Logística** e da **importância das features da Árvore de Decisão**.

## 📊 **Resultados e Conclusão**

A análise dos modelos e das variáveis revelou insights valiosos sobre a evasão de clientes:

-   **Fatores Chave de Evasão:** Os modelos identificaram consistentemente o **tempo de contrato**, o **tipo de contrato** e o **serviço de internet (Fibra Óptica)** como os fatores de maior impacto na decisão de evasão.
-   **Modelo Vencedor:** O modelo de **Regressão Logística** não apenas previu a evasão com mais precisão, mas também forneceu uma visão clara e interpretável sobre a contribuição de cada variável.

## 📈 **Estratégias de Retenção Propostas**

Com base nos resultados, as seguintes ações estratégicas são recomendadas para a Telecom-X:

-   **Incentivar a Fidelização:** Focar na migração de clientes de contratos mensais para planos de longo prazo (anuais ou bienais) através de incentivos e benefícios.
-   **Melhorar a Qualidade da Fibra Óptica:** Investigar e resolver os problemas associados a este serviço, que está fortemente correlacionado com a evasão de clientes.
-   **Monitorar Clientes de Alto Valor:** Criar um sistema para identificar clientes com alto **`Faturamento_Total`** e oferecer atendimento proativo e personalizado para garantir sua satisfação e lealdade.

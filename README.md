# Teste de Performance 1: Previsão de Doenças Cardíacas com KNN

Este repositório contém o primeiro Teste de Performance (TP) do bloco de Machine Learning, focado na construção de um modelo de classificação para prever a presença de doenças cardíacas.

### Objetivo

O projeto visa aplicar conceitos fundamentais de Machine Learning para resolver um problema de classificação binária, utilizando dados clínicos reais para prever se um paciente possui ou não uma doença cardíaca.

### Base de Dados

O dataset utilizado é o **"UCI Heart Disease Dataset"**, um dos mais conhecidos para tarefas de classificação. 
* **Contexto:** Ele contém 303 amostras e 13 atributos clínicos de pacientes, como idade, sexo, pressão arterial, níveis de colesterol, etc.
* **Alvo (Target):** A variável alvo indica a presença (1) ou ausência (0) de doença cardíaca.
* **Fonte:** O dataset pode ser encontrado em plataformas como o [Kaggle](https://www.kaggle.com/datasets/redwankarimsony/heart-disease-data).

### Etapas do Projeto

O desenvolvimento do modelo seguiu um pipeline clássico de Machine Learning:

1.  **Análise Exploratória e Pré-processamento de Dados:**
    * Carregamento e inspeção inicial do dataset para entender a estrutura e as características dos dados.
    * Divisão dos dados em conjuntos de **treino (80%)** e **teste (20%)**.
    * Padronização das features numéricas com o `StandardScaler` do Scikit-Learn para que todas tivessem a mesma escala, um requisito importante para o algoritmo KNN.

2.  **Treinamento e Otimização do Modelo KNN:**
    * Implementação do algoritmo **K-Nearest Neighbors (KNN)**, um modelo baseado em instância que classifica novos dados com base na similaridade com seus vizinhos.
    * Realização de um **ajuste de hiperparâmetros** para encontrar o valor ideal de **K** (o número de vizinhos). Foram testados múltiplos valores de K para identificar aquele que resultava na maior acurácia no conjunto de teste.

3.  **Avaliação de Performance:**
    * O desempenho do modelo final (com o K otimizado) foi avaliado no conjunto de teste, que o modelo nunca havia visto antes.
    * A principal métrica utilizada para a avaliação foi a **acurácia (accuracy)**, que mede a proporção de previsões corretas.

4.  **Conclusão e Resultados:**
    * O modelo KNN, após a otimização, demonstrou ser uma ferramenta eficaz para a tarefa de classificação, alcançando uma acurácia de **94.57%** no conjunto de teste.
    * O projeto serviu como uma excelente introdução prática ao fluxo de trabalho de um projeto de classificação, desde a preparação dos dados até a avaliação final do modelo.

# Projeto: Análise e Modelagem de Dados de Crédito e Censo com Machine Learning

# Análise e Modelagem de Dados de Crédito e Censo

Este projeto utiliza técnicas de análise e modelagem de dados para explorar duas bases de dados distintas: uma de crédito e outra do censo. O objetivo é preprocessar os dados, aplicar técnicas de visualização e preparar os dados para futuros modelos de machine learning.

## Estrutura do Projeto

1. **Exploração e Limpeza dos Dados de Crédito:**
   - Carregamento dos dados
   - Tratamento de valores inconsistentes
   - Tratamento de valores faltantes

2. **Exploração e Limpeza dos Dados do Censo:**
   - Carregamento dos dados
   - Tratamento de atributos categóricos com LabelEncoder e OneHotEncoder

3. **Modelagem e Preparação dos Dados:**
   - Separação entre variáveis previsoras e classe
   - Escalonamento dos atributos com StandardScaler

4. **Divisão em Treinamento e Teste:**
   - Divisão dos dados em conjuntos de treinamento e teste para ambas as bases

5. **Modelagem com Naive Bayes, Árvore de Decisão e Random Forest:**
   - Treinamento e avaliação dos modelos Naive Bayes, Árvore de Decisão e Random Forest

6. **Comparação de Resultados:**
   - Análise e comparação das métricas de desempenho dos modelos

## Resultados da Análise e Modelagem

### Base de Dados de Crédito

#### Naive Bayes
- **Acurácia:** 0.938
- **Relatório de Classificação:**
  
|                 |   precision |   recall |   f1-score |   support |
|:----------------|------------:|---------:|-----------:|----------:|
| 0               |    0.95     |  0.98    |   0.97     |   436     |
| 1               |    0.84     |  0.64    |   0.73     |    64     |
| accuracy        |             |          |   0.94     |    500    |
| macro avg       |    0.89     |  0.81    |   0.85     |    500    |
| weighted avg    |    0.93     |  0.94    |   0.93     |    500    |


#### Árvore de Decisão
- **Acurácia:** 0.982
- **Relatório de Classificação:**

|                 |   precision |   recall |   f1-score |   support |
|:----------------|------------:|---------:|-----------:|----------:|
| 0               |    0.99     |  0.99    |   0.99     |   436     |
| 1               |    0.91     |  0.95    |   0.93     |    64     |
| accuracy        |             |          |   0.98     |   500     |
| macro avg       |    0.95     |  0.97    |   0.96     |   500     |
| weighted avg    |    0.98     |  0.98    |   0.98     |   500     |



#### Random Forest
- **Acurácia:** 0.984
- **Relatório de Classificação:**

|                 |   precision |   recall |   f1-score |   support |
|:----------------|------------:|---------:|-----------:|----------:|
| 0               |    0.99     |  0.99    |   0.99     |   436     |
| 1               |    0.95     |  0.92    |   0.94     |    64     |
| accuracy        |             |          |   0.98     |   500     |
| macro avg       |    0.97     |  0.96    |   0.96     |   500     |
| weighted avg    |    0.98     |  0.98    |   0.98     |   500     |


#### kNN
- **Acurácia:** 0.986
- **Relatório de Classificação:**

|                 |   precision |   recall |   f1-score |   support |
|:----------------|------------:|---------:|-----------:|----------:|
| 0               |    0.99     |  0.99    |   0.99     |   436     |
| 1               |    0.94     |  0.95    |   0.95     |    64     |
| accuracy        |             |          |   0.99     |   500     |
| macro avg       |    0.97     |  0.97    |   0.97     |   500     |
| weighted avg    |    0.99     |  0.99    |   0.99     |   500     |


#### Regressão Logística
- **Acurácia:** 
- **Relatório de Classificação:**


#### SVM
- **Acurácia:** 
- **Relatório de Classificação:**


#### Redes Neurais
- **Acurácia:** 
- **Relatório de Classificação:**


### Base de Dados do Censo

#### Naive Bayes
- **Acurácia:** 0.477
- **Relatório de Classificação:**

|                 |   precision |   recall |   f1-score |   support |
|:----------------|------------:|---------:|-----------:|----------:|
| <=50k           |    0.97     |   0.32   |   0.48     |   3693    |
| >50k            |    0.31     |   0.97   |   0.48     |   1192    |
| accuracy        |             |          |   0.48     |   4885    |
| macro avg       |    0.64     |   0.64   |   0.48     |   4885    |
| weighted avg    |    0.81     |   0.48   |   0.48     |   4885    |  


#### Árvore de Decisão
- **Acurácia:** 0.810
- **Relatório de Classificação:**

|                 |   precision |   recall |   f1-score |   support |
|:----------------|------------:|---------:|-----------:|----------:|
| <=50k           |    0.88     |   0.87   |   0.87     |   3693    |
| >50k            |    0.61     |   0.61   |   0.61     |   1192    |
| accuracy        |             |          |   0.81     |   4885    |
| macro avg       |    0.74     |   0.74   |   0.74     |   4885    |
| weighted avg    |    0.81     |   0.81   |   0.81     |   4885    |  


#### Random Forest
- **Acurácia:** 0.850
- **Relatório de Classificação:**

|                 |   precision |   recall |   f1-score |   support |
|:----------------|------------:|---------:|-----------:|----------:|
| <=50k           |    0.88     |   0.93   |   0.90     |   3693    |
| >50k            |    0.73     |   0.62   |   0.67     |   1192    |
| accuracy        |             |          |   0.85     |   4885    |
| macro avg       |    0.81     |   0.77   |   0.79     |   4885    |
| weighted avg    |    0.85     |   0.85   |   0.85     |   4885    | 


#### kNN
- **Acurácia:** 0.829
- **Relatório de Classificação:**

|                 |   precision |   recall |   f1-score |   support |
|:----------------|------------:|---------:|-----------:|----------:|
| <=50k           |    0.86     |   0.93   |   0.89     |   3693    |
| >50k            |    0.71     |   0.51   |   0.59     |   1192    |
| accuracy        |             |          |   0.83     |   4885    |
| macro avg       |    0.78     |   0.72   |   0.74     |   4885    |
| weighted avg    |    0.82     |   0.83   |   0.82     |   4885    | 


#### Regressão Logística
- **Acurácia:** 
- **Relatório de Classificação:**


#### SVM
- **Acurácia:** 
- **Relatório de Classificação:**


#### Redes Neurais
- **Acurácia:** 
- **Relatório de Classificação:**



## Conclusão

Na base de dados de crédito, o modelo xxxxxxxxx apresentou a melhor acurácia...

Na base de dados do censo, o modelo yyyyyyy  teve um desempenho superior... 

O relatório de classificação indica que o ZZZZZZZ conseguiu capturar melhor as nuances dos dados.

Esses resultados destacam a importância de avaliar múltiplos modelos para entender qual se ajusta melhor aos dados específicos de cada caso.

## Como Executar

1. Clone o repositório.
2. Instale as dependências necessárias:
   ```sh
   pip install pandas numpy seaborn matplotlib plotly scikit-learn yellowbrick


Com essas adições, o código e o README.md estão prontos para serem usados diretamente no GitHub, com todos os detalhes necessários para replicar o projeto e entender os resultados.

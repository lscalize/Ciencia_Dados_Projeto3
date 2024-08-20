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

5. **Modelagem com Naive Bayes, Árvore de Decisão, Random Forest, kNN, Regressão logística, SVM e Redes neurais:**
   - Treinamento e avaliação dos modelos Naive Bayes, Árvore de Decisão, Random Forest, kNN, Regressão logística, SVM e Redes neurais

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
- **Acurácia:** 0.946
- **Relatório de Classificação:**

|                 |   precision |   recall |   f1-score |   support |
|:----------------|------------:|---------:|-----------:|----------:|
| 0               |    0.97     |  0.97    |   0.97     |   436     |
| 1               |    0.79     |  0.78    |   0.79     |    64     |
| accuracy        |             |          |   0.95     |   500     |
| macro avg       |    0.88     |  0.88    |   0.88     |   500     |
| weighted avg    |    0.95     |  0.95    |   0.95     |   500     |

#### SVM
- **Acurácia:** 0.988
- **Relatório de Classificação:**

|                 |   precision |   recall |   f1-score |   support |
|:----------------|------------:|---------:|-----------:|----------:|
| 0               |    0.99     |  1.00    |   0.99     |   436     |
| 1               |    0.97     |  0.94    |   0.95     |    64     |
| accuracy        |             |          |   0.99     |   500     |
| macro avg       |    0.98     |  0.97    |   0.97     |   500     |
| weighted avg    |    0.99     |  0.99    |   0.99     |   500     |



#### Redes Neurais
- **Acurácia:** 0.998
- **Relatório de Classificação:**

|                 |   precision |   recall |   f1-score |   support |
|:----------------|------------:|---------:|-----------:|----------:|
| 0               |    1.00     |  1.00    |   1.00     |   436     |
| 1               |    0.98     |  1.00    |   0.99     |    64     |
| accuracy        |             |          |   1.00     |   500     |
| macro avg       |    0.99     |  1.00    |   1.00     |   500     |
| weighted avg    |    1.00     |  1.00    |   1.00     |   500     |


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
- **Acurácia:** 0.849
- **Relatório de Classificação:**

|                 |   precision |   recall |   f1-score |   support |
|:----------------|------------:|---------:|-----------:|----------:|
| <=50k           |    0.88     |   0.93   |   0.90     |   3693    |
| >50k            |    0.73     |   0.61   |   0.66     |   1192    |
| accuracy        |             |          |   0.85     |   4885    |
| macro avg       |    0.80     |   0.77   |   0.78     |   4885    |
| weighted avg    |    0.84     |   0.85   |   0.84     |   4885    | 



#### SVM
- **Acurácia:** 0.850
- **Relatório de Classificação:**

|                 |   precision |   recall |   f1-score |   support |
|:----------------|------------:|---------:|-----------:|----------:|
| <=50k           |    0.87     |   0.94   |   0.90     |   3693    |
| >50k            |    0.75     |   0.58   |   0.66     |   1192    |
| accuracy        |             |          |   0.85     |   4885    |
| macro avg       |    0.81     |   0.76   |   0.78     |   4885    |
| weighted avg    |    0.84     |   0.85   |   0.84     |   4885    | 



#### Redes Neurais
- **Acurácia:** 0.816
- **Relatório de Classificação:**

|                 |   precision |   recall |   f1-score |   support |
|:----------------|------------:|---------:|-----------:|----------:|
| <=50k           |    0.87     |   0.89   |   0.88     |   3693    |
| >50k            |    0.64     |   0.59   |   0.61     |   1192    |
| accuracy        |             |          |   0.82     |   4885    |
| macro avg       |    0.75     |   0.74   |   0.75     |   4885    |
| weighted avg    |    0.81     |   0.82   |   0.81     |   4885    | 


## Conclusão

## Base de Dados de Crédito

A análise dos modelos de machine learning aplicados à base de dados de crédito revelou insights importantes:

- **Redes Neurais** apresentaram a melhor performance geral, com uma acurácia de **0.998** e um f1-score quase perfeito tanto para a classe majoritária quanto para a minoritária. Este modelo mostrou-se altamente eficaz para esse conjunto de dados, sendo o mais adequado para aplicações críticas onde a precisão é essencial.

- **SVM** e **kNN** também mostraram desempenhos notáveis, com acurácias de **0.988** e **0.986**, respectivamente. Esses modelos são bons candidatos para tarefas onde o equilíbrio entre precisão e eficiência computacional é necessário.

- **Random Forest** e **Árvore de Decisão** tiveram desempenhos similares, com acurácias de **0.984** e **0.982**, respectivamente. Ambos os modelos conseguiram capturar bem os padrões da base de dados, mas mostraram uma leve tendência a superestimar a classe majoritária.

- **Regressão Logística** e **Naive Bayes** apresentaram desempenhos inferiores em comparação aos outros modelos, com acurácias de **0.946** e **0.938**. Esses modelos, embora menos precisos, ainda podem ser úteis em cenários onde a interpretabilidade do modelo é uma prioridade.

Em suma, **Redes Neurais** é o modelo mais indicado para a base de dados de crédito, seguido de perto por **SVM** e **kNN**, dependendo das restrições computacionais e da necessidade de explicabilidade.

## Base de Dados do Censo

A análise da base de dados do censo trouxe desafios adicionais, especialmente devido à natureza desbalanceada dos dados:

- **SVM**, **Random Forest**, e **Regressão Logística** mostraram-se como as abordagens mais eficazes, com acurácias em torno de **0.850** e f1-scores equilibrados para ambas as classes. Esses modelos são altamente recomendados para este conjunto de dados, especialmente em cenários onde a classificação precisa de ambas as classes é essencial.

- **Árvore de Decisão** e **kNN** também apresentaram bons desempenhos, com acurácias de **0.810** e **0.829**, respectivamente. Eles podem ser considerados em contextos onde a interpretabilidade ou a simplicidade do modelo são preferenciais.

- **Naive Bayes** foi o modelo com o pior desempenho, com uma acurácia de **0.477**, demonstrando uma significativa limitação ao lidar com dados desbalanceados. Esse modelo não é recomendado para este tipo de aplicação, a menos que seja feita uma reavaliação do pré-processamento ou um ajuste no balanço das classes.

Portanto, **SVM**, **Random Forest**, e **Regressão Logística** são as escolhas mais robustas para a base de dados do censo, com **Árvore de Decisão** e **kNN** sendo alternativas viáveis em situações específicas.

## Ajuste de Parâmetros e Otimização

Além disso, é importante ressaltar que para a base do censo, onde os resultados foram um pouco piores, há ainda a possibilidade de ajuste de parâmetros e otimização. Foram sugeridas as seguintes técnicas para melhorar a performance dos modelos:

- **Grid Search**: Busca exaustiva de combinações de parâmetros pré-definidos para encontrar a melhor configuração.
- **Random Search**: Seleção aleatória de combinações de parâmetros, que permite explorar uma maior variedade de opções em menos tempo.

Esta conclusão destaca a eficácia de cada modelo aplicado aos dois conjuntos de dados e orienta o leitor sobre qual modelo seria mais adequado dependendo do cenário de aplicação.


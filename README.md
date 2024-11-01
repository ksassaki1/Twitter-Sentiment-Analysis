# 📊 **Projeto de Classificação de Textos com NLP**

Este projeto utiliza três modelos de **Machine Learning** - `Naive Bayes`, `Regressão Logística` e `Random Forest` - para realizar a classificação de textos em um conjunto de dados de **tweets**. O objetivo é comparar a capacidade desses modelos em identificar padrões nos textos e fornecer previsões se o texto apresenta um sentimento positivo ou negativo.

---

## 🎯 **Objetivo**
- Utilizar **Naive Bayes**, **Logistic Regression**, e **Random Forest** para realizar a classificação de textos em sentimentos positivos ou negativos.
- Avaliar o desempenho de cada modelo utilizando métricas adequadas, como acurácia, precisão, revocação e F1-score.
- Demonstrar o uso de diferentes pipelines de pré-processamento (`text_basic`, `text_spacy`, `text_nltk`) para a preparação dos dados.

---

## 🛠 **Tecnologias e Ferramentas Usadas**
- **Linguagem:** Python
- **Bibliotecas:**
  - `pandas`: Para manipulação e preparação dos dados.
  - `scikit-learn`: Para modelagem de Machine Learning, métricas de avaliação e pré-processamento.
  - `spacy` e `nltk`: Para pré-processamento dos textos.
  - `Matplotlib`: Para visualização dos resultados (opcional).

---

## 📂 **Estrutura do Projeto**
### **Arquivos e Diretórios**
- **`text_classification_project.ipynb`**: Notebook principal contendo:
  - Preparação e limpeza dos dados.
  - Nuvem de palavras mais comuns separadas por positivas e negativas e por pré-processamento NLP.
  - Treinamento dos modelos **Naive Bayes**, **Logistic Regression**, e **Random Forest**.
  - Visualização dos resultados e métricas de desempenho.

## 📊 **Nuvem de Palavras**
Abaixo estão exemplos de nuvens de palavras geradas a partir dos tweets classificados como positivos e negativos:

### Nuvem de Palavras - Sentimento Positivo
![Nuvem de Palavras - Sentimento Positivo]([image](https://github.com/user-attachments/assets/4e29bbfa-5caf-4c43-87b4-1d4214089194)
)

### Nuvem de Palavras - Sentimento Negativo
![Nuvem de Palavras - Sentimento Negativo]([image](https://github.com/user-attachments/assets/8d8d168b-26b9-4bbf-9df3-ec81e33e09af)
)

---

## 🧠 **Modelos Implementados**
- **Naive Bayes:**
  - Modelo probabilístico que assume independência entre as características e é muito eficiente para problemas de classificação de texto.

- **Logistic Regression:**
  - Modelo linear que realiza a classificação usando uma função sigmoide, útil para detecção de padrões lineares nos dados.

- **Random Forest:**
  - Conjunto de árvores de decisão que realiza classificações robustas e melhora a precisão reduzindo o overfitting.

- **Pipelines de Pré-Processamento NLP:**
  - **text_basic:** Realiza uma limpeza básica dos textos, removendo URLs, menções e caracteres especiais, útil para uma abordagem simples de pré-processamento.
  - **text_spacy:** Utiliza a biblioteca spaCy para lematização e remoção de stopwords, permitindo uma análise mais profunda e refinada dos textos.
  - **text_nltk:** Utiliza a biblioteca NLTK para tokenização e lematização, sendo uma alternativa ao spaCy para processamento de linguagem natural.

**Nota sobre NLP**: O processamento de linguagem natural (NLP) é uma etapa fundamental para preparar os textos de forma que possam ser usados pelos modelos de Machine Learning. Neste projeto, foram utilizados diferentes métodos de NLP para avaliar qual técnica de pré-processamento forneceria melhores resultados na classificação de sentimentos dos tweets.

---

## 📊 **Resultados Encontrados**
Durante os experimentos, os três modelos foram avaliados utilizando os diferentes pipelines de pré-processamento (`text_basic`, `text_spacy`, `text_nltk`). Aqui estão os principais resultados encontrados:

- **Pipeline `text_basic`**:
  - **Logistic Regression** apresentou o melhor desempenho, com uma acurácia de **78%**, seguido por `Naive Bayes` e `Random Forest` ambos com acurácia de **76%**.

- **Pipeline `text_spacy`**:
  - **Logistic Regression** também foi o melhor modelo, com uma acurácia de **75%**, enquanto `Naive Bayes` e `Random Forest` obtiveram acurácias de **74%**.

- **Pipeline `text_nltk`**:
  - **Logistic Regression** mais uma vez se destacou, alcançando uma acurácia de **76%**, enquanto `Naive Bayes` e `Random Forest` obtiveram **75%**.

**Conclusão Geral**: O modelo **Logistic Regression** foi consistentemente o melhor entre os três, apresentando o desempenho mais robusto em todos os pipelines de pré-processamento. O pipeline `text_basic` teve um desempenho ligeiramente superior em comparação aos outros métodos de pré-processamento.

---

## 🚀 **Próximos Passos**
- Testar os modelos com outros conjuntos de dados para verificar a generalização.
- **Ajustar Hiperparâmetros** dos Modelos:
  - Explorar técnicas como `GridSearchCV` ou `RandomizedSearchCV` para encontrar melhores parâmetros.
- **Dashboard Interativo**:
  - Desenvolver um dashboard utilizando **Streamlit** ou **Dash** para exibir as previsões e métricas de forma interativa.

---

## 📊 **Base de Dados Utilizada**
Este projeto utilizou a base de dados [Sentiment140](https://www.kaggle.com/datasets/kazanova/sentiment140), que contém 1,6 milhões de tweets rotulados para análise de sentimento.

### **Contexto**
Este é o dataset Sentiment140, que contém 1.600.000 tweets extraídos utilizando a API do Twitter. Os tweets foram anotados para indicar o sentimento:
- `0` = Sentimento **negativo**
- `4` = Sentimento **positivo`

### **Estrutura dos Dados**
O dataset contém os seguintes 6 campos:
- **target**: Polaridade do tweet (`0` = negativo, `2` = neutro, `4` = positivo)
- **ids**: Identificador do tweet (exemplo: `2087`)
- **date**: Data do tweet (exemplo: `Sat May 16 23:58:44 UTC 2009`)
- **flag**: Consulta realizada (`lyx`). Se não houver consulta, o valor é `NO_QUERY`
- **user**: Usuário que fez o tweet (exemplo: `robotickilldozr`)
- **text**: Texto do tweet (exemplo: `"Lyx is cool"`)

Neste projeto, foram utilizadas apenas as classes `0` (negativo) e `4` (positivo) para a classificação de sentimentos.

---

## 👤 **Autor**
Guilherme Koiti Tanaka Sassaki  
[LinkedIn](https://www.linkedin.com/in/guilherme-sassaki-10b81ba7/)


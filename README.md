# 📊 **Projeto de Classificação de Textos com Modelos de Machine Learning**

Este projeto utiliza três modelos de **Machine Learning** - `Naive Bayes`, `Regressão Logística` e `Random Forest` - para realizar a classificação de textos em um conjunto de dados de **tweets**. O objetivo é comparar a capacidade desses modelos em identificar padrões nos textos e fornecer previsões precisas.

---

## 🎯 **Objetivo**
- Utilizar **Naive Bayes**, **Logistic Regression**, e **Random Forest** para realizar a classificação de textos.
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
  - Nuvem de palavras mais comuns positivas e negativas de pré-processamento NLP.
  - Treinamento dos modelos **Naive Bayes**, **Logistic Regression**, e **Random Forest**.
  - Comparação entre os três modelos.
  - Visualização dos resultados e métricas de desempenho.

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
- **Equilibrar as Classes**:
  - Usar técnicas de balanceamento, como `SMOTE`, para melhorar a classificação de classes minoritárias.
- **Dashboard Interativo**:
  - Desenvolver um dashboard utilizando **Streamlit** ou **Dash** para exibir as previsões e métricas de forma interativa.

---

## 📊 **Base de Dados Utilizada**
Este projeto utilizou a base de dados [Sentiment140](https://www.kaggle.com/datasets/kazanova/sentiment140), que contém 1,6 milhões de tweets rotulados para análise de sentimento.
- As classes foram rotuladas como `0` para sentimentos **negativos** e `4` para sentimentos **positivos**.

---

## 📝 **Licença**
Este projeto é licenciado sob a [Licença MIT](LICENSE).

---

## 👤 **Autor**
Guilherme Koiti Tanaka Sassaki  
[LinkedIn](https://www.linkedin.com/in/guilherme-sassaki-10b81ba7/)



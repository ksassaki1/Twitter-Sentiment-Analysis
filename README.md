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

## 📊 **Sugestões de Aperfeiçoamento**
1. **Normalização dos Dados:** Utilize escaladores como `StandardScaler` ou `MinMaxScaler` para garantir que os dados estejam na mesma escala, melhorando o desempenho dos modelos.
2. **Validação Cruzada:** Implementar uma técnica como **Stratified K-Fold** para uma validação mais robusta e confiável.
3. **Visualização das Métricas:** Adicionar gráficos de barras para comparação visual das métricas de desempenho entre os modelos e as classes.
4. **Implementação de Modelos Adicionais:** Testar modelos como `SVM` ou `Gradient Boosting` para enriquecer a análise comparativa.
5. **Otimização de Pipeline:** Automatizar o pré-processamento e a modelagem com **Pipeline** do `scikit-learn` para facilitar a reprodutibilidade.

---

## 📝 **Licença**
Este projeto é licenciado sob a [Licença MIT](LICENSE).

---

## 👤 **Autor**
Guilherme Koiti Tanaka Sassaki  
[LinkedIn](https://www.linkedin.com/in/guilherme-sassaki-10b81ba7/)


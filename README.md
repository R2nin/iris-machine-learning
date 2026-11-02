# 🌸 Classificação do Dataset Iris — Machine Learning

**FEMA/IMESA — 4º Bacharelado em Ciência da Computação**  
**Disciplina:** Inteligência Artificial | **Prof.:** Talo

[![Abrir no Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/R2nin/iris-machine-learning/blob/master/iris_naive_bayes.ipynb)

---

## Sobre o projeto

Trabalho de Machine Learning que aplica dois algoritmos de classificação sobre o clássico **Dataset Iris**, comparando seus desempenhos por meio de Matrizes de Confusão e Acurácia.

O notebook foi desenvolvido no **Google Colab** combinando:
- **Python** — interface interativa com menu de seleção e visualizações
- **R** (via `rpy2`) — treinamento e avaliação dos modelos de ML

---

## Dataset

| Atributo | Descrição |
|---|---|
| `SepalLengthCm` | Comprimento da sépala (cm) |
| `SepalWidthCm` | Largura da sépala (cm) |
| `PetalLengthCm` | Comprimento da pétala (cm) |
| `PetalWidthCm` | Largura da pétala (cm) |
| `Species` | Classe alvo: *setosa*, *versicolor* ou *virginica* |

- 150 amostras — 50 por espécie
- Fonte: [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/53/iris)

---

## O que o notebook faz

1. **Carrega e prepara** o dataset Iris (split 80% treino / 20% teste, estratificado)
2. **Treina o Modelo 1:** Naive Bayes
3. **Treina o Modelo 2:** escolhido pelo usuário via menu interativo
   - 🌳 Árvore de Decisão (`rpart`)
   - 🌲 Random Forest (`randomForest`)
   - ⚡ SVM — Support Vector Machine (`kernlab`)
4. **Avalia** ambos os modelos: Matriz de Confusão + Acurácia
5. **Compara** o desempenho dos dois algoritmos automaticamente

---

## Como usar

1. Clique no badge **Open in Colab** acima
2. Execute as células em ordem (`Shift+Enter`)
3. Na célula do menu, selecione o 2º algoritmo desejado
4. Clique em **▶ Executar análise**

---

## Pacotes R utilizados

| Pacote | Função principal |
|---|---|
| `e1071` | `naiveBayes()` |
| `caret` | `createDataPartition()`, `confusionMatrix()` |
| `rpart` | `rpart()` — Árvore de Decisão |
| `randomForest` | `randomForest()` |
| `kernlab` | `ksvm()` — SVM |

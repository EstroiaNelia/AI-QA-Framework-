## Hoje aprendi:

Hoje estudei a Matriz de Confusão (Confusion Matrix) e as principais métricas utilizadas na avaliação de modelos de classificação.

### Matriz de Confusão

docs/images/confusion_matrix.jpg

### Conceitos Principais

- **Verdadeiro Positivo (TP)**: o modelo prevê corretamente a classe positiva.
- **Verdadeiro Negativo (TN)**: o modelo prevê corretamente a classe negativa.
- **Falso Positivo (FP)**: o modelo prevê positivo quando a classe real é negativa (Erro Tipo I).
- **Falso Negativo (FN)**: o modelo prevê negativo quando a classe real é positiva (Erro Tipo II).

### Métricas de Avaliação

- **Accuracy (Exatidão)** = (TP + TN) / (TP + TN + FP + FN)
- **Precision (Precisão)** = TP / (TP + FP)
- **Recall (Sensibilidade)** = TP / (TP + FN)
- **Specificity (Especificidade)** = TN / (TN + FP)

### Reflexão

Compreendi que a Accuracy pode ser enganadora quando existem classes desbalanceadas. Nesses casos, métricas como Precision, Recall e F1-Score fornecem uma avaliação mais fiável do desempenho do modelo.

Dúvidas:

Preciso entender melhor:
- Benchmark suits
- Performance benchmark metrics
- Balanced datasets
- Imbalanced datasets
- LLM evals ragas

Ideias para o Framework:
...
Termos novos:
- Benchmark suits
- Performance benchmark metrics
- Balanced datasets
- Imbalanced datasets
- LLM evals ragas

Questões que gostaria de discutir com o Atlas:
Gostaria de perceber melhor as fórmulas aprendidas e sobre as - LLM evals ragas.

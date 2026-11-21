# 2. Fundamentos de Machine Learning (15% da prova)

**Ideia central:** o modelo aprende padrões a partir de dados. Ciclo: treinar, validar, testar com dados novos e usar.

## Tipos de aprendizado
- **Supervisionado:** dados com rótulo. Classificação e regressão (regressão linear, árvore de decisão, random forest).
- **Não supervisionado:** sem rótulo. Clusterização (k-means), redução de dimensionalidade, anomalias.
- **Por reforço:** agente aprende por tentativa e erro, com recompensa.
- **Semissupervisionado:** poucos dados rotulados e muitos sem rótulo.

## Conceitos
- **Features:** variáveis de entrada. **Label:** o que se quer prever.
- **Treino, validação e teste:** aprende, ajusta e avalia com dados nunca vistos.
- **Overfitting:** vai bem no treino e mal em dados novos. **Underfitting:** vai mal até no treino.
- **Viés x variância:** viés alto leva a underfitting, variância alta leva a overfitting.

## Métricas
- **Classificação:** acurácia, precisão (dos previstos positivos, quantos eram), recall (dos positivos reais, quantos achou) e F1.
- **Regressão:** MAE, MSE, RMSE e R².
- **Matriz de confusão:** verdadeiros e falsos positivos e negativos.

## Quando usar o quê
- Fraude (poucos casos): acurácia engana, olhe precisão e recall.
- Perder um caso é grave (exame médico): priorize o recall.

## Pegadinhas
- Acurácia alta não significa modelo bom com classes desbalanceadas.
- "Sem rótulos" aponta para não supervisionado.
- Mais dados e mais variedade ajudam a reduzir overfitting.

## Perguntas de fixação
1. Diferença entre supervisionado e não supervisionado? (Com e sem rótulo.)
2. Vai muito bem no treino e mal no teste. Qual o problema? (Overfitting.)
3. Por que a acurácia pode enganar na fraude? (Um modelo que diz "nunca é fraude" teria acurácia alta e seria inútil.)

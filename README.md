# Classificacao de Compra de Veiculos com SVM

## Sobre o Projeto

Este projeto aplica o algoritmo Support Vector Machine (SVM) para prever a intencao de compra de veiculos por parte de clientes, utilizando como base dados demograficos como idade, salario anual e genero. O trabalho faz parte de uma serie de exercicios comparativos de modelos de Machine Learning, complementando uma analise anterior realizada com XGBoost sobre o mesmo dataset.

## Metodologia

Partimos de uma base com 1.000 registros, previamente tratada (remocao de identificadores, encoding de variaveis categoricas e analise de correlacao). Dois modelos SVM foram treinados e avaliados: o primeiro com kernel linear e o segundo com kernel polinomial de grau 3. Os dados foram padronizados com StandardScaler antes do treinamento, etapa essencial para o funcionamento adequado do SVM.

## Resultados

O SVM com kernel polinomial superou o linear em todas as metricas, alcancando 87.50% de Accuracy contra 85.50%, alem de Precision superior na classe positiva (0.91 vs 0.86). Na comparacao com o XGBoost da atividade anterior, este ultimo manteve a lideranca como modelo mais robusto para este tipo de problema, reafirmando sua eficacia em dados tabulares com poucas features. Ainda assim, o SVM Poly demonstrou ser uma alternativa competitiva, especialmente em cenarios que demandam modelos mais simples.

**Tecnologias:** Python, Scikit-learn (SVM, StandardScaler), Pandas, Seaborn, Matplotlib.

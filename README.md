# SuperHeroes
Modelagem de base de dados de super-heróis (Clusterização, classificação e regressão)

Este teste técnico foi dividido em 3 etapas:
  1 - Clusterização
  2 - Classificação
  3 - Regressão

Não foi meu melhor trabalho, mas como foi realizado em poucas horas, vale a pena adicioná-lo. 

1- Clusterização

A base de dados era majoritariamente composta de dados booleanos e categóricos. Além disso, as variáveis numéricas possuiam muitos valores faltantes e por isso optamos por não usá-las.
Este cenário me levou a optar pela clusterização hierárquica ao invés do clássico K-Means. Também apliquei PCA. O resultado se mostrou interessante.

2- Classificação

O objetivo era encontrar um modelo que previsse quais personagens eram bons e quais eram maus com um desempenho melhor do que Naïve Bayes.
A regressão logística se mostrou a melhor opção. Modelos baseados em árvore tiveram pior desempenho.
A métrica de desempenho utilizada foi o Kappa de Cohen, uma vez que a base estava desbalanceada e não foram fornecido maiores detalhes sobre a importância dos erros.

3- Regressão

O objetivo era gerar um modelo para prever o peso a partir de diversas característica do personagem.
Apliquei vários modelos tentando buscar um maior R². Devido à grande quantidade de outliers, modelos de SVM tiveram um mau desempenho.
Curiosamente, o melhor modelo foi a regressão Lasso, uma vez que a penalização contrabalanceava os outliers.

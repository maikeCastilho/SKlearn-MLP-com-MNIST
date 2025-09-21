# Classificação de Dígitos MNIST com Scikit-Learn

Este projeto utiliza a base de dados MNIST (handwritten digits) para treinar uma rede neural artificial usando o `MLPClassifier` da biblioteca Scikit-Learn.

## Estrutura do projeto
- Carregamento do dataset MNIST via `fetch_openml`.
- Pré-processamento (normalização dos pixels entre 0 e 1).
- Divisão em treino (60k imagens) e teste (10k imagens).
- Treinamento de uma MLP simples.
- Comparação de resultados **com e sem PCA**.

## Correções aplicadas
- Normalização foi feita **antes** do treino.
- Aumentado o número de iterações (`max_iter`) para permitir convergência adequada.
- Testado também um modelo com PCA para redução de dimensionalidade.

## Resultados esperados
- Sem PCA: acurácia ~97% no conjunto de teste.
- Com PCA (100 componentes): acurácia um pouco menor (~95–96%), porém com **treinamento mais rápido**.

## Como executar
1. Abra o Jupyter Notebook.
2. Execute todas as células em ordem.
3. Compare os resultados de acurácia com e sem PCA.

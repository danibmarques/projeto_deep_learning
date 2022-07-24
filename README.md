# Model Card - Projeto Deep Learning
Este projeto é uma proposta de modelo para o treinamento de um algoritmo _Deep Learning_.

# Detalhes do modelo
- Estudo de caso de um problema de classificação multiclasse. 
- Através de ferramentas como **Google Colab**, **Tensor Flow** e **Keras**, foi desenvolvido um modelo de aprendizagem profunda, um MLP (_Multi Layer Perceptron_).
- Os dados obtidos no treinamento foram armazenados no **Weights and Biases**, para melhor rastreamento dos resultados.

# Uso pretendido
Destinado para provar os fundamentos do conceito de _Deep Learning_. 

<img src="https://user-images.githubusercontent.com/44613658/180632141-f6ed8f07-1bcb-486a-8ec6-463c0f96efd4.JPG" width="400" height="300" >

# Fatores
A partir de dados de entrada com algumas características da flor íris como `sepal length in cm, sepal width in cm, petal length in cm, petal width in cm` poder determinar de forma automatizada qual a classe que a respectiva flor pertence (`Iris-setosa, Iris-versicolor, Iris-virginica`).

# Dados de avaliação
O dataset utilizado neste projeto está disponível em UCI Machine Learning Repository, ([website](https://archive.ics.uci.edu/ml/machine-learning-databases/iris/)).

Neste trabalho também foram utilizadas algumas técnicas de melhor aprendizado e melhor generalização, a fim de obter melhores parâmetros para o _hyperparameter tuning_.

# Métricas
- Para as técnicas de melhor aprendizagem foram utilizadas a configuração da capacidade com o ajuste dos nós e camadas e a configuração da velocidade de aprendizagem com a taxa de aprendizagem.
- Para as técnicas de melhor generalização foram utilizadas a restrição dos pesos e o desacoplamento de camadas com dropout.
- A métrica que será considerada para a avaliação é a `accuracy`. Espera-se com o modelo de aprendizado atingir uma acurácia em torno de 95 e 97%, que é o razoável para este conjunto de dados.

# Análise Quantitativa
- 1º método Melhor Aprendizagem (à esquerda ajuste na quantidade de nós e à direita ajuste na quantidade de camadas):

<img src="https://user-images.githubusercontent.com/44613658/180644080-668aa674-1395-47ec-99a8-8ca597660a93.png" width="300" height="200" >    <img src="https://user-images.githubusercontent.com/44613658/180644147-03c4050e-f099-48fb-9218-ee490ce9adb2.png" width="300" height="200" >


- 2º método Melhor Aprendizagem - ajuste na taxa de aprendizagem:

<img src="https://user-images.githubusercontent.com/44613658/180644321-541b7199-5079-4ec9-a3ce-cbb3f4b55671.png" width="500" height="400" >


- 1º método Melhor Generalização - restrição dos pesos:

<img src="https://user-images.githubusercontent.com/44613658/180645703-f4a452f0-0e1f-4240-895a-338e4cc68f26.png" width="600" height="300" >

- 2º método Melhor Generalização - Dropout

<img src="https://user-images.githubusercontent.com/44613658/180646122-0449074a-8e53-48ee-8f2e-2b9a9c4752a2.png" width="600" height="300" >


- Visão geral do resultado final carregado na plataforma **Weights and Biases**:

<img src="https://user-images.githubusercontent.com/44613658/180646230-0afb1404-f0f6-41d5-ab9d-ef669396fa2e.png" width="700" height="300" >














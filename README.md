# Machine Learning

Resolução de problemas de Machine Learning, buscando ajudar no entendimento desta disciplina com exemplos dos algoritmos com códigos em Python explicados.
Os códigos estarão separados nas categorias abaixo, com o nome do arquivo e uma breve descrição do que ele representa

### Pipeline de dados
  * Análise Exploratória Descritiva
    - 1.1-AED-Iris.ipynb: Este exemplo apresenta uma solução para entender os dados do dataset Iris, desde a elaboração do Data Frame a partir dos array, até a geração de gráficos para suporte visual do que se tem no conjunto de dados. Possui explicações um pouco mais detalhadas dos códigos e o que eles representam.
    - 1.2-AED-FraudDetection.ipynb: Exploração do dataset FraudDetection do Kaggle. Após as técnicas iniciais, foi calculada a correlação para entender um pouco mais os dados em relação ao problema proposto. Apesar dos valores terem sido baixos, separei as variáveis que mais tem correlação com a variável alvo. Montei gráficos de dispersão e também histogramas para entender como os dados estão apresentados.
    - 1.3-AED-MNist.ipynb: Exploração de dados do dataset Mnist, já trabalhado com valores tabulares para todos os 784 pixels originais das imagens com 28x28 pixels dos digitos numéricos.

### Aprendizado Supervisionado
  * Classificação
    - 2.1-KNN_FraudDetection.ipynb: KNN (K-Nearest Neighbors) é um algoritmo de classificação por instância, que a cada execução faz a comparação do elemento a ser predito com todos os outros elementos do conjunto de dados e compara a distância (por padrão, Euclidiana [que pode ser encontrada pelo cálculo de Pitágoras]). A partir da quantidade de K elementos mais próximos é definida a classe a qual aquele novo elemento pertence. Neste exemplo foi utilizado o Dataset Fraud Detection.
    - 2.2-DecisionTree_FraudDetection.ipynb: Decision Tree (Árvore de Decisão) é um algoritmo de classificação por modelo, que permite criar uma árvore de busca. Sua explicabilidade é alta, dado que é possível entender facilmente quais foram os critérios utilizados para cada quebra de ramificação, desde a raíz até a folha da árvore. Neste exemplo foi utilizado o Dataset Fraud Detection.
    - 2.3-KNN_MNist.ipynb: Exemplo de implementação de KNN utilizando a base de dados MNist, desde o momento da aquisição do dado até a geração da matriz de confusão (com a impressão de um caracter para ajudar no entendimento).
    - 2.4-DecisionTree_MNist.ipynb: Implementação de uma árvore de decisão na base de dados MNist, gerando inclusive a visualização da árvore desde a raiz até as folhas.
    - 2.5-MultiLayerPerceptron_MNist.ipynb: Exemplo de implantação de uma Rede Neural de multiplas camadas com a arquitetura Multi-Layer Perceptron. A rede foi treinada inicialmente com três camadas ocultas contendo 400, 200 e 50 neurônios inicialmente.
    
### Boas práticas
  * Validação Cruzada
    - 3.1-CrossValidation_Iris.ipynb: Este exemplo de código explica de forma rápida como funciona a validação cruzada e implementa uma alternativa de (re)uso para que os modelos sejam treinados com os mesmos dados. Para fins didáticos, foi utilizado o dataset Iris que possui apenas 150 observações e facilita o entendimento.
  * Grid Search
    - 3.2-GridSearch_KNN_Iris.ipynb: O Grid Search auxilia na escolha dos melhores hiperparâmetros para treinar o seu modelo. É possível definir quais são as configurações desejadas para testar o treino, e com isso, o modelo é treina com um plano cartesiano combinando todas as variações definidas. O resultado apresenta a melhor combinação testada, e essa configuração pode ser utilizada para treinar seu modelo final.
  * Serialização de Modelo treinado
    - 3.3-Gerar_Pickle.ipynb: Salvar o modelo treinado em um Pickle ou um ONNX permite que o modelo seja serializado em um objeto unico, e recuperado quando precisar. É util para manter uma foto do modelo treinado, e não precisar retreinar todas as vezes que for utilizar o modelo

### Comparação de algoritmos
Utilizando a base de dados MNIST e a partir dos algoritmos KNN, DecisionTree e Multi-layer Perceptron, rodar o Grid Search com Stratified K-Fold para encontrar a melhor hiper-parametrização em cada um dos modelos. Serializar com Pickle o modelo campeão de cada algoritmo. Carregar todos os pickles em um novo Jupyter, montar uma base de dados de teste com Hold-out 80/20 e rodar o mesmo conjunto de dados de teste em cada um dos modelos carregados a partir dos Pickles e comparar os resultados obtidos.
  * 5.1-MNIST_KNN.ipynb: Melhor hiper-parametrização encontrada para o algoritmo KNN
  * 5.2-MNIST_DT.ipynb: Melhor hiper-parametrização encontrada para o algoritmo Decision Tree
  * 5.3-MINST_MLP.ipynb: Melhor hiper-parametrização encontrada para o algoritmo Multi-Layer Perceptron
  * 5.4-MNIST_ComparacaoAlgoritmos.ipynb: Comparação dos resultados dos algoritmos avaliados
  * 5.5-MINST_GAN.ipynb: Criação de uma rede Geradora e uma Discriminadora, para criar novos dígitos
  * 5.6-MNIST_ConclusaoEstudo.ipynb: É carregada uma rede geradora (Rede GAN) e inventado um dígito. Em seguida, o dígito é convertido em um array de pixels e então é usado como entrada nos três modelos para que seja feita a predição.
  
   
## Como colaborar?
Esta playlist tem vídeos explicativos para ajudar em **Colaboração de Projetos**: https://www.youtube.com/playlist?list=PLrakQQfctUYX37CRv3fomYfKwDe0NLmsk

Sempre que pensar em algo interessante e quiser colaborar com o repositório, **faça um *Fork* deste repositório** e adicione os arquivos no seu *repo*. Abra a *Issue* e Faça um *Pull Request*

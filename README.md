# Machine Learning

Resolução de problemas de Machine Learning, buscando ajudar no entendimento desta disciplina com exemplos dos algoritmos com códigos em Python explicados.
Os códigos estarão separados nas categorias abaixo, com o nome do arquivo e uma breve descrição do que ele representa

### Pipeline de dados
  * Análise Exploratória Descritiva
    - 1.1-AED-Iris.ipynb: Este exemplo apresenta uma solução para entender os dados do dataset Iris, desde a elaboração do Data Frame a partir dos array, até a geração de gráficos para suporte visual do que se tem no conjunto de dados. Possui explicações um pouco mais detalhadas dos códigos e o que eles representam.
    - 1.2-AED-FraudDetection.ipynb: Exploração do dataset FraudDetection do Kaggle. Após as técnicas iniciais, foi calculada a correlação para entender um pouco mais os dados em relação ao problema proposto. Apesar dos valores terem sido baixos, separei as variáveis que mais tem correlação com a variável alvo. Montei gráficos de dispersão e também histogramas para entender como os dados estão apresentados.

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
   
## Como colaborar?
Esta playlist tem vídeos explicativos para ajudar em **Colaboração de Projetos**: https://www.youtube.com/playlist?list=PLrakQQfctUYX37CRv3fomYfKwDe0NLmsk

Sempre que pensar em algo interessante e quiser colaborar com o repositório, **faça um *Fork* deste repositório** e adicione os arquivos no seu *repo*. Abra a *Issue* e Faça um *Pull Request*

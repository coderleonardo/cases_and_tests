# **Prevendo o range de salário de uma pessoa**

<figure align="center">
<img src="https://media-exp1.licdn.com/dms/image/C4D0BAQF5qVHC8HSZUQ/company-logo_200_200/0/1597176769890?e=1667433600&v=beta&t=Fthq9l_xi3wYEwcK98i70qjID_NlWmUtLi-kgaw2GdY" alt="Indicium" width="25%"/>

<figure-caption>**INDICIUM**</figure-caption>
</figure>

O projeto em questão é idealizado como parte do processo seletivo para formação em Ciência de Dados oferecido pela [Indicium](https://www.linkedin.com/company/indiciumtech/), via programa Lighthouse.

O projeto em questão tem como objetivo implementar um modelo que seja capaz de prever o salário anual de uma pessoa com base nas características fornecidas pelo dataset em questão, no caso se a pessoa irá ganhar um salário ">= 50K" ou "< 50k".

Neste problema de **classificação** iremos utilizar o conjunto de dados *wage_train* para treinar nosso modelo e posteriormente o conjunto de dados *wage_test* para prevermos os salários em um novo conjunto. 

Formalizado o problema, vamos começar. 

<figure align="center">
<img src="https://media3.giphy.com/media/26BRL3pw98MWNOy0U/giphy.gif?cid=ecf05e47b2ydwom483t14fbqgxwjadqft5gqrfyaav60o8cr&rid=giphy.gif&ct=g" width="20%" />
</figure>

## Como usar este repositório?

O repositório em questão contém a base de dados para treinamento, "wage_train.csv". Basta rodar o arquivo Jupyter Notebook e ao final importar o arquivo
"wage_test.csv" para utilizar na função "pipeline" dentro do Jupyter Notebook para obter as novas predições.

## Tabela de conteúdo

01. Importação das bibliotecas centrais e Leitura da base de dados

02. Explorando a base de dados

03. Pré-Processamento da base de dados e Seleção das features a serem usadas
  - Selecionando as features para o problema em questão  
  - Tranformando as variáveis categóricas para o tipo numérico adequado
  - Upsampling com SMOTE - Synthetic Minority Over-sampling Technique

04. Seleção do modelo
  - Divisão entre treino e teste (divisão básica padrão)
  - Modelo LogisticRegression  
  - Modelo SGDClassifier  
  - RandomForestClassifier

05. Implementando a Regressão Logística num novo conjunto de dados

### Bibliotecas usadas
  - pandas para manipulação dos dados;
  - matplotlib para visualização dos dados;
  - seaborn para visualização dos dados;
  - sklearn para implementação dos modelos de aprendizado e métricas;
  - imbalanced-learn para tratamento de classe desbalanceadas.

## Conclusões

O projeto acima foi somente uma parte de muitas possibilidades para a solução do problema em questão. Obviamente ainda existem muitos pontos de melhorias que podem ser implementados, alguns como:
  - Analisar como outros algoritmos como One-Hot-Encoder mudam a perfomance do modelo implementado, dado que o algoritmo Label Encoder pode introduzir algum viés que antes não existia no problema;

  - Implementar técnicas de tunning de hiperparâmetros como GridSearch para buscar a melhor combinação possível de hiperparâmetros para cada algoritmo estudado;

  - Aplicar métodos de validação cruzada de modo a eliminar possíveis viés devido à divisão "train_test_split" que simplesmente divide nosso conjunto de dados entre treino e teste, sem aproveitar todas as possibilidades do nosso dataset;

  - Analisar se as features selecionadas são de fato as melhores e se existe outra combinação que pode trazer melhorias para a classificação, etc.

De modo geral, sempre é proveitoso implementar a solução de um problema do zero, uma vez que traz novos conhecimentos e reforça outros. 

Deste modo, agradeço à [Indicium](https://www.linkedin.com/company/indiciumtech/) pela a oportunidade, que novamente foi muito proveitosa.

<figure align="center">
<img src="https://media2.giphy.com/media/xUPOqo6E1XvWXwlCyQ/giphy.gif?cid=ecf05e47chp6w1wusr7f3izsa1sx0n6vce9mg1nkv8vortwe&rid=giphy.gif&ct=g" width="40%" />
</figure>

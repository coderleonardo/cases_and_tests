# Desafio Final Imersão Dados - Problema de Drug Discovery
![Machine Learning aplicado à Biologia](https://github.com/coderleonardo/imersao-dados-desafio-final/blob/main/Notebooks/Machine%20Learning%20aplicado%20%C3%A0%20Biologia.jpg?raw=true)

## Sobre o projeto
O projeto em questão é proposto como desafio final da Imersão Dados da [Alura](https://www.alura.com.br), e tem como base o desafio proposto pelo Laboratory for Innovation Science at Harvard: Mechanisms of Action (MoA) Prediction. Can you improve the algorithm that classifies drugs based on their biological activity?

## Motivação
"As pesquisas biomédicas estão cada vez mais interdisciplinares e sofisticadas e os dados gerados nesses estudos são cada vez mais volumosos e complexos, tornando a ciência de dados essencial no desenvolvimento da farmacologia." (Trecho retirado da bibliografia teórica).

## Objetivo do projeto
Este projeto tem como objetivo melhorar os algoritmos de classificação de drogas baseado nos seus mecanismos de ação (MoA). Formalmente queremos resolver um problema de classificação com vários rótulos.

### Qual é o mecanismo de ação (MoA) de uma droga? E por que isto é importante?

No passado, os cientistas derivavam drogas de produtos naturais ou eram inspirados por remédios tradicionais. Drogas muito comuns, como o paracetamol, conhecido nos Estados Unidos como acetaminofeno, foram colocadas em uso clínico décadas antes que os mecanismos biológicos que impulsionam suas atividades farmacológicas fossem compreendidos. 
<br><br>
Hoje, com o advento de tecnologias mais poderosas, a descoberta de medicamentos mudou das abordagens inesperadas do passado para um modelo mais direcionado baseado na compreensão do mecanismo biológico subjacente de uma doença. 
<br><br>
Nessa nova estrutura, os cientistas buscam identificar um alvo proteico associado a uma doença e desenvolver uma molécula que possa modular essa proteína alvo. Como uma abreviação para descrever a atividade biológica de uma determinada molécula, os cientistas atribuem um rótulo conhecido como mecanismo de ação ou MoA.

### Como determinamos os MoAs de um novo medicamento?

Uma abordagem é tratar uma amostra de células humanas com a droga e, em seguida, analisar as respostas celulares com algoritmos que buscam semelhança com padrões conhecidos em grandes bancos de dados genômicos, como bibliotecas de expressão gênica ou padrões de viabilidade celular de drogas com MoAs conhecidos.

## Breve resumo do estudo

Na análise em questão buscamos explorar todos os dados presentes nos experimentos e resultados. Tiramos algumas conclusões de modo a filtrar nossa linha de raciocínio para que pudéssemos elaborar nosso modelo de Machine Learning.

Após a modelagem de alguns modelos, observamos que mesmo não obtendo o resultado mais ideal, dadas todas as considerações que serão apresentadas no texto, concluímos que obtivemos um resultado razoalmente satisfatório para o nosso modelo de classificação binária sobre o mecanismo de ação (MoA).

## Conteúdo do projeto
(1) Importando as bibliotecas necessárias para a análise dos dados

(2) Importando a base de dados do experimento

(2.1) Analisando os valores presentes em cada coluna

(3) Análise exploratória do conjunto de dados do experimento

(3.1) Relação entre tratamento com_droga e tratamento com_controle

(3.2) Relação entre os tempos para o início da análise

(3.4) Drogas (ou compostos) que mais aparecem no experimento

(3.5) Analisando os valores de alguns genes

(3.5.1) Genes analisados: g-0, g-5, g-10 e g-15

(3.6) Descrição geral dos dados

(3.6.1) Histograma da média sobre as expressões gênicas (genes)

(3.6.2) Gráfico sobre os valores mínimos e máximos das expressões gênicas

(3.6.3) Avaliando o comportamento das Linhagens celulares

(3.6.4) Tabela de frequência de dose x tempo para cada 
tipo de tratamento

(3.6.5) Analisando a correlação - caso particular entre os genes g-0 e g-8

(3.6.6) Correlação entre todos os genes

(4) Importando a base de dados dos resultados obtidos

(5) Análise exploratória do conjunto de dados dos resultados

(5.1) Identificando quantas vezes cada mecanismo de ação foi ativado

(5.2) Conjunto total de ações ativadas por cada droga - avaliando pelo "id" da droga

(6) Modelo de Machine Learning

(6.1) Problema de classificação binária

(6.1.1) Regressão Logística

(6.1.2) Árvore de decisão

(6.1.2.1) Árvore com 3 camadas

(6.1.2.2) Várias árvores com camadas diferentes

(6.1.3) Random Forest - modelo com várias árvores aleatórias (mais dados usados na análise)

(6.1.4) Neighbors Classifier

(7) Conclusões

## Fontes
### Bibliografia teórica e matemática
  * [1] [Leia mais sobre curva Gaussiana clicando aqui.](https://www.inf.ufsc.br/~andre.zibetti/probabilidade/normal.html)
  * [2] [Leia mais sobre Histogramas clicando aqui.](https://www.alura.com.br/artigos/o-que-e-um-histograma?utm_source=gnarus&utm_medium=timeline)
  * [3] [Leia mais sobre como escolher um modelo de Machine Learning para seu problema clicando aqui.](https://scikit-learn.org/stable/tutorial/machine_learning_map/index.html)
  * [4] [Drug Discovery - Passado, presente e futuro.](https://docs.google.com/document/d/10EhrQBChlyYIcff3to7PrCQi5HcNk2r-zd2ZCKPtcz8/edit)
  * [5] [Expressão gênica: o caminho da informação biológica.](https://drive.google.com/file/d/1VNP08ffCiGD8cqaBkdHATWSX8Yxfm3dj/view?usp=sharing)
  * [6] [Mechanisms of Action (MoA) Prediction. Can you improve the algorithm that classifies drugs based on their biological activity? - Página oficial do desafio proposto pelo Laboratory for Innovation Science at Harvard.](https://www.kaggle.com/c/lish-moa)
  * [7] [Como saber se seu modelo de Machine Learning está funcionando mesmo?](https://paulovasconcellos.com.br/como-saber-se-seu-modelo-de-machine-learning-está-funcionando-mesmo-a5892f6468b)

### Bibliotecas usadas
  * Pandas - Análise de dados: https://pandas.pydata.org
  * Numpy - Computação científica com Python: https://numpy.org
  * Matplotlib - Visualização de dados: https://matplotlib.org
  * Seaborn - Visualização estatística de dados: https://seaborn.pydata.org
  * Scikit-learn - Machine Learning com Python: https://scikit-learn.org/stable/

## Agradecimentos
Gostaria de agradecer à [Alura](https://www.alura.com.br) pela oportunidade de participar desta imersão estudando um assunto totalmente novo para mim (que é a ciência de dados aplicada à Biologia) e também por proporcionar tamanho em num período tão curto de tempo.
<br><br>
Gostaria de agradecer também aos instrutores [Guilherme Silveira](https://www.linkedin.com/in/guilhermeazevedosilveira/), [Vanessa Leiko](https://www.linkedin.com/in/vanessa-leiko-oikawa-cardoso/) e [Thiago Gonçalves](https://www.linkedin.com/in/thiago-gonçalves-santos/), que nos auxiliaram e guiaram ao longo desse estudo.

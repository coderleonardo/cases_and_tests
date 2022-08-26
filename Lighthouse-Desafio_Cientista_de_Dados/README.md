# **Prevendo o *churn* (abandono de clientes) de um banco**

## Descrição do notebook

O objetivo aqui é prever o churn (abandono de clientes) de um banco de dados fictício de uma instituição financeira. 

Para isso são fornecidos dois datasets: um dataset chamado *abandono_clientes* composto por 10000 linhas e 13 colunas de informação (features), sendo uma coluna “Exited” composta por dados binários: **1 se o cliente abandonou o banco**, **0 se não**.

O segundo dataset possui 1000 linhas e 12 colunas e não possui a coluna “Exited”. 
Vamos prever essa coluna a partir do modelo de Machine Learning escolhido ao treinarmos sobre o conjunto de dados *abandono_clientes*.

Note que de acordo com o descrito acima temos um problema de **classificação binária**.

## Tabela de Conteúdo e Descrição
1. Importação dos dados

2. Análise Exploratória dos dados
	* Análise das features representativas do nosso dataframe
	
3. Pré-processamento dos dados

4. Modelos de Machine Learning (usando Train-Test-Split)
	* Preparando os dados que vamos usar
	* Definindo uma baseline
	* Modelo KNN
	* Modelo SVM
	* Modelo Random Forest
	* Conclusão usando Train-Test-Split
		- Usando esta divisão para conjunto de treino e teste temos que os modelos de classificação usados não desempenham um bom papel, o que era de se esperar devido ao desbalanceamento dos dados a serem previstos.

Vamos analisar agora os modelos usando o método de Validação Cruzada.
	
5. Modelos de Machine Learning (usando Validação Cruzada)
	* Random Forest com Validação Cruzada
	* Modelo SVM com Validação Cruzada
	* Conclusões sobre os modelos com a aplicação da Validação Cruzada
		- Como em geral o Random Forest é um modelo de classificação bom, uma vez também que é baseado em Ensemble, vamos escolher tal modelo como sendo nosso modelo de classificação (com cv=30), uma vez que se comparado aos outros modelos analisados aqui ele é o com melhores métricas.

Tal escolha se faz principalmente pelo fato do tempo para uma análise ainda mais profunda (com técnicas de sintonia de hiperparâmetros, por exemplo) ser limitado.
	
6. Implementação do nosso modelo Random Forest com Validação Cruzada

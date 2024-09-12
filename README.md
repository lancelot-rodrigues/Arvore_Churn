Previsão de Churn de Clientes com Machine Learning

Este projeto utiliza técnicas de Machine Learning para prever a probabilidade de churn (evasão) de clientes de uma agência bancária. O objetivo é identificar os clientes com maior risco de cancelar o serviço para que a empresa possa tomar medidas preventivas. A seguir, detalhamos o passo a passo de como o modelo foi construído.
Passo a Passo da Construção do Modelo

1. Introdução
   
Empresas orientadas por dados maximizam seus resultados ao utilizar informações extraídas dos dados para tomar decisões. A retenção de clientes é um indicador chave de qualidade do serviço; portanto, prever o churn é essencial para minimizar a perda de clientes. Este projeto demonstra como aplicar um modelo de Machine Learning para prever quais clientes estão em risco de churn.

3. Importação dos Dados

Os dados utilizados neste projeto foram coletados de um conjunto de dados de churn de uma agência bancária. Eles foram importados diretamente de um repositório público no GitHub para garantir acesso fácil e rápido.

4. Análise Exploratória dos Dados

Antes de modelar, foi realizada uma análise exploratória dos dados para entender as variáveis mais relevantes. Essa análise incluiu:
•	Verificação de valores nulos ou inconsistências.
•	Análise de correlação entre as variáveis.
•	Entendimento das distribuições dos dados, especialmente as variáveis de entrada (ex.: idade, saldo, número de produtos, etc.).

5. Pré-Processamento dos Dados

O pré-processamento é um passo crítico para a construção de modelos de Machine Learning. As seguintes etapas foram realizadas:
•	Normalização dos dados: Foi utilizado o StandardScaler para normalizar os dados numéricos, garantindo que todas as variáveis estivessem na mesma escala.
•	Codificação de variáveis categóricas: As variáveis categóricas, como o país de origem, foram convertidas para um formato numérico usando técnicas como One-Hot Encoding.

6. Divisão dos Dados

Os dados foram divididos em conjuntos de treino e teste para avaliar o desempenho do modelo:
•	70% dos dados foram usados para treinar o modelo.
•	30% dos dados foram usados para testar e validar o modelo.

7. Treinamento do Modelo
   
O modelo utilizado foi um Random Forest Classifier, escolhido pela sua robustez e precisão em problemas de classificação. O modelo foi treinado utilizando os dados de entrada pré-processados e ajustado para otimizar sua performance.

9. Avaliação do Modelo

A avaliação do modelo foi feita utilizando métricas como:
•	Acurácia: Percentual de previsões corretas.
•	Matriz de Confusão: Para entender os verdadeiros positivos, falsos positivos, etc.
•	AUC-ROC: Medida da capacidade do modelo de distinguir entre classes.
10. Previsão com Dados de Entrada Manual
Para tornar o modelo mais interativo, foi implementada uma funcionalidade que permite a inserção manual dos dados do cliente, possibilitando prever a probabilidade de churn em tempo real. O usuário pode inserir características do cliente e obter um resultado imediato.

11. Conclusão

O modelo final permite prever com eficácia os clientes em risco de churn, fornecendo uma ferramenta poderosa para a tomada de decisões preventivas.

Licença
Este projeto é licenciado sob a Licença MIT, o que significa que você pode utilizá-lo, modificá-lo e distribuí-lo livremente, desde que mantenha os créditos aos autores originais e inclua uma cópia da licença em quaisquer distribuições.

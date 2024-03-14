# Projeto de Vendas de Veículos

## Análise Exploratória de Dados

Como primeira parte do projeto, dei início a uma análise exploratória dos dados, avaliando a relação entre as variáveis e retirando algumas informações pertinentes durante a análise.

- Contagem de vendas mês a mês
- Faturamento mês a mês
- Distribuição de vendas entre os sexos masculino e feminino
- Preferências de compra entre os diferentes estilos de carroceria dos veículos
- Regiões com maior volume de vendas de veículos

Essas e outras análises estão detalhadas no notebook [aqui](https://github.com/A1b3rt0M3rcad0/car_sales_project/blob/main/notebooks/eda.ipynb).

Após a análise, selecionei os gráficos e dados que melhor representam as vendas na base de dados para criar o seguinte dashboard:

![Dashboard](https://raw.githubusercontent.com/A1b3rt0M3rcad0/car_sales_project/main/images/dashboard.png)

## Modelo

Na segunda parte do projeto, iniciei a criação de um modelo capaz de prever tanto o número de vendas do próximo mês quanto o faturamento. Para isso, foram necessárias algumas manipulações nos dados, principalmente nas datas, e uma reorganização dos mesmos. A partir disso, foram criadas novas colunas, como:

- Billing/Sellings (Faturamento por Venda, ou também podemos chamar de ticket médio de venda).
- Média Móvel 3 (duas médias móveis, tanto para a coluna de Sellings quanto para a de Billing).

Após as manipulações, os dados foram agrupados somando mês a mês as vendas e o faturamento. No entanto, devido à baixa quantidade de dados, não foi possível obter a convergência do modelo. Para que isso fosse possível, seria necessário coletar mais dados e realizar um novo experimento. Foram utilizadas métricas como Mean Squared Error (MSE) e Mean Absolute Error (MAE) para avaliar o desempenho do modelo. 

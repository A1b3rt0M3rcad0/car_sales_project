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

Na segunda fase do projeto, dei início à construção de um modelo com o objetivo de prever tanto o número de vendas do próximo mês quanto o faturamento. Para isso, precisei realizar diversas manipulações nos dados, principalmente relacionadas às datas, além de reorganizá-los de forma adequada. Durante esse processo, foram criadas novas colunas, incluindo:

- Billing/Sellings (Faturamento por Venda, ou também conhecido como ticket médio de venda).
- Média Móvel 3 (duas médias móveis, tanto para a coluna de Sellings quanto para a de Billing).
  
Após as manipulações, os dados foram agregados mensalmente, somando as vendas e o faturamento de cada mês. No entanto, devido à escassez de dados disponíveis, não foi possível alcançar a convergência do modelo. Para resolver essa questão, seria necessário coletar mais dados e realizar um novo experimento. Durante a avaliação do desempenho do modelo, foram utilizadas métricas como Mean Squared Error (MSE) e Mean Absolute Error (MAE).

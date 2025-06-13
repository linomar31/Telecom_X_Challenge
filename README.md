# Análise de Evasão de Clientes (Churn) na Telecom X

Este projeto consiste na análise exploratória de dados para identificar os fatores que levam os clientes da Telecom X a cancelar seus serviços. O objetivo é fornecer insights que possam ser utilizados para desenvolver estratégias eficazes de retenção de clientes.

## Sumário

- [Introdução](#introdução)
- [Limpeza e Tratamento de Dados](#limpeza-e-tratamento-de-dados)
- [Análise Exploratória de Dados](#análise-exploratória-de-dados)
- [Conclusões e Insights](#conclusões-e-insights)
- [Recomendações](#recomendações)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)

## Introdução

A evasão de clientes (churn) é um desafio significativo para empresas de telecomunicações. Compreender por que os clientes cancelam é fundamental para melhorar a satisfação, aumentar a retenção e garantir o crescimento sustentável. Esta análise explora um conjunto de dados de clientes da Telecom X para desvendar os principais motivadores do churn.

## Limpeza e Tratamento de Dados

Os dados foram obtidos de um arquivo JSON e processados utilizando a biblioteca Pandas. As principais etapas de limpeza e tratamento incluíram:

- **Normalização de Dados:** Dicionários aninhados foram expandidos em colunas separadas.
- **Tratamento de Valores Nulos:** Valores ausentes na coluna 'TotalCharges' foram preenchidos com a mediana.
- **Padronização de Nomes:** Nomes de colunas foram convertidos para minúsculas e espaços substituídos por underscores.
- **Conversão de Tipos de Dados:** Colunas categóricas binárias (Yes/No, Male/Female) e a variável alvo Churn foram convertidas para representação numérica (1/0).

## Análise Exploratória de Dados

A análise exploratória utilizou visualizações gráficas para identificar padrões e tendências. Abaixo estão alguns dos gráficos gerados:

### Distribuição de Clientes que Cancelaram

Este gráfico mostra a proporção de clientes que cancelaram em relação ao total.

![Distribuição de Churn](https://github.com/linomar31/Telecom_X_Challenge/blob/main/gr%C3%A1ficos/cancelaram%20ou%20n%C3%A3o.png)

### Distribuição de Cancelamento por Gênero

Este gráfico compara a taxa de churn entre clientes masculinos e femininos.

![Churn por Gênero](https://github.com/linomar31/Telecom_X_Challenge/blob/main/gr%C3%A1ficos/genero.png)

### Distribuição de Cancelamento por Tipo de Contrato

Este gráfico ilustra como o tipo de contrato influencia a taxa de churn.

![Churn por Contrato](https://github.com/linomar31/Telecom_X_Challenge/blob/main/gr%C3%A1ficos/tipo_contrato.png)

### Distribuição de Encargos Mensais por Cancelamento

Este histograma compara a distribuição dos encargos mensais para clientes que cancelaram e não cancelaram.

![Encargos Mensais por Churn](https://github.com/linomar31/Telecom_X_Challenge/blob/main/gr%C3%A1ficos/encargos_mensais.png)

### Distribuição de Encargos Totais por Cancelamento

Este histograma compara a distribuição dos encargos totais para clientes que cancelaram e não cancelaram.

![Encargos Totais por Churn](https://github.com/linomar31/Telecom_X_Challenge/blob/main/gr%C3%A1ficos/encargos_totais.png)

### Distribuição de Tempo de Contrato por Cancelamento

Este histograma compara a distribuição do tempo de contrato (tenure) para clientes que cancelaram e não cancelaram.

![Tempo de Contrato por Churn](https://github.com/linomar31/Telecom_X_Challenge/blob/main/gr%C3%A1ficos/tempo_contrato_meses.png)

## Conclusões e Insights

A análise revelou que os principais fatores associados ao churn na Telecom X incluem:

- **Contratos Mensais:** Clientes com contratos de curto prazo apresentam uma probabilidade significativamente maior de cancelar.
- **Tempo de Contrato (Tenure):** Clientes novos com pouco tempo de contrato são mais suscetíveis ao churn.
- **Encargos Mensais:** Clientes com encargos mensais mais altos tendem a ter uma maior probabilidade de churn.

## Recomendações

Com base nos insights, recomendamos as seguintes ações para a Telecom X:

1.  **Foco na Retenção de Clientes Novos:** Implementar programas de integração e acompanhamento nos primeiros meses.
2.  **Incentivo a Contratos de Longo Prazo:** Oferecer benefícios atraentes para clientes que optarem por contratos anuais ou bienais.
3.  **Análise de Preços:** Avaliar a estrutura de preços dos planos, especialmente para os de maior custo.
4.  **Fortalecer Serviços de Valor Agregado:** Investigar a influência de serviços adicionais no churn e aprimorá-los se necessário.
5.  **Segmentação de Clientes:** Identificar clientes em maior risco de churn e direcionar campanhas de retenção personalizadas.

## Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

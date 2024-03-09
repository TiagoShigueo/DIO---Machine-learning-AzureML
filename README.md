# Passo a passo AzureML
## Configurações básicas
- Nome do trabalho: mslearn-bike-automl
- Nome do novo experimento: mslearn-bike-rental
- Descrição: Automated machine learning for bike rental prediction

## Tipo de tarefa e dados
- Selecione o tipo de tarefa: Regressão
- Criar novo dataset

### Tipo de dado
- Nome: bike-rentals
- Descrição: Historic bike rental data
- Tipo: Tabular

### Origem do dado
- Arquivo WEB
- WEB URL: https://aka.ms/bike-rentals

### Configurações
- Tipo de formato: Delimitado
- Delimitador: Vírgula
- Codificação: ETF-8
- Cabeçalho: Somente o primeiro arquivo possui cabeçalho

- Selecionar Criar
- Marcar bike-rentals para continuar a automação

## Configuração da tarefa
- Coluna alvo: Rentals (integer)

### Configurações adicionais
- Métrica primária: Normalized root mean squared error

### Limitações
- Max trials: 3
- Max concurrent trials: 3
- Max nodes: 3
- Metric score threshold: 0.085
- Timeout: 15
- Iteration timeout: 15
- Enable early termination: Selected
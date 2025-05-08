# Telecom X - Análise de Evasão de Clientes

Este projeto realiza uma análise exploratória de dados (EDA) sobre a evasão de clientes (churn) da empresa fictícia Telecom X. O objetivo é entender os padrões de cancelamento e fornecer insights úteis para reduzir a perda de clientes.

## Estrutura do Projeto

```
telecom_x_churn_analysis/
├── data/
│   └── telecom_churn.csv          # Dados brutos fornecidos
│   └── telecom_churn_clean.csv    # Dados limpos após o ETL
├── results/
│   └── churn_distribution.png     # Gráfico da distribuição de churn
│   └── churn_por_contrato.png     # Gráfico de churn por tipo de contrato
│   └── tenure_vs_charges.png      # Gráfico de tenure vs. fatura mensal
├── telecom_churn_analysis.py      # Script principal com ETL e EDA
└── README.md                      # Descrição do projeto
```

## O que o script faz

1. **Carrega os dados**: Lê o arquivo CSV com os dados dos clientes.
2. **Trata os dados**: Remove duplicatas, trata valores ausentes e erros de formatação.
3. **Cria colunas adicionais**: Gera a coluna `Contas_Diarias` com base no faturamento mensal.
4. **Padroniza valores binários**: Converte "Sim"/"Não" e similares em 1 e 0.
5. **Apresenta estatísticas descritivas**: Média, mediana, desvio padrão e outras métricas.
6. **Gera visualizações**: Cria gráficos úteis para identificar padrões e tendências.

## Como executar

1. Instale as bibliotecas necessárias:
```bash
pip install pandas matplotlib seaborn
```

2. Execute o script:
```bash
python telecom_churn_analysis.py
```

3. Verifique os resultados na pasta `results/`.

## Objetivo

Ajudar a equipe de Data Science da Telecom X a entender os motivos da evasão e embasar estratégias para retenção de clientes.

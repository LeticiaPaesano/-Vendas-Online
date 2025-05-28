# 📊 Vendas Online

## 🎯 Objetivo

Este projeto tem como objetivo analisar os resultados de um evento promocional de 5 dias realizado por uma empresa de vendas online. A proposta é identificar o(a) cliente com a maior compra durante o período, premiar esse cliente e fornecer subsídios para decisões comerciais futuras baseadas em dados.

---

## 🗂️ Conjunto de Dados

O arquivo de entrada é um JSON chamado `dados_vendas_clientes.json`, contendo:

- **Data da venda**: data em que ocorreram as compras;
- **Cliente**: lista com nomes dos clientes que compraram no respectivo dia;
- **Valor da compra**: lista com os valores pagos por cada cliente no mesmo dia.

> Estrutura aninhada por dia de venda, exigindo tratamento com `json_normalize` e reestruturação manual.

---

## 🛠️ Tecnologias Utilizadas

- Python 3.11+
- [Pandas](https://pandas.pydata.org/) (tratamento e análise de dados)
- Google Colab (ambiente de desenvolvimento)
- JSON (formato de entrada)

---

## ⚙️ Etapas do Projeto

### 1. Importação dos dados
Leitura do arquivo `.json` com a biblioteca `json` e acesso à chave principal `dados_vendas`.

### 2. Normalização da estrutura
Transformação de listas aninhadas (clientes e valores) em registros linha a linha com estrutura tabular.

### 3. Criação do DataFrame
Construção do DataFrame `df_vendas`, contendo:
- `Data da compra`
- `Cliente`
- `Valor da compra` (convertido de string com símbolo `R$` para `float`)

### 4. Análise da maior compra
Identificação do índice da maior compra no período e extração do cliente vencedor, com apresentação formatada do resultado.

---

## 🏆 Resultado Final

O projeto identificou corretamente o(a) cliente com a maior compra da semana, fornecendo:
- Nome do cliente
- Valor da compra (formato monetário)
- Data da compra

---

## 👩‍💻 Autora

Letícia – Cientista de Dados em formação, com foco em dados comerciais e financeiros.  

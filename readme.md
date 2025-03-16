# Estrutura do Projeto de IA para Análise de Vendas

## Objetivo
O projeto consiste em uma estrutura de dados de vendas de produtos em três sites. Os dados brutos serão analisados por uma IA Self Service, onde o cliente poderá interagir para obter insights e tomar decisões estratégicas. As respostas geradas pela IA serão disponibilizadas no formato de tabela.

## Estrutura de Diretórios
A organização do projeto segue a seguinte estrutura:

```
dataset-gameshop/
│-- data/
│   │-- processed_data/
│   │   ├── meganium_sales_data.xlsx
│   │-- raw_data/
│   │   ├── meganium_sales_data_aliexpress.csv
│   │   ├── meganium_sales_data_etsy.csv
│   │   ├── meganium_sales_data_shopee.csv
│-- insights/
│   ├── keep.me
│-- prompts/
│   ├── chatgpt_prompts.md
│-- scripts/
```

### Conteúdo das Pastas

- **data/**: Armazena os dados de vendas, incluindo os dados brutos e processados.
  - **processed_data/**: Contém `meganium_sales_data.xlsx`, um arquivo consolidado de dados processados.
  - **raw_data/**: Contém os arquivos de vendas brutos extraídos de diferentes plataformas:
    - `meganium_sales_data_aliexpress.csv`
    - `meganium_sales_data_etsy.csv`
    - `meganium_sales_data_shopee.csv`

- **insights/**: Contém arquivos de análise de dados gerados pelo sistema. Inclui `keep.me` como marcador.

- **prompts/**: Contém prompts utilizados para gerar insights na IA. O arquivo `chatgpt_prompts.md` contém as perguntas e respostas extraídas dos dados.

- **scripts/**: Pasta destinada a armazenar scripts utilizados no processamento e análise dos dados.

## Exemplos de Insights Gerados pela IA

### Qual mês do ano teve mais vendas?

O mês com maior volume de vendas foi **agosto de 2024**, com um total de **4.310** vendas.

| Mês        | Total de Vendas |
|------------|:---------------:|
| Maio/2024  | 1040            |
| Junho/2024 | 1770            |
| Julho/2024 | 2300            |
| Agosto/2024| 4310            |
| Setembro/2024 | 3430        |
| Outubro/2024  | 3080        |

### Qual comprador fez mais de uma compra?

- Não há registros de clientes que realizaram mais de uma compra com base nos dados disponíveis.

### Qual é o produto mais vendido por país?

| País        | Produto Mais Vendido | Quantidade |
|------------|---------------------|------------|
| Austrália  | CubeXX              | 13         |
| Canadá     | 40XXV               | 19         |
| França     | 35XX                | 12         |
| Alemanha   | 40XXV               | 7          |
| Japão      | 40XXV               | 11         |
| Reino Unido| 35XX                | 7          |
| EUA        | RG353M              | 4          |

### Qual é o produto mais vendido por site?

| Site       | Produto Mais Vendido | Quantidade |
|-----------|----------------------|------------|
| AliExpress | 35XX                | 14         |
| Etsy       | 40XXV                | 17         |
| Shopee     | CubeXX               | 18         |

### Qual é o país que mais compra nossos produtos?

| País        | Quantidade Comprada |
|------------|---------------------|
| Canadá     | 46                  |
| França     | 36                  |
| Austrália  | 28                  |
| Japão      | 27                  |
| Alemanha   | 23                  |
| Reino Unido| 13                  |
| EUA        | 5                   |

### Maior desconto aplicado por site

| Site       | Maior Desconto Aplicado |
|-----------|-------------------------|
| AliExpress | 105.86                 |
| Etsy       | 137.78                 |
| Shopee     | 158.09                 |

### Produto mais caro e mais barato

| Categoria    | Produto | Preço Unitário |
|-------------|---------|---------------|
| Mais Caro   | RG353M  | 110           |
| Mais Barato | 28XX    | 70            |


# DOCUMENTAÇÃO

## Objetivo:

Crir um modelo de análise de dados que faça a classificação dos clientes, por meio de um score de crédito, a partir da análise de dados e a avaliação do rsico relativo que possa classificar os solicitantes em diferentes categorias de risco com base em sua probabilidade de inadimplência. utilize a mattriz de confusão e a realização de consultas complexas no BigQuery.

## Case

Com a diminuição das taxas de juros, aumentou-se a demanda por crédito e o Banco "Super Caja" esta enferentando dificuldades para realizar a análise de crédito pois seu processo de análise pe manual.
Diante disto, propõe-se uma solução de automação do processo de análise por meio de técnicas avançadas de análise de dados. O objetivo é melhorar a eficiência e a precisão na avaliação de risco de crédito e reduzir o risco de empréstimos não reembolsáveis.
Esta proposta também destaca a integração de uma métrica existente de pagamento em atraso, fortalecendo assim a capacidade do modelo.

## Ferramentas utilizadas:

Google BigQuery: Data warehouse que permite o processamento de grandes volumes de dados.
Google Colab: Plataforma para trabalhar com a linguagem de programação Python em Notebooks.
Apresentações Google: ferramenta para  criação e edição de apresnetações.
Google Looker Studio: ferramenta para criação e edição de painéis e relatórios de dados.

## Linguagens utilizadas:

SQL no BigQuery e Python no Google Colab.

## Base de dados utilizadas:

Os dados estão divididos em 4 tabelas:

![Arquivos_base de dados](https://github.com/keiladelre/Projeto-Risco-Relativo/assets/171286176/b2e593c7-0ebf-4d30-91e4-1b6ceb5bc896)

- Dados do usuário/ cliente.
  
  ![Campos_tabela 1](https://github.com/keiladelre/Projeto-Risco-Relativo/assets/171286176/581dd14a-ada9-41f6-8911-f25de92c6ddf)

- Dados do tipo de empréstimo.
  
![Campos_tabela 2](https://github.com/keiladelre/Projeto-Risco-Relativo/assets/171286176/e73b37cc-f617-4129-9c75-deb353990504)
 
- Comportamento de pagamento desses empréstimos.
  
![Campos_tabela 3](https://github.com/keiladelre/Projeto-Risco-Relativo/assets/171286176/c5262b36-fbd1-460c-a906-b8b0f544b161)

- Informação dos clientes já identificados como inadimplentes.
  
![Campos tabela 4](https://github.com/keiladelre/Projeto-Risco-Relativo/assets/171286176/fc871396-2233-42c1-bccd-ac6b024f5142)


## Processar e preparar a base de dados:

- Conectar/ importar dados para a ferramenta.

Após baixar os 4 arquivos .csv, importei os arquivos para o Google BigQuery, criando uma tabela para cada arquivo, sem alterar os nomes dos arquivos:

![Tabelas BigQuery](https://github.com/keiladelre/Projeto-Risco-Relativo/assets/171286176/39a23ffa-100c-45ac-a6bd-b50ca8e0e7b4)




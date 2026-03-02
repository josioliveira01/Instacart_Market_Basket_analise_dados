# 🥕 Instacart Market Basket Analysis

Este projeto simula o fluxo de trabalho real de um Analista de Dados, utilizando o dataset anonimizado da plataforma **Instacart** disponível no Kaglle. O objetivo central é transformar dados brutos em inteligência de mercado, focando em sazonalidade, retenção e estratégias de recomendação baseadas em afinidade.

## 🚀 Objetivos do Projeto
**Analisar os dados**: Analisar os dados anonimizados de 3 milhões de pedidos de supermercado de mais de 200.000 usuários do Instacart, disponibilizados de forma aberta pelo Instacart.  
**Data Wrangling**: Limpeza e união de múltiplas tabelas relacionais.  
**Análise Exploratória (EDA)**: Identificação de padrões de sazonalidade e retenção de usuários.  
**Market Basket Analysis**: Aplicação do algoritmo Apriori para identificar associações de alta afinidade.

## 📂 Estrutura do Pipeline (Notebooks)
O projeto foi desenvolvido em ambiente local (VS Code/Python):

1.  **`01_ingestao_e_exploracao.ipynb`**: Ingestão via API do Kaggle e inspeção inicial de qualidade.
2.  **`02_preparacao_dados_etl.ipynb`**: Processo de ETL e integração das tabelas `orders`, `products`, `departments` e `aisles`.
3.  **`03_analise_descritiva_base_integrada.ipynb`**: Análise estatística de 3,2 milhões de pedidos e 206 mil clientes.
4.  **`04_outras_analises.ipynb`**: Extração de padrões comportamentais, cálculo de **Lift** e mapeamento de fluxo inter-departamental.

## 🛠️ Tecnologias Utilizadas

**Linguagem:** Python   
**Ambiente:** VS Code  
**Bibliotecas de Dados:** Pandas, Mlxtend (Apriori/Association Rules)

## 📈 Insights Estratégicos

### 1. Sazonalidade e Comportamento
**Janela de Oportunidade**: Picos de pedidos concentrados aos **domingos e segundas-feiras**, com ápice de conversão entre **10h e 16h**.  
**Ciclo de Retorno**: 50% dos clientes realizam novos pedidos em até 8 dias, com um forte hábito de recompra semanal (pico no 7º dia).  
**Fidelização**: Identificamos um gargalo crítico de retenção entre o **4º e o 10º pedido** por usuário.

### 2. O "Segundo Caminho" do Cliente

Ao aplicar uma técnica de **filtragem por exclusão** no departamento de Hortifrúti (Produce), mapeamos o fluxo real de transição:  
**24,6%** dos clientes migram imediatamente para **Laticínios e Ovos** após garantirem seus itens frescos.

## 🧪 Planos de Validação (Testes A/B)
**Upselling**: Validar se a recomendação direta de Bananas para compradores de Maçãs reduz a fricção e aumenta o número de itens na cesta.
**Conversão de Cesta**: Exibir atalhos para Laticínios assim que o segundo item de Hortifrúti for adicionado, visando o fechamento da "Cesta Essencial".

## 🚧 Limitações e Futuro
O algoritmo Apriori trata transações como conjuntos simultâneos. Para exploração futura, recomenda-se o uso da métrica **`add_to_cart_order`** para mapear o funil de decisão em tempo real, identificando gatilhos de consumo e momentos de maior suscetibilidade ao impulso.

## 📄 Documentação Técnica e Estratégica
Para uma análise detalhada de cada etapa do projeto, incluindo gráficos e planos de ação, acesse o relatório completo:

[![Relatório em PDF]()](https://github.com/josioliveira01/Instacart_Market_Basket_analise_dados/blob/main/Instacart_Documenta%C3%A7%C3%A3o_projeto.pdf)

## 📊 Visualização dos Dados
Os resultados das análises foram consolidados em um dashboard executivo para facilitar a tomada de decisão da equipe de Marketing.

[![Visualizar Dashboard](https://img.shields.io/badge/Acessar-Dashboard_PDF-blue?style=for-the-badge&logo=google-analytics)](https://github.com/josioliveira01/Instacart_Market_Basket_analise_dados/blob/main/dash_supermercado.pdf)

## 🎤 Apresentação (Slides)
Este documento foi estruturado para uma reunião de tomada de decisão com a equipe de Marketing, traduzindo métricas estatísticas em planos de ação claros.

[![Visualizar Slides](https://img.shields.io/badge/Acessar-Slides_Apresentação-orange?style=for-the-badge&logo=microsoft-powerpoint)](https://github.com/josioliveira01/Instacart_Market_Basket_analise_dados/blob/main/Apresentação_rotas_consumidores.pdf)


## 👤 Autor

**Josiane de Oliveira da Silva**  
[LinkedIn – Josiane de Oliveira da Silva](https://www.linkedin.com/in/josioliveirasilva/?locale=en_US)

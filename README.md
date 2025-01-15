# Segmentação de Clientes

## Visão Geral

Este projeto tem como objetivo segmentar clientes utilizando análise de dados, técnicas estatísticas e algoritmos de clusterização (K-Means). O objetivo é identificar grupos de clientes com características semelhantes e fornecer insights estratégicos para otimizar campanhas de marketing.

## Base de Dados

- **Fonte:** Kaggle - Customer Personality Analysis
- **Data da Extração:** 2 de janeiro de 2025

## Objetivos

- Realizar análise exploratória e estatística para identificar padrões de comportamento dos clientes.
- Criar variáveis derivadas para melhorar a clusterização.
- Aplicar PCA (Análise de Componentes Principais) para reduzir a dimensionalidade de variáveis contínuas.
- Utilizar o algoritmo K-Means para agrupar clientes em segmentos distintos.
- Gerar insights acionáveis para apoiar decisões de negócios.

## Principais Variáveis

- **Educação:** Simplificada em "Sem Graduacao," "Graduacao" e "Pos_Graduacao."
- **Total_Gastos:** Total gasto pelo cliente.
- **Idade:** Idade do cliente calculada a partir do ano de nascimento.
- **Filhos:** Total de crianças (crianças + adolescentes) em um domicílio.
- **Convivencia:** Classificada como "Sozinho(a)" (solteiro) ou "Parceiro(a)" (com parceiro).
- **Anos_Relacionamento:** Tempo de relacionamento com a empresa em anos.

## Técnicas e Ferramentas

- **Análise Exploratória de Dados (EDA):** Entendimento de distribuições, correlações e outliers.
- **Testes Estatísticos:** Shapiro-Wilk, Mann-Whitney U, ANOVA, teste de Dunn.
- **Redução de Dimensionalidade:** PCA para variáveis contínuas.
- **Clusterização:** K-Means com avaliação pelos métodos do Cotovelo e Silhueta.
- **Visualizações:** Matplotlib, Seaborn.

## Resultados

### Insights da Segmentação

#### Cluster 0 (Premium)
- **Perfil:** Clientes de alta renda com altos gastos, focados principalmente em produtos premium como vinhos e carnes.
- **Renda média:** Alta, com poder aquisitivo considerável.
- **Preferências:** Produtos de maior valor agregado, como vinhos e carnes.
- **Comportamento de compra:** Utilizam diversos canais, com destaque para lojas físicas e catálogos.
- **Aceitação de campanhas:** Geralmente baixa, indicando que preferem compras não influenciadas por promoções.

#### Cluster 1 (Exclusivos)
- **Perfil:** Clientes de alta renda com comportamento sofisticado e o maior gasto médio por compra.
- **Renda média:** Muito alta.
- **Preferências:** Compram produtos premium e apresentam grande receptividade às campanhas de marketing.
- **Comportamento de compra:** Engajam-se mais com campanhas, utilizando tanto lojas físicas quanto canais digitais.
- **Destaque:** Este cluster apresenta maior potencial para ações promocionais personalizadas, dada sua alta taxa de aceitação de campanhas.

#### Cluster 2 (Estáveis)
- **Perfil:** Famílias de renda média alta com hábitos de consumo equilibrados.
- **Renda média:** Moderada, sustentando um padrão de vida confortável.
- **Preferências:** Equilíbrio entre diferentes categorias de produtos, sem predileção específica.
- **Comportamento de compra:** Regular, com compras bem distribuídas entre os canais disponíveis.
- **Aceitação de campanhas:** Baixa, sugerindo que preferem escolhas independentes.

#### Cluster 3 (Essenciais)
- **Perfil:** Clientes de baixa renda, priorizando compras essenciais e promoções.
- **Renda média:** Baixa, limitando o volume de compras.
- **Preferências:** Produtos básicos e compras com descontos.
- **Comportamento de compra:** Realizam compras em menor quantidade, principalmente em lojas físicas.
- **Destaque:** Alta sensibilidade a preços, com maior engajamento em campanhas que ofereçam benefícios econômicos.

#### Cluster 4 (Econômicos)
- **Perfil:** Famílias de renda média que buscam o melhor custo-benefício.
- **Renda média:** Moderada, mas com foco na economia.
- **Preferências:** Prioridade em promoções e produtos acessíveis.
- **Comportamento de compra:** Compram tanto em lojas físicas quanto digitais, mas sempre priorizando descontos.
- **Aceitação de campanhas:** Baixa, mas podem ser ativados por ofertas atrativas de custo-benefício.

## Principais Descobertas

- **Renda vs. Gastos:** Existe uma forte correlação positiva entre a renda e os gastos. Clientes com maior poder aquisitivo (Clusters Premium e Exclusivos) gastam mais em produtos premium, enquanto aqueles com menor renda (Clusters Essenciais e Econômicos) priorizam o custo-benefício.
- **Preferência de Canal:** As lojas físicas são amplamente preferidas, seguidas por compras online e, por último, catálogos. Clusters de maior renda mostram maior uso do catálogo.
- **Campanhas:** A aceitação geral de campanhas é baixa, mas o Cluster Exclusivos se destaca como o grupo mais receptivo a ofertas direcionadas.

## Conclusões

A análise de segmentação revelou diferenças significativas entre os grupos de clientes, permitindo a criação de estratégias de marketing altamente personalizadas. Exemplos de abordagens incluem:

- **Premium e Exclusivos:** Personalizar promoções de produtos premium (como vinhos e carnes) para maximizar o engajamento e fidelidade. Utilizar canais como catálogos e campanhas exclusivas com maior detalhamento e sofisticação.
- **Essenciais e Econômicos:** Oferecer descontos em produtos básicos e campanhas que destaquem benefícios econômicos. A comunicação pode ser voltada para a relevância do custo-benefício, utilizando canais mais acessíveis como lojas físicas e digitais.
- **Estáveis:** Apesar de possuírem um comportamento equilibrado, podem ser ativados por campanhas que incentivem compras adicionais em categorias onde já possuem hábitos de consumo.

Essa segmentação possibilita maior eficiência em ações promocionais e melhor alocação de recursos, maximizando o impacto em diferentes perfis de clientes.

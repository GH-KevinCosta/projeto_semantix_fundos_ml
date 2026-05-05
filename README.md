# Segmentação de Fundos de Investimento no Brasil com Machine Learning

## Projeto de Parceria | Semantix

Este projeto apresenta uma solução de ciência de dados aplicada ao mercado financeiro. O objetivo é segmentar fundos de investimento brasileiros em grupos semelhantes, utilizando técnicas de análise exploratória de dados e machine learning não supervisionado.

> Este material tem finalidade educacional e não representa recomendação de investimento.

---

## 1. Problema real

O mercado brasileiro possui muitos fundos de investimento com características distintas de patrimônio líquido, número de cotistas, captação, resgate, retorno e volatilidade. Essa variedade torna difícil comparar produtos financeiros de forma objetiva.

A pergunta central do projeto é:

**É possível agrupar fundos de investimento em perfis semelhantes usando dados públicos e machine learning?**

---

## 2. Coleta de dados

A fonte pública planejada para o projeto é o Portal de Dados Abertos da CVM, especialmente os dados de fundos de investimento.

Foram consideradas variáveis como:

- patrimônio líquido médio;
- número médio de cotistas;
- captação total;
- resgate total;
- captação líquida;
- movimentação total;
- retorno no período;
- volatilidade da cota.

Essas variáveis permitem comparar fundos por porte, movimentação, comportamento de retorno e risco.

---

## 3. Análise exploratória

A análise exploratória buscou entender:

- a distribuição do patrimônio líquido dos fundos;
- a relação entre patrimônio líquido e número de cotistas;
- a movimentação relativa dos fundos;
- diferenças de retorno e volatilidade entre perfis;
- possíveis padrões naturais nos dados.

Foram usadas visualizações como histogramas, gráficos de dispersão, gráficos de barras e projeção dos clusters em duas dimensões.

---

## 4. Modelagem

O modelo escolhido foi o **K-means**, uma técnica de machine learning não supervisionado usada para agrupamento.

Antes da modelagem, as variáveis foram padronizadas com `StandardScaler`, pois o K-means é sensível à escala dos dados.

Também foi aplicado **PCA** para reduzir a dimensionalidade e visualizar os grupos encontrados em um plano 2D.

---

## 5. Avaliação do modelo

A avaliação foi feita com **Silhouette Score**, métrica que mede o quanto os grupos formados estão separados e internamente coesos.

O projeto testa diferentes valores de `k` e seleciona o número de clusters com melhor resultado.

---

## 6. Conclusões

O projeto mostra que técnicas de machine learning podem ajudar a transformar dados públicos de fundos de investimento em perfis analíticos interpretáveis.

A segmentação permite identificar grupos como:

- fundos de maior porte;
- fundos menores;
- fundos com maior movimentação;
- fundos com maior retorno e volatilidade.

Essa abordagem pode apoiar análises de mercado, comparação entre fundos e criação de dashboards financeiros.

---

## 7. Arquivos da entrega

Esta entrega contém apenas os arquivos obrigatórios:

- `README.md`: documentação em Markdown;
- `notebook.ipynb`: notebook executado com código, tabelas, gráficos, modelagem e conclusões.

---

## 8. Autor

Nome: Kevin Costa  
Curso: Cientista de Dados  
Projeto: Parceria Semantix  

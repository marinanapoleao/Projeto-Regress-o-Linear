# Projeto Regressão Linear - Previsão do preço de imóveis dadas as variáveis
<img width="1408" height="768" alt="Gemini_Generated_Image_mxzr4dmxzr4dmxzr" src="https://github.com/user-attachments/assets/0ea18e0e-97b6-4ab3-a8b6-660cfcc42fa4" />

## 📌 Sobre o Projeto

Desenvolvimento de modelos de regressão linear simples e múltipla para analisar a relação entre as características de imóveis para aluguel e seus valores, utilizando dados imobiliários e técnicas de análise estatística e Machine Learning.


## 🎯 Objetivo

Aplicar modelos de regressão linear para compreender como as características dos imóveis se relacionam com seus valores e avaliar a capacidade preditiva dos modelos utilizando dados de treino e teste.


## 📋​ Problema de Negócio / Pergunta de Pesquisa

É possível estimar o valor de um imóvel para aluguel a partir de suas características? Em que medida variáveis como metragem, número de quartos, banheiros, suítes e vagas de garagem ajudam a explicar a variação dos valores imobiliários?


## 📊 Fonte de Dados

Dataset ALUGUEL_MOD12.csv, contendo informações sobre imóveis para aluguel, incluindo valor do aluguel, valor do condomínio, metragem, número de quartos, banheiros, suítes e vagas de garagem.


## 🛠️ Tecnologias Utilizadas

- Python
  
- Pandas — manipulação e análise de dados
  
- Matplotlib, Seaborn e Plotly — visualização de dados
  
- Scikit-learn — divisão entre treino e teste e construção dos modelos de regressão linear
  
- Statsmodels — recursos de análise estatística importados no projeto



## 🔍 Metodologia

* Exploração inicial dos dados e verificação dos tipos de variáveis e valores ausentes.


* Análise estatística descritiva e investigação de possíveis valores extremos.


* Criação de categorias para diferenciar imóveis de mercado padrão e de luxo, conforme as faixas identificadas na análise.


* Análise exploratória bivariada, com gráficos para investigar relações entre as variáveis.


* Análise de correlação para identificar associações entre as características dos imóveis e seus valores.


* Separação dos dados em conjuntos de treino e teste.


* Construção e avaliação de modelos de regressão linear simples e múltipla, utilizando o coeficiente de determinação \(R^2\) para avaliar o ajuste.


## 📈 Resultados e Métricas

#### Modelo 1 — Regressão Linear Simples

- Variável independente: Metragem.

- Variável dependente: Valor_Condominio.

*Coeficiente de determinação (R²)*

Treinamento: 64,19%

Teste: 67,05%

Equação da regressão:

\[
Y=-117,84+10,56X
\]

*Y = valor do condomínio; X = metragem do imóvel.*

#### Modelo 2 — Regressão Linear Múltipla

- Variáveis independentes: Valor_Aluguel, Metragem, N_Quartos, N_banheiros, N_Suites, N_Vagas e quatro variáveis categóricas codificadas.

- Variável dependente: Valor_Condominio.

*Coeficiente de determinação (R²)*

Treinamento: 76,47%

Teste: 78,57%

O modelo de Regressão Linear Múltipla apresentou melhor desempenho, explicando aproximadamente 78,57% da variabilidade do valor do condomínio na base de teste.

## 💡Principais Insights e Implicações

- A metragem apresentou forte correlação positiva com o valor do condomínio (r = 0,81).

- A metragem, isoladamente, não explica totalmente o valor do condomínio, indicando a influência de outras características dos imóveis.

- Foi identificada uma correlação forte entre número de suítes e número de banheiros (r = 0,92).

- A análise dos outliers demonstrou a necessidade de considerar imóveis de diferentes padrões de mercado, levando à classificação entre Mercado Padrão e Mercado de Luxo.

- A Regressão Linear Múltipla apresentou desempenho superior ao modelo simples, com aumento do R² de teste de 67,05% para 78,57%.

- Os resultados de treinamento e teste foram próximos, indicando consistência no desempenho dos modelos nessas duas amostras.

*Implicação para o negócio:* a utilização de múltiplas características dos imóveis permite estimativas mais explicativas do valor do condomínio, podendo auxiliar análises comparativas e avaliações do mercado imobiliário.

## 👩‍💻 Sobre a Autora

Desenvolvido por Marina Napoleão — Cientista de Dados / Analista de Dados. 
### LinkedIn <https://www.linkedin.com/in/marina-napoleao/>
### GitHub <https://github.com/marinanapoleao> 

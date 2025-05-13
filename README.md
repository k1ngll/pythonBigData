
# 🎬 Análise de Filmes Sequenciais com Dados do TMDB

## 📌 Sobre o Projeto
Este projeto analisa sequências de filmes com o objetivo de identificar padrões de sucesso em franquias cinematográficas. Utilizamos dados do **Kaggle (TMDB Movies Dataset 2023 - 930k filmes)** e da **API TMDB**, considerando métricas como **ROI**, **avaliação do público**, **popularidade** e **gêneros** para definir sucesso.

## 🛠 Tecnologias Utilizadas
- **Python** para análise de dados
- **Pandas** e **NumPy** para tratamento de dados
- **Matplotlib** e **Seaborn** para visualizações
- **TMDB API** para dados adicionais de coleções/franquias
- **Google Colab** como ambiente de desenvolvimento

## 📊 Etapas do Projeto

### 1️⃣ Coleta de Dados
- Dataset principal: [TMDB Movies Dataset 2023 (Kaggle)](https://www.kaggle.com/datasets/asaniczka/tmdb-movies-dataset-2023-930k-movies)
- Complementação com dados da **TMDB API**, especialmente para identificar franquias (`belongs_to_collection`).

### 2️⃣ Seleção e Limpeza
Colunas mantidas:
- `id`, `title`, `release_date`, `budget`, `revenue`, `vote_average`, `vote_count`, `popularity`, `genres`, `production_companies`, `original_language`

Colunas descartadas:
- `imdb_id`, `original_title`, `status`, `adult`, `runtime`, `spoken_languages`, `tagline`, `overview`, `poster_path`, `backdrop_path`, `homepage`, `production_countries`, `keywords`

### 3️⃣ Definição de Sucesso
Critérios adotados para um filme de franquia ser considerado bem-sucedido:
- **ROI > 0,5**
- **Avaliação ≥ 7,0**
- **Popularidade estável ou crescente**

### 4️⃣ Análise
- Avaliação da performance de filmes dentro de suas franquias.
- Comparação de ROI, nota e popularidade entre o primeiro, segundo e terceiro filmes.
- Impacto de gêneros e produtoras no sucesso das sequências.
- Análise específica de filmes brasileiros (`original_language == 'pt'`).

### 5️⃣ Resultados e Insights
- Identificação de franquias com bom desempenho financeiro e crítico.
- Gêneros que tendem a ter melhores resultados em sequências (ex: ação, aventura).
- Indícios de saturação em certas franquias a partir da terceira sequência.

## 📂 Estrutura do Repositório
```
├── data/                    # Arquivos CSV e dados processados
├── notebooks/               # Notebooks Google Colab
│   ├── 01_coleta_e_limpeza.ipynb
│   ├── 02_analise_exploratoria.ipynb
│   └── 03_modelagem_sucesso.ipynb
├── src/                     # Scripts Python
│   ├── coleta_tmdb.py
│   ├── limpeza.py
│   ├── analise.py
├── README.md                # Este documento
```

## 🚀 Como Executar
1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```
2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
3. Execute os notebooks no Google Colab.

## 👥 Integrantes
- Christian Oliveira  
- Maria Eduarda  
- Rafaela  
- Uiles  
- Sena  

## 📎 Referências
- [TMDB API](https://developer.themoviedb.org/docs)
- [Dataset no Kaggle](https://www.kaggle.com/datasets/asaniczka/tmdb-movies-dataset-2023-930k-movies)
- [Pandas](https://pandas.pydata.org/)
- [Matplotlib](https://matplotlib.org/)
- [Seaborn](https://seaborn.pydata.org/)

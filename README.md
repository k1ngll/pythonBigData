# 🌱 Previsão Climática para Agricultura na Bahia

## 📌 Sobre o Projeto
Este projeto tem como objetivo coletar, analisar e prever condições climáticas na Bahia para auxiliar no planejamento agrícola. Utilizamos a **API WeatherAPI** para obter dados históricos e em tempo real sobre temperatura, precipitação e velocidade do vento, permitindo estimar a viabilidade de cultivos em diferentes meses do ano.

## 🛠 Tecnologias Utilizadas
- **Python** para processamento de dados e análise estatística
- **Pandas e NumPy** para manipulação e tratamento de dados
- **Matplotlib e Seaborn** para visualização de dados
- **Scikit-learn** para modelagem e previsões
- **Streamlit** para criar um dashboard interativo

## 📊 Etapas do Projeto

### 1️⃣ Coleta de Dados
- Usamos a **WeatherAPI** para obter dados históricos e atuais do clima em diversas cidades da Bahia.
- Os dados incluem **temperatura média mensal, dias chuvosos e velocidade do vento**.

### 2️⃣ Análise Exploratória
- Limpeza e organização dos dados (remoção de valores nulos e outliers).
- Cálculo de **médias mensais e sazonais**.
- Identificação de padrões climáticos regionais.

### 3️⃣ Modelagem de Dados
- Testamos modelos de **Machine Learning**, incluindo:
  - **Regressão Linear** para prever temperatura
  - **Modelo ARIMA** para prever chuvas e vento
  - **Redes Neurais** para uma abordagem mais robusta
- Comparação dos modelos para escolher o mais eficiente.

### 4️⃣ Visualização dos Dados
- Criamos **gráficos interativos** para facilitar a análise.
- Utilizamos **Streamlit** para desenvolver um **dashboard dinâmico** que exibe previsões futuras.

### 5️⃣ Conclusão e Recomendações
- Identificação dos **melhores meses para o plantio de culturas específicas**.
- Sugestão de estratégias para lidar com seca ou excesso de chuvas.

## 📂 Estrutura do Repositório
```
├── data/               # Dados brutos e tratados
├── notebooks/          # Jupyter Notebooks para análise
├── src/               # Código-fonte do projeto
│   ├── coleta.py      # Script para coletar dados da API
│   ├── analise.py     # Análise exploratória dos dados
│   ├── modelagem.py   # Modelos de previsão climática
│   ├── visualizacao.py # Gráficos e dashboards
├── README.md          # Documento atual
```

## 🚀 Como Executar o Projeto
1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```
2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
3. Execute a coleta de dados:
   ```bash
   python src/coleta.py
   ```
4. Rode a análise exploratória e modelagem:
   ```bash
   python src/analise.py
   python src/modelagem.py
   ```
5. Execute o dashboard para visualizar os resultados:
   ```bash
   streamlit run src/visualizacao.py
   ```

## 📌 Integrantes
- Christian Oliveria
- Maria Eduarda
- Rafaela
- Uiles
- Sena

## 📎 Referências
- [WeatherAPI](https://www.weatherapi.com/) - Fonte dos dados climáticos
- [Scikit-learn](https://scikit-learn.org/) - Machine Learning
- [Streamlit](https://streamlit.io/) - Dashboard interativo




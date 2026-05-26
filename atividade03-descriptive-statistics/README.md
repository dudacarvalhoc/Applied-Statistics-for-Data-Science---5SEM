# 📊 Atividade 03 — Estatística Descritiva com Python
 
**Disciplina:** Estatística Aplicada à Ciência de Dados
**Grupo:** CTRL + ALT + DELAS
 
## 👥 Integrantes
 
| Nome | RA |
|------|-----|
| Maria Eduarda Cortellini | 52420167 |
| Karen Arwen | 52420075 |
| Beatriz Antunes | 52420663 |
| Luiz Franzon | 52421183 |
| Daniele Tavares | 52420099 |
| Giovanna Fogaça | 52421068 |
 
---
 
## 🎯 Objetivo
 
Aplicar técnicas de **estatística descritiva** sobre um dataset de **restaurantes no Brasil**, utilizando medidas de tendência central, dispersão e visualizações gráficas para compreender o comportamento dos dados.
 
---
 
## 📦 Sobre os dados
 
- **Dataset:** Restaurantes no Brasil
- **Formato:** CSV
- **Variáveis principais:**
  - `faturamento_mensal` — faturamento mensal do restaurante
  - `lucro_estimado` — lucro estimado
  - `ticket_medio` — valor médio por pedido
  - `numero_pedidos_dia` — quantidade de pedidos por dia
  - `nota_media` — avaliação média do restaurante
  - `tipo` — tipo/categoria do restaurante
---
 
## 🛠️ Bibliotecas utilizadas
 
- `pandas` — manipulação de dados
- `numpy` — operações numéricas
- `matplotlib` — visualizações
---
 
## 📈 Análises realizadas
 
### 1️⃣ Exploração inicial
- Visualização das primeiras linhas
- Dimensões do dataset (`shape`)
- Informações gerais (`info`)
- Identificação de valores ausentes
### 2️⃣ Estatística descritiva — Faturamento mensal
- Média, mediana, moda
- Variância e desvio padrão
- Amplitude, mínimo e máximo
### 3️⃣ Estatística descritiva — Nota média
- Mesmas medidas aplicadas para análise de avaliações
### 4️⃣ Visualizações
- 📉 Histograma do faturamento mensal
- 📦 Boxplot do faturamento mensal
- 📊 Histograma da nota média
- 🔵 Scatter plot: Faturamento × Lucro estimado
- 📊 Gráfico de barras: Faturamento médio por tipo de restaurante
### 5️⃣ Análise de correlação
Matriz de correlação entre: `faturamento_mensal`, `lucro_estimado`, `numero_pedidos_dia`, `ticket_medio`, `nota_media`
 
---
 
## 💡 Conclusões
 
- A análise estatística descritiva permitiu compreender o comportamento dos dados de restaurantes
- Medidas de tendência central (média, mediana, moda) e dispersão (variância, desvio padrão, amplitude) ajudaram a identificar padrões e variações
- Os gráficos facilitaram a visualização da distribuição e da relação entre variáveis
- As bibliotecas Pandas, NumPy e Matplotlib se mostraram eficientes para manipulação, análise e visualização
---
 
## 📁 Estrutura da pasta
 
```
atividade-03-estatistica-descritiva/
├── README.md
├── notebook/
│   └── codigo_atv03.ipynb
└── data/
    └── dataset_restaurantes_brasil.csv
```
 
---
 
## ▶️ Como executar
 
1. Clone o repositório
2. Instale as dependências:
   ```bash
   pip install pandas numpy matplotlib
   ```
3. Abra o notebook no Jupyter, Google Colab ou VSCode
4. Ajuste o caminho do CSV conforme seu ambiente:
   ```python
   df = pd.read_csv('caminho/para/dataset_restaurantes_brasil.csv')
   ```

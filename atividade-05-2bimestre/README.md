# 😴 Atividade 05 — EDA: Sleep Health and Lifestyle
 
**Disciplina:** Estatística Aplicada à Ciência de Dados (APEX)
**Bimestre:** 2º
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
 
Realizar uma **Análise Exploratória de Dados (EDA)** completa sobre o *Sleep Health and Lifestyle Dataset*, investigando padrões de sono e como eles se relacionam com fatores demográficos, de saúde e comportamentais.
 
---
 
## 📦 Sobre os dados
 
- **Dataset:** Sleep Health and Lifestyle Dataset
- **Fonte:** [Kaggle](https://www.kaggle.com/)
- **Registros:** 374 indivíduos
- **Colunas:** 13 variáveis
### Variáveis principais
 
| Variável | Tipo | Descrição |
|----------|------|-----------|
| `Gender` | Categórica | Gênero |
| `Age` | Numérica | Idade |
| `Occupation` | Categórica | Profissão |
| `Sleep Duration` | Numérica | Duração do sono (horas) |
| `Quality of Sleep` | Numérica | Qualidade do sono (1–10) |
| `Physical Activity Level` | Numérica | Nível de atividade física |
| `Stress Level` | Numérica | Nível de estresse |
| `BMI Category` | Categórica | Categoria de IMC |
| `Blood Pressure` | Texto | Pressão arterial (sistólica/diastólica) |
| `Heart Rate` | Numérica | Frequência cardíaca |
| `Daily Steps` | Numérica | Passos diários |
| `Sleep Disorder` | Categórica | Distúrbio do sono |
 
---
 
## 🛠️ Bibliotecas utilizadas
 
- `pandas` — manipulação de dados
- `numpy` — operações numéricas
- `matplotlib` — visualizações base
- `seaborn` — visualizações estatísticas
---
 
## 🔄 Etapas da análise
 
### 0️⃣ Preparação do ambiente
Importação de bibliotecas e configuração do estilo visual.
 
### 1️⃣ Carregamento e inspeção inicial
Dimensões, primeiras/últimas linhas, tipos de dados e estatísticas descritivas.
 
### 2️⃣ Qualidade dos dados
- Tratamento dos NaN em `Sleep Disorder` como categoria `"None"` (não são valores faltantes — representam ausência de distúrbio)
- Identificação e documentação de duplicatas
- Remoção da coluna `Person ID` (sem valor analítico)
- **Separação de `Blood Pressure`** em `Systolic_BP` e `Diastolic_BP`
- Padronização de categorias (`Normal Weight` → `Normal`)
### 3️⃣ Análise univariada
- Medidas resumo das variáveis numéricas
- Histogramas e boxplots
- Tabelas de frequência das variáveis categóricas
### 4️⃣ Análise bivariada
- Matriz de correlação (Pearson)
- Estresse × Qualidade do sono
- Duração × Qualidade do sono
- Qualidade do sono por IMC
- Distúrbios do sono por IMC (tabela cruzada)
- Duração do sono por gênero
- Qualidade do sono por profissão
### 5️⃣ Síntese interpretativa
Conexão dos achados em insights articulados.
 
---
 
## 💡 Principais insights
 
### 🔥 Insight 1 — Estresse é o fator mais determinante
Correlação de **-0,90** entre nível de estresse e qualidade do sono — praticamente perfeita. Nenhuma outra variável chegou perto disso. Reduzir o estresse parece ser a alavanca mais eficaz para melhorar o sono.
 
### ⚖️ Insight 2 — IMC fora do normal = quase certeza de distúrbio
- IMC **Normal:** apenas 7% têm algum distúrbio do sono
- IMC **Overweight:** 87% têm algum distúrbio
- IMC **Obese:** **100%** têm algum distúrbio
### ⏱️ Insight 3 — Duração e qualidade caminham juntas
Correlação positiva entre horas de sono e percepção de qualidade.
 
### 👔 Insight 4 — Profissão influencia o sono
Diferenças marcantes na qualidade do sono entre profissões.
 
---
 
## 📁 Estrutura da pasta
 
```
atividade-05-eda-sleep-health/
├── README.md
├── notebook/
│   └── eda_sleep_health.ipynb
└── data/
    └── Sleep_health_and_lifestyle_dataset.csv
```
 
---
 
## ▶️ Como executar
 
1. Baixe o dataset no [Kaggle](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset)
2. Instale as dependências:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Abra o notebook no Jupyter ou Google Colab
4. Ajuste o caminho do CSV conforme seu ambiente

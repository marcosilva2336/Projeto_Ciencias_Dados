# Análise de Dados e Modelos Preditivos para Diagnóstico

Este projeto realiza uma análise detalhada de dados de diagnóstico de câncer de mama e aplica modelos de machine learning para prever a presença de células malignas ou benignas. Ele utiliza técnicas de pré-processamento, análise exploratória e treinamento de diferentes modelos, além de uma avaliação comparativa dos resultados.

---

## 📋 Tabela de Conteúdos

1. [Descrição do Projeto](#descrição-do-projeto)
2. [Tecnologias Utilizadas](#tecnologias-utilizadas)
3. [Estrutura do Projeto](#estrutura-do-projeto)
4. [Pré-processamento dos Dados](#pré-processamento-dos-dados)
5. [Análise Exploratória](#análise-exploratória)
6. [Treinamento e Avaliação dos Modelos](#treinamento-e-avaliação-dos-modelos)
7. [Modelos Utilizados e Resultados](#modelos-utilizados-e-resultados)
8. [Como Executar o Projeto](#como-executar-o-projeto)
9. [Possíveis Melhorias](#possíveis-melhorias)
10. [Autor](#autor)

---

## 📝 Descrição do Projeto

Este projeto tem como objetivo analisar os dados do conjunto "Breast Cancer Wisconsin Diagnostic Dataset". O foco principal é identificar padrões que diferenciem diagnósticos benignos e malignos, e aplicar modelos preditivos para ajudar no diagnóstico.  

Inclui:
- Pré-processamento de dados.
- Análise exploratória detalhada com visualizações.
- Treinamento e avaliação de quatro modelos de machine learning.
- Comparação das métricas de desempenho dos modelos.

---

## 🛠️ Tecnologias Utilizadas

Este projeto foi desenvolvido utilizando as seguintes tecnologias:

- **Linguagem:** Python 3.x
- **Bibliotecas e ferramentas:**
  - `pandas` - Manipulação e limpeza de dados.
  - `matplotlib` - Visualização de dados.
  - `seaborn` - Gráficos estatísticos e correlações.
  - `scikit-learn` - Implementação dos modelos de machine learning.

---

## 🔄 Pré-processamento dos Dados

1. **Carregamento do Dataset**:
   - Dataset carregado com `pandas`.

2. **Tratamento de Colunas**:
   - Removidas colunas irrelevantes como `id` e `Unnamed: 32`.

3. **Conversão de Valores Alfanuméricos**:
   - Mapeamento do diagnóstico para valores numéricos:
     - Maligno (M) -> 1
     - Benigno (B) -> 0

4. **Normalização e Escala**:
   - Aplicação de técnicas para ajustar os dados à mesma escala para os modelos.

---

## 🔍 Análise Exploratória

- **Estatísticas descritivas**:
  - Média, mediana e desvio padrão das variáveis.

- **Visualizações**:
  - Histogramas para verificar distribuições.
  - Gráficos de dispersão para explorar correlações.
  - Heatmap da matriz de correlação para identificar relações entre as variáveis.

---

## 🤖 Treinamento e Avaliação dos Modelos

Os dados foram divididos em:
- **80% para treino**.
- **20% para teste**.

Modelos treinados:
1. **Regressão Logística**
2. **Random Forest**
3. **Support Vector Machine (SVC)**
4. **K-Nearest Neighbors (KNN)**

### Métricas de Avaliação:
- **Acurácia:** Porcentagem de predições corretas.
- **Precisão:** Taxa de predições positivas corretas (Maligno).
- **Recall:** Capacidade do modelo de encontrar todas as instâncias de Maligno.
- **F1-Score:** Média harmônica entre precisão e recall.

---

## 📊 Modelos Utilizados e Resultados

| Modelo                | Acurácia | Precisão (Maligno) | Recall (Maligno) | F1-Score (Maligno) |
|-----------------------|----------|--------------------|------------------|--------------------|
| Regressão Logística   | 0.95     | 0.92               | 0.94             | 0.93               |
| Random Forest         | 0.97     | 0.96               | 0.97             | 0.96               |
| Support Vector Machine| 0.96     | 0.94               | 0.96             | 0.95               |
| K-Nearest Neighbors   | 0.93     | 0.90               | 0.92             | 0.91               |

> Observação: Os valores podem variar dependendo da semente aleatória usada para dividir os dados.

---

## ▶️ Como Executar o Projeto

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/projeto-diagnostico.git

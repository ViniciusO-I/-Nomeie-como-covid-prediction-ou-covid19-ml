# 🧠 Predição de Mortalidade por COVID-19 com Árvore de Decisão

Este projeto utiliza um conjunto de dados reais de pacientes diagnosticados com COVID-19 para prever a chance de óbito com base em características clínicas e demográficas. O objetivo foi aplicar técnicas de análise exploratória de dados (EDA) e aprendizado de máquina para entender os principais fatores de risco e treinar um modelo de classificação.

> Projeto desenvolvido e praticado no ambiente de trabalho atual, com base em estudos conduzidos no Google Colab.

---

## 🎯 Objetivos

- Realizar análise exploratória de dados com visualizações intuitivas
- Identificar correlações entre variáveis clínicas e mortalidade
- Treinar e avaliar um modelo de árvore de decisão
- Explorar o impacto da profundidade do modelo na acurácia

---

## ⚙️ Tecnologias Utilizadas

- **Python 3.10**
- **Pandas** – manipulação de dados
- **Seaborn & Matplotlib** – visualização
- **Scikit-learn** – machine learning (árvore de decisão, avaliação)

---

## 📊 Etapas do Projeto

1. **Carregamento e pré-processamento dos dados**
   - Substituição de valores inválidos (97, 98, 99 → NaN)
   - Conversão de variáveis categóricas
   - Criação da coluna `DIED` baseada na data de falecimento

2. **Análise Exploratória**
   - Distribuição de idade (`sns.histplot`)
   - Contagem de variáveis por sexo
   - Correlação entre comorbidades e óbito

3. **Treinamento do Modelo**
   - Separação entre treino/teste
   - Treinamento com `DecisionTreeClassifier` (max_depth ajustável)
   - Avaliação: Acurácia, Relatório de Classificação, Matriz de Confusão

4. **Visualização da Árvore e Desempenho**
   - Árvore plotada com `plot_tree`
   - Comparação de acurácia com diferentes profundidades (`max_depth`)

---

## 📈 Resultados

- **Acurácia do modelo:** ~45,5% (com profundidade 3)
- Variáveis com maior impacto no modelo: **idade, asma, obesidade, DPOC**
- O modelo apresentou resultados modestos, condizentes com a simplicidade da árvore e possíveis desequilíbrios nos dados

---

## 🧠 Melhorias Futuras

- Testar modelos mais robustos (RandomForest, XGBoost)
- Balancear o dataset (oversampling/undersampling)
- Aplicar validação cruzada
- Criar um dashboard interativo com Streamlit ou Power BI

---

## 📁 Imagens do Projeto

<p align="center">
  <img src="imgs/arvore_decisao.png" width="600"><br>
  <em>Árvore de decisão gerada pelo modelo</em><br><br>
  <img src="imgs/histograma_idade.png" width="500"><br>
  <em>Distribuição de idade dos pacientes</em><br><br>
  <img src="imgs/acuracia_profundidade.png" width="500"><br>
  <em>Acurácia por profundidade da árvore</em>
</p>

---

## ✍️ Autor

**Vinicius Rodrigues de Oliveira**  
📚 Estudante de Análise e Desenvolvimento de Sistemas - FIAP  
🔧 Técnico em Automação Industrial | Transição para Tecnologia  


---

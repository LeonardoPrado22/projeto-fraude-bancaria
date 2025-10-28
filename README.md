# 🧠 Projeto EBAC – Detecção de Fraudes Bancárias

🎥 [Apresentação do Projeto]((https://docs.google.com/presentation/d/1EP6gpsHYqn-qv4hvykJa40piyijW5tHB1cjKuOeChag/edit?usp=sharing)

Este projeto tem como objetivo desenvolver e otimizar um **modelo preditivo para detecção de fraudes financeiras**, aplicando técnicas de balanceamento e otimização de hiperparâmetros para maximizar o desempenho do modelo e reduzir o impacto de falsos negativos — o erro mais custoso em um contexto bancário.  

A base utilizada já foi previamente **reduzida por PCA (Análise de Componentes Principais)**, etapa realizada antes da disponibilização dos dados.

---

## 📥 1. Coleta e Preparação dos Dados

Os dados foram obtidos a partir de uma **base simulada de transações bancárias**, composta por variáveis comportamentais e características das operações financeiras.  

Durante a etapa de coleta e preparação, foram realizadas as seguintes ações:
- Importação do dataset em formato `.csv` com a biblioteca **pandas**.  
- Inspeção inicial com os métodos `head()`, `info()` e `describe()`.  
- Análise de valores ausentes e inconsistentes.  

Essas etapas garantiram a integridade e qualidade da base para as análises posteriores.

---

## 🔍 2. Exploração e Análise dos Dados (EDA)

A análise exploratória teve como foco identificar **padrões comportamentais entre transações legítimas e fraudulentas**, bem como avaliar a distribuição das classes.  

Vale destacar que a **base já foi disponibilizada após o processo de PCA**, o que significa que as variáveis originais foram transformadas em componentes principais, reduzindo a dimensionalidade e otimizando a performance dos modelos.

### Principais etapas:
- **Análise estatística descritiva** das variáveis numéricas.  
- **Visualizações** com **histogramas**, **boxplots** e **gráficos de dispersão** para observar tendências e outliers.  
- **Correlação entre componentes** utilizando **matriz de correlação** e **heatmap**.  

Essas análises permitiram compreender melhor os padrões de fraude e orientar a escolha dos algoritmos mais adequados.

---

## ⚙️ 3. Modelagem Preditiva

Após o entendimento da base, iniciou-se o processo de modelagem com foco em **classificação binária** (fraude vs. não fraude).

### Etapas seguidas:
1. **Divisão dos dados** em conjuntos de treino e teste com `train_test_split`.  
2. **Tratamento do desbalanceamento** utilizando **SMOTE (Synthetic Minority Oversampling Technique)**.  
3. Teste de diferentes modelos, incluindo:
   - **Random Forest**
   - **Logistic Regression**
   - **XGBoost**
4. **Otimização de hiperparâmetros** com `RandomizedSearchCV` para maximizar o **F1-Score**.  
5. **Avaliação do desempenho** com métricas como:
   - **F1-Score**
   - **Precision**
   - **Recall**
   - **Matriz de Confusão**

O modelo final escolhido apresentou excelente equilíbrio entre precisão e recall, priorizando a detecção de fraudes (redução de falsos negativos).

---

## 🧩 Conclusão

1. O modelo conseguiu atingir **alto desempenho na detecção de fraudes**, mesmo com uma base altamente desbalanceada.  
2. O **uso de uma base já reduzida por PCA**, aliado ao **SMOTE**, contribuiu para aprimorar a performance e reduzir o tempo de treinamento.  
3. O **Random Forest otimizado** se mostrou o modelo mais eficiente, com melhor trade-off entre precisão e recall.  
4. Em um contexto real, essa abordagem pode **minimizar perdas financeiras significativas**, identificando com maior eficiência transações suspeitas.  

📅 **Data:** Outubro / 2025  
👨‍💻 **Autor:** Leonardo Prado  
📚 **Curso:** Ciência de Dados – EBAC  




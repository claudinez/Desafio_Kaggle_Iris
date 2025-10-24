# 📊 Desafio Kaggle – Iris Dataset

## Descrição do Projeto
Este projeto utiliza o **dataset Iris**, um clássico da estatística e do machine learning, contendo medidas de flores de três espécies: **Setosa, Versicolor e Virginica**.  

O objetivo é construir uma **análise exploratória** e **modelos preditivos** capazes de classificar corretamente a espécie da flor com base em suas medidas (comprimento e largura de sépalas e pétalas).

---

## Metodologia

1. **Importação dos Dados**  
   - O dataset foi carregado diretamente do GitHub em um DataFrame Pandas.  
   - Foi verificada a integridade dos dados, sem valores nulos ou inconsistentes.  

2. **Análise Exploratória (EDA)**  
   - Distribuição das espécies com gráficos de barras interativos usando **Plotly**.  
   - Boxplots para comparar distribuições de **comprimento de sépalas e pétalas** entre espécies.  
   - **Scatter matrix interativa** para visualizar relações entre todas as medidas, destacando padrões e separações entre espécies.  

3. **Preparação dos Dados**  
   - Separação entre **features** (colunas numéricas) e **target** (espécie).  
   - Conversão da variável target em números usando `LabelEncoder`.  
   - Divisão em conjuntos **treino (80%)** e **teste (20%)** mantendo proporção das classes (`stratify`).  

4. **Construção de Modelos de Classificação**  
   - Modelos testados: **K-Nearest Neighbors (KNN)**, **Decision Tree** e **Random Forest**.  
   - Avaliação via **acurácia, relatório de classificação e matriz de confusão**.  

---

## Resultados

### Distribuição das Espécies
| Espécie           | Quantidade |
|------------------|------------|
| Iris-setosa       | 50         |
| Iris-versicolor   | 50         |
| Iris-virginica    | 50         |

### Desempenho dos Modelos
| Modelo           | Acurácia (Teste) | Observações |
|-----------------|-----------------|-------------|
| K-Nearest Neighbors | 96-97%        | Versicolor às vezes confundida com Virginica |
| Decision Tree      | 96-97%        | Fácil separação da Setosa |
| Random Forest      | 97-100%       | Mais robusto, combina várias árvores |

### Dificuldades Observadas
- **Versicolor** apresenta alguma sobreposição com **Virginica**, sendo mais difícil de classificar.  
- **Setosa** é facilmente separável devido às diferenças claras nas medidas.

---

## Visualizações Interativas

- **Gráfico de Barras:** distribuição de espécies  
  ![Barras](link_para_screenshot_barras.png)  

- **Boxplots:** comparativo de medidas de sépalas e pétalas  
  ![Boxplots](link_para_screenshot_boxplots.png)  

- **Scatter Matrix:** dispersão de todas as medidas  
  ![Scatter Matrix](link_para_screenshot_scatter.png)  

> Substitua os links acima pelos **links gerados no Google Colab** ou imagens exportadas.

---

## Próximos Passos

- **Otimização de hiperparâmetros** dos modelos (ex: `n_neighbors`, profundidade das árvores).  
- **Feature engineering**: criar novas features, como razão entre comprimento e largura.  
- **Validação cruzada**: para métricas mais confiáveis.  
- **Testar outros algoritmos**: SVM, Gradient Boosting, redes neurais.  
- **Dashboards interativos** com Plotly Dash ou Streamlit para visualização dinâmica do dataset.  

---

## Conclusão

Este projeto demonstrou como explorar e modelar dados de forma completa:  
- Através da **EDA interativa**, foi possível identificar padrões claros entre espécies.  
- A **modelagem com múltiplos algoritmos** mostrou alta acurácia, com Random Forest sendo o mais robusto.  
- A documentação e os gráficos podem ser usados diretamente em **portfólio ou apresentações**.



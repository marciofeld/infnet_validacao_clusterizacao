# Validação de Modelos de Clustericação [24E4_3]

## PROJETO DA DISCIPLINA - ENTREGA FINAL

## Aluno: Marcio Feldmann
## Repositório Público GitHub: https://github.com/marciofeld/infnet_validacao_clusterizacao

Este projeto realiza uma análise comparativa de técnicas de clusterização aplicadas a dados de vacinação contra COVID-19. Foram utilizados diferentes algoritmos de agrupamento, como **K-Means** e **DBSCAN**, para identificar padrões nas campanhas de vacinação entre diferentes países.

## **Objetivo**
O objetivo deste projeto é comparar e validar diferentes técnicas de clusterização usando dados reais de vacinação. A análise ajuda a compreender como diferentes algoritmos se comportam com o mesmo conjunto de dados e como validar seus resultados usando métricas apropriadas.

---

## **Etapas do Projeto**

### **1. Importação de Bibliotecas e Dados**
- Foram utilizadas bibliotecas como `pandas`, `numpy`, `matplotlib`, `seaborn` e `scikit-learn` para manipulação de dados, visualizações e clusterização.
- Os dados foram carregados do dataset "COVID-19 World Vaccination Progress", contendo informações sobre vacinação em diferentes países.

### **2. Pré-Processamento**
- **Tratamento de Dados Faltantes**:
  - Remoção de registros sem informações relevantes
  - Preenchimento de valores ausentes usando medianas
- **Normalização dos Dados**:
  - Uso do `StandardScaler` para padronizar as variáveis
- **Tratamento de Outliers**:
  - Remoção de valores extremos usando o método IQR

### **3. Aplicação de Algoritmos de Clusterização**
- **K-Means**:
  - Determinação do número ótimo de clusters usando índice de silhueta
  - Implementação do algoritmo com os parâmetros otimizados
- **DBSCAN**:
  - Determinação do eps usando análise de vizinhos mais próximos
  - Identificação automática de clusters e ruído

### **4. Interpretação dos Resultados**
- Análise comparativa dos agrupamentos gerados por cada algoritmo
- Avaliação usando diferentes métricas de validação
- Interpretação dos padrões de vacinação identificados

### **5. Visualização**
- Gráficos de distribuição das variáveis
- Visualização dos clusters formados
- Análise da qualidade dos agrupamentos

---

## **Principais Resultados**
- O **K-Means** forneceu grupos bem definidos e equilibrados
- O **DBSCAN** identificou eficientemente outliers e padrões não-esféricos
- A análise revelou diferentes perfis de vacinação entre os países

---

## **Fontes de Dados**
Os dados utilizados foram obtidos do dataset "COVID-19 World Vaccination Progress", disponível no Kaggle, que inclui métricas de vacinação por país ao longo do tempo.

---

## **Arquivos Gerados**
Durante a execução do notebook, foram gerados os seguintes arquivos:
- `requirements.txt`: Lista de dependências do projeto
- `resultados_clusters_kmeans.txt`: Análise detalhada dos clusters gerados

---

## **Referências**
- [Scikit-Learn Documentation](https://scikit-learn.org/stable/)
- [K-means Clustering](https://scikit-learn.org/stable/modules/clustering.html#k-means)
- [DBSCAN Clustering](https://scikit-learn.org/stable/modules/clustering.html#dbscan)
- [Silhouette Score](https://scikit-learn.org/stable/modules/clustering.html#silhouette-coefficient)
- [Clustering Performance Evaluation](https://scikit-learn.org/stable/modules/clustering.html#clustering-performance-evaluation)
- [COVID-19 World Vaccination Progress](https://www.kaggle.com/datasets/gpreda/covid-world-vaccination-progress)

---
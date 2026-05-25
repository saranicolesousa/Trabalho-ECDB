# Extração de Conhecimento de Dados (ECDB)

Este repositório contém os trabalhos práticos desenvolvidos no âmbito da unidade curricular, com foco na exploração, análise multivariada e modelação preditiva de dados em contextos biológicos e químicos.

## 👥 Autores (Grupo 8)
* **Bruno Ferreira** (PG58814)
* **Joana Maia** (PG58816)
* **Sara Sousa** (PG59766)

---

## 📁 Trabalhos Desenvolvidos

### 📊 [Trabalho Prático 1: [Inserir Título do Trabalho 1]](./Trabalho_1)

**Contextualização:**
[Cole aqui o texto introdutório que já tinha sobre o Trabalho 1, descrevendo o objetivo principal e o dataset utilizado.]

**Pipeline de Análise:**
1. **[Etapa 1]:** [Descrição do que fizeram...]
2. **[Etapa 2]:** [Descrição do que fizeram...]
3. **[Etapa 3]:** [Descrição do que fizeram...]
*(Adapte estas etapas de acordo com o que já tinha no README original do Trabalho 1)*

---

### 🔬 [Trabalho Prático 2: Espectroscopia Raman](./Trabalho_2)

**Contextualização:**
O objetivo fundamental deste trabalho consiste na análise de dados de espectroscopia Raman para a identificação de padrões vibracionais e agrupamento automático de compostos orgânicos. A análise foca-se em 11 compostos (Grupo 8), avaliando se a assinatura vibracional captada pela espectroscopia Raman é suficiente para segregar e identificar automaticamente as diferentes funções químicas (álcoois, solventes clorados, aminas, ésteres e ácidos).

**Pipeline de Análise:**
O fluxo de trabalho foi estruturado nas seguintes etapas metodológicas:

1. **Análise Visual e Descritiva:** Comparação visual dos espectros médios e identificação das bandas Raman relevantes e padrões vibracionais de cada molécula.
2. **Pré-processamento Espectroscópico:** 
   * Tratamento de valores omissos pela mediana.
   * Suavização através do filtro Savitzky-Golay.
   * Correção de linha de base via algoritmo ALS (*Asymmetric Least Squares*).
   * Normalização das intensidades por SNV (*Standard Normal Variate*).
3. **Redução de Dimensionalidade:** Projeção da informação num espaço de menor dimensão para visualização e mitigação de ruído, aplicando **PCA**, **t-SNE** e **UMAP**.
4. **Análise Não Supervisionada (*Clustering*):** Agrupamento automático dos espectros utilizando **K-Means**, **Algrupamento Hierárquico (critério de Ward)** e **DBSCAN**.
5. **Interpretação e Aprendizagem Máquina:** Interpretação química dos grupos formados, correlacionando-os com as respetivas famílias químicas, e treino de modelos de classificação para previsão de propriedades.

---

## 📂 Estrutura do Repositório

O repositório encontra-se organizado em diretórios independentes para cada trabalho:

```text
Trabalho-ECDB/
├── Trabalho_1/                      # Ficheiros e notebooks referentes ao TP1
├── Trabalho_2/                      # Ficheiros e notebooks referentes ao TP2
│   ├── outputs/                     # Gráficos e resultados exportados
│   ├── grupo8.ipynb                 # Jupyter Notebook da análise Raman
│   ├── raman_data.csv               # Matriz de dados espectrais bruta
│   └── compound_data.xlsx           # Metadados dos compostos
├── requirements.txt                 # Dependências do projeto
└── README.md                        # Documentação principal

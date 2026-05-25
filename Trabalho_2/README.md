# Extração de Conhecimento de Dados de Espectroscopia Raman

Este repositório contém o desenvolvimento do **Trabalho Prático 2**, focado na análise de conjuntos de dados de espectroscopia Raman de compostos orgânicos utilizando a linguagem Python.

## Objetivos do Projeto
O objetivo principal é explorar padrões nos espetros Raman, comparar compostos e construir modelos preditivos que permitam distinguir moléculas com base nas suas intensidades em diferentes valores de *Raman Shift*.

## Contextualização e Compostos Analisados

A **espectroscopia Raman** é uma técnica analítica não destrutiva que se baseia na dispersão inelástica da luz (Efeito Raman) para fornecer uma "impressão digital" vibracional das moléculas. Cada composto químico apresenta um padrão único de picos de intensidade em diferentes valores de *Raman Shift* ($cm^{-1}$), que correspondem às vibrações específicas das ligações químicas presentes na sua estrutura.

O conjunto de dados analisado compreende **1225 espectros** distribuídos por **11 compostos orgânicos** puros, medidos sob diferentes tempos de exposição (variando de 2.0s a 30.0s). Os compostos estão divididos em 5 famílias funcionais:

| Família Funcional | Compostos Analisados |
| :--- | :--- | 
| **Solventes Clorados** | Chloroform, Dichloromethane 
| **Álcoois e Polióis** | Ethanol, Ethylene glycol, Diethylene glycol
| **Hidrocarbonetos e Aminas** | Cyclohexane, Diethylamine 
| **Compostos Carbonilados** | Diethyl malonate, Ethyl acetate
| **Sulfóxidos e Ácidos** | Dimethyl sulfoxide (DMSO), Formic acid 

## Pipeline de Análise
O projeto está organizado seguindo o seguinte fluxo de trabalho:

1. **Análise Exploratória & Descrição:** Carregamento dos dados e identificação das variáveis de *Raman Shift*.
2. **Pré-processamento Espectroscópico:**
   - Suavização através do filtro polinomial **Savitzky-Golay** ($window=11, order=2$).
   - Correção de linha de base via **Mínimos Quadrados Assimétricos (ALS)** para remoção do fundo de fluorescência.
   - Normalização por SNV (Standard Normal Variate) para mitigação de efeitos multiplicativos de escala.
4. **Análise Estatística e Visual:**
   - Estatística descritiva e comparação de espectros médios.
   - Identificação de bandas Raman relevantes.
5. **Análise Multivariada Não Supervisionada:**
   - Redução de dimensionalidade (PCA, t-SNE).
   - Clustering (K-Means e Algoritmo Aglomerativo) dos espetros e interpretação dos grupos.
7. **Aprendizagem Máquina Preditiva:**
   - Treino, otimização e validação cruzada de modelos de classificação (Regressão Logística, SVM, Random Forest e KNN).

## Estrutura do Repositório
* `outputs/`: Pasta com os resultados obtidos (gráficos, tabelas).
* `grupo8.ipynb`: Jupyter Notebook principal com todo o código de análise, justificações e interpretações dos resultados.
* `raman_data.csv`: Conjunto de dados original em formato CSV.
* `compound_data.xlsx`: Conjunto de dados complementar ou metadados dos compostos em formato Excel.
* `README.md`: Documentação principal do projeto.

## Como Reproduzir
1. Clone o repositório.
2. Certifique-se de manter os ficheiros `raman_data.csv` e `compound_data.xlsx` no mesmo diretório do notebook.
3. Instale as dependências necessárias
4. Execute o notebook `grupo8.ipynb`.
---
**Autores:** Bruno Ferreira pg58814, Joana Maia pg58816, Sara Sousa pg59766

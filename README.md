# Expressão Génica Espacial no Carcinoma do Ovário
### Unidade Curricular: Extração de Conhecimento de Dados Biológicos

Este repositório contém o trabalho desenvolvido no âmbito da Unidade Curricular **"Extração de Conhecimento de Dados Biológicos"**, inserida no Mestrado em Bioinformática da Universidade do Minho (ano letivo 2025/2026).

O projeto foca-se no desenvolvimento de um fluxo de trabalho (*workflow*) em **R/Bioconductor** para a análise de dados biológicos, abrangendo desde o processamento inicial até à modelação preditiva.

---

## Conjunto de Dados Selecionado

* **Título:** Ovarian Cancer (Foundation Medicine / Gray, 2024) 
* **Fonte:** [cBioPortal](https://www.cbioportal.org/study/summary?id=ovary_geomx_gray_foundation_2024)
* **Referência:** Gray et al., 2024.
* **Descrição dos dados:**
    * **Transcriptómica & Proteómica Espacial:** Dados obtidos através da tecnologia GeoMx Digital Spatial Profiler (DSP).
    * **Metadados Clínicos:** Inclui informações detalhadas sobre as amostras e a localização espacial.
* **Dimensão:** 567 amostras

---

## Metodologia e Fases do Trabalho

O trabalho está estruturado em três fases principais de desenvolvimento:

### Fase 1: Exploração e Processamento
* **Explicação dos Dados:** Origem, relevância biológica e contextualização biológica.
* **Pré-processamento:** Scripts em R para carregamento, filtragem de baixa qualidade e normalização dos dados.
* **Sumarização:** Estatística descritiva e exploração visual com recurso a gráfocos (histogramas, boxplots de normalização).
* **Análise Estatística:** Expressão diferencial entre diferentes regiões ou estados clínicos e análise de enriquecimento.

### Fase 2: Análise Não Supervisionada
* **Agrupamento:** Clustering de genes e/ou amostras.
* **Redução de Dimensionalidade:** Aplicação de PCA (Principal Component Analysis), MDS ou outras análises não supervisionadas para visualização da separação das amostras.

### Fase 3: Modelação e Predição
* **Análise Preditiva:** Implementação de algoritmos de Machine Learning (Classificação/Regressão).
* **Comparação de Modelos:** Avaliação de desempenho entre pelo menos dois modelos distintos.
* **Seleção de Atributos:** Identificação da importância de genes ou proteínas específicas para o diagnóstico/prognóstico.

---

## Autores (Grupo 8)

* **Bruno Ferreira** - PG58814
* **Joana Maia** - PG58816
* **Sara Sousa** - PG59766

---
*Mestrado em Bioinformática - Universidade do Minho*

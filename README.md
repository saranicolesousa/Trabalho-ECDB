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

Os ficheiros de dados não estão incluídos neste repositório devido ao seu tamanho.
Para correr o pipeline, descarregue os dados do estudo **Ovarian Cancer (Gray, 2024)** em [cBioPortal](https://www.cbioportal.org/study/summary?id=ovary_geomx_gray_foundation_2024) e coloque os ficheiros na pasta `database_ovario/` na raiz do repositório.

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
## Estrutura do Repositório (Fase 1)
Todos os ficheiros relativos à primeira etapa do trabalho encontram-se no diretório `fase1/`.

### Código e Relatórios
* **fase1_trabalho_G8.Rmd**: Script em RMarkdown contendo todo o pipeline de análise.
* **fase1_trabalho_G8.html**: Versão compilada do trabalho para leitura em browser.

### Dados Processados (`/data_processed`)
* **Metadata_Processado.csv**: Metadados clínicos após limpeza e filtragem.
* **Expressao_mRNA_Alinhada.csv**: Matriz de expressão génica normalizada e alinhada com as amostras clínicas.

### Resultados da Análise (`/results`)
* **Expressao_Diferencial_...csv**: Resultados completos do teste de expressão diferencial.
* **Genes_Significativos_DE.csv**: Lista filtrada de genes com significância estatística.
* **fGSEA_Hallmark_...csv**: Resultados da análise de enriquecimento de conjuntos de genes (Gene Set Enrichment Analysis).
* **comparacoes_significativas_dunn.csv**: Resultados do teste post-hoc de Dunn para comparações múltiplas.

## Estrutura do Repositório (Fase 2)
Todos os ficheiros relativos à segunda etapa do trabalho encontram-se no diretório `fase2/`. Nos ficheiros .Rmd, algumas linhas de código foram colocadas em comentário para melhorar a legibilidade do documento e focar a apresentação nos resultados mais relevantes.

### Notas sobre esta entrega
Esta fase inclui também uma versão atualizada do relatório da Fase 1, com as seguintes melhorias:
* **Referenciação bibliográfica:** O documento foi revisto e complementado com citações e bibliografia no formato APA, garantindo o rigor científico das fontes utilizadas.

### Código e Relatórios
* **fase1_trabalho_G8_v2.Rmd**: Versão atualizada do relatório da Fase 1.
* **fase1_trabalho_G8_v2.html**: Versão compilada do relatório atualizado da Fase 1.
* **fase2_trabalho_G8.Rmd**: Script em RMarkdown contendo o pipeline de análise não supervisionada.
* **fase2_trabalho_G8.html**: Versão compilada do trabalho da Fase 2 para leitura em browser.

### Ficheiros de Bibliografia (`/references`)
* **referencias_fase1.bib**: Ficheiro BibTeX com todas as referências bibliográficas utilizadas na Fase 1.
* **referencias_fase2.bib**: Ficheiro BibTeX com todas as referências bibliográficas utilizadas na Fase 2.
* **apa.csl**: Ficheiro de estilo de citação no formato APA.

### Resultados da Análise (`/results`)
* **PCA_Scores_Fase2.csv**: Coordenadas das amostras no espaço PCA.
* **PCA_Proteica_Scores_Fase2.csv**: Coordenadas das amostras no espaço PCA para dados proteómicos.
* **PCA_Loadings_Fase2.csv**: Contribuição de cada gene para as componentes principais, permitindo a interpretação biológica dos eixos de variação.
* **UMAP_Coordenadas_Fase2.csv**: Coordenadas das amostras resultantes da redução de dimensionalidade por UMAP.
* **MDS_Coordenadas_Fase2.csv**: Coordenadas das amostras resultantes do Escalonamento Multidimensional Clássico (MDS/PCoA).
* **tSNE_Coordenadas_Fase2.csv**: Coordenadas das amostras resultantes da redução de dimensionalidade por t-SNE.
* **Kmeans_Clusters_Fase2.csv**: Atribuição de cada amostra ao respetivo cluster K-means (k=3), com identificadores de amostra e variáveis clínicas associadas.
* **Kmeans_Contingencia_Fase2.csv**: Tabela de contingência cruzando os clusters K-means com o tipo de lesão (`LESIONSTYPES`), para interpretação biológica dos agrupamentos.
---

## Autores (Grupo 8)

* **Bruno Ferreira** - PG58814
* **Joana Maia** - PG58816
* **Sara Sousa** - PG59766

---
*Mestrado em Bioinformática - Universidade do Minho*

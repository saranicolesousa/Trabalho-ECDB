# Trabalho-Extração de Conhecimento de Dados Biológicos
Este repositório contém o trabalho desenvolvido no âmbito da Unidade Curricular "Extração de Conhecimento de Dados Biológicos" do Mestrado em Bioinformática da Universidade do Minho (ano letivo 2025/2026).

O projeto foca-se no desenvolvimento de um fluxo de trabalho (workflow) em R/Bioconductor para a análise de dados biológicos, abrangendo desde o processamento inicial até à modelação preditiva.

## Resumo do Conjunto de Dados Escolhido

**Título:** Ovarian Cancer (Gray Foundation, Cancer Discov 2024)

**Fonte:** [cBioPortal](https://www.cbioportal.org/study/summary?id=ovary_geomx_gray_foundation_2024)

**Tipo de Dados:** 
* Transcriptómica de microrregiões (GeoMx mRNA-Seq)
* Imagens Multiplex (CyCIF - frações de tipos celulares)
* Intensidade de marcadores p53
* Metadados Clínicos (Estado de Mutação BRCA, estadiamento HGSOC, etc.)

**Dimensão:** 567 amostras com dados de expressão genética (mRNA-Seq)
  
## Metodologia e Fases do Trabalho

O trabalho está estruturado em três fases de desenvolvimento:

### Fase 1 
* **Explicação dos Dados:** Origem, relevância e contextualização biológica.
* **Pré-processamento:** Scripts em R para carregamento, filtragem e normalização.
* **Sumarização:** Estatística descritiva e exploração visual com recurso a gráficos.
* **Análise Estatística:** Expressão diferencial e análise de enriquecimento.

### Fase 2 
* **Agrupamento:** Clustering de genes e/ou amostras.
* **Redução de Dimensionalidade:** Aplicação de MDS ou outras análises não supervisionadas.

### Fase 3
* **Análise Preditiva:** Implementação de Machine Learning (Classificação/Regressão).
* **Comparação de Modelos:** Avaliação de desempenho entre pelo menos dois modelos distintos.
* **Seleção de Atributos:** Identificação da importância de genes específicos.

## Autores
* Bruno Filipe Caçador Ferreira (PG58814)
* Joana Filipa Vilaça Maia (PG58816)
* Sara Nicole Pereira De Sousa (PG59766)	

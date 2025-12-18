# 🦠 Análise Exploratória de Óbitos por Septicemia (2015–2022)

Este projeto realiza uma **análise exploratória dos óbitos por septicemia (sepse)** no período de **2015 a 2022**, utilizando dados públicos do **DATASUS (SIM)**. O estudo foi desenvolvido em dois níveis:
- **Brasil (2015–2022)**, com análise temporal, gênero e correlação com indicadores socioeconômicos;
- **Estado de São Paulo (2015–2022)**, com análise detalhada por gênero e faixa etária.

O objetivo principal é **traçar o perfil das mortes por septicemia** e compreender sua relação com fatores demográficos e socioeconômicos.

---

## 🗂️ Base de Dados

- **Fonte:** DATASUS – Sistema de Informações sobre Mortalidade (SIM)
- **Período:** 2015 a 2022
- **Abrangência:** Brasil e Estado de São Paulo
- **Classificação das causas:** CID-10

### Principais variáveis
- Gênero  
- Idade  
- Causa básica do óbito (CID-10)  
- Ano do óbito  

Dados socioeconômicos adicionais:
- **PIB** (Produto Interno Bruto)
- **IDHM** (Índice de Desenvolvimento Humano)

Fontes: DATASUS e IBGE (IPEADATA)

---

## 🔎 Metodologia

1. Extração dos dados de mortalidade por septicemia a partir do SIM/DATASUS.
2. Filtragem das causas de óbito associadas à septicemia (CID-10 – A40, A41, P36, entre outras).
3. Consolidação de todas as categorias em uma única variável: **Septicemia**.
4. Análises realizadas:
   - Estatísticas descritivas das causas de óbito
   - Análise temporal dos óbitos por gênero
   - Distribuição por faixa etária (São Paulo)
   - Análise de correlação entre óbitos, PIB e IDHM (Brasil)

---

## 📈 Principais Resultados

### Brasil (2015–2022)
- Total de **193.220 óbitos por septicemia**.
- As causas mais frequentes foram:
  - **A419 – Septicemia não especificada**
  - **P369 – Septicemia bacteriana não especificada do recém-nascido**
- Os óbitos por gênero apresentaram crescimento semelhante ao longo do tempo:
  - Feminino: **97.427 (50,42%)**
  - Masculino: **95.737 (49,54%)**
- Observou-se **pico acentuado entre 2021 e 2022**.
- Correlação entre variáveis:
  - Óbitos × PIB: **0,07** (relação nula)
  - Óbitos × IDHM: **-0,52** (relação moderada e negativa)
  - PIB × IDHM: **-0,22** (relação fraca)

➡️ Regiões ou períodos com **maior IDHM tendem a apresentar menos óbitos por septicemia**.

---

### Estado de São Paulo (2015–2022)
- Total de **31.425 óbitos por septicemia**.
- Principais causas:
  - **A418 – Outras septicemias especificadas**
  - **A419 – Septicemia não especificada**
- Distribuição por gênero:
  - Feminino: **15.873 óbitos**
  - Masculino: **15.548 óbitos**
- A análise etária mostrou:
  - Maior concentração de óbitos em **idosos (70 a 90 anos)**.
  - Presença de óbitos em bebês, porém em menor proporção.
- Crescimento gradual dos óbitos ao longo do tempo, com pico entre **2021 e 2022**.

---

## 🧠 Conclusões

Os resultados indicam que a **septicemia é uma importante causa de mortalidade no Brasil**, afetando principalmente **idosos** e apresentando crescimento significativo nos anos mais recentes.  

A análise reforça que:
- O **PIB isoladamente não explica** a mortalidade por septicemia.
- O **IDHM apresenta relação inversa** com o número de óbitos, evidenciando a importância de fatores como acesso à saúde, infraestrutura sanitária e condições de vida.
- A alta proporção de casos classificados como “não especificados” sugere **limitações nos registros clínicos e diagnósticos**.

O estudo destaca a necessidade de:
- Diagnóstico mais rápido e eficaz da sepse;
- Fortalecimento das políticas públicas de saúde;
- Atenção especial a grupos vulneráveis, como idosos e recém-nascidos.

---

## 📚 Referências

- DATASUS – Ministério da Saúde  
  https://datasus.saude.gov.br/

- IBGE / IPEADATA  
  https://www.ipeadata.gov.br/

- Drauzio Varella – Sepse (Septicemia)  
  https://drauziovarella.uol.com.br/doencas-e-sintomas/sepse-septicemia/

- EBSERH – Dia Mundial da Sepse  
  https://www.gov.br/ebserh/

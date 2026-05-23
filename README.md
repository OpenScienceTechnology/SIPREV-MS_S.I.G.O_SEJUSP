# 🚺 SIPREV-Mulher/MS — Sistema Inteligente de Predição e Mapeamento da Violência contra a Mulher

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![Scikit--learn](https://img.shields.io/badge/scikit--learn-ML-F7931E?logo=scikitlearn)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Deep%20Learning-FF6F00?logo=tensorflow)
![Status](https://img.shields.io/badge/status-academic%20project-green)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

> 📊 **Notebook:** `SIPREV_Mulher_SIGO_SEJUSP_MS_v2.ipynb`  
> 🧠 **Tema:** Ciência de Dados, Machine Learning, Deep Learning e Visualização Geoespacial  
> 📍 **Recorte territorial:** Mato Grosso do Sul — Brasil  
> 🗂️ **Base principal:** CVLI — Crimes Violentos Letais Intencionais, Sistema S.I.G.O / SEJUSP-MS  
> 📅 **Período analisado no notebook:** 2016–2025  
> 🎓 **Contexto acadêmico:** Tópicos Interdisciplinares III — Ciência dos Dados — UFMS Digital — 2026.1  
> 👤 **Autor:** VIANA  

---

## 🗂️ Repositório

```text
https://github.com/OpenScienceTechnology/DATA_SEJUSP-MS
```

---

## 📌 Sobre o projeto

O **SIPREV-Mulher/MS** é um notebook analítico desenvolvido para apoiar o estudo, o mapeamento e a previsão de padrões de violência contra a mulher no estado de **Mato Grosso do Sul**, com base em dados públicos de segurança registrados no conjunto **CVLI — Crimes Violentos Letais Intencionais** da **SEJUSP-MS**/**S.I.G.O**.

O projeto combina técnicas de:

- 🧹 **tratamento e padronização de dados**;
- 📊 **análise exploratória de dados**;
- 🗺️ **visualização geográfica e mapas interativos**;
- 📈 **indicadores municipais e temporais**;
- 🤖 **modelos de Machine Learning**;
- 🧠 **modelos de Deep Learning**;
- 🚨 **classificação de risco municipal**;
- 📦 **exportação automática de resultados**.

A proposta central é transformar dados brutos de ocorrências em **informação analítica, visual e preditiva**, apoiando estudos acadêmicos, projetos de extensão, prototipagem de sistemas inteligentes e análises públicas sobre segurança, gênero e políticas de prevenção.

---

## 🎯 Objetivos

### ✅ Objetivo geral

Construir um pipeline analítico em Python para processar, visualizar, classificar e prever indicadores associados à violência contra a mulher em Mato Grosso do Sul, utilizando dados públicos da SEJUSP-MS e técnicas de Ciência de Dados.

### 🎯 Objetivos específicos

- 📥 Carregar dados públicos do repositório `DATA_SEJUSP-MS`;
- 🧼 Padronizar colunas, datas, municípios, tipos criminais e indicadores derivados;
- 🧾 Criar variáveis temporais, criminais, geográficas e sintéticas;
- 🗺️ Gerar mapas interativos por município e taxa de incidência;
- 📊 Produzir tabelas e gráficos sobre vítimas, anos, meses, bairros e indicadores;
- 🏆 Construir ranking municipal completo dos 79 municípios de MS;
- 🤖 Treinar modelos de regressão, classificação e detecção de anomalias;
- 🧠 Testar arquiteturas de Deep Learning, como LSTM, GRU e MLP;
- 📄 Gerar relatórios técnicos em `.txt`, tabelas `.csv`, gráficos `.png`, mapas `.html` e modelos serializados;
- 📦 Compactar automaticamente todos os resultados em um arquivo `.zip`.

---

## 🧱 Estrutura geral do notebook

O notebook está organizado em blocos funcionais:

| Bloco | Descrição |
|---|---|
| 🧩 **A. Setup e carregamento** | Detecta ambiente, cria diretórios, instala dependências e carrega o dataset |
| 📊 **A. Ocorrências** | Analisa vítimas por município, ano, mês, faixa etária estimada, tipo de crime, bairros e relacionamentos |
| 🏆 **B. Ranking municipal** | Gera ranking completo dos municípios, comparação com a média estadual e mapas de risco |
| 📄 **C. Relatórios TXT + CSV** | Exporta relatórios tabulares em texto e tabelas em CSV |
| 🤖 **D. Modelos treinados** | Treina modelos de ML, DL e detecção de anomalias |
| 📦 **E. Exportação** | Gera sumário de outputs e compacta os resultados em ZIP |
| 📋 **Relatório executivo** | Cria uma síntese final com indicadores, modelos e recomendações |

---

## 🗂️ Fonte dos dados

A fonte principal utilizada pelo notebook é o conjunto público:

- **Base:** CVLI — Crimes Violentos Letais Intencionais  
- **Órgão:** SEJUSP-MS — Secretaria de Estado de Justiça e Segurança Pública de Mato Grosso do Sul  
- **Sistema:** S.I.G.O  
- **Repositório utilizado no notebook:** `OpenScienceTechnology/DATA_SEJUSP-MS`  
- **Arquivo bruto esperado:** `crimes-violentos-letais-intencionais-sejusp.csv`

URL configurada no notebook:

```python
https://raw.githubusercontent.com/OpenScienceTechnology/DATA_SEJUSP-MS/refs/heads/main/Dataset/crimes-violentos-letais-intencionais-sejusp.csv
```

O notebook também verifica se existe um arquivo local chamado:

```text
crimes-violentos-letais-intencionais-sejusp.csv
```

Caso exista, ele será usado antes do download remoto.

---

## ⚙️ Tecnologias e bibliotecas utilizadas

### 🧮 Manipulação e análise de dados

- `pandas`
- `numpy`
- `openpyxl`
- `pyarrow` ou `fastparquet`

### 📊 Visualização estatística

- `matplotlib`
- `seaborn`
- `plotly`

### 🗺️ Geoprocessamento e mapas

- `folium`
- `folium.plugins`
- `geopandas`
- `shapely`

### 🤖 Machine Learning

- `scikit-learn`
- `xgboost`
- `lightgbm`
- `imbalanced-learn`
- `joblib`

### 🧠 Deep Learning

- `tensorflow`
- `keras`

### 📄 Relatórios e exportação

- `texttable`
- `requests`
- `tqdm`
- `kaleido`
- `zipfile`
- `pathlib`
- `datetime`

---

## 🧪 Modelos implementados

O notebook treina e compara diferentes modelos para tarefas de regressão, classificação, detecção de anomalias e aprendizado profundo.

### 🌲 Random Forest

- **Random Forest Regressor**
  - Previsão do número de casos CVLI no mês seguinte por município.
- **Random Forest Classifier**
  - Classificação municipal em níveis de risco: baixo, médio e alto.

### 🚀 Gradient Boosting

- **XGBoost Regressor**
- **XGBoost Classifier**
- **LightGBM Regressor**
- **LightGBM Classifier**

### 🚨 Detecção de anomalias

- **Isolation Forest**
  - Identificação de municípios e períodos com comportamento estatisticamente atípico.

### 🧠 Redes neurais

- **LSTM**
  - Modelo recorrente para previsão temporal.
- **GRU**
  - Modelo recorrente alternativo, mais leve que LSTM.
- **MLP**
  - Rede neural densa para classificação de risco.

---

## 📈 Principais análises geradas

O notebook produz análises sobre:

- 🏙️ vítimas por município;
- 📅 evolução anual dos registros;
- 🗓️ distribuição mensal;
- ⏰ distribuição por turno;
- 🚺 feminicídio consumado;
- ⚠️ feminicídio tentado;
- 🏠 violência doméstica;
- 🚔 homicídio doloso;
- 🧭 bairros de maior e menor incidência;
- 👥 relação autor × vítima;
- 👩 faixa etária estimada das vítimas;
- 👨 faixa etária estimada dos autores;
- 📌 ranking dos 79 municípios;
- 🧮 taxas por 100 mil habitantes;
- 🧍 taxa por 100 mil mulheres;
- 🔥 classificação municipal de risco;
- 🤖 desempenho comparativo dos modelos.

---

## 🧬 Variáveis e indicadores derivados

Durante o processamento, o notebook cria variáveis derivadas, como:

| Variável | Descrição |
|---|---|
| `ano` | Ano do fato |
| `mes` | Mês do fato |
| `dia_semana` | Dia da semana |
| `trimestre` | Trimestre do fato |
| `periodo` | Período ano-mês |
| `fim_semana` | Indicador binário para sábado/domingo |
| `hora_num` | Hora numérica extraída do campo de hora |
| `turno` | Madrugada, manhã, tarde, noite ou ignorado |
| `tipo_crime` | Classificação principal do tipo de ocorrência |
| `nm_municipio` | Município padronizado |
| `delegacia` | Delegacia extraída do número/ano |
| `is_deam` | Indica se há referência à DEAM |
| `flag_feminicidio` | Feminicídio consumado |
| `flag_fem_tentada` | Feminicídio tentado |
| `flag_hom_doloso` | Homicídio doloso |
| `flag_viol_domestica` | Violência doméstica |
| `flag_estupro` | Estupro |
| `taxa_100k` | Taxa por 100 mil habitantes |
| `taxa_fem_100k` | Taxa por 100 mil mulheres |
| `classe_risco` | Classificação municipal de risco |

---

## ⚠️ Observação metodológica importante

O dataset CVLI utilizado no notebook **não contém campo direto de idade da vítima ou do autor**. Por isso, o notebook cria faixas etárias sintéticas por distribuição probabilística reprodutível, usando `seed=42`.

Essas variáveis são úteis para **simulação, prototipagem e visualização acadêmica**, mas **não devem ser interpretadas como idade real das pessoas envolvidas**.

Recomenda-se substituir essas estimativas por dados oficiais sempre que houver acesso a bases públicas com idade, sexo, vínculo, escolaridade ou outros atributos demográficos validados.

---

## 📁 Estrutura de diretórios gerada

Após a execução, o notebook cria a seguinte estrutura:

```text
.
├── SIPREV_Mulher_SIGO_SEJUSP_MS_v2.ipynb
├── crimes-violentos-letais-intencionais-sejusp.csv
├── models/
│   ├── rf_regressao.pkl
│   ├── rf_classificacao.pkl
│   ├── xgb_regressao.pkl
│   ├── xgb_classificacao.pkl
│   ├── lgb_regressao.pkl
│   ├── lgb_classificacao.pkl
│   ├── isolation_forest.pkl
│   ├── siprev_lstm.h5
│   ├── siprev_gru.h5
│   └── siprev_mlp.h5
├── outputs/
│   ├── A_painel_sintese.html
│   ├── maps/
│   │   ├── A_mapa_total_cvli.html
│   │   ├── A_mapa_feminicidio.html
│   │   ├── A_mapa_taxa_100k.html
│   │   └── B4_ranking_municipal.html
│   ├── graficos/
│   │   ├── A2_vitimas_ano.png
│   │   ├── A3_vitimas_mes.png
│   │   ├── A4_faixa_etaria_vitima.png
│   │   ├── A5_taxa_fem_100k.png
│   │   ├── A6_bairros.png
│   │   ├── A7_relacionamentos.png
│   │   ├── A8_faixa_etaria_autor.png
│   │   ├── A9_painel_sintese.png
│   │   ├── B2_posicao_vs_media.png
│   │   ├── B3_maior_menor_indicadores.png
│   │   ├── B5_comparativo_municipal.png
│   │   ├── B6_indicadores_cidade.png
│   │   ├── B7_ranking_indicadores_empilhado.png
│   │   └── D_comparativo_modelos.png
│   ├── tabelas/
│   │   ├── A1_vitimas_municipio.csv
│   │   ├── A2_vitimas_ano.csv
│   │   ├── A3_vitimas_mes.csv
│   │   ├── A4_faixa_etaria_vitima.csv
│   │   ├── A5_taxa_fem_100k.csv
│   │   ├── A6_bairros_incidencia.csv
│   │   ├── A7_relacionamentos.csv
│   │   ├── A8_faixa_etaria_autor.csv
│   │   ├── B1_ranking_municipal_completo.csv
│   │   ├── B3_maior_menor_indicador.csv
│   │   └── D_comparativo_modelos.csv
│   └── relatorios/
│       ├── C1_ranking_completo.txt
│       ├── C2_maior_menor_indicador.txt
│       ├── C3_bairros_maior_incidencia.txt
│       ├── C4_bairros_menor_incidencia.txt
│       ├── C5_vitimas_por_ano.txt
│       ├── C6_relacionamentos.txt
│       ├── C7_faixa_etaria.txt
│       ├── C8_indicadores_cidade.txt
│       ├── D_modelo_rf_regressao.txt
│       ├── D_modelo_rf_classificacao.txt
│       ├── D_modelo_xgb.txt
│       ├── D_modelo_lgb.txt
│       ├── D_modelo_isolation_forest.txt
│       ├── D_modelo_lstm.txt
│       ├── D_modelo_gru.txt
│       ├── D_modelo_mlp.txt
│       ├── D_comparativo_modelos.txt
│       └── E_relatorio_executivo.txt
└── SIPREV_SESUSP_Resultados.zip
```

> 📝 **Nota:** o notebook gera o ZIP com o nome `SIPREV_SESUSP_Resultados.zip`. Como o projeto se refere à **SEJUSP-MS**, recomenda-se renomear o arquivo para `SIPREV_SEJUSP-MS_Resultados.zip` em versões futuras.

---

## 🚀 Como executar o projeto

### 1️⃣ Clonar o repositório

```bash
git clone https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git
cd SEU-REPOSITORIO
```

### 2️⃣ Criar ambiente virtual

#### Windows

```bash
python -m venv .venv
.venv\Scripts\activate
```

#### Linux/macOS

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3️⃣ Instalar dependências

```bash
pip install --upgrade pip
pip install pandas numpy matplotlib seaborn plotly folium geopandas shapely scikit-learn xgboost lightgbm imbalanced-learn tensorflow joblib texttable requests tqdm openpyxl kaleido unidecode pyarrow
```

### 4️⃣ Abrir o notebook

```bash
jupyter notebook SIPREV_Mulher_SIGO_SEJUSP_MS_v2.ipynb
```

ou:

```bash
jupyter lab
```

### 5️⃣ Executar todas as células

No Jupyter:

```text
Kernel > Restart & Run All
```

No Google Colab:

```text
Ambiente de execução > Executar tudo
```

---

## ☁️ Execução no Google Colab

O notebook possui detecção automática de ambiente:

```python
try:
    import google.colab
    IS_COLAB = True
except ImportError:
    IS_COLAB = False
```

Quando executado no Google Colab, o arquivo `.zip` com os resultados pode ser baixado automaticamente ao final da execução.

---

## 📦 Exportação dos resultados

A função principal de exportação é:

```python
exportar_resultados("SIPREV_SESUSP_Resultados.zip")
```

Ela compacta:

- 🗺️ mapas interativos `.html`;
- 📊 gráficos `.png`;
- 📑 tabelas `.csv`;
- 📄 relatórios `.txt`;
- 🤖 modelos treinados `.pkl` e `.h5`;
- 📁 dataset bruto, se disponível.

---

## 📊 Exemplos de saídas geradas

### 🗺️ Mapas

- `A_mapa_total_cvli.html`
- `A_mapa_feminicidio.html`
- `A_mapa_taxa_100k.html`
- `B4_ranking_municipal.html`

### 📈 Gráficos

- `A2_vitimas_ano.png`
- `A3_vitimas_mes.png`
- `A5_taxa_fem_100k.png`
- `B6_indicadores_cidade.png`
- `D_comparativo_modelos.png`

### 📄 Relatórios

- `C1_ranking_completo.txt`
- `C5_vitimas_por_ano.txt`
- `D_comparativo_modelos.txt`
- `E_relatorio_executivo.txt`

### 🤖 Modelos

- `rf_regressao.pkl`
- `rf_classificacao.pkl`
- `xgb_regressao.pkl`
- `lgb_regressao.pkl`
- `isolation_forest.pkl`
- `siprev_lstm.h5`
- `siprev_gru.h5`
- `siprev_mlp.h5`

---

## 🧠 Interpretação dos modelos

Os modelos treinados devem ser entendidos como **instrumentos de apoio analítico**, e não como mecanismos automáticos de decisão pública.

### 📌 Recomendações de uso

- Usar os resultados para identificar padrões e priorizar investigação;
- Comparar indicadores entre municípios e períodos;
- Cruzar os achados com dados oficiais complementares;
- Atualizar periodicamente a base;
- Validar modelos com especialistas em segurança pública, saúde coletiva, políticas para mulheres e ética em IA.

### ⚠️ Cuidados

- Correlação não implica causalidade;
- Dados públicos podem conter subnotificação;
- Ausência de variável não significa ausência do fenômeno;
- Modelos podem reproduzir vieses presentes nos dados;
- Resultados preditivos exigem validação antes de qualquer uso operacional.

---

## 🔐 Ética, LGPD e responsabilidade

Este projeto utiliza dados públicos agregados e tem finalidade **acadêmica, científica e social**. Mesmo assim, análises de violência exigem responsabilidade metodológica e ética.

### Princípios adotados

- 🛡️ Não expor dados pessoais sensíveis;
- 🧭 Priorizar análise agregada por município, ano, mês e indicadores;
- ⚖️ Evitar uso punitivo ou discriminatório dos modelos;
- 🔎 Explicitar limitações dos dados e das estimativas;
- 🤝 Orientar o uso para prevenção, acolhimento, políticas públicas e pesquisa.

---

## 🧩 Limitações conhecidas

- A base CVLI não representa todos os tipos de violência contra a mulher;
- Pode haver subnotificação, inconsistência textual ou lacunas de preenchimento;
- Algumas variáveis são extraídas por expressões regulares a partir de campos textuais;
- As faixas etárias de vítima e autor são estimativas sintéticas;
- O notebook usa centroides municipais aproximados para mapas;
- O desempenho dos modelos depende da atualização e da qualidade da base;
- A análise cobre o período configurado no notebook: **2016–2025**.

---

## 🛠️ Possíveis melhorias futuras

- 📅 Atualizar o período para incluir dados de 2026;
- 🧾 Integrar bases complementares, como SINAN, Ligue 180, IBGE e Atlas da Violência;
- 🧠 Adicionar interpretabilidade com SHAP e Permutation Importance;
- 🗺️ Utilizar malhas geográficas oficiais dos municípios;
- 📊 Criar dashboard interativo com Streamlit, Dash ou Power BI;
- 🧪 Implementar validação temporal mais robusta;
- 🔐 Criar módulo de governança algorítmica e auditoria de vieses;
- 📚 Produzir relatório científico em formato ABNT;
- 🌐 Transformar o notebook em uma aplicação web para consulta pública.

---

## 🧾 Sugestão de estrutura para publicação no GitHub

```text
SIPREV-Mulher-MS/
├── README.md
├── LICENSE
├── requirements.txt
├── SIPREV_Mulher_SIGO_SEJUSP_MS_v2.ipynb
├── data/
│   ├── raw/
│   └── processed/
├── outputs/
│   ├── maps/
│   ├── graficos/
│   ├── tabelas/
│   └── relatorios/
├── models/
└── docs/
```

---

## 📋 Exemplo de `requirements.txt`

```txt
pandas
numpy
matplotlib
seaborn
plotly
folium
geopandas
shapely
scikit-learn
xgboost
lightgbm
imbalanced-learn
tensorflow
joblib
texttable
requests
tqdm
openpyxl
kaleido
unidecode
pyarrow
```

---

## 🧪 Reprodutibilidade

Para melhorar a reprodutibilidade, o notebook utiliza:

- `random_state=42` em modelos de Machine Learning;
- `seed=42` para geração das faixas etárias sintéticas;
- validação temporal com `TimeSeriesSplit`;
- exportação automática de relatórios e modelos treinados.

Ainda assim, resultados de Deep Learning podem variar conforme:

- versão das bibliotecas;
- CPU/GPU utilizada;
- ambiente de execução;
- número de épocas executadas;
- implementação interna do TensorFlow/Keras.

---

## 🧑‍💻 Como contribuir

Contribuições são bem-vindas! Algumas possibilidades:

1. 🍴 Faça um fork do projeto;
2. 🌿 Crie uma branch:

```bash
git checkout -b melhoria-nova-analise
```

3. 💻 Faça suas alterações;
4. ✅ Teste o notebook;
5. 📤 Envie um pull request.

---

## 📚 Aplicações possíveis

Este notebook pode ser utilizado em:

- 🎓 projetos acadêmicos de Ciência de Dados;
- 🧪 pesquisa aplicada em segurança pública;
- 📊 estudos de indicadores sociais;
- 🗺️ análise territorial de violência;
- 🤖 protótipos de sistemas inteligentes;
- 🏛️ apoio à formulação de políticas públicas;
- 👩‍⚖️ estudos sobre violência de gênero;
- 📈 monitoramento preventivo de risco municipal.

---

## 📝 Citação sugerida

```bibtex
@misc{viana_siprev_mulher_ms_2026,
  author       = {VIANA},
  title        = {SIPREV-Mulher/MS: Sistema Inteligente de Predição e Mapeamento da Violência contra a Mulher em Mato Grosso do Sul},
  year         = {2026},
  note         = {Notebook acadêmico em Python para análise de dados públicos da SEJUSP-MS},
  howpublished = {GitHub repository}
}
```

---

## 📄 Licença

Este projeto pode ser distribuído sob a licença **MIT**, desde que preservados os créditos autorais, a finalidade acadêmica e a responsabilidade ética na utilização dos dados.

---

## 👤 Autor

**VIANA**  
🎓 Ciência dos Dados — UFMS Digital  
📚 Disciplina: Tópicos Interdisciplinares III  
📅 Semestre: 2026.1  

---

## 🌟 Mensagem final

> 💡 A tecnologia útil é aquela que transforma dados públicos em conhecimento socialmente responsável, apoiando prevenção, acolhimento e tomada de decisão baseada em evidências.

**SIPREV-Mulher/MS** — Ciência de Dados aplicada à compreensão e prevenção da violência contra a mulher em Mato Grosso do Sul. 🚺📊🧠

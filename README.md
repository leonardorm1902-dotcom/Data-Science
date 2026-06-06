# 🏠 Airbnb NYC (Albany) — Exploratory Data Analysis

> Análise exploratória dos dados públicos do Airbnb na cidade de Albany, capital do estado de Nova York (EUA).

---

## 📌 Objetivo

Explorar o dataset do Airbnb de Albany (NY) para entender o comportamento dos preços, a distribuição dos imóveis e os fatores que influenciam o custo das hospedagens na região.

---

## 🗂️ Sobre o Dataset

- **Fonte:** [Inside Airbnb](http://insideairbnb.com/get-the-data.html)
- **Cidade:** Albany, Nova York — EUA
- **Dimensões:** ~478 linhas × 16 colunas

### Variáveis principais

| Coluna | Descrição |
|--------|-----------|
| `id` | ID único do imóvel |
| `name` | Nome do anúncio |
| `host_id` | ID do anfitrião |
| `neighbourhood` | Bairro (Ward) do imóvel |
| `latitude` / `longitude` | Localização geográfica |
| `room_type` | Tipo de acomodação |
| `price` | Preço por noite (USD) |
| `minimum_nights` | Mínimo de noites para reserva |
| `number_of_reviews` | Número de avaliações |
| `availability_365` | Dias disponíveis no ano |

> ⚠️ As colunas `neighbourhood_group` e `license` foram descartadas por conterem 100% de valores ausentes.

---

## 🔍 Perguntas Respondidas

1. Quantos atributos e entradas o dataset possui?
2. Qual o percentual de valores ausentes por variável?
3. Como se distribui cada variável? Existem outliers?
4. Qual a correlação entre as variáveis numéricas?
5. Qual tipo de imóvel é mais alugado no Airbnb?
6. Quais são os bairros mais caros de Albany?

---

## 📊 Principais Insights

- **75%** dos imóveis custam menos de **$122/noite**, mas o máximo chega a **$1.078**
- O tipo de quarto mais comum é **Entire home/apt**, seguido de **Private room**
- O **Fifteenth Ward** (Buckingham Lake) é o bairro com maior preço médio
- A correlação entre as variáveis numéricas é, em geral, baixa
- Após remoção de outliers (`price > $400` e `minimum_nights > 30`), a distribuição ficou mais representativa

---

## 🛠️ Tecnologias Utilizadas

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4c72b0?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

---

## ▶️ Como Executar

### 1. Clone o repositório
```bash
git clone https://github.com/SEU_USERNAME/airbnb-albany-eda.git
cd airbnb-albany-eda
```

### 2. Instale as dependências
```bash
pip install -r requirements.txt
```

### 3. Adicione o dataset
Baixe o arquivo `listings.csv` em [Inside Airbnb → Albany](http://insideairbnb.com/get-the-data.html) e coloque em `data/raw/listings.csv`

### 4. Execute o notebook
```bash
jupyter notebook notebooks/Projeto_01_Analisando_Dados_do_Airbnb_NY_Albany.ipynb
```

---

## 📝 Conclusão

A análise demonstrou como etapas de pré-processamento — tratamento de valores ausentes e remoção de outliers — são essenciais para resultados mais precisos. Após a limpeza, foi possível explorar com mais clareza o comportamento dos preços e a distribuição geográfica dos imóveis em Albany.

---

## 👤 Autor

**Leonardo Rodrigues Machado**

[![LinkedIn]www.linkedin.com/in/leonardo-rodrigues-machado-196a84193


---

*Projeto desenvolvido como parte da minha jornada de aprendizado em Ciência de Dados* 🚀

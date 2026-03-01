# 📊 CD – Análise de Desempenho no ENEM

Projeto desenvolvido na disciplina de Ciência de Dados com o objetivo de identificar perfis de desempenho no ENEM por meio de técnicas de clusterização não supervisionada.

---

## 🎯 Objetivo

- Identificar perfis de desempenho dos participantes do ENEM.
- Analisar fatores correlatos como renda familiar e tipo de escola.
- Estimar o percentual de estudantes de baixa renda no grupo de alto desempenho.
- Avaliar se escolas públicas conseguem mitigar desigualdades socioeconômicas.

---

## 📁 Fonte dos Dados

Os dados utilizados são os **Microdados do ENEM**, disponibilizados publicamente pelo INEP.

Página oficial:  
https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/microdados/enem

Arquivo utilizado neste projeto:  
https://download.inep.gov.br/microdados/microdados_enem_2023.zip

⚠️ **Importante:**  
O arquivo de dados **não está incluído no repositório**, pois possui tamanho elevado.

---

## 📦 Estrutura do Projeto

```
cd-analise-desempenho-enem/
│
├── Dados/                 ← (pasta deve permanecer vazia no repositório)
│
├── PROJETO_4_Desempenho_Escolar_no_ENEM.ipynb
├── requirements.txt
└── README.md
```

---

## ⚙️ Como Reproduzir o Projeto

### 1️⃣ Clonar o repositório

```bash
git clone https://github.com/seu-usuario/cd-analise-desempenho-enem.git
cd cd-analise-desempenho-enem
```

---

### 2️⃣ Criar ambiente virtual (opcional, recomendado)

**Linux/Mac**

```bash
python -m venv .venv
source .venv/bin/activate
```

**Windows**

```bash
python -m venv .venv
.venv\Scripts\activate
```

---

### 3️⃣ Instalar dependências

```bash
pip install -r requirements.txt
```

---

### 4️⃣ Baixar e inserir os dados

1. Baixe o arquivo:
   https://download.inep.gov.br/microdados/microdados_enem_2023.zip

2. Extraia o conteúdo.

3. Copie o arquivo:

   ```
   MICRODADOS_ENEM_2023.csv
   ```

4. Coloque dentro da pasta:

   ```
   Dados/
   ```

A estrutura final deve ficar assim:

```
Dados/
└── MICRODADOS_ENEM_2023.csv
```

---

## ▶️ Executando o Projeto (VS Code)

1. Abra a pasta do projeto no **VS Code**.
2. Abra o arquivo:

   ```
   PROJETO_4_Desempenho_Escolar_no_ENEM.ipynb
   ```

3. Execute todas as células (**Run All**) ou célula por célula.

O notebook utiliza o seguinte caminho para leitura do arquivo:

```python
df = pd.read_csv(
    "Dados/MICRODADOS_ENEM_2023.csv",
    sep=";",
    encoding="latin-1"
)
```

---

## 🤖 Algoritmos Utilizados

- **K-Means**
- **Clusterização Hierárquica (Ward)**
- **DBSCAN**

---

## 📊 Métricas de Avaliação

- Silhouette Score  
- Calinski-Harabasz  
- Davies-Bouldin  
- Método do Cotovelo (Inércia)  
- ARI (Adjusted Rand Index)  

---

## 📈 Principais Resultados

- Identificação de dois grandes perfis de desempenho acadêmico.
- Associação consistente entre renda familiar e desempenho.
- Maior proporção de alto desempenho em escolas privadas e federais.
- Evidência de que fatores socioeconômicos influenciam significativamente o desempenho.

---

## ⚠️ Observações

- Projeto acadêmico desenvolvido para a disciplina de Ciência de Dados.
- Utiliza dados públicos e anonimizados.
- O dataset não está incluído no repositório devido ao seu tamanho.

---

## 👨‍💻 Autores

- **12311BSI303** — Diogo Arantes Borges Andrade  
- **1241BSI355** — Leandro Coutinho Cesário Júnior  
- **12311BSI282** — Vitor Silva Medeiros  
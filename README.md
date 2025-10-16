# 🐍 Py-SQL GitHub Data Project

Este projeto demonstra, na prática, como integrar **Python** e **SQL** para manipular, transformar e analisar dados — tudo dentro de um pipeline estruturado e versionado com **Git e GitHub**.

O projeto foi desenvolvido como parte dos estudos na pós graduação em **Engenharia de Dados e Inteligência Artificial** da Faculdade Anhanguera, aplicando boas práticas de organização, versionamento e reprodutibilidade.

---

## 📂 Estrutura do Projeto
```
py-sql-github-data-project/
│
├── data/ # Dados locais (não versionados)
│ ├── dados_duckdb.db # Banco de dados DuckDB
│
├── landing/ # Dados coletados em formato bruto (CSV)
│ ├── z0019_1.csv
│ └── z0019_2.csv
│
├── scripts/ # Notebooks Jupyter para exploração e análise
│ ├── ingestao.ipynb
│ ├── refinamento.ipynb
│ └── enriquecimento.ipynb
│
├── .gitignore # Arquivos ignorados pelo Git
└── README.md # Este arquivo 🙂
```
---

## 🚀 Etapas do Pipeline

1. **Ingestão de Dados**
   - Leitura de arquivos CSV da pasta `landing/`;
   - Armazenamento no banco DuckDB;
   - Verificações de schema e tipos de dados.

2. **Refinamento**
   - Limpeza de colunas, padronização e tratamento de valores nulos;
   - Conversão de tipos e normalização dos dados.

3. **Enriquecimento**
   - Combinação de tabelas;
   - Criação de novas métricas e indicadores;
   - Geração de datasets analíticos.

---

## ⚙️ Como Executar Localmente

### 1 - Criar ambiente virtual

```bash
python -m venv venv

```
Ativar:

* Windows

```bash
venv\Scripts\activate
```
* Linux

```bash
source venv/bin/activate
```

## 2 - Instalar dependências:
```bash
pip install -r requirements.txt
```
## 3 - Executar os scripts

Você pode rodar as etapas separadamente:

```bash
python scripts/ingestao.py
python scripts/refinamento.py
python scripts/enriquecimento.py
```
Ou abrir os notebooks:

```bash
jupyter notebook
```
Principais Tecnologias:

| Categoria              | Ferramenta   |
| ---------------------- | ------------ |
| Linguagem              | Python 3     |
| Banco de Dados         | DuckDB       |
| Manipulação de Dados   | Pandas       |
| Notebooks              | Jupyter      |
| Controle de Versão     | Git + GitHub |

🧾 Boas Práticas Implementadas
✅ Estrutura de diretórios padronizada ✅ Versionamento limpo com .gitignore ✅ Scripts separados por etapas do pipeline ✅ Documentação organizada e reproduzível ✅ Uso de ambiente virtual e requirements.txt

🧑‍💻 Autor
César Augusto Fernandes

📍 Brasil

💼 Engenheiro de Dados em formação

🔗 GitHub

🪪 Licença
Este projeto é de uso livre para fins educacionais e experimentais. Sinta-se à vontade para estudar, adaptar e compartilhar.

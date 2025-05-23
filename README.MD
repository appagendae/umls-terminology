# UMLS Terminology – Clinical Term Analysis with Python

Este repositório contém um notebook desenvolvido para análise de termos clínicos utilizando a API da UMLS (Unified Medical Language System). É voltado a estudantes do curso de IA Aplicada à Saúde, com foco na compreensão da primeira atividade formativa.

## 📌 Objetivos do Projeto

- Explorar a API da UMLS para buscar conceitos e termos clínicos.
- Demonstrar técnicas de pré-processamento textual aplicadas a registros médicos.
- Facilitar o entendimento de como ontologias clínicas podem ser utilizadas em IA aplicada à saúde.
- Servir como base prática para atividades da disciplina **IA Aplicada à Saúde** – PUCPR.

## 🧠 Conceitos Envolvidos

- Terminologias biomédicas padronizadas (ex: SNOMED CT, MeSH, LOINC).
- Identificadores únicos de conceitos (CUIs).
- Pré-processamento de linguagem natural (tokenização, normalização).
- Acesso programático via API REST.
- Uso de bibliotecas Python como `requests`, `pandas`, `sklearn` e `matplotlib`.

## 📂 Estrutura do Repositório

```

umls-terminology/
│
├── UMLS_text_analysis.ipynb      # Notebook principal com análise e comentários
├── requirements.txt              # Dependências do projeto
├── .env.example                  # Exemplo de arquivo .env para a chave da UMLS API
└── README.md                     # Este arquivo

````

## ⚙️ Como Usar

1. **Clone este repositório:**

```bash
git clone https://github.com/appagendae/umls-terminology.git
cd umls-terminology
````

2. **Crie um ambiente virtual (opcional, mas recomendado):**

```bash
python -m venv venv
source venv/bin/activate  # no Windows: venv\Scripts\activate
```

3. **Instale as dependências:**

```bash
pip install -r requirements.txt
git clone git@github.com:appagendae/PortugueseClinicalNER.git
```

> Utilizei como base os arquivos do repositório PortugueseClinicalNER. Deixe esse conteúdo salvo na mesma pasta do notebook.

4. **Configure sua chave da UMLS API:**

Crie um arquivo `.env` com o seguinte conteúdo:

```env
API_KEY_UMLS=YOUR_UMLS_API_KEY
```

> ⚠️ Você precisa obter uma chave gratuita se cadastrando em: [https://uts.nlm.nih.gov/uts/signup-login](https://uts.nlm.nih.gov/uts/signup-login)

5. **Execute o notebook:**

Abra o Jupyter Notebook ou o VSCode e execute o arquivo `UMLS_text_analysis.ipynb`.

## 🧪 Exemplos de Uso

* Buscar o CUI (Concept Unique Identifier) de termos como "diabetes mellitus".
* Mapear termos clínicos para múltiplas ontologias.
* Gerar visualizações básicas da distribuição de termos em conjuntos de dados clínicos.
* Atenção especial no passo 6. Pode demorar muito dependendo de quantos itens processar de uma vez.

## 🙋‍♀️ Para quem é este projeto?

Este projeto é ideal para:

* Estudantes de IA Aplicada à Saúde.
* Profissionais de TI que atuam com dados clínicos.
* Interessados em IA com foco em terminologia médica.

## 📚 Recursos Complementares

* [UMLS Documentation](https://www.nlm.nih.gov/research/umls/index.html)
* [UMLS API Reference](https://documentation.uts.nlm.nih.gov/rest/home.html)
* [SNOMED CT Browser](https://browser.ihtsdotools.org/)
* [BioPortal Ontologies](https://bioportal.bioontology.org/)

## 📄 Licença

Este projeto está licenciado sob os termos da **MIT License** – veja o arquivo [LICENSE](LICENSE) para detalhes.

---

## 🌐 English Summary

This repository contains a Python notebook that demonstrates how to access and process clinical terms using the UMLS API. It's part of the Applied AI in Healthcare course at PUCPR and aims to help students understand biomedical terminologies and use them in real-world AI applications.
# 🧠 MVP — Gestão de Locações de Espaços Publicitários em Lojas

Este projeto foi desenvolvido como parte da disciplina de Engenharia de Dados da pós-graduação da PUC-Rio.

O objetivo foi construir um pipeline analítico para a **gestão de espaços publicitários locados dentro de lojas físicas**, permitindo gerar insights relevantes para a área de trade marketing.

> **Observação:** Foram utilizados dados do ambiente profissional do autor (Bemol S.A.), porém, **nenhuma informação sensível foi utilizada**. Alguns dados foram alterados ou anonimizados com o único objetivo de **evitar qualquer identificação direta de registros reais**.

---

## 🎯 Objetivo

Criar uma solução de dados que permita:
- Analisar os fornecedores que mais investem em ativações nas lojas
- Identificar os espaços mais e menos utilizados
- Avaliar a taxa de ocupação por loja
- Melhorar a tomada de decisão da área de trade marketing

---

## 🧱 Estrutura do Pipeline

O pipeline foi construído com base no modelo em camadas:

```
📁 Bronze → Dados crus importados do DBFS  
📁 Silver → Dados tratados, normalizados e modelados  
📁 Gold   → Tabelas analíticas para responder perguntas de negócio
```

A modelagem utilizada foi o **esquema estrela**, com:
- `dim_espaco`: dimensão dos espaços publicitários disponíveis
- `fato_locacao`: tabela fato com as locações realizadas

---

## 🛠️ Tecnologias e Ferramentas

- **Databricks** (PySpark + Delta Lake)
- **Python**
- **DBFS**
- **Markdown**
- **matplotlib** (visualizações)
- **GitHub** (entrega e versionamento)

---

## 📂 Estrutura do Repositório

```
.
├── notebook_mvp.ipynb                            # Notebook com código, análises e Markdown estruturado
├── notebook_mvp.dbc                              # Versão opcional para reimportar diretamente no Databricks
├── Analises do problema proposta e autoavaliacao.pdf  # Documento com análise do problema e autoavaliação final
├── imagens/                                      # Evidências visuais da execução e análise (prints organizados)
├── README.md                                     # Este arquivo de documentação
```

---

## 📸 Evidências da Execução

Os resultados foram registrados por meio de **screenshots** das execuções no Databricks, disponíveis na pasta `imagens/`.

As evidências incluem:

1. ✅ Coleta dos dados via DBFS  
2. ✅ Leitura e persistência na camada Bronze  
3. ✅ Transformações e filtragem na Silver  
4. ✅ Modelagem em esquema estrela  
5. ✅ Construção das tabelas Gold  
6. ✅ Gráficos de análise com interpretação de cada pergunta do negócio

---

## 📎 Formatos Exportados

- `notebook_mvp.ipynb`: Notebook interativo com códigos, análises, Markdown e gráficos (recomendado)
- `notebook_mvp.dbc`: Alternativa para importação no próprio ambiente Databricks
- `Analises do problema proposta e autoavaliacao.pdf`: Documento complementar com reflexões, análises e autoavaliação final

---

## ✍️ Autor

**Gean Cunha**  
Pós-graduação em Engenharia de Software – PUC-Rio  



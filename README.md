# Q&A Técnico com LLM + RAG

Este é um projeto base de um aplicativo de perguntas e respostas técnicas usando a arquitetura RAG (Retrieval-Augmented Generation) com LangChain e OpenAI.

## Requisitos

- Python 3.10+

- Conta na OpenAI (para embeddings e geração de respostas)

## Instalação

```bash
git clone https://github.com/seu-usuario/qa-tecnico-rag-llm.git
cd qa-tecnico-rag-llm
python -m venv venv
source venv/bin/activate  # ou .\venv\Scripts\activate no Windows
pip install -r requirements.txt
```

Crie um arquivo `.env` com sua chave da OpenAI:

```env
OPENAI_API_KEY=sk-...
```

## Indexação dos documentos

Coloque seus documentos em `data/docs` e execute:

```bash
python -m app.ingest
```

## Executando a aplicação

```bash
streamlit run app/main.py
```

## Exemplo de uso

Digite perguntas como:

- "Como funciona o algoritmo A*?"

- "O que é o padrão Singleton?"

##  To-do

- Integração com Stack Overflow

- Suporte a arquivos HTML e DOCX

- Filtro por data ou fonte

- Feedback do usuário

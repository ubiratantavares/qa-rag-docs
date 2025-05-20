O repositório base do projeto **Q\&A Técnico com LLM + RAG** foi criado com a seguinte estrutura:

```
qa-tecnico-rag-llm/
├── app/
│   ├── main.py            # Interface com Streamlit
│   ├── qa_chain.py        # Cadeia RAG com LangChain
│   ├── ingest.py          # Indexação de documentos
│   ├── config.py          # Chaves e configs
├── data/docs/             # Documentos técnicos
├── requirements.txt       # Dependências
└── README.md              # Instruções completas
```

### Próximos Passos

1. Crie um arquivo `.env` com sua chave da OpenAI.

2. Adicione arquivos técnicos em `data/docs/`.

3. Execute `python -m app.ingest` para indexar os dados.

4. Inicie com `streamlit run app/main.py`.

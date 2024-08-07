# NLP-2024-1
## Trabalho Final de NLP
**Amanda Spellen** - 22153134
**Lucas Darcio** - 22153138

Esse repo contém os entregáveis para o trabalho final para a disciplina de TEBD (NLP) do ano de 2024/1.

## Descrição dos arquivos:
- `Relatório - TP03 (NLP 2024/1)`: relatório contendo a descrição detalhada de todos os processos realizados em cada etapa do trabalho
- `artefatos`: contém os arquivos de saída gerados em cada etapa do trabalho, e que são usados em outras etapas:
	- `legislacao_dataset.zip`: os dados pré-processados dos documentos legislativos
	- `instructions.json`: arquivo de instruções sintéticas
	- `TinyLlama-1.1B-Fine-Tuned.zip`: pasta com os adaptadores gerados pelo LoRA
	- `testes_fine_tuning.json`: a coleção de testes e resultados feitos com o modelo com fine-tuning e baseline
	- `vectorstore_1000_chunks.db.zip` e `vectorstore_1200_chunks.db.zip`: pastas com os documentos e embeddings usados no RAG, com a versão menos (1000 chunks) e mais granular (1200 chunks) do banco de dados

- `codigos`: os notebooks onde os artefatos foram gerados:
	- `TP03 - Geracao de instrucoes.ipynb`: com base nos dados pré-processados, gera mais de 1000 instruções sintéticas
	- `TP03 - Fine-Tuning`: usa as instruções sintéticas para treinar um LLM para o tema de legislação acadêmica
	- `TP03 - RAG`: com base nos dados pré-processados, cria um banco de dados vetorial e usa embeddings para incluir trechos interessantes de documentos como contexto para modelo

> Nota: os notebooks foram criados para serem executados no Google Colaboratory.

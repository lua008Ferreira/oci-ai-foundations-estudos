# 5. Portfólio de IA da OCI, OCI Generative AI e Oracle 23ai (25% da prova)

Itens marcados com (confirmar no curso) não estavam na fonte principal e podem mudar.

## Portfólio em camadas
- **Infraestrutura de IA:** GPUs e redes rápidas. (confirmar no curso)
- **ML e ciência de dados:** **OCI Data Science** (você constrói o modelo).
- **Serviços prontos:** Generative AI, Language, Vision, Speech e Document Understanding.
- **IA nas aplicações:** recursos embutidos em produtos Oracle. (confirmar no curso)

**Regra de ouro:** serviço pronto (pré-treinado) resolve uma tarefa sem treinar nada. Data Science é para construir o próprio modelo.

## OCI Generative AI
- Acesso a **modelos fundacionais prontos**, com personalização, agentes e integração com dados da empresa.
- **Fine-tuning** com técnicas como **LoRA** e **T-Few**.
- Playground, clusters dedicados e agentes com RAG. (confirmar no curso)
- Os modelos disponíveis mudam; confira no curso.

## RAG
1. Documentos viram embeddings, guardados em um banco vetorial.
2. A pergunta vira vetor.
3. O sistema busca os trechos mais parecidos.
4. Os trechos vão no prompt e o LLM responde com base neles.

Vantagens: dados atualizados, menos alucinação e sem retreinar.

## Oracle Database 23ai
- **AI Vector Search:** guarda vetores (embeddings) e faz busca por similaridade no banco, ao lado dos dados de negócio. (confirmar no curso)
- **Select AI:** perguntas em linguagem natural que viram SQL. (confirmar no curso)

## Pegadinhas
- Dados que mudam sempre: RAG. Estilo ou tarefa muito específica com dados rotulados: fine-tuning.
- Busca por significado: embeddings e busca vetorial.
- Serviço pronto não exige treinar. Data Science exige construir o modelo.

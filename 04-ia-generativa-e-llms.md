# 4. IA Generativa e LLMs (15% da prova)

**Ideia central:** IA generativa **cria conteúdo novo**. Um **LLM** é um transformer treinado com enormes volumes de texto, que **prevê o próximo token**.

## Conceitos
- **Token:** pedaço de texto. Custo e limites são medidos em tokens.
- **Janela de contexto:** quantos tokens o modelo considera de uma vez.
- **Parâmetros:** os pesos do modelo.
- **Modelo fundacional:** treinado de forma geral e adaptado a várias tarefas.
- **Multimodal:** mais de um tipo de dado.
- **Tipos de transformer:** só encoder (entende, como o BERT), só decoder (gera, como o GPT), encoder-decoder (traduz e resume, como o T5).

## Parâmetros de geração
- **Temperature:** baixa = previsível, alta = variada e criativa.
- **Top-k / top-p:** limitam as opções de próxima palavra.
- **Max tokens:** tamanho máximo da resposta.
- **Stop sequence:** onde o modelo para.
- **Penalidades de frequência e presença:** reduzem repetição.

## Engenharia de prompt
**Zero-shot** (sem exemplo), **few-shot** (com exemplos), **chain-of-thought** (raciocínio passo a passo). Melhora a resposta sem treinar o modelo.

## Três formas de personalizar um LLM
| Técnica | O que faz | Quando usar |
|---|---|---|
| **Prompt engineering** | Melhora pelo prompt | Primeiro passo, barato |
| **RAG** | Busca trechos externos e coloca no prompt | Dados da empresa que mudam; reduz alucinação |
| **Fine-tuning** | Treina com dados próprios | Estilo ou tarefa muito específica, com dados rotulados |

**RAG por dentro:** documentos viram **embeddings**, guardados em um **banco vetorial**. A pergunta também vira vetor, o sistema busca os mais parecidos (similaridade) e envia ao LLM.

## Riscos
**Alucinação**, viés, vazamento de dados sensíveis e **prompt injection**. Mitigações: RAG, revisão humana, filtros e governança.

## Pegadinhas
- Dados que mudam sempre: RAG, não fine-tuning.
- Temperatura alta não deixa o modelo mais correto, só mais variado.
- Fine-tuning exige dados rotulados, custo e tempo. RAG não retreina.

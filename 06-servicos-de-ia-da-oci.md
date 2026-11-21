# 6. Serviços de IA da OCI (20% da prova)

Fonte principal: artigo "O ecossistema de OCI AI", da Alura.

| Serviço | O que faz | Exemplo |
|---|---|---|
| **OCI Language** | Texto: idioma, sentimento, frases-chave, entidades, PII, tradução | Analisar avaliações de clientes |
| **OCI Vision** | Imagem: objetos, classificação, OCR, rostos | Achar defeitos em peças |
| **OCI Speech** | Áudio para texto (ASR), inclusive em tempo real; saída JSON e SRT | Legendar vídeos e ligações |
| **OCI Document Understanding** | Texto, tabelas e pares chave-valor de documentos; classificação | Ler notas fiscais |
| **OCI Data Science** | Construir, treinar, implantar e monitorar modelos em Python | Modelo de previsão |
| **OCI Generative AI** | Modelos fundacionais prontos, personalização e agentes | Chatbots e resumos |

## Truque de memória (o tipo de dado aponta o serviço)
Texto: Language. Imagem: Vision. Voz: Speech. Documento: Document Understanding. Texto gerado: Generative AI. Modelo próprio: Data Science.

**Modelos personalizados:** Language, Vision e Document Understanding permitem treinar modelos personalizados. O ponto de partida é pré-treinado.

## OCI Data Science
- Notebooks (JupyterLab) e Python.
- **Model Catalog** guarda os modelos; dá para implantar e consumir por API.
- Princípios: **Accelerated**, **Collaborative** e **Enterprise Grade**.

## Formas de acesso
Console OCI, API REST, SDKs (Python, Java e outros) e OCI CLI.

## Pegadinhas
- Vision x Document Understanding: foto de objeto é Vision. Documento com campos e tabelas é Document Understanding.
- Speech converte voz em texto. O sentimento do texto é do Language.
- PII é detectado pelo Language.

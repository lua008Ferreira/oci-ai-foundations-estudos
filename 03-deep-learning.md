# 3. Deep Learning (15% da prova)

**Ideia central:** ML com **redes neurais de muitas camadas**. Aprende as características dos dados sozinho. Funciona muito bem com dados não estruturados (imagem, texto, áudio), mas pede muitos dados e GPUs.

## Como uma rede neural funciona
- **Neurônio:** recebe entradas, multiplica por **pesos**, soma e passa por uma **função de ativação**.
- **Camadas:** entrada, ocultas e saída. "Profundo" = muitas camadas ocultas.
- **Treino:** o modelo erra, mede o erro pela **função de perda** e ajusta os pesos por **backpropagation**, usando o **gradiente descendente**.
- **Época:** uma passada completa pelos dados de treino.

## Arquiteturas
| Arquitetura | Boa para | Palavra-chave |
|---|---|---|
| **CNN** | Imagens | Filtros que detectam bordas e formas |
| **RNN** | Sequências | "Memória" do passo anterior |
| **LSTM** | Sequências longas | RNN que lembra melhor |
| **Transformer** | Texto e linguagem (base dos LLMs) | Atenção, processa em paralelo |
| **GAN** | Gerar imagens e dados sintéticos | Gerador x discriminador |

**Atenção (transformers):** mede quais partes da entrada importam mais para o contexto. Processa a sequência em paralelo.

## ML tradicional x deep learning
- **ML tradicional:** menos dados, mais fácil de explicar, a pessoa escolhe as variáveis.
- **Deep learning:** muitos dados e GPU, "caixa-preta", aprende as variáveis sozinho.

## Termos complementares
- **Funções de ativação:** ReLU, sigmoide e softmax (probabilidades na saída de classificação multiclasse).
- **Hiperparâmetros:** definidos antes do treino (taxa de aprendizado, camadas, épocas). **Parâmetros (pesos):** aprendidos no treino.
- **Contra overfitting:** mais dados, **dropout** e **early stopping**.
- **Transfer learning:** reaproveitar um modelo treinado e adaptar à sua tarefa.
- **Treino x inferência:** aprender (caro, GPU) x usar o modelo pronto.

## Quando usar o quê
Imagem: CNN. Texto: transformer. Sequências curtas: RNN/LSTM. Dados sintéticos: GAN. Poucos dados ou necessidade de explicar: ML tradicional.

## Pegadinhas
- Deep learning não é sempre melhor: com poucos dados, ML tradicional costuma ir melhor.
- Backpropagation ajusta os pesos, não gera a resposta.
- Hiperparâmetros antes do treino, pesos durante o treino.


# Large Language Models

## Lesson Goal:

Participants train and evaluate microgpt, a pocket-size LLM.

## Time Frame:

90'

## Key Concepts:

- tokenize
- embedding layer
- attention block
- MLP
- unembedding layer
- softmax

## Key Phrases

*"LLMs convert tokens to embeddings and embeddings to tokens"*

## Warmup:

- give microgpt code to participants
- ask them to run it (including the helper script to download the data)
- insert some print statements to check the internal states (parameter arrays, loss function during training, output prog)
- prepare a few questions

## Content Delivery:

- give participants the full list of tokens in ChatGPT (https://emaggiori.com/chatgpt-all-tokens/)
- let them work on prepared questions, e.g.:

  what is the difference between a token and a word?
  in what situtations does the difference matter?

- explain the rough structure, draw a schematic:

IN -> EMBEDDING -> [ATT + MLP] x 96 -> UNEMBEDDING -> SOFTMAX -> token prob

- explain where temperature comes in

## Equations:

Attention(Q, K, V) = softmax(QK^T / sqrt(d)) * V

## Material:
 
GPT3 by numbers:

- 200 billion parameters total
- context size 2048 (feels tiny 2 years later)
- distinct tokens: 50257
- embedding dimension: 12288
- attention blocks: 96
- attention heads per block: 96
- key dimension in attention: 128

Total parameters:

- embedding layer: 12000 x 50000 = 600M
- unembedding layer: 12000 x 50000 = 600M
- attention block 4 matrices of size 128 x 96 x 96 x 12000
- MLP part: 2 x 12000 x 50000

should be around 200B in total

## Comments:

- to make any sense out of it, the particpants should have a good idea about ANNs in general and gradient descent
- see the 3blue1brown video explaining LLMs

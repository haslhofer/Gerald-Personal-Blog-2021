---
title: Interesting Papers
date: "2021-10-24T23:46:37.121Z"
template: "post"
draft: false
slug: "interesting-papers"
category: "Notes"
tags:
  - "Science"
description: "Summaries of interesting papers I read"
socialImage: "/media/image-2.jpg"
---
# Rethinking Attention with Performers

[Paper on arxiv](https://arxiv.org/abs/2009.14794v3)


## Things I don't yet understand

### What is the canonical Transformer architecture
From [Wikipedia](https://en.wikipedia.org/wiki/Transformer_(machine_learning_model)): leverages **attention**, which differentially weighs the significance of each part of the input. Attention lets a model draw context from any position of the preceding sequence.

It adopts a **encoder / decoder architecture**
- Encoder generates encoding of which parts of the input are relevant to each other
- Decoder generates an output sequence - takes all encodings and their contextual data to achieve that goal

From [Transfomers Explained](https://towardsdatascience.com/transformers-explained-visually-part-1-overview-of-functionality-95a6dd460452):
- Transformers inherently deal with sequences (input and output)
- Encoder has 
    - self-attention layer 
    - feed-forward layer
    - residual skip connection
    - "layer norm" layer
- Decoder has
    - self-attention layer
    - encoder / decoder attention
    - feed forward layer

Training:
- Input sequence converted into embeddings (with positional encoding)
- Encoder converts embeddings into encodings
- Target sequence pre-pended with start-of-sentence token, converted into embedding, fed to decoder
- Generate encoded representation (together with Encoder representation)
- Output layer converts it into output sequence
- Back propagation -> generate gradients 

### What is a feed-forward layer

### What is a residual skip conneciton

### Difference between embedding and encoding

### How does back propagation work
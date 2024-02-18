
> [!Info] Explanation
> Reading List is usually simply a list that one can keep to add, new reading material. In another episode of the blog we will explore how to set up google chrome or the ARC browser to quickly add links, and snippets directly into this note and have it being up to date. Subscribe to the [newsletter here](https://ilyashabanov.substack.com/), if you don't want to miss it. 


# Comparison between **transformer-based** models and **RNNs (Recurrent Neural Networks)** for various NLP tasks:

1. **“A Comparative Study on Transformer vs RNN in Speech Applications”**:
    
    - This study focuses on the performance of **Transformer** models compared to conventional **RNNs** in various speech processing tasks, including automatic speech recognition (ASR), speech translation (ST), and text-to-speech (TTS). [The paper reveals insights and benefits of using Transformers for ASR and other related applications](https://arxiv.org/abs/1909.06317)[1](https://arxiv.org/abs/1909.06317).
2. **“Transformers are Multi-State RNNs”**:
    
    - While this paper primarily discusses transformers, it provides an interesting perspective. It demonstrates that decoder-only transformers can be conceptualized as infinite multi-state RNNs. [This work bridges the gap between the two architectures and sheds light on their similarities](https://arxiv.org/abs/2401.06104)[2](https://arxiv.org/abs/2401.06104).
3. **“Overview of the Transformer-based Models for NLP Tasks”**:
    
    - Although this paper doesn’t directly compare transformers and RNNs, it provides an overview of transformer-based models in NLP tasks. [It could serve as a useful reference for understanding the transformer architecture and its applications](https://annals-csis.org/proceedings/2020/drp/pdf/20.pdf)[3](https://annals-csis.org/proceedings/2020/drp/pdf/20.pdf).
4. **“From RNNs to Transformers”**:
    
    - This article discusses the paradigm shift from RNNs to transformers in sequence-based tasks. [While it doesn’t present research findings, it provides insights into why transformers have gained prominence in NLP](https://www.baeldung.com/cs/rnns-transformers-nlp)[4](https://www.baeldung.com/cs/rnns-transformers-nlp).

## RNN in CSNMT

Certainly! Let’s explore the state-of-the-art research related to **Recurrent Neural Networks (RNNs)** in the context of **code-switched Neural Machine Translation (NMT)**:

1. **“Code-Switching with Word Senses for Pretraining in Neural Machine Translation”**:
    
    - This recent work introduces **Word Sense Pretraining for Neural Machine Translation (WSP-NMT)**.
    - It leverages word sense-specific information from **Knowledge Bases** to improve translation quality in code-switching scenarios.
    - [The approach shows significant improvements in overall translation quality and robustness across various challenging data and resource-scarce scenarios](https://arxiv.org/abs/2310.14050v1)[1](https://arxiv.org/abs/2310.14050v1).
2. **“Code-Switching for Enhancing NMT with Pre-Specified Translation”**:
    
    - This paper explores leveraging user-provided translations to constrain NMT.
    - It categorizes methods into placeholder tags for lexicon words and hard constraints during decoding.
    - [The study discusses how these methods impact translation fidelity](https://arxiv.org/abs/2310.14050v1)[2](https://aclanthology.org/N19-1044/).
3. **“Code-Switching for Enhancing NMT with Pre-Specified Translation”**:
    
    - Another study investigates code-switching for enhancing NMT with pre-specified translation.
    - [It explores shared embeddings, pointer networks, and the copying mechanism to improve translation quality](https://arxiv.org/abs/2310.14050v1)[3](https://arxiv.org/pdf/1904.09107v4.pdf).

While RNNs have been widely used in NLP, their performance in code-switching scenarios may be limited due to challenges like long-range dependencies and handling rare words. Researchers continue to explore novel architectures and techniques to enhance RNN-based models for code-switching. 🌟📚

For more detailed insights, I recommend reading the full papers linked above. They provide valuable information on RNNs in code-switching contexts.

----
Positional embeddings play a crucial role in **transformer-based architectures** by providing information about the order of tokens in a sequence. While the original transformer model introduced a simple sinusoidal positional encoding, there have been subsequent improvements to enhance this mechanism. Let’s explore some ways to improve positional embeddings:

1. **Learnable Positional Embeddings**:
    
    - Instead of using fixed sinusoidal functions, consider making positional embeddings **learnable**.
    - Train the model to adaptively adjust the embeddings based on the specific task and data.
2. **Relative Positional Encodings**:
    
    - Recent research has focused on **relative positional encodings**.
    - These embeddings capture the relative distances between tokens, allowing the model to learn context-aware positional information.
    - [Explore methods like **relative sinusoidal encodings** or **relative position encodings based on attention patterns**](https://arxiv.org/abs/2009.13658)[1](https://arxiv.org/abs/2009.13658).
3. **Hybrid Approaches**:
    
    - Combine absolute positional encodings (like sinusoidal functions) with relative positional information.
    - This hybrid approach can capture both global and local context.
4. **Positional Encoding Variants**:
    
    - Investigate alternative positional encoding functions beyond sine and cosine waves.
    - Consider using **Gaussian functions**, **learned embeddings**, or **non-linear transformations**.
5. **Task-Specific Positional Embeddings**:
    
    - Design positional embeddings that are specific to the task.
    - For example, in code-switching NMT, consider embeddings that capture language switches or domain-specific positions.
6. **Positional Embeddings for Segments**:
    
    - If your input contains segments (e.g., sentences, paragraphs), create separate positional embeddings for each segment.
    - This can help the model distinguish between different parts of the input.
7. **Attention Distance Reduction**:
    
    - Investigate how different positional embeddings affect the attention distance in the final layers.
    - Some embeddings may lead to shorter attention spans, which could be beneficial for certain tasks.

Remember that the choice of positional embeddings depends on the specific problem, dataset, and architecture. Experimentation and thorough evaluation are essential to determine the most effective approach for your use case! 🌟🚀

[For more detailed insights, you can explore research papers like “Improve Transformer Models with Better Relative Position Embeddings” and “A Simple and Effective Positional Encoding for Transformers” linked in the previous responses](https://arxiv.org/abs/2009.13658)[1](https://arxiv.org/abs/2009.13658)[2](https://aclanthology.org/2021.emnlp-main.236.pdf).
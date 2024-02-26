---
doi: 
category: literaturenote  
tags: Transformer, language identification, done LR  
citekey: songSwitchGLATMultilingualParallel2022  
status: unread
Rating: 0/5
Title: switch-GLAT: Multilingual Parallel Machine Translation Via Code-Switch Decoder
ShortSummary: Multilingual machine translation aims to develop a single model for multiple language directions. However, existing multilingual models based on Transformer are limited in terms of both translation performance and inference speed. In this paper, we propose switch-GLAT, a non-autoregressive multilingual machine translation model with a code-switch decoder. It can generate contextual code-switched translations for a given source sentence, and perform code-switch back-translation, greatly boosting multilingual translation performance. In addition, its inference is highly efficient thanks to its parallel decoder. Experiments show that our proposed switch-GLAT outperform the multilingual Transformer with as much as 0.74 BLEU improvement and 6.2x faster decoding speed in inference.
dateread: {DATE}
---

> [!Cite]
> Song, Z., Zhou, H., Qian, L., Xu, J., Cheng, S., Wang, M., & Li, L. (2022, January 28). _switch-GLAT: Multilingual Parallel Machine Translation Via Code-Switch Decoder_. International Conference on Learning Representations. [https://openreview.net/forum?id=5HvpvYd68b](https://openreview.net/forum?id=5HvpvYd68b)
  
>[!Synth]  
>**Contribution**::  
>  
>**Related**:: 
>  
  
>[!md]-
>**FirstAuthor**:: Song, Zhenqiao  
>**Author**:: Zhou, Hao  
>**Author**:: Qian, Lihua  
>**Author**:: Xu, Jingjing  
>**Author**:: Cheng, Shanbo  
>**Author**:: Wang, Mingxuan  
>**Author**:: Li, Lei  
~  
>**Title**:: switch-GLAT: Multilingual Parallel Machine Translation Via Code-Switch Decoder
>**Year**:: 2022
>**Citekey**:: songSwitchGLATMultilingualParallel2022
>**itemType**:: conferencePaper
  
> [!LINK]-
> 
> [Full Text PDF](file://C:\Users\Wong\Zotero\storage\S4J9XJY7\Song%20et%20al.%20-%202022%20-%20switch-GLAT%20Multilingual%20Parallel%20Machine%20Transla.pdf) 
> [switch-GLAT.pdf](file://C:\Users\Wong\Zotero\storage\2FZF2KSQ\switch-GLAT.pdf).
  
> [!Abstract]-
>
> Multilingual machine translation aims to develop a single model for multiple language directions. However, existing multilingual models based on Transformer are limited in terms of both translation performance and inference speed. In this paper, we propose switch-GLAT, a non-autoregressive multilingual machine translation model with a code-switch decoder. It can generate contextual code-switched translations for a given source sentence, and perform code-switch back-translation, greatly boosting multilingual translation performance. In addition, its inference is highly efficient thanks to its parallel decoder. Experiments show that our proposed switch-GLAT outperform the multilingual Transformer with as much as 0.74 BLEU improvement and 6.2x faster decoding speed in inference.
>.

> [!tldr]- Summary
> A short summary - or an abstract in 3 sentences, relating to YOU. What did YOU find interesting about this paper. 

> [!quote]- Quotable
> Imagine you would quote this paper in your publication. How would you do it? It is probably just one sentence followed by the reference. It is the most intense condensation of the information in this paper and forces you to be on point. 


# Notes  
>  
>#language-identification #code-switch-back-translation

# SummaryTitle: switch-GLAT: Multilingual Parallel Machine Translation via Code-Switch Decoder1

Authors: Zhenqiao Song, Hao Zhou, Lihua Qian, Jingjing Xu, Shanbo Cheng, Mingxuan Wang, Lei Li

Abstract: The paper proposes a non-autoregressive multilingual neural machine translation model that can generate contextual code-switched translations and perform code-switch back-translation12. The model outperforms multilingual Transformer in both speed and translation quality on three datasets.

Introduction: The paper argues that multilingual non-autoregressive translation models can achieve better multilingual translation performance and efficiency, due to their capability of generating high quality code-switched translations3.

The paper introduces switch-GLAT, a multilingual version of GLAT, which employs a code-switch decoder and a code-switch back-translation objective41. The paper shows that switch-GLAT can produce better-aligned cross-lingual representations and improve translation performance on various language pairs.

Multilingual Neural Machine Translation: The authors review the recent advances and challenges in multilingual neural machine translation (NMT), which aims to translate multiple languages using a single model.

Universal Encoder and Decoder: The authors introduce the concept of universal encoder and decoder, which are shared across all languages and can learn cross-lingual representations and transfer knowledge between languages.

Zero-Shot Translation: The authors discuss the problem of zero-shot translation, which is to translate between language pairs that are not seen during training, and present some methods to improve it, such as pivot-based translation, shared subword units, and language-specific adapters.

Code-Switching and Low-Resource Languages: The authors highlight the importance of code-switching and low-resource languages for multilingual NMT, and propose some techniques to handle them, such as code-switch back-translation, data selection, and knowledge distillation.

# Insight

The document is a conference paper about switch-GLAT, a non-autoregressive multilingual machine translation model that can generate code-switched translations and perform code-switch back-translation12.

The main idea of switch-GLAT is to use a code-switch decoder that can produce contextual translated words in arbitrary languages with the help of token-level language tags, and then use the generated code-switched translations to enhance the cross-lingual representations and the multilingual translation performance.

The paper proposes a scheduled code-switch training method that balances the influence of multilingual training and code-switch back-translation, and gradually increases the complexity and diversity of the code-switched data3.

The paper conducts experiments on three merged datasets with different levels of multilingualism, and shows that switch-GLAT outperforms the multilingual Transformer and other baselines in both effectiveness and efficiency4. The paper also analyzes the quality of the learned cross-lingual representations through word induction and sentence retrieval tasks5.

# Problem

The problem of this research is to develop a non-autoregressive multilingual machine translation model that can achieve better translation performance and faster decoding speed than existing multilingual models based on Transformer. The authors argue that non-autoregressive models have the potential to generate high-quality code-switched translations, which can improve the cross-lingual alignment and transferability of the model. They propose switch-GLAT, a model that incorporates a code-switch decoder and a code-switch back-translation strategy1.

# Limitation

Data scarcity: The authors acknowledge that the availability of multilingual corpora is a major bottleneck for multilingual NAT models, especially for low-resource languages. They suggest that future work could explore methods to leverage monolingual data or synthetic data to improve the model performance.

Model capacity: The authors also admit that the model capacity is a crucial factor for multilingual models, as they observe that increasing the model size brings better results for switch-GLAT12. They propose that future work could investigate more efficient architectures or parameter sharing schemes to handle the large number of languages and directions.

# Method

The method of this research is to propose switch-GLAT, a non-autoregressive multilingual neural machine translation model that can generate code-switched translations and perform code-switch back-translation12. The model consists of a code-switch decoder, which can produce contextualized translations in arbitrary languages with the help of token-level language tags, and a code-switch back-translation module, which can enhance the cross-lingual representations and the translation performance34. The model is trained on three merged datasets with different language pairs and evaluated on various tasks, such as translation quality, cross-lingual word induction, and sentence retrieval. The model is shown to outperform multilingual Transformer in both effectiveness and efficiency.

# Model

According to the web page context, the model used by this research is:

switch-GLAT: A non-autoregressive multilingual neural machine translation model that incorporates a code-switch decoder and a code-switch back-translation strategy12.

Code-switch decoder: A parallel decoder that can generate contextual code-switched translations for a given source sentence by using token-level language tags34.

Code-switch back-translation: A data augmentation technique that reverses the pairs of source sentences and code-switched target sentences to improve the cross-lingual representations and translation performance56.

--

Glancing Transformer (GLAT):

GLAT is a variant of the Transformer architecture.

It is specifically designed for non-autoregressive neural machine translation (NAT).

GLAT enables high-quality translation with significantly faster decoding speed.

Notably, GLAT does not modify the network architecture but focuses on training methods to learn word interdependencies.--

A non-autoregressive multilingual neural machine translation model that can generate contextual code-switched translations and perform code-switch back-translation12. It is based on the glancing transformer (GLAT) architecture, which uses a parallel decoder and a glancing sampling strategy.

--

The glancing sampling strategy is a key component in the glancing Transformer (GLAT), a non-autoregressive neural machine translation (NAT) model. Let’s break down what it entails:

Purpose:

The goal of glancing sampling is to enable GLAT to generate sentences in a one-iteration way, avoiding the need for iterative inference during decoding.

It strikes a balance between efficiency and translation quality.

Adaptive Sampling:

GLAT employs an adaptive glancing sampling strategy during training.

Here’s how it works:

During the first decoding pass (similar to vanilla NAT), GLAT predicts words based on the input sequence.

If the current reference (target sentence) is deemed “difficult” for fitting, GLAT performs a second decoding pass.

In the second pass, GLAT samples words from the reference using the glancing sampling strategy.

Only the second decoding pass updates the model parameters.

Gradually, as the model learns, it reduces the percentage of glancing sampling, ensuring it can generate the entire sentence in a single pass.

Representation Usage:

Unlike traditional masked language models (MLMs) that use a [MASK] token, GLAT directly uses representations from the encoder at corresponding positions.

This approach enhances interactions between the sampled words and signals from the encoder.

Benefits:

GLAT achieves significant improvements (around 5 BLEU points) compared to vanilla NAT on standard benchmarks without sacrificing inference speed-up.

It even outperforms iterative approaches like Mask-Predict on certain language pairs.

The gradual learning process ensures smoother single-pass parallel generation1.

In summary, the glancing sampling strategy allows GLAT to strike a balance between translation quality and decoding efficiency by adaptively sampling from the reference during training1..  
  
  
# Annotations%% begin annotations %%  
  
  
  
### Imported: 2024-02-26 4:44 am
  
  
<mark style="background-color: #ff6666">Quote</mark>  
> Transformer  
  
<mark style="background-color: #ff6666">Quote</mark>  
> limited in terms of both translation performance and inference speed  
  
<mark style="background-color: #ff6666">Quote</mark>  
> code-switch decoder  
  
<mark style="background-color: #ff6666">Quote</mark>  
> by employing the token-level language tag  
  
<mark style="background-color: #ff6666">Quote</mark>  
> gains multilingual translation ability through multilingual training  
  
<mark style="background-color: #ff6666">Quote</mark>  
> can generate code-switched translations in arbitrary languages with the help of token-level language tag  
  
<mark style="background-color: #ff6666">Quote</mark>  
> the indicative language tag, we add it to the first layer input and final layer outpu  
  
<mark style="background-color: #ff6666">Quote</mark>  
> due to its token-level characteristics.  
  
<mark style="background-color: #ff6666">Quote</mark>  
> relatively close on linguistics.  
  
<mark style="background-color: #ff6666">Quote</mark>  
> are distant languages on linguistics and their relationships are more difficult to learn  
  
<mark style="background-color: #ff6666">Quote</mark>  
> adding token-level language tags to the vanilla NAT  
  
  
%% end annotations %%

%% Import Date: 2024-02-26T04:45:10.551+08:00 %%

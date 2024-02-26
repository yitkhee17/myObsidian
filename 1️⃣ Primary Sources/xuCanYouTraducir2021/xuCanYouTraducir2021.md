---
doi: 10.48550/arXiv.2105.04846
category: literaturenote  
tags: Computer Science - Computation and Language  
citekey: xuCanYouTraducir2021  
status: unread
Rating: 0/5
Title: Can You Traducir This? Machine Translation for Code-Switched Input
ShortSummary: Code-Switching (CSW) is a common phenomenon that occurs in multilingual geographic or social contexts, which raises challenging problems for natural language processing tools. We focus here on Machine Translation (MT) of CSW texts, where we aim to simultaneously disentangle and translate the two mixed languages. Due to the lack of actual translated CSW data, we generate artificial training data from regular parallel texts. Experiments show this training strategy yields MT systems that surpass multilingual systems for code-switched texts. These results are confirmed in an alternative task aimed at providing contextual translations for a L2 writing assistant.
dateread: {DATE}
---

> [!Cite]
> Xu, J., & Yvon, F. (2021). _Can You Traducir This? Machine Translation for Code-Switched Input_ (arXiv:2105.04846). arXiv. [https://doi.org/10.48550/arXiv.2105.04846](https://doi.org/10.48550/arXiv.2105.04846)
  
>[!Synth]  
>**Contribution**::  
>  
>**Related**:: 
>  
  
>[!md]-
>**FirstAuthor**:: Xu, Jitao  
>**Author**:: Yvon, François  
~  
>**Title**:: Can You Traducir This? Machine Translation for Code-Switched Input
>**Year**:: 2021
>**Citekey**:: xuCanYouTraducir2021
>**itemType**:: preprint
>**DOI**:: 10.48550/arXiv.2105.04846
  
> [!LINK]-
> 
> [arXiv Fulltext PDF](file://C:\Users\Wong\Zotero\storage\CUMU3N83\Xu%20and%20Yvon%20-%202021%20-%20Can%20You%20Traducir%20This%20Machine%20Translation%20for%20Cod.pdf).
  
> [!Abstract]-
>
> Code-Switching (CSW) is a common phenomenon that occurs in multilingual geographic or social contexts, which raises challenging problems for natural language processing tools. We focus here on Machine Translation (MT) of CSW texts, where we aim to simultaneously disentangle and translate the two mixed languages. Due to the lack of actual translated CSW data, we generate artificial training data from regular parallel texts. Experiments show this training strategy yields MT systems that surpass multilingual systems for code-switched texts. These results are confirmed in an alternative task aimed at providing contextual translations for a L2 writing assistant.
>.

> [!tldr]- Summary
> A short summary - or an abstract in 3 sentences, relating to YOU. What did YOU find interesting about this paper. 

> [!quote]- Quotable
> Imagine you would quote this paper in your publication. How would you do it? It is probably just one sentence followed by the reference. It is the most intense condensation of the information in this paper and forces you to be on point. 


# Notes  
>  
>#data-augmentation #translation

# Summary

Topic: The paper discusses the problem of machine translation for code-switched texts, where two languages are mixed in the input1.

Motivation: Code-switching is a common phenomenon in multilingual communities, especially in social media and user-generated content, but it poses challenges for natural language processing tools2.

Approach: The authors propose to use artificial code-switched data generated from regular parallel texts to train neural machine translation models that can translate code-switched texts into monolingual texts.

Results: The authors show that their models outperform bilingual and multilingual baselines on code-switched texts, and also achieve competitive results on a task of translating L1 fragments in an L2 context.

# Insight

The document is about machine translation for code-switched input, which is a phenomenon where speakers or writers mix two languages within a single utterance or text1.

The authors propose a method to generate artificial code-switched data from regular parallel texts, and use it to train neural machine translation systems that can handle both monolingual and code-switched inputs2.

The authors evaluate their models on two language pairs: English-Spanish and English-French, and show that their models outperform baseline systems that have not seen code-switched data on both monolingual and code-switched test sets.

The authors also apply their models to the SemEval 2014 Task 5: L2 Writing Assistant, which requires translating L1 fragments in an L2 context, and achieve state-of-the-art results for English-Spanish and competitive results for French-English3.

# Problem Statement

The research focuses on the problem of code-switching input for machine translation. Code-switching occurs when language users combine two or more languages within a single discourse or utterance. While multilingual humans can seamlessly switch between languages, multilingual neural machine translation (NMT) models struggle with sudden changes in input. The challenge lies in effectively translating code-switched texts, which are prevalent in multilingual communities, especially in social media and user-generated content. The study explores how code-switched data affects machine translation systems and suggests that viewing multilingualism as an opportunity rather than an obstacle is crucial for natural language processing12.

# Limitation

Monolingual Bias: Most existing machine translation systems are designed to work with monolingual data, which limits their ability to handle code-mixed text effectively. These systems may not adequately support code-switched language, which is prevalent in daily communications and social media platforms12.

Lack of Robustness: Multilingual neural machine translation models are not robust to sudden changes in input caused by code-switching. While humans can seamlessly switch between languages, NMT models struggle with this phenomenon34.

Limited Training Data: Code-switched data is relatively scarce compared to monolingual data. Training robust models requires a substantial amount of code-switched examples, which can be challenging to obtain1.

Semantic Challenges: Code-switching introduces semantic complexities, such as context-dependent word meanings and cultural nuances. Handling these challenges effectively remains an open problem1.

Evaluation Metrics: Existing evaluation metrics may not fully capture the quality of code-switched translations. Developing specialized evaluation methods for code-switching remains an area of research1.

In summary, while code-switching presents interesting opportunities for NLP, addressing its limitations requires further investigation and innovative approaches.

# Method

The model addresses code-switching by employing a novel approach that disentangles and translates the two mixed languages simultaneously. Here are the key steps in handling code-switching:

Artificial Code-Switched Data Generation: Due to the scarcity of actual translated code-switched data, the authors create artificial code-switched training examples from regular parallel texts. These artificial examples simulate the mixing of languages found in real-world code-switched texts.

Neural Machine Translation (NMT) Training: The model is trained using these artificial code-switched examples alongside monolingual data. The NMT system learns to handle both monolingual and code-switched inputs during training1.

Evaluation on Code-Switched Texts: The authors evaluate the trained model on code-switched test sets. The results demonstrate that their approach outperforms bilingual and multilingual baselines, highlighting the effectiveness of their method in handling mixed-language texts.

Application to L2 Writing Assistance: The model is also applied to the SemEval 2014 Task 5, where it translates L1 fragments in an L2 context2. The achieved state-of-the-art results for English-Spanish and competitive results for French-English further validate the model’s capabilities.

In summary, the model’s innovative training strategy enables it to effectively handle code-switching, benefiting both machine translation and language assistance tasks.

# Model

Transformer base: A popular and powerful model that relies on attention mechanisms to encode and decode sequences of words.

Fairseq: An open-source toolkit for sequence modeling that implements the Transformer base architecture and other variants.

Byte Pair Encoding (BPE): A subword segmentation method that reduces the vocabulary size and handles rare words by splitting them into smaller units.

this research applies the fairseq model with some modifications to the training scheme and the hyperparameters. The authors use the fairseq implementation of Transformer base (Vaswani et al., 2017) with a hidden size of 512 and a feedforward size of 20481. They optimize with Adam, set up with an initial learning rate of 0.0007 and an inverse square root weight decay schedule, as well as 4000 warmup steps2. They also use mixed precision and a batch size of 8192 tokens for 300k iterations on 4 V100 GPUs3. They do not share the embedding matrices and use a shared source-target inventory built with Byte Pair Encoding (BPE) of 32K merge operations4.

**CS**

1. [Go to annotation](zotero://open-pdf/library/items/CUMU3N83?page=1&annotation=undefined) “The Matrix Language Frame (MLF) theory (Myers-Scotton, 1997) defines the concept of matrix and embedded languages where the matrix language is the main language that the sentence structure should conform to and notably provides the syntactic morphemes, while the influence of the embedded language is lesser and is mostly manifested in the insertion of content morphemes.” ([Xu and Yvon, 2021, p. 1](zotero://select/library/items/BDTN2QGZ))
2. [Go to annotation](zotero://open-pdf/library/items/CUMU3N83?page=1&annotation=undefined) “Code-switching however remains understudied in natural language processing (NLP) (Aguilar and Solorio, 2020), and most work to date has focused on token-level language identification (LID) (Samih et al., 2016) and on language models for Automatic Speech Recognition (Winata et al., 2019). More tasks are being considered lately, such as Named Entity Recognition (Aguilar et al., 2018), Part-of-Speech tagging (Ball and Garrette, 2018) or Sentiment Analysis (Patwa et al., 2020).” ([Xu and Yvon, 2021, p. 1](zotero://select/library/items/BDTN2QGZ))
3. 9i

[Go to annotation](zotero://open-pdf/library/items/CUMU3N83?page=7&annotation=undefined) “Research in the area of NLP for CSW has mostly focused on CSW Language Modeling, especially for Automatic Speech Recognition (Pratapa et al., 2018; Garg et al., 2018; Gonen and Goldberg, 2019;Winata et al., 2019; Lee and Li, 2020). Evaluation tasks, benchmarks have also been prepared for LID in user generated CSW content (Zubiaga et al., 2016; Molina et al., 2016), Named Entity Recognition (Aguilar et al., 2018), Part-of-Speech tagging (Ball and Garrette, 2018; Aguilar et al., 2020; Khanuja et al., 2020) and Sentiment Analysis (Patwa et al., 2020). CSW was also found useful in foreign language teaching: Renduchintala et al. (2019a,b) showed that replacing words by their counterparts in foreign language helps to learn foreign language vocabulary.” ([Xu and Yvon, 2021, p. 7](zotero://select/library/items/BDTN2QGZ))

[Go to annotation](zotero://open-pdf/library/items/CUMU3N83?page=7&annotation=undefined) “Huang and Yates (2014) used CSW corpus to improve word alignment and statistical MT. Dinu et al. (2019) experienced replacing and concatenating source terminology constraints by the corresponding translation(s) to boost the accuracy of term translations. Song et al. (2019a)” ([Xu and Yvon, 2021, p. 7](zotero://select/library/items/BDTN2QGZ)).  
  
  
# Annotations%% begin annotations %%  
  
  
%% end annotations %%

%% Import Date: 2024-02-26T03:09:09.293+08:00 %%

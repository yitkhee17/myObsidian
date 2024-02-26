---
doi: 10.1080/14790718.2023.2224013
category: literaturenote  
tags: Machine translation, done LR, automatic evaluation, code-switching, human evaluation, lexico-semantic enrichment, Vietnamese, read again when writing evaluation  
citekey: nguyenCodeswitchingInputMachine2023a  
status: unread
Rating: 0/5
Title: Code-switching input for machine translation: a case study of Vietnamese–English data
ShortSummary: Multilingualism presents both a challenge and an opportunity for Natural Language Processing, with code-switching representing a particularly interesting problem for computational models trained on monolingual datasets. In this paper, we explore how code-switched data affects the task of Machine Translation, a task which only recently has started to tackle the challenge of multilingual data. We test three Machine Translation systems on data from the Canberra Vietnamese–English Codeswitching Natural Speech Corpus (CanVEC) and evaluate translation output using both automatic and human metrics. We find that, perhaps counter-intuitively, Machine Translation performs better on code-switching input than monolingual input. In particular, comparison of human and automatic evaluation suggests that codeswitching input may boost the semantic faithfulness of the translation output, an effect we term lexico-semantic enrichment. We also report two cases where this effect is most and least clear in Vietnamese–English, namely gender-neutral 3SG pronouns and interrogative constructions respectively. Overall, we suggest that Machine Translation, and Natural Language Processing more generally, ought to view multilingualism as an opportunity rather than an obstacle.Abbreviations: 1: First person; 2: Second person; 3: Third person; CLF: Classifier; COP: Copula; DET: Determiner; PL: Plural; POSS: Possessive marker; PRT: Particle; PST: Past tense; Q: Question marker; SG: Singular
dateread: {DATE}
---

> [!Cite]
> Nguyen, L., Mayeux, O., & Yuan, Z. (2023). Code-switching input for machine translation: A case study of Vietnamese–English data. _International Journal of Multilingualism_, _0_(0), 1–22. [https://doi.org/10.1080/14790718.2023.2224013](https://doi.org/10.1080/14790718.2023.2224013)
  
>[!Synth]  
>**Contribution**::  
>  
>**Related**:: 
>  
  
>[!md]-
>**FirstAuthor**:: Nguyen, Li  
>**Author**:: Mayeux, Oliver  
>**Author**:: Yuan, Zheng  
~  
>**Title**:: Code-switching input for machine translation: a case study of Vietnamese–English data
>**Year**:: 2023
>**Citekey**:: nguyenCodeswitchingInputMachine2023a
>**itemType**:: journalArticle
>**Journal**::*International Journal of Multilingualism*
>**Volume**:: 0
>**Issue**:: 0
>**Pages**:: 1-22
>**DOI**:: 10.1080/14790718.2023.2224013
  
> [!LINK]-
> 
> [Full Text PDF](file://C:\Users\Wong\Zotero\storage\GSKXZDNI\Nguyen%20et%20al.%20-%202023%20-%20Code-switching%20input%20for%20machine%20translation%20a%20ca.pdf).
  
> [!Abstract]-
>
> Multilingualism presents both a challenge and an opportunity for Natural Language Processing, with code-switching representing a particularly interesting problem for computational models trained on monolingual datasets. In this paper, we explore how code-switched data affects the task of Machine Translation, a task which only recently has started to tackle the challenge of multilingual data. We test three Machine Translation systems on data from the Canberra Vietnamese–English Codeswitching Natural Speech Corpus (CanVEC) and evaluate translation output using both automatic and human metrics. We find that, perhaps counter-intuitively, Machine Translation performs better on code-switching input than monolingual input. In particular, comparison of human and automatic evaluation suggests that codeswitching input may boost the semantic faithfulness of the translation output, an effect we term lexico-semantic enrichment. We also report two cases where this effect is most and least clear in Vietnamese–English, namely gender-neutral 3SG pronouns and interrogative constructions respectively. Overall, we suggest that Machine Translation, and Natural Language Processing more generally, ought to view multilingualism as an opportunity rather than an obstacle.Abbreviations: 1: First person; 2: Second person; 3: Third person; CLF: Classifier; COP: Copula; DET: Determiner; PL: Plural; POSS: Possessive marker; PRT: Particle; PST: Past tense; Q: Question marker; SG: Singular
>.

> [!tldr]- Summary
> A short summary - or an abstract in 3 sentences, relating to YOU. What did YOU find interesting about this paper. 

> [!quote]- Quotable
> Imagine you would quote this paper in your publication. How would you do it? It is probably just one sentence followed by the reference. It is the most intense condensation of the information in this paper and forces you to be on point. 


# Notes  
>  
>#evaluate-code-switch-input

# Summary

Introduction: The paper explores how code-switched data affects machine translation, using Vietnamese–English as a case study1. It evaluates three multilingual NMT systems on natural speech data and compares human and automatic metrics.

Machine translation for code-switching: The paper reviews the state-of-the-art approaches and challenges for translating code-switched text, and highlights the need for more work on low-resource languages and qualitative analysis2.

Data: The paper introduces CanVEC, a corpus of natural Vietnamese–English code-switched speech, and describes how it collected reference translations for 100 clauses from the corpus.

Methodology: The paper explains how it used three multilingual NMT models (Google Translate, mBART-50, and M2M) to translate both monolingual Vietnamese and code-switched Vietnamese/English into English3. It also describes the automatic and human evaluation methods and metrics used to assess the translation quality.

# Insight

The document is a research paper on code-switching input for machine translation, focusing on a case study of Vietnamese–English data1.

The paper explores how code-switched data affects the task of machine translation, a task which only recently has started to tackle the challenge of multilingual data2.

The paper tests three machine translation systems on data from the Canberra Vietnamese–English Codeswitching Natural Speech Corpus (CanVEC) and evaluates translation output using both automatic and human metrics.

The paper finds that, perhaps counter-intuitively, machine translation performs better on code-switching input than monolingual input3. In particular, comparison of human and automatic evaluation suggests that code-switching input may boost the semantic faithfulness of the translation output, an effect termed lexico-semantic enrichment45.

The paper also reports two cases where this effect is most and least clear in Vietnamese–English, namely gender-neutral 3SG pronouns and interrogative constructions respectively.

The paper suggests that machine translation, and natural language processing more generally, ought to view multilingualism as an opportunity rather than an obstacle6

# Problem

The problem of this research is to explore how code-switched data affects the task of machine translation, a task which only recently has started to tackle the challenge of multilingual data1. The authors focus on the evaluation of machine translation for natural Vietnamese–English code-switched data, a low-resource language combination that has received little research attention2. The authors aim to determine how well current machine translation technologies handle natural code-switched data, and to identify specific linguistic phenomena that machine translation systems consistently handle well or badly3.

# Limitation

The focus on Vietnamese–English code-switching, which may not be generalisable to other language pairs or language types.

The small size of the test set (100 clauses), which may not capture the full diversity and complexity of code-switching phenomena.

The lack of qualitative analysis on the syntactic and pragmatic aspects of code-switching, which may affect the translation quality and naturalness.

# Method

this research is to evaluate three machine translation systems on code-switched Vietnamese-English data, using both automatic and human metrics. The authors use the following steps:

They randomly select 100 code-switched clauses from the CanVEC corpus, a natural speech corpus of Vietnamese immigrants in Australia1.

They obtain reference translations for these clauses into monolingual English and Vietnamese from two bilingual annotators2.

They use Google Translate, mBART-50, and M2M as the machine translation systems, and translate the code-switched clauses into English using each system.

They compare the machine translations with the reference translations using automatic metrics such as BLEU, chrF, and TER.

They also conduct human evaluation by rating the machine translations in terms of grammaticality, fluency, and semantic faithfulness3.

# Model

Google Translate: a popular online service that supports 133 languages and uses multilingual neural machine translation (NMT)2.

mBART-50: a multilingual NMT model that provides support for 50 languages, trained with multilingual finetuning of pretrained multilingual Bidirectional and Auto-Regressive Transformers (mBART)34.

M2M: a multilingual NMT model that can translate directly between any pair of 100 languages, trained with parallel sentences mined from CommonCrawl5.

# State of art

, the state-of-the-art approaches for machine translation for code-switched data are:

Multilingual neural machine translation (NMT) models that can translate from multiple source languages into target languages, such as Google Translate, mBART-50, and M2M (Firat et al., 2017; Johnson et al., 2017; Fan et al., 2021)1.

Augmentation techniques that enhance existing NMT systems with code-switched data, such as synthetic code-mixed parallel corpus, data debiasing, and domain adaptation (Appicharla et al., 2021; Dhar et al., 2018; Gupta et al., 2021).

Evaluation methods that measure the quality of code-switched translation output, such as automatic metrics (BLEU, chrF2, TER) and human evaluation (Fluency, Grammaticality, Semantic faithfulness) (Chen et al., 2022; Liu et al., 2020).

# Challenges in csw

Lack of parallel corpora: Code-switched data is scarce and often not aligned with monolingual data, making it difficult to train and evaluate MT systems.

Language identification: Code-switched text may contain switches at various levels (word, phrase, sentence), and MT systems need to accurately identify the language of each segment before translating it.

Syntactic and semantic integration: Code-switched text may combine language-specific grammatical features and idiomatic expressions, and MT systems need to handle the syntactic and semantic compatibility of the mixed languages.

Evaluation metrics: Code-switched text may have multiple valid translations, and existing automatic evaluation metrics may not capture the meaning and grammaticality of the output.

---

-Previous Work

1. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=2&annotation=undefined) “handling code-switched input as in (1) & (2) (Himabindu et al., 2022; Johnson et al., 2017; Nguyen & Bryant, 2020; Solorio et al., 2021; Vissamsetti et al., 2022).” ([Nguyen et al., 2023, p. 2](zotero://select/library/items/B37PWHVK))
2. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=2&annotation=undefined) “Automatic machine translation (MT), in particular, has seen a rise in interest in this area (Chen et al., 2022).” ([Nguyen et al., 2023, p. 2](zotero://select/library/items/B37PWHVK))
3. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=2&annotation=undefined) “Spanish/English (Weller et al., 2022; Xu & Yvon, 2021) and Hindi/English (Appicharla et al., 2021; Jadhav et al., 2022)” ([Nguyen et al., 2023, p. 2](zotero://select/library/items/B37PWHVK))

---

State of Art

[Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=2&annotation=undefined) “three state of-the-art MT models – Google Translate (Johnson et al., 2017), mBart-50 (Tang et al., 2020) and M2M (Fan et al., 2021)” ([Nguyen et al., 2023, p. 2](zotero://select/library/items/B37PWHVK))

-> [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=2&annotation=undefined) “The results show that models are better at preserving the semantic faithfulness of CSW input compared to monolingual input.” ([Nguyen et al., 2023, p. 2](zotero://select/library/items/B37PWHVK))

---

History of MT in CS

1. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=3&annotation=undefined) “Sequence-to-sequence neural machine translation (NMT) employs the encoder–decoder framework (Bahdanau et al., 2015; Cho et al., 2014; Kalchbrenner & Blunsom, 2013; Sutskever et al., 2014)” ([Nguyen et al., 2023, p. 3](zotero://select/library/items/B37PWHVK))
    
    1. Architecture types to build encoder or decoder: [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=3&annotation=undefined) “Recurrent Neural Networks (RNN) (Bahdanau et al., 2015), Convolutional Neural Networks (CNN) (Gehring et al., 2017), and Transformers (Vaswani et al., 2017).” ([Nguyen et al., 2023, p. 3](zotero://select/library/items/B37PWHVK))
    2. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=3&annotation=undefined) “Transformers are the most widely used for multilingual NMT, and state-of-the-art results have been reported (Fan et al., 2021; Tang et al., 2020).” ([Nguyen et al., 2023, p. 3](zotero://select/library/items/B37PWHVK))
2. Multilingual models
    
    1. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=3&annotation=undefined) “translate from multiple source languages into target languages (Firat et al., 2017; Johnson et al., 2017; Xu & Yvon, 2021).” ([Nguyen et al., 2023, p. 3](zotero://select/library/items/B37PWHVK))
    2. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=3&annotation=undefined) “has the advantage of efficiently sharing the parameters of the models (Firat et al., 2017; Johnson et al., 2017)” ([Nguyen et al., 2023, p. 3](zotero://select/library/items/B37PWHVK))
    3. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=3&annotation=undefined) “considerably improving the performance of MT systems for low-resourced languages.” ([Nguyen et al., 2023, p. 3](zotero://select/library/items/B37PWHVK)) “possibility of translating between language pairs that were not seen during training, commonly known as zero-shot translation (Firat et al., 2017; Johnson et al., 2017).” ([Nguyen et al., 2023, p. 3](zotero://select/library/items/B37PWHVK))
    4. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=3&annotation=undefined) “models are still designed to expect monolingual input and output on both ends of the translation” ([Nguyen et al., 2023, p. 3](zotero://select/library/items/B37PWHVK))

---

Code-switched translation system

**Gap**

1. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=3&annotation=undefined) “No current machine translation system is designed to support code-switched text (Çetinoğlu et al., 2016; Menacer et al., 2019).” ([Nguyen et al., 2023, p. 3](zotero://select/library/items/B37PWHVK))
2. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=3&annotation=undefined) “Although MT for code-switching has gathered more research attention in recent years (see e.g. Chen et al., 2022 for an overview), there is still relatively little work being done in this area” ([Nguyen et al., 2023, p. 3](zotero://select/library/items/B37PWHVK))
3. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=3&annotation=undefined) “Some recent attempts include testing Google Translate on translating CSW into a third language (Johnson et al., 2017), or tweaking/building translation models from English to CSW text and vice versa (Dhar et al., 2018; Gupta et al., 2021; Solorio et al., 2021). Dhar et al. (2018), for example, created a parallel corpus of Hindi/English using previously available CSW sentences (N = 6088) from a dataset created and released by Gupta et al. (2016), and augmented run-of-the-mill MT approaches to achieve improved translations.” ([Nguyen et al., 2023, p. 3](zotero://select/library/items/B37PWHVK))

---

Evaluation Method

1. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=3&annotation=undefined) “It is also worth noting, however, that almost all of the limited number of works available for MT on code-switching mainly rely on automatic evaluation metrics (Dhar et al., 2018; Gupta et al., 2021; Xu & Yvon, 2021).” ([Nguyen et al., 2023, p. 3](zotero://select/library/items/B37PWHVK))
2. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=4&annotation=undefined) “automatic evaluation can offer fast and inexpensive feedback.” ([Nguyen et al., 2023, p. 4](zotero://select/library/items/B37PWHVK))
3. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=4&annotation=undefined) “several metrics have been proposed and used (Papineni et al., 2002; Popović, 2015; Snover et al., 2006), most mainly capture lexical similarities between the system output and the references provided by human experts, without measuring semantics or grammaticality directly.” ([Nguyen et al., 2023, p. 4](zotero://select/library/items/B37PWHVK))
    
    1. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=4&annotation=undefined) “Dhar’s study (2018), for example, only used BLEU, Word Error Rate (WER) and Translation Error Rate (TER) to evaluate the output’s quality. Although these metrics have been shown to correlate well with human judgement for monolingual output (Graham & Baldwin, 2014; Popović, 2015), little is known about whether these conclusions extend to code-switching.” ([Nguyen et al., 2023, p. 4](zotero://select/library/items/B37PWHVK))
4. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=4&annotation=undefined) “The lack of qualitative analysis is particularly problematic in a language-mixing context, where language-specific grammatical features and idiomatic expressions are frequently combined.” ([Nguyen et al., 2023, p. 4](zotero://select/library/items/B37PWHVK))
    
    1. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=4&annotation=undefined) “Johnson et al. (2017), who briefly reported a lack of naturalness in the system output when using Google’s multilingual zero-shot translation model for the task of translating Japanese and Korean into English.” ([Nguyen et al., 2023, p. 4](zotero://select/library/items/B37PWHVK))

---

Result

1. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=10&annotation=undefined) “Google Translate outperforms mBART-50 and M2M on all three metrics, suggesting that Google Translate is the best MT system amongst these three when eval” ([Nguyen et al., 2023, p. 10](zotero://select/library/items/B37PWHVK))
2. [Go to annotation](zotero://open-pdf/library/items/GSKXZDNI?page=12&annotation=undefined) “according to both automatic and human evaluation metrics, CSW data does improve some results of MT. This finding is both unsurprising and surprising; unsurprising because although CSW input is considered partly translated input and hence giving the models an easier task, but surprising because these models have not been trained on CSW data before. In what follows, we further probe the specific linguistic aspects to which enhancement from CSW input apply” ([Nguyen et al., 2023, p. 12](zotero://select/library/items/B37PWHVK)).  
  
  
# Annotations%% begin annotations %%  
  
  
  
### Imported: 2024-02-26 5:19 am
  
  
<mark style="background-color: #ffd400">Quote</mark>  
> An encoder first reads and encodes an entire input sequence into hidden state representations, and a decoder then generates an output sequence by predicting the next word based on the input sequence and all the previously generated words.  
  
  
%% end annotations %%

%% Import Date: 2024-02-26T05:20:14.370+08:00 %%

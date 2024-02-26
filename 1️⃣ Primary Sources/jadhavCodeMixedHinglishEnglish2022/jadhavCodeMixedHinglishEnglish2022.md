---
doi: 10.1109/ICSCDS53736.2022.9760834
category: literaturenote  
tags:   
citekey: jadhavCodeMixedHinglishEnglish2022  
status: unread
Rating: 0/5
Title: Code-Mixed Hinglish to English Language Translation Framework
ShortSummary: Indians, like many other non-English speakers around the world, avoid using single code in their social media conversations. They use transliteration and blend multiple languages to exhibit their linguistic proficiency by randomly merging English words (English-Hindi, English-Spanish, etc.). As a result, a large amount of unstructured text is generated because of the wide use of social media applications. Code-mixing (CM) is a fast-evolving field of study in the domain of text mining. The present situation of various social media posts, blogs, and reviews have a large use of code-mixed messages, due to its modern yet localized way of speaking. Linguistic codes from various languages are used for different purposes. Code-mixed Hindi and English is a typical practice observed in India's day-to-day language usage. Most people have already started to consider this mixing as a new language which has given birth to a brand new language termed “Hinglish”. Hinglish is majorly used among the younger generation, as observed in the code-mixed data obtained via social sites and various other platforms. This mixing of languages stands as a new challenge to the concept of machine translation. It is important to recognize the foreign elements in a language and process them appropriately. As a result, a translation mechanism is needed to assist monolingual users, as well as for easier comprehension by language processing models. This paper proposes a pipelined mechanism for machine translation of a bi-lingual language i.e. Hinglish to monolingual English in this paper.
dateread: {DATE}
---

> [!Cite]
> Jadhav, I., Kanade, A., Waghmare, V., Chandok, S. S., & Jarali, A. (2022). Code-Mixed Hinglish to English Language Translation Framework. _2022 International Conference on Sustainable Computing and Data Communication Systems (ICSCDS)_, 684–688. [https://doi.org/10.1109/ICSCDS53736.2022.9760834](https://doi.org/10.1109/ICSCDS53736.2022.9760834)
  
>[!Synth]  
>**Contribution**::  
>  
>**Related**:: 
>  
  
>[!md]-
>**FirstAuthor**:: Jadhav, Ishali  
>**Author**:: Kanade, Aditi  
>**Author**:: Waghmare, Vishesh  
>**Author**:: Chandok, Sahej Singh  
>**Author**:: Jarali, Ashwini  
~  
>**Title**:: Code-Mixed Hinglish to English Language Translation Framework
>**Year**:: 2022
>**Citekey**:: jadhavCodeMixedHinglishEnglish2022
>**itemType**:: conferencePaper
>**Pages**:: 684-688
>**DOI**:: 10.1109/ICSCDS53736.2022.9760834
  
> [!LINK]-
> 
> [IEEE Xplore Full Text PDF](file://C:\Users\Wong\Zotero\storage\FT6495UN\Jadhav%20et%20al.%20-%202022%20-%20Code-Mixed%20Hinglish%20to%20English%20Language%20Translatio.pdf).
  
> [!Abstract]-
>
> Indians, like many other non-English speakers around the world, avoid using single code in their social media conversations. They use transliteration and blend multiple languages to exhibit their linguistic proficiency by randomly merging English words (English-Hindi, English-Spanish, etc.). As a result, a large amount of unstructured text is generated because of the wide use of social media applications. Code-mixing (CM) is a fast-evolving field of study in the domain of text mining. The present situation of various social media posts, blogs, and reviews have a large use of code-mixed messages, due to its modern yet localized way of speaking. Linguistic codes from various languages are used for different purposes. Code-mixed Hindi and English is a typical practice observed in India's day-to-day language usage. Most people have already started to consider this mixing as a new language which has given birth to a brand new language termed “Hinglish”. Hinglish is majorly used among the younger generation, as observed in the code-mixed data obtained via social sites and various other platforms. This mixing of languages stands as a new challenge to the concept of machine translation. It is important to recognize the foreign elements in a language and process them appropriately. As a result, a translation mechanism is needed to assist monolingual users, as well as for easier comprehension by language processing models. This paper proposes a pipelined mechanism for machine translation of a bi-lingual language i.e. Hinglish to monolingual English in this paper.
>.

> [!tldr]- Summary
> A short summary - or an abstract in 3 sentences, relating to YOU. What did YOU find interesting about this paper. 

> [!quote]- Quotable
> Imagine you would quote this paper in your publication. How would you do it? It is probably just one sentence followed by the reference. It is the most intense condensation of the information in this paper and forces you to be on point. 


# Notes  
>  
>#translation

# Summary

# Insight

1. It proposes a pipelined mechanism for machine translation of a bi-lingual language, i.e. Hinglish, to monolingual English2.

The paper addresses the challenge of translating code-mixed data, which is a common phenomenon in social media platforms, especially among bilingual speakers of Hindi and English. Code-mixed data poses difficulties for existing machine translation systems, as it requires a large amount of parallel corpus and a robust language identification module.

The paper introduces an additional layer of language identification and segmentation, which tags each word in the code-mixed sentence as either Hindi or English, and splits the sentence into sub-sequences of the same language3. These sub-sequences are then back-transliterated or translated using pre-existing transliteration and translation models, respectively4.

The paper evaluates the proposed framework by comparing it with Google Neural Machine Translation (GNMT), a state-of-the-art system for machine translation. The paper reports that the proposed framework outperforms GNMT by a significant margin in terms of BLEU score, TER score, and WER score, which are standard metrics for machine translation quality. The paper also discusses the limitations and future work of the proposed framework.

# Problem

The problem of this research is to develop a framework for machine translation of code-mixed Hinglish (Hindi-English) language to monolingual English1. Code-mixed Hinglish is a common practice among bilingual speakers in India, especially on social media platforms, but it poses many challenges for existing machine translation systems, such as language identification, transliteration, and translation2. The authors propose a pipelined mechanism that consists of four stages: language tagging, back-transliteration, translation, and post-processing. The goal is to help monolingual users understand and analyze the code-mixed Hinglish text, as well as to improve the performance of natural language processing models on code-mixed data.

# Limitation

Ambiguity errors: The system may misidentify or mistranslate some words that have different meanings in Hindi and English, such as “uss”, “are”, and “to”.

Gender agreement: The system may not handle the verb changes according to the gender of the noun in Hindi, such as “dekhi” and “dekha”.

Language variety: The system only targets the translation of Hindi-English code-mixed data, and may not be extended to other languages or dialects.

# Method

the model used by this research is a pipelined mechanism for machine translation of a bi-lingual language, i.e. Hinglish (Hindi-English code-mixed language) to monolingual English1. The pipeline consists of four stages:

Language identification and segmentation: This stage assigns a language label (Hindi or English) to each word in the code-mixed sentence and divides it into sub-sequences of the same language23.

Language transliteration: This stage converts the romanized Hindi segments to the Devanagari script using pre-existing transliteration systems.

Language translation: This stage translates the English segments to Hindi using a neural machine translation system, and then translates the joined Hindi segments to English using the same system4.

Evaluation metrics: This stage evaluates the performance of the proposed system using BLEU, TER, and WER scores and compares it with the existing Google NMT system.

# Model

The model types used for each stage in the proposed framework are as follows:

Language identification and segmentation:1

The model used for this stage is not explicitly mentioned in the document. However, it involves tagging each word in the code-mixed sentence as either Hindi or English and splitting the sentence into sub-sequences of the same language2.

Language transliteration:

The document does not specify the exact transliteration model used. It refers to “pre-existing transliteration systems” for converting romanized Hindi segments to the Devanagari script3. These systems could be rule-based or statistical models.

Language translation:

For translating English segments to Hindi, the document employs a neural machine translation (NMT) system4. The details of the specific NMT architecture or model are not provided.

Evaluation metrics:

The evaluation metrics used are BLEU (Bilingual Evaluation Understudy), TER (Translation Edit Rate), and WER (Word Error Rate). These metrics assess the quality of translation and compare the proposed framework with the existing Google Neural Machine Translation system..  
  
  
# Annotations%% begin annotations %%  
  
  
%% end annotations %%

%% Import Date: 2024-02-26T03:31:00.747+08:00 %%

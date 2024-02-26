---
doi: 
category: literaturenote  
tags:   
citekey: sternerTongueSwitcherFineGrainedIdentification2023a  
status: unread
Rating: 0/5
Title: TongueSwitcher: Fine-Grained Identification of German-English Code-Switching
ShortSummary: This paper contributes to German-English code-switching research. We provide the largest corpus of naturally occurring German-English code-switching, where English is included in German text, and two methods for code-switching identification. The first method is rule-based, using wordlists and morphological processing. We use this method to compile a corpus of 25.6M tweets employing German-English code-switching. In our second method, we continue pretraining of a neural language model on this corpus and classify tokens based on embeddings from this language model. Our systems establish SoTA on our new corpus and an existing German-English code-switching benchmark. In particular, we systematically study code-switching for language-ambiguous words which can only be resolved in context, and morphologically mixed words consisting of both English and German morphemes. We distribute both corpora and systems to the research community.
dateread: {DATE}
---

> [!Cite]
> Sterner, I., & Teufel, S. (2023, October 11). _TongueSwitcher: Fine-Grained Identification of German-English Code-Switching_. Sixth Workshop on Computational Approaches to Linguistic Code-Switching. [https://openreview.net/forum?id=heYrTpKRny](https://openreview.net/forum?id=heYrTpKRny)
  
>[!Synth]  
>**Contribution**::  
>  
>**Related**:: 
>  
  
>[!md]-
>**FirstAuthor**:: Sterner, Igor  
>**Author**:: Teufel, Simone  
~  
>**Title**:: TongueSwitcher: Fine-Grained Identification of German-English Code-Switching
>**Year**:: 2023
>**Citekey**:: sternerTongueSwitcherFineGrainedIdentification2023a
>**itemType**:: conferencePaper
  
> [!LINK]-
> 
> [Sterner_Teufel_2023_TongueSwitcher.pdf](file://C:\Users\Wong\Zotero\storage\286GBF87\Sterner_Teufel_2023_TongueSwitcher.pdf).
  
> [!Abstract]-
>
> This paper contributes to German-English code-switching research. We provide the largest corpus of naturally occurring German-English code-switching, where English is included in German text, and two methods for code-switching identification. The first method is rule-based, using wordlists and morphological processing. We use this method to compile a corpus of 25.6M tweets employing German-English code-switching. In our second method, we continue pretraining of a neural language model on this corpus and classify tokens based on embeddings from this language model. Our systems establish SoTA on our new corpus and an existing German-English code-switching benchmark. In particular, we systematically study code-switching for language-ambiguous words which can only be resolved in context, and morphologically mixed words consisting of both English and German morphemes. We distribute both corpora and systems to the research community.
>.

> [!tldr]- Summary
> A short summary - or an abstract in 3 sentences, relating to YOU. What did YOU find interesting about this paper. 

> [!quote]- Quotable
> Imagine you would quote this paper in your publication. How would you do it? It is probably just one sentence followed by the reference. It is the most intense condensation of the information in this paper and forces you to be on point. 


# Notes  
>  
>#code-switching identification

# Summary

produce naturally occurring german-english cs data. analyse [[language ambiguous words that can only be disambiguated by context analysis]]. [[Morphologically mixed words]] consisting of both english and German morphemes.

- **Research question**: How does recent experience in a bilingual's second language (L2) affect their processing of words that exist in both languages in their first language (L1)?¹[1]

- **Background**: Previous studies have shown that processing of cognates (words with the same meaning and form in both languages) and interlingual homographs (words with the same form but different meanings in both languages) in L2 can be influenced by recent experience in L1, but the reverse direction of priming has not been explored²[2].

- **Method**: Dutch-English bilinguals first read sentences in English (L2) containing cognates, interlingual homographs or translation equivalents, and then made semantic relatedness judgements to these words in Dutch (L1)³[3]⁴[4].

- **Hypothesis**: The authors predicted that priming from L2 to L1 would be observed for both cognates and interlingual homographs, and that the priming effect would be greater than the previously observed priming effect from L1 to L2⁵[5].

1. Page 1 - Line 72. Page 1 - Line 103. Page 2 - Line 174. Page 1 - Line 135. Page 5 - Line 4

---

# Result

- **Cross-lingual priming from L2 to L1**. The authors found significant cross-lingual priming effects for interlingual homographs, but not for cognates, when the words were primed in English (L2) and tested in Dutch (L1)¹[1]. This suggests that recent experience in L2 can influence lexical processing in L1, especially for words with different meanings across languages.

- **No asymmetry in cross-lingual priming**. The authors compared their results with a previous experiment that used the reverse direction of priming (from L1 to L2) and found no significant differences in the magnitude or direction of the priming effects. This indicates that cross-lingual priming is symmetrical and bidirectional, contrary to some previous studies that reported an asymmetry favoring L1-to-L2 priming.

- **No cognate facilitation or interlingual homograph inhibition in L1**²[2]. The authors also analysed the unprimed data and found no evidence for faster or more accurate responses to cognates than to translation equivalents, or slower or less accurate responses to interlingual homographs than to translation equivalents, in the Dutch semantic relatedness task. This contrasts with previous findings that showed such effects in L2, suggesting that word type effects are modulated by language dominance and task demands.

1. Page 1 - Line 16

2. Page 1 - Line 32

---

# Method

They find rule-based systems (tongueSwitcher) work fine in identify cs word while neural model excel in identify language ambiguous word.

*run comprehensive experiments across island sizes and also calculate token-level and entity-level F1 scores, which shows the success of their system for both hard and easier cases.

---

# Limitation

1. rule-based: rules may only fit to current language pairs. adaptation to other language may be a challenge. require manual supervision on the rule set.
2. training wordlists: require neither high quality lexica nor human annotated training material. the quality of model limit to the quality of the wordlists.
3. **Sample size and representativeness**: The authors only recruited 106 Dutch–English bilinguals, who may not be representative of other bilingual populations. They also acknowledged that their sample size was constrained by their budget and power analysis.
4. **Task differences**: The authors used a semantic relatedness task to measure the effects of priming and word type, which may not tap into the same processes as other tasks such as lexical decision or picture naming. They also noted that the semantic relatedness task may have been too easy for their highly proficient participants, reducing the sensitivity of the task.
5. **Direction of priming**: The authors only tested the effect of priming from L2 to L1, but not from L1 to L2. They compared their results to a previous experiment that used the opposite direction of priming, but this comparison may not be valid due to potential differences in stimuli, participants, and experimental settings.

---

The problem that this research paper addresses is how **prior experience in one language can influence the processing of words in another language**, especially for words that have the same form but different meanings across languages (e.g. angel in English and Dutch). “Recent experience with these words in the L1 can influence the processing of cognates and interlingual homographs in the L2. Cross lingual priming effect occurs when exposure to a word or phrase in one language affects the subsequent processing of a similar word or phrase in a different language.” For example, processing of cognates may be speeded up, while processing of interlingual homographs may be delayedThe authors investigate whether this cross-lingual priming effect is symmetrical or asymmetrical, and whether it depends on the direction of language switching (from L1 to L2 or vice versa), the task demands, and the word type (cognates, interlingual homographs, or translation equivalents).

---

# Future Work

Cross-lingual priming in other language pairs: The authors note that their results may not generalize to other language pairs that differ more in orthography or phonology than Dutch and English. They propose to test whether cross-lingual priming effects are modulated by the degree of similarity between languages.

Cross-lingual priming in other tasks: The authors point out that their semantic relatedness task may not capture all aspects of word-meaning processing. They suggest using other tasks that tap into different levels of semantic representation, such as semantic categorization or word association.

Cross-lingual priming in other contexts: The authors acknowledge that their experimental context may not reflect the natural language-switching situations that bilinguals encounter in their daily lives. They propose to investigate how cross-lingual priming is affected by factors such as language mode, frequency of language switching, and task demands.

---

# Cross-Lingual Priming

cross-lingual priming is a effect cause by the occurrence of word A in language I, affecting the processing of word A in language B. Cross-lingual priming is indeed the effect where the occurrence of a word (let’s call it “word A”) in one language (Language I) influences the processing of the same or related word (“word A”) in another language (Language B). It’s a fascinating phenomenon that sheds light on how our minds connect and process words across different languages.

## What is Cross-Lingual Priming?

Cross-lingual priming refers to a fascinating phenomenon observed in bilingual individuals. It occurs when exposure to a word or concept in one language (let’s call it Language A) influences the processing of related words or concepts in another language (Language B), and vice versa.

In simpler terms, if you encounter a word in your first language (L1), it can affect how you process a similar word in your second language (L2), and vice versa.

Examples of Cross-Lingual Priming:

Imagine you’re a bilingual speaker of English (L1) and French (L2). Here are some examples:

1. Cognates: Words that look and mean the same in both languages (e.g., “hotel” in English and “hôtel” in French). When you encounter “hotel” in English, it may make you recognize the French equivalent more quickly.
2. Interlingual Homographs: Words that have the same spelling but different meanings across languages (e.g., “bat” meaning a flying mammal in English and a sports equipment in Dutch). Recent exposure to “bat” in English might influence how you process it in Dutch.
3. Idioms: Non-compositional phrases with figurative meanings (e.g., “kick the bucket”). If you encounter the translated version of an idiom from L1 in L2, you’ll recognize it, but its figurative meaning may be processed more slowly.

## Why Study Cross-Lingual Priming?

Understanding cross-lingual priming helps us explore how bilinguals access and organize their mental lexicon (the mental dictionary of words).

It sheds light on how languages interact in the bilingual mind and how prior experience in one language affects the other.

Researchers use various tasks (semantic relatedness, lexical decision, etc.) to investigate these effects.

## Research Questions and Future Directions:

Researchers study whether cross-lingual priming is symmetrical (works both ways) or asymmetrical (stronger in one direction).

They explore how factors like language similarity, task demands, and context influence cross-lingual priming.

Future work could involve testing other language pairs, using different tasks, and examining real-world language-switching scenarios.

In summary, cross-lingual priming provides valuable insights into bilingual cognition and the intricate connections between languages in our minds. As you delve deeper into this concept, consider how it impacts language processing, memory, and communication for bilingual individuals.

---

# Process a word in the context of cross-lingual priming:

1. Pronunciation:
    
    When we process a word, we often start by pronouncing it in our minds or even aloud.
    
    For example, if you encounter the word “apple,” you might mentally say its pronunciation: /ˈæpəl/.
    
2. Understanding:
    
    Understanding a word involves grasping its meaning. This can happen at different levels:
    
    1. Lexical Level: Recognizing that “apple” refers to a fruit.
    2. Semantic Level: Understanding that an apple is a sweet, edible fruit typically with red or green skin.
    
    This understanding allows us to connect the word to our existing knowledge.
    
3. **Translation** (if applicable):
    
    In the context of cross-lingual priming, translation plays a role.
    
    If you encounter the word “pomme” (French for “apple”), your mind might automatically connect it to the English word “apple.”
    
    So, processing involves recognizing the translation equivalence between words in different languages.
    
4. Activation in the Mental Lexicon:
    
    Our mental lexicon is like an internal dictionary where we store information about words.
    
    When we process a word, we activate its representation in this mental lexicon.
    
    This activation influences subsequent processing of related words.
    
5. Speed and Accuracy:
    
    Processing speed matters. If you recognize a word quickly, it suggests efficient processing.
    
    Accuracy matters too. Correctly identifying the meaning of a word is crucial.
    
6. Task-Specific Processing:
    
    Different tasks (e.g., reading, listening, speaking, or semantic judgments) involve distinct aspects of word processing.
    
    Cross-lingual priming studies use tasks like semantic relatedness (judging how related two words are) or lexical decision (deciding if a string of letters is a valid word).
    

In summary, when we process a word, we engage in a complex dance of pronunciation, understanding, translation (if applicable), and activation in our mental lexicon. Cross-lingual priming explores how these processes interact across languages, revealing fascinating insights into bilingual cognition.

---.  
  
  
# Annotations%% begin annotations %%  
  
  
  
### Imported: 2024-02-26 2:35 am
  
  
<mark style="background-color: #ffd400">Quote</mark>  
> The first method is rule-based, using wordlists and morphological processing.  
  
<mark style="background-color: #ffd400">Quote</mark>  
> pretraining of a neural language model on this corpus and classify tokens based on embeddings from this language model.  
  
<mark style="background-color: #ffd400">Quote</mark>  
> study code-switching for language-ambiguous words which can only be resolved in context  
  
<mark style="background-color: #ffd400">Quote</mark>  
> Many NLP systems are currently developed to be capable of handling text from informal contexts. Code-switching places new pressure on these, particularly for applications that require the recognition and precise extraction of meaning from codeswitched text, or even the generation of such text. Available NLP tools lag behind in this respect (Aguilar and Solorio, 2020; Do ̆ gruöz et al., 2021); in particular large language models perform best when fine-tuned on natural code-switching data (Santy et al., 2021). Our work is aimed towards NLP tools that can better unde  
  
  
%% end annotations %%

%% Import Date: 2024-02-26T02:35:47.686+08:00 %%

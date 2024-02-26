---
doi: 10.21437/Interspeech.2020-1936
category: literaturenote  
tags:   
citekey: manghatMalayalamEnglishCodeSwitchedGrapheme2020  
status: unread
Rating: 0/5
Title: Malayalam-English Code-Switched: Grapheme to Phoneme System
ShortSummary: 
dateread: {DATE}
---

> [!Cite]
> Manghat, S., Manghat, S., & Schultz, T. (2020). Malayalam-English Code-Switched: Grapheme to Phoneme System. _Interspeech 2020_, 4133–4137. [https://doi.org/10.21437/Interspeech.2020-1936](https://doi.org/10.21437/Interspeech.2020-1936)
  
>[!Synth]  
>**Contribution**::  
>  
>**Related**:: 
>  
  
>[!md]-
>**FirstAuthor**:: Manghat, Sreeja  
>**Author**:: Manghat, Sreeram  
>**Author**:: Schultz, Tanja  
~  
>**Title**:: Malayalam-English Code-Switched: Grapheme to Phoneme System
>**Year**:: 2020
>**Citekey**:: manghatMalayalamEnglishCodeSwitchedGrapheme2020
>**itemType**:: conferencePaper
>**Publisher**:: ISCA
>**Pages**:: 4133-4137
>**DOI**:: 10.21437/Interspeech.2020-1936
  
> [!LINK]-
> 
> [Manghat et al_2020_Malayalam-English Code-Switched.pdf](file://C:\Users\Wong\Zotero\storage\HBT7SBM6\Manghat%20et%20al_2020_Malayalam-English%20Code-Switched.pdf).
  
> [!Abstract]-
>.

> [!tldr]- Summary
> A short summary - or an abstract in 3 sentences, relating to YOU. What did YOU find interesting about this paper. 

> [!quote]- Quotable
> Imagine you would quote this paper in your publication. How would you do it? It is probably just one sentence followed by the reference. It is the most intense condensation of the information in this paper and forces you to be on point. 


# Notes  
>  
>#speech-to-text #code-switch-identification

# Summary

The document is about developing a grapheme to phoneme (G2P) system for Malayalam-English code-switched speech, which is a challenging task due to the different orthographies and phonologies of the two languages.  This system identifies overlapping phonemes between English and Malayalam and applies rules to handle intra-word code-switching scenarios

The authors use a conversational speech corpus of 20 hours of Malayalam-English code-switched speech, as well as Twitter text data to identify the special cases and rules for handling intra-word code-switching1.

The authors propose a rule-based G2P system that can handle both monolingual and intra-word code-switched words, by identifying the root and tail parts of the words and applying appropriate rules for phoneme mapping and concatenation.

The authors evaluate their G2P system on a test set of 420 reference words, and report a phoneme error rate (PER) of 3.2% for monolingual Malayalam, 2.1% for Malayalam-English intra-word code-switching, and 3.8% for English-Malayalam intra-word code-switching. They also analyze the coverage and sources of errors of their system.

# Problem Statement

The problem that this research addresses is the lack of a grapheme-to-phoneme (G2P) system for Malayalam-English code-switched speech, which is common among bilingual speakers of Malayalam and English. Code-switched speech involves mixing elements of two or more languages within a conversation or utterance1. The paper focuses on the special case of intra-word code-switching, where a single word contains parts from both languages. For example, Directorന്െറ (Directorinte) is an English-Malayalam intra-word code-switched word2. The paper proposes a G2P system that can handle such cases and generate phonetic transcriptions for Malayalam-English code-switched speech34.

# Limitation

The G2P system is based on a pilot dataset of Malayalam-English code-switched speech data, which may not cover all the possible cases and scenarios of code-switching12.

The system does not handle the special cases of code-switching occurring with names of person, places and entity, which may require additional rules or resources3.

The system does not consider the accented English in the code-switched speech, which may affect the pronunciation and phoneme mapping of the English words.

The system does not address the issues of dialectal variation and social media influence on the Malayalam language, which may introduce new words and slang terms that are not in the dictionary.

# Methodology

In the context of the research paper, the proposed rule-based G2P system employs the following steps to recognize such words:

Segmentation: The system identifies the root and tail parts of the word. The root corresponds to the language of origin (Malayalam or English), while the tail represents the code-switched part.

Phoneme Mapping: For the root part, the system maps the graphemes (letters) to their corresponding phonemes (speech sounds) based on language-specific rules. Similarly, it maps the code-switched tail to its phonetic representation.

Concatenation: The system concatenates the phonemes of the root and tail to form the complete phonetic transcription of the intra-word code-switched word.

By analyzing the overlapping phonemes and applying appropriate rules, the system ensures accurate phonetic representations for these complex words, which is crucial for various natural language processing tasks.

# ! No Clear boundary in the csw:

handling cases where there is no clear boundary between the root and tail parts of a code-switched word is a crucial challenge. Here’s how the system addresses this issue:

Segmentation Challenges:

In intra-word code-switching, some words seamlessly blend both Malayalam and English elements without clear demarcation.

Identifying the exact boundary between the root (language-specific part) and the tail (code-switched part) can be tricky.

Approach:

The proposed rule-based G2P system analyzes the overlapping phonemes between Malayalam and English.

It identifies common phonemes that occur in both languages, even when they are part of the same word.

By considering these shared phonemes, the system determines the likely boundary between the root and tail.

Example:

Consider the code-switched word “kuttikal (കുട്ടികൾ)”:

The root is “kuttikal,” which means “children” in Malayalam.

The tail is the English letter “s.”

The system identifies the overlapping phoneme “k” as the boundary.

Adaptability:

While this approach works well for Malayalam-English code-switching, it may need adjustments for other language pairs with different phonologies and orthographies.

Handling unclear boundaries requires robust rules and context-aware analysis.

In summary, the system leverages shared phonemes to make informed decisions about the root-tail segmentation, ensuring accurate phonetic transcriptions for complex code-switched words.  
  
  
# Annotations%% begin annotations %%  
  
  
%% end annotations %%

%% Import Date: 2024-02-26T02:33:11.310+08:00 %%

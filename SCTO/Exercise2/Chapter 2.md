# Chapter 2: Incorporating Source Syntax in NMT

In the previous chapter, we explored the foundations of Neural Machine Translation (NMT). Now, let’s delve deeper into an intriguing aspect: **modeling source syntax** to enhance translation accuracy.
![[Pasted image 20240204124130.jpg]]![[Pasted image 20240204124132.jpg]]![[Pasted image 20240204124140.jpg]]![[Pasted image 20240204124142.jpg]]

<iframe width="560" height="315" src="https://www.youtube.com/embed/D1kSz6qZ288?si=gAYB1MnoMSHqeOlg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## The Role of Source Syntax

While linguistics-free NMT models implicitly learn syntactic information from source sentences, explicit incorporation of **source syntax** can yield further improvements. In this chapter, we explore how to integrate syntax into NMT effectively.

### Linearizing Parse Trees

1. **Structural Label Sequences**:
    
    - We linearize parse trees of source sentences, obtaining structural label sequences.
    - These sequences represent the syntactic structure of the input.
2. **Syntactic Encoders**:
    
    - We propose three types of encoders to incorporate source syntax:
        - **Parallel RNN Encoder**: Learns word and label annotation vectors in parallel.
        - **Hierarchical RNN Encoder**: Learns vectors in a two-level hierarchy.
        - **Mixed RNN Encoder**: Stitchingly learns word and label annotation vectors over mixed sequences.

### Experimental Insights

- **Chinese-to-English Translation**:
    - Experimentation demonstrates that all three proposed syntactic encoders improve translation accuracy.
    - [Surprisingly, the simplest **Mixed RNN Encoder** achieves the best performance, with a significant improvement of **1.4 BLEU points**](https://aclanthology.org/P17-1064/)[1](https://aclanthology.org/P17-1064/).

### Unveiling the Benefits

An in-depth analysis reveals how source syntax benefits NMT:

1. **Improved Alignment**:
    
    - Syntactic information aids in aligning source and target sequences during translation.
2. **Handling Complex Structures**:
    
    - Syntax-aware encoders capture complex sentence structures more effectively.
3. **Reduced Ambiguity**:
    
    - Explicit syntax reduces ambiguity, leading to more accurate translations.

In the next chapter, we’ll explore additional refinements and delve into practical techniques for enhancing NMT. Syntax is our secret weapon in the quest for better translations! 🌐📝

---

[For further exploration, you can refer to Philipp Koehn’s comprehensive treatment of NMT in his](https://aclanthology.org/P17-1064/) [2](http://www2.statmt.org/nmt-book/). It covers various aspects, including syntax integration and challenges.
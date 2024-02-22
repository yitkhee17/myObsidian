[CONFLATOR: Incorporating Switching Point based Rotatory Positional Encodings for Code-Mixed Language Modeling](https://openreview.net/forum?id=B3ykB9aIu7)

- transformer work fine, but cannot reproduce positional information made(?). SO, positional encoding is introduced to collect the information of the word and its position. 
	- "Though transformers are capable and powerful, they cannot always encode positional information since they are non-recurrent. Therefore, to enrich word information and incorporate positional information, positional encoding is defined." 

- [[Switching Points(SPs)]] challenges the CS LMs.
	- " We hypothesize that Switching Points (SPs), i.e., junctions in the text where the language switches (L1 -> L2 or L2 -> L1), pose a challenge for CM Language Models (LMs), and hence give special emphasis to SPs in the modeling process."
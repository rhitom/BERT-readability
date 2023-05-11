# BERT-readability
Computing Ranked Sentence Readability Score using BERT

###**INTRODUCTION**##
In an effort to calculate a clear, intuitive readability score for a given document, I used BERT to compute a **Ranked Sentence Readability Score (RSRS)** for a given document. The Ranked Sentence Readability Score calculates readability based on the likelihood that a word will appear next in a sentence. Using likelihood, sentence length, and word position, I calculated the RSRS for each sentence in a document, and then averaged the sentences' scores to produce the readability score for the document as a whole. 

To develop a readablity score that is clear and intuitive without losing the nuance and rigor of the RSRS, I used three techniques to map RSRS: min-max scaling, z-score normalization, and boxcox transformation.

To measure how well these transformed scores align with human experience, I calculate the raw readability score along with the scaled, standardized, and BoxCox-transformed scores. I planned to ask users to select the score that best represented their experience reading the document. However, I did not have the time to integrate human feedback in this experiment. From cursory first-glance analysis of the article with the maximum readability score of 200 randomly sampled articles, generating a simple percentage scale of readability appears to be most effective at producing a clear, intuitive readability score. 

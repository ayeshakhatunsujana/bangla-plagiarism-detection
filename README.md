## Semantic Plagiarism Detection of Bangla: Paraphrase Generation and Sentence Embedding using Language Model
Bangla, the seventh most spoken language in the world, remains underrepresented in the development of advanced NLP tools. Plagiarism detection is especially critical in low-resource languages like Bangla, where traditional plagiarism detection tools often fail to detect complex paraphrasing and semantic similarity. To address this, I have proposed a hybrid approach for semantic plagiarism detection in Bangla by combining paraphrase generation and sentence embedding using Large Language Models (LLMs). Models such as BanglaT5, and multilingual versions of BART are employed for paraphrasing. To measure semantic similarity between original and paraphrased texts, I have used Bangla-BERT. Evaluation metrics including F1-score ans BERTScore are used to assess performance. My findings shows that Bangla-T5 performed good than mBART in different threshold.

<p align="center">
  <img src="/img.png" alt="Archi" width="700" height="350"/>
</p>
<p align="center">
  Figure 01: An Architecture of Semantic Plagiarism Detection of Bangla using Paraphrase Generation and Sentence Embedding.
</p>

#### Features
-   Paraphrase Generation of Bangla Sentences using Pretrained mBART, Bangla-T5 and GPT-4o-mini
-   Matching the paraphrase using Sentence Embeding like BERT
-   Calculate Similarity for Different Thresholds (0.55-0.85)
-   Calculate the performance matrics like F1, BERT, ROUGE, BLEU, and BART scores
-   Create the plots of F1 score and BERT score 

#### Project Structure
-   bangla-plagiarism-detector.ipynb: Main script for data processing, modeling, and visualization.
-   dataset.py: modified data which is collected from hugginf face.
-   full_environment.yml: List of required Python libraries.
-   README.md: The project instructions.

#### Dataset
-   The dataset consists of the following columns:
    sentence1: First sentence.
    sentence2: Second sentence.
    label: 1 denotes paraphrase and 0 denotes non-paraphrase.
    link: https://huggingface.co/datasets/bracealround/BnPC-A-Gold-Standard-Bangla-Paraphrase-Corpus 

#### Result Analysis
This plot shows the Bangla-BERT similarity scores for three language models—Bangla-T5, mBART, and GPT-4o-mini—at different thresholds used for Bangla plagiarism detection. The BERT score measures how semantically close the generated paraphrase is to the reference sentence.

From the plot, we can see that GPT-4o-mini consistently achieves the highest BERT scores, peaking at 0.95 and staying above 0.92 across all thresholds, which indicates strong semantic understanding. Bangla-T5 also performs well, maintaining a steady BERT score of around 0.86. In contrast, mBART has the lowest scores, remaining flat at 0.75 throughout, suggesting weaker semantic similarity in its paraphrases. Overall, GPT-4o-mini demonstrates the best semantic match quality, while mBART lags behind, and Bangla-T5 performs moderately well.

<p align="center">
  <img src="/output.png" alt="result" width="700" height="350"/>
</p>
<p align="center">
  Figure 02: Performance Comparison of Bangla-t5, mBART and GPT-4o-mini .
</p>

#### Conclusion
In conclusion one observation I would like to share is that paraphrase generation did not significantly improve the results in this case. As we know, language models often struggle with low-resource languages like Bangla. However, better performance might be achieved by fine-tuning the language model and experimenting with different types of prompting strategies.

#### Instructions
-  Clone the repository
-  Install dependencies
-  I have also attched the code in zip file into the D2L

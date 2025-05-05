## Semantic Plagiarism Detection of Bangla: Paraphrase Generation and Sentence Embedding using Language Model
Bangla, the seventh most spoken language in the world, remains underrepresented in the development of advanced NLP tools. Plagiarism detection is especially critical in low-resource languages like Bangla, where traditional plagiarism detection tools often fail to detect complex paraphrasing and semantic similarity. To address this, I have proposed a hybrid approach for semantic plagiarism detection in Bangla by combining paraphrase generation and sentence embedding using Large Language Models (LLMs). Models such as BanglaT5, and multilingual versions of BART are employed for paraphrasing. To measure semantic similarity between original and paraphrased texts, I have used Bangla-BERT. Evaluation metrics including F1-score ans BERTScore are used to assess performance. My findings shows that Bangla-T5 performed good than mBART in different threshold.

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

####  Instructions
-  Clone the repository
-  Install dependencies
-  I have also attched the code in zip file into the D2L

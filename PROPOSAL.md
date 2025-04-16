Hi all, here is my proposal.

**Modeling Experiment Proposal:** 

Semantic Plagiarism Detection Task using a Bangla Paraphrase

**Reasons for Choosing this Dataset:** 

There are mainly two reasons for selecting this dataset. One is that the dataset contains Bangla sentence pairs labelled as paraphrases or non-paraphrases, which is essential for detecting semantic plagiarism. The second reason, or we can say the motivation behind the choice of this dataset, is that since semantic plagiarism detection is a growing concern, especially with AI-generated content, this dataset provides an ideal test case. 

**How Model will Differ from Existing one:**
Actually, much work has been done in this particular area on high-resource languages like English, but I want to know how low-resource languages like Bangla work using transformers for Semantic Plagiarism Detection Task.  

Dataset from Hugging Face: [https://huggingface.co/datasets/bracealround/BnPC-A-Gold-Standard-Bangla-Paraphrase-Corpus](https://huggingface.co/datasets/bracealround/BnPC-A-Gold-Standard-Bangla-Paraphrase-Corpus) 

**Modeling Approach:** 

 I will be using a hybrid approach combining paraphrase generation and sentence embedding techniques. My pipeline includes paraphrase generation using transformer models like T5, sentence embeddings using Sentence-BERT, and measuring similarity using the F1 score. I’ll evaluate the model using the above metrics and experiment with different paraphrase models to identify the best approach for detecting semantic plagiarism.

My GitHub repository link: 

[https://github.com/ayeshakhatunsujana/bangla-plagiarism-detection](https://github.com/ayeshakhatunsujana/bangla-plagiarism-detection) 


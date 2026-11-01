# IU Data Analysis – NLP Analysis of Consumer Complaints

## Project Description

This project analyzes consumer complaints using Natural Language Processing (NLP). The goal is to identify recurring topics and patterns in a collection of consumer complaint texts.

The project uses a sample of 1,000 consumer complaints from the Consumer Financial Protection Bureau (CFPB).

## Dataset

- **Source:** [Hugging Face – CFPB Consumer Complaints](https://huggingface.co/datasets/claritystorm/cfpb-consumer-complaints)
- **Original sample size:** 1,000 records
- **Records containing complaint texts:** 271
- **Final dataset after cleaning:** 263 unique complaint texts
- **Text column:** `consumer_narrative`

## Methods and Technologies

The analysis was implemented in Python using Google Colab.

The following methods and libraries were used:

- **Pandas:** Data loading and preprocessing
- **NumPy:** Numerical operations
- **Scikit-learn:** Text vectorization and topic modeling
- **CountVectorizer:** Word frequency representation
- **TF-IDF:** Term importance weighting
- **LDA (Latent Dirichlet Allocation):** Topic modeling
- **NMF (Non-negative Matrix Factorization):** Topic modeling
- **Gensim:** Topic coherence evaluation
- **Matplotlib:** Data visualization

## Project Workflow

1. Loading and exploring the dataset
2. Removing missing and duplicate complaint texts
3. Text preprocessing and cleaning
4. Text vectorization using CountVectorizer and TF-IDF
5. Topic modeling using LDA and NMF
6. Testing different topic numbers from 2 to 10
7. Evaluating topic coherence using the C_v metric
8. Interpreting and visualizing the identified topics

## Results

The topic coherence evaluation indicated that NMF with six topics achieved the highest coherence score within the tested range.

- **Selected method:** NMF
- **Selected number of topics:** 6
- **Coherence score (C_v):** 0.6114
- **Final dataset:** 263 complaint texts

The identified topics include identity theft, consumer privacy, inaccurate credit reports, late payment disputes, debt collection and mortgage-related complaints.

## How to Run

1. Open the Jupyter Notebook `IU_Data_Analysis_NLP_Phase2.ipynb`.
2. Upload or open it in Google Colab.
3. Run the code cells sequentially.
4. Install the required libraries if necessary.

## Limitations

The analysis is based on a sample of 1,000 records, of which 263 contain unique complaint texts after preprocessing. Therefore, the results should not be considered representative of all consumer complaints.

Topic labels are interpretations of the most relevant words and complaint examples identified by the models.

---

**Project:** IU – Projekt: Data Analysis (DLBDSEDA02_D)  
**Task:** NLP Techniques for Text Collection Analysis

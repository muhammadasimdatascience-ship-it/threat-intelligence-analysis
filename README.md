# Threat Intelligence Analysis for Data Security

Information System Security · Assignment 02 · Guizhou University  
Muhammad Asim Iqbal

This Google Colab notebook compares classical and neural sentiment models on Chinese text and uses LDA to identify recurring topics. A keyword screening exercise illustrates how a reviewer might prioritize text for follow-up. The review corpus provides sentiment labels, and keyword matches require human validation.

## Run the project

1. Download the notebook and upload it to Google Colab.
2. Upload your course copy of `waimai_10k.csv` to `/content` in the same runtime. To use a different corpus, change `DATASET` or `CSV_PATH` in Step 1.
3. Run all cells in order. A GPU is optional. Fill in your student details in your private Colab copy.
4. Download the generated results ZIP. It contains the Word report draft, figures, evaluation tables, cleaning audit, and run settings. Add your own interpretation and screenshots to the report.

## Methods

| Stage | Approach |
| --- | --- |
| Data preparation | Unicode normalization, identifier pattern masking, jieba segmentation, deduplication, and a shared stratified train/validation/test split |
| Traditional ML | Majority baseline, logistic regression, linear SVM, and multinomial Naive Bayes |
| Deep learning | TextCNN, GRU, and BiLSTM |
| Evaluation | Macro F1, ROC AUC, average precision, confusion matrices, and error analysis by review length |
| Topic mining | Count-based LDA with held-out topic summaries and exploratory keyword screening |

The notebook fits its vocabulary and feature transformations on training data. The results and report are generated when you run it.

## Data reference

The default corpus is described in the [ChineseNlpCorpus repository](https://github.com/SophonPlus/ChineseNlpCorpus/tree/master/datasets/waimai_10k). Record the source of the copy you use in the notebook configuration.

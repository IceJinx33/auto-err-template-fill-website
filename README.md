## $\color{#F8CD46}INTRODUCTION$

Recent works proposing modern NLP models for the document-level information extraction tasks (Du et al., 2021; Li et al., 2021; Jain et al., 2020) have their performance measured by different datasets via varying metrics, with limited, often manual analysis of model errors which are less informative (e.g., scores alone cannot detail model’s tendency to assign incorrect types to selected noun phrases, or frequency of spurious templates/clustering generation). There has not been a systematic investigation on models’ error profiles across domain-diverse document-level IE datasets.

In this work, we introduce several representative document-level IE datasets. Then, inspired by the work of Kummerfeld and Klein (2013) on tackling the error analysis challenge for coreference resolution, we introduce a framework for automating the process of error analysis for document-level information extraction tasks. This framework automatically transforms the predicted outputs into the desired extraction structures, through a set of transformations (Figure 1), and then maps each transformation or a set of transformations into sensible and linguistically motivated error types (Table 1). We apply two state-of-the-art neural methods to three document-level information extraction tasks from multiple domains including the scientific literature. One method (i.e., GTT (Du et al., 2021) is designed for doc-level extraction; the other is DyGIE++ (Wadden et al., 2019), sentence-level extraction augmented with clustering to create the doc-level representation. We also replace their base pre-trained model with SciBERT (Beltagy et al., 2019). We analyse their behaviors and errors in their predictions via our automatic framework.

## $\color{#F8CD46}DATASETS$

==Repository includes==
- scripts for preprocessing human plural-response data,
- scripts/notebooks for building the trigram baseline from the Leipzig corpus extraction,
- scripts/notebooks for probing gBERT and mBERT,
- scripts for computing JSD and uncertainty metrics,
- scripts for statistical testing and figure generation,
- final report.


==Data availability and inputs==
This project uses two data sources:
- Human plural judgment dataset (author-created; not publicly licensed) 
- Leipzig Corpora Collection (German Web Corpus, 2021 release, downloaded from the Leipzig/Wortschatz project website.

Raw corpus files are not redistributed in the repository. 
The smaller dataframes for the analysis scripts are included.


==Steps==
1) Set up the environment (Dependencies are listed in: requirements.txt)

2) Prepare data

3) Preprocess human responses and map plural classes (human_results.csv)

4) Build trigram baseline from corpus extraction (build_corpus.ipynb, trigram_model.csv)

5) Run BERT probing (gBERT and mBERT) (all_results.csv, bertanalysis copy.ipynb)

6) Compute evaluation metrics (all_results.csv, bertanalysis copy.ipynb)

7) Run statistical tests (all_results.csv, bertanalysis copy.ipynb)

8) Generate figures and tables (all_results.csv, bertanalysis copy.ipynb)


==Notes on reproducibility limitations==
- The human judgment dataset is author-created and may not be fully public; if restricted, the repository includes scripts and documentation but not raw participant-level data.
- Some results may vary slightly across library/model versions (especially Transformer tokenization/probing internals).
- Paths in notebooks may need to be adapted to local setups.
- The Leipzig corpus is large; preprocessing can be time-consuming and may require substantial disk space.

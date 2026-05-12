# Predicting-P-granule-mRNA-Stability-from-Primary-Structure-in-Early-C.-elegans-Embryogenesis
## Introduction:

P-granules in the model organism *Caenorhabditis elegans* are enriched with maternally derived mRNAs in the early phases of embryogenesis, but a significant proportion of these transcripts are degraded before reaching primordial germ cells (PGCs). These cells are the embryonic precursors for gametes, which are the responsible for passing genetic information down to offspring. Only a small proportion of stable maternally derived mRNAs are maintained and passed on to the germline, however the mechanisms underlying this process are a topic of ongoing research. P-granule association alone does not determine whether maternally derived mRNAs are maintained or degraded (Scholl et al.). The aim of this project is to investigate whether information found within the primary structure of mRNA is sufficient for predicting the stability of maternally derived mRNAs in P-granules during the early phases of embryogenesis.

### Ground truth dataset:

https://datadryad.org/downloads/file_stream/3243524

### Ground truth data description:

The ground truth dataset contains label information for maternally derived mRNA molecule fate in P-granules during early phase embroyonic development in c. elegans. The dataset was derived from experimentally validated single-molecule fluorescence in situ hybridization (smFISH). Labels are contained within the 'Groups' column, where 'Group I' represents **stable** mRNAs in P-granules and 'Group II' represents **degraded** mRNAs in P-granules.

Preprocessing changes labels to:

Group I = 0 (stable)

Group II = 1 (degraded)

### Feature sets:

This project will explore four different feature sets that were derived from sequence information found in the primary mRNA structure.

1) `kmers_features.csv`: 4-mer count matrix of 3' untranslated region (3'UTR)
2) `utr_length.csv`: 3'UTR lengths
3) `rna_structure.csv`: Minimum free energy of secondary structure with paired and unpaired fractions
4) `lunp_feature_matrix.csv`: Average pair probabilities for locally stable secondary structures



### References:

Alyshia Scholl, Yihong Liu, Geraldine Seydoux; Caenorhabditis elegans germ granules accumulate hundreds of low translation mRNAs with no systematic preference for germ cell fate regulators. Development 1 July 2024; 151 (13): dev202575. doi: https://doi.org/10.1242/dev.202575

Ronny Lorenz, Stephan H. Bernhart, Christian Höner zu Siederdissen, Hakim Tafer, Christoph Flamm, Peter F. Stadler, and Ivo L. Hofacker. ViennaRNA package 2.0. Algorithms for Molecular Biology, 6(1):26, 2011. doi:10.1186/1748-7188-6-26.

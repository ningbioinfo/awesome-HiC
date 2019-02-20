# Awesome-HiC [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Awesome collections of HiC-seq analysing softwares

The eukaryotic genome have hierarchical three_dimensional conformation, where physical contacts between chromatin have been proved to govern the regulation of gene expression. High-resolution chromosome conformation capture sequencing (HiC-seq) has been one of the most important methods to investigate the 3D genome since its first publication in 2009\. Since then, numerous of softwares and packages have been developed to facilitate the analysis of HiC-seq data.

Here is a curated **awesome** list of HiC-seq data related softwares/packages/intro-papers that are recommended for HiC data analysis and research.

Your contributions are always welcome!

## Contents

- [Pipelines](#Pipelines)
- [Toolkits](#Toolkits)
- [Mapping](#Mapping)
- [Normalisation](#Normalisation)
- [Visualisation](#Visualisation)
- [Significant contacts identification](#Significant-contacts-identification)
- [Topologically-Associated Domains identification](#Topologically-associated-domains-identification)
- [Other awesome HiC softwares](#Other-awesome-softwares-related-to-HiC-seq)
- [HiC-seq introduction papers](#HiC-seq-introduction-papers)

---

## Pipelines

_Pipelines to process HiC-seq data from raw/trimmed data input to interactions/matrices output_

- [HiC-Pro](https://github.com/nservant/HiC-Pro) - An easy configured pipeline that can process raw data/trimmed data all the way to HiC interaction matrix, it is one of the most popular pipeline with a user-friendly documentation and it plays well with HPC.
- [Juicer](https://github.com/aidenlab/juicer) - Comes with a comprehensive Wiki and provides a couple of other tools for downstream analysis like a browser called JuiceBox for visualisation. The performance is very fast and it plays well with HPC, but it is not designed for data with relative low resolution.
## Toolkits

_Toolkits that containing multiple tools to analyse HiC-seq data_

- [diffHiC](http://www.bioconductor.org/packages/release/bioc/html/diffHic.html) - Well documented user's guide and it has multiple functions for filtering, normalisation and identifying differential HiC interactions from multiple datasets. It is a R package so it can work well with lots of other R packages.
- [Homer](http://homer.ucsd.edu/homer/interactions/) - Recently updated a new HiC workflow, including alignment, quality control, filtering, generating interaction matrix and normalisation, identifying TADs and loops. It can also generate configure file for circos plots.
- [TADbit](https://github.com/3DGenomes/TADbit) - A python library that contains multiple functions for analysing HiC data with its own TADs calling algorithm, and it has a well documented tutorial.
- [HiTC](https://bioconductor.org/packages/release/bioc/html/HiTC.html) - Developed by the author of HiC-Pro.

## Mapping

_Softwares/packages to conduct alignments and filtering of HiC-seq data_

- [HiCUP](https://www.bioinformatics.babraham.ac.uk/projects/hicup/) - Provides well documented tutorial including YouTube videos, and it can generate a interactive html report as a result.
- Other mapping strategies can be found in pipelines & Toolkits.

## Normalisation

_Softwares/packages to conduct matrix normalisation of HiC-seq data_

- Explicit fashion

  - [HiCNorm](http://www.people.fas.harvard.edu/~junliu/HiCNorm/) - Included in the HiTC R package.

- Implicit fashion

  - [Iterative Correction and Eigenvector decomposition (ICE)](https://bitbucket.org/mirnylab/hiclib) - Included in the HiC-Pro pipeline.

## Visualisation

_Softwares/packages to conduct visualisation of HiC-seq data_

- [JuiceBox](https://github.com/aidenlab/Juicebox) - A part of the Juicer toolkit and it can also customise multiple types of data tracks, and it can plot gene loops on heatmaps.
- [HiCPlotter](https://github.com/kcakdemir/HiCPlotter) - Compatible with the HiC-Pro pipeline and easy to use.
- [Sushi](https://bioconductor.org/packages/release/bioc/html/Sushi.html) - A R package and one of the function is to take common HiC matrix as input to plot a heatmap.
- [HiGlass](http://higlass.io/) - A web-based browser and can also be run locally within a Docker container.

## Significant contacts identification

_Algorithms to identify significant contacts_

- [FitHiC](https://github.com/ay-lab/fithic) - Provides a two-step spline-fitting procedure and binomial model to identify significant interactions.
- [CHiCAGO](http://regulatorygenomicsgroup.org/chicago) - This model only works for capture HiC data, it uses negative binomial random model to model read counts and uses poisson random model to model sequencing errors and artefacts.

## Topologically-Associated Domains identification

_Algorithms to identify Topologically-Associated Domains (TADs)_

- [rGMAP](https://github.com/wbaopaul/rGMAP) - A R package including TADs calling functions and plotting functions for visualisation, and it is able to identify sub-TADs.
- [HiTAD](https://github.com/XiaoTaoWang/TADLib) - A python library and has a comprehensive documentation for all the functions.
- [TopDom](http://zhoulab.usc.edu/TopDom/) - An easy to use R package.

## Other awesome softwares related to HiC-seq

_Other softwares/packages_

- [HiC-QC](https://github.com/ningbioinfostruggling/HiC-QC) - QC for preliminary HiC libraries.
- [Boost-HiC](https://github.com/LeopoldC/Boost-HiC) - HiC patterns detection from low resolution HiC data.
- [HiCPlus](https://github.com/zhangyan32/HiCPlus) - Resolution Enhancement of HiC interaction heatmap.

## HiC-seq introduction papers

_Introduction papers/tutorials of HiC-seq_

- [Comprehensive mapping of long-range interactions reveals folding principles of the human genome](http://science.sciencemag.org/content/326/5950/289) - The first paper describing HiC-seq.

- [Technical review: a Hitchhiker's guide to chromosome conformation capture. In Plant Chromatin Dynamics](https://link.springer.com/protocol/10.1007/978-1-4939-7318-7_14) - Awesome review of introducing all chromosome conformation capture assays.

- [Genome-wide mapping and analysis of chromosome architecture](https://www.nature.com/articles/nrm.2016.104#ref85) - Awesome review of HiC-seq normalisation methods and some of the TADs calling approaches.

- [A 3D map of the human genome at kilobase resolution reveals principles of chromatin looping](https://www.sciencedirect.com/science/article/pii/S0092867414014974?via%3Dihub) - Highest resolution of HiC-seq data available, and includes an awesome video explaining the 3D genome.

## License

This work is licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License](https://creativecommons.org/licenses/by-nc/4.0/).

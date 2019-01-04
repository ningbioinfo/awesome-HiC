# Awesome-HiC [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Awesome collections of HiC-seq analysing softwares

The eukaryotic genome have hierarchical three_dimensional conformation, where physical contacts between chromatin have been proved to govern the regulation of gene expression. High-resolution chromosome conformation capture sequencing (HiC-seq) has been one of the most important methods to investigate the 3D genome since its first publication in 2009\. Since then, numerous of softwares and packages have been developed to facilitate the analysis of HiC-seq data.

Here is a curated **awesome** list of HiC-seq data related softwares/packages/intro-papers that are recommended for HiC data analysis and research.

Your contributions are always welcome!

## Contents

- [Comprehensive pipelines](#Comprehensive-pipelines)
- [Toolkits](#Toolkits)
- [Mapping & Filtering](#Mapping-filtering)
- [Normalisation](#Normalisation)
- [Visualisation](#Visualisation)
- [Significant contacts identification](#Significant-contacts-identification)
- [Topologically-Associated Domains identification](#Topologically-associated-domains-identification)
- [Other awesome HiC softwares](#Other-awesome-softwares-related-to-HiC-seq)
- [HiC-seq introduction papers/tutorials](#HiC-seq-introduction-papers/tutorials)

--------------------------------------------------------------------------------

## Comprehensive pipelines

_Pipelines to process HiC-seq data from raw/trimmed data input to interactions/matrices output_

- [HiC-Pro](https://github.com/nservant/HiC-Pro) ![made-with-bash](https://img.shields.io/badge/Bash-1f425f.svg) ![made-with-python](https://img.shields.io/badge/Python-organge.svg) - It is an easy configured pipeline that can process raw data/trimmed data all the way to HiC interaction matrix, it is one of the most popular pipeline with a user-friendly documentation and it plays well with HPC.
- [Juicer](https://github.com/aidenlab/juicer) ![made-with-java](https://img.shields.io/badge/Java-yellow.svg) - It comes with a comprehensive Wiki, has a couple of other tools for downstream analysis like a browser called JuiceBox for visualisation. The performance is very fast and it plays well with HPC, but it is not designed for data with relative low resolution.

## Toolkits

_Toolkits that containing multiple tools to analyse HiC-seq data_

- [diffHiC](http://www.bioconductor.org/packages/release/bioc/html/diffHic.html) ![made-with-r](https://img.shields.io/badge/R-blue.svg) - It has a well documented user's guide and it has multiple functions for filtering, normalisation and identifying differential HiC interactions from multiple datasets. It is a R package so it can work well with lots of other R packages.
- [Homer](http://homer.ucsd.edu/homer/interactions/) ![made-with-perl](https://img.shields.io/badge/Perl-green.svg) - It recently updated a new HiC workflow, including alignment, quality control, filtering, generating interaction matrix and normalisation, identifying TADs and loops. It can also generate configure file for circos plots.
- [TADbit](https://github.com/3DGenomes/TADbit) ![made-with-python](https://img.shields.io/badge/Python-organge.svg) - It is a python library that contains multiple functions for analysing HiC data with its own TADs calling algorithm, and it has a well documented tutorial.
- [HiTC](https://bioconductor.org/packages/release/bioc/html/HiTC.html) ![made-with-r](https://img.shields.io/badge/R-blue.svg) - It is developed by the author of HiC-Pro.

## Mapping & Filtering

_Softwares/packages to conduct alignments and filtering of HiC-seq data_

- [HiCUP](https://www.bioinformatics.babraham.ac.uk/projects/hicup/) ![made-with-perl](https://img.shields.io/badge/Perl-green.svg) ![made-with-r](https://img.shields.io/badge/R-blue.svg) - It has a well documented tutorial including youtube videos, and it can generate a interactive html report as a result.
- Other mapping strategies can be found in pipelines & Toolkits.

## Normalisation

_Softwares/packages to conduct matrix normalisation of HiC-seq data_

- Explicit fashion

  - [HiCNorm](http://www.people.fas.harvard.edu/~junliu/HiCNorm/) ![made-with-r](https://img.shields.io/badge/R-blue.svg) - It is included in the HiTC R package.

- Implicit fashion

  - [Iterative Correction and Eigenvector decomposition (ICE)](https://bitbucket.org/mirnylab/hiclib) ![made-with-python](https://img.shields.io/badge/Python-organge.svg) - It is included in the HiC-Pro pipeline.

## Visualisation

_Softwares/packages to conduct visualisation of HiC-seq data_

- [JuiceBox](https://github.com/aidenlab/Juicebox) ![made-with-java](https://img.shields.io/badge/Java-yellow.svg) - It is a part of the Juicer toolkit and it can also customise multiple types of data tracks, and it can plot gene loops on heatmaps.
- [HiCPlotter](https://github.com/kcakdemir/HiCPlotter) ![made-with-python](https://img.shields.io/badge/Python-organge.svg) - It is compatible with the HiC-Pro pipeline and easy to use.
- [Sushi](https://bioconductor.org/packages/release/bioc/html/Sushi.html) ![made-with-r](https://img.shields.io/badge/R-blue.svg) - It is a R package and one of the function is to take common HiC matrix as input to plot a heatmap.
- [HiGlass](http://higlass.io/) ![made-with-web](https://img.shields.io/badge/Web-based-brown.svg) - It is a web-based browser and can also be run locally within a Docker container.

## Significant contacts identification

_Algorithms to identify significant contacts_

- [FitHiC](https://github.com/ay-lab/fithic) ![made-with-python](https://img.shields.io/badge/Python-organge.svg) - It uses a two-step spline-fitting procedure and binomial model to identify significant interactions.
- [CHiCAGO](http://regulatorygenomicsgroup.org/chicago) ![made-with-r](https://img.shields.io/badge/R-blue.svg) - This model only works for capture HiC data, it uses negative binomial random model to model read counts and uses poisson random model to model sequencing errors and artefacts.

## Topologically-Associated Domains identification

_Algorithms to identify Topologically-Associated Domains (TADs)_

- [rGMAP](https://github.com/wbaopaul/rGMAP) ![made-with-r](https://img.shields.io/badge/R-blue.svg) - It is a R package including TADs calling functions and plotting functions for visualisation, and it is able to identify sub-TADs.
- [Armatus](https://github.com/kingsfordgroup/armatus) ![made-with-cpp](https://img.shields.io/badge/Cpp-black.svg) - It has executable binaries for MacOS, Ubuntu and Linux and it is easy to use.
- [HiTAD](https://github.com/XiaoTaoWang/TADLib) ![made-with-python](https://img.shields.io/badge/Python-organge.svg) - It is a python library and has a comprehensive documentation for all the functions.
- [TopDom](http://zhoulab.usc.edu/TopDom/) ![made-with-r](https://img.shields.io/badge/R-blue.svg) - It is a R package.

## Other awesome softwares related to HiC-seq

_Other softwares/packages_

- [HiC-QC](https://github.com/ningbioinfostruggling/HiC-QC) ![made-with-python](https://img.shields.io/badge/Python-organge.svg) - QC for preliminary HiC libraries.
- [Boost-HiC](https://github.com/LeopoldC/Boost-HiC) ![made-with-python](https://img.shields.io/badge/Python-organge.svg) - HiC patterns detection from low resolution HiC data.
- [HiCPlus](https://github.com/zhangyan32/HiCPlus) ![made-with-python](https://img.shields.io/badge/Python-organge.svg) - Resolution Enhancement of HiC interaction heatmap.

## HiC-seq introduction papers/tutorials

_Introduction papers/tutorials of HiC-seq_

- [Lieberman-Aiden, E., Van Berkum, N.L., Williams, L., Imakaev, M., Ragoczy, T., Telling, A., Amit, I., Lajoie, B.R., Sabo, P.J., Dorschner, M.O. and Sandstrom, R., 2009\. **Comprehensive mapping of long-range interactions reveals folding principles of the human genome.** science, 326(5950), pp.289-293.](http://science.sciencemag.org/content/326/5950/289) - The first paper describing HiC-seq.

- [Grob, S. and Cavalli, G., 2018\. **Technical review: a Hitchhiker's guide to chromosome conformation capture. In Plant Chromatin Dynamics** (pp. 233-246). Humana Press, New York, NY.](https://link.springer.com/protocol/10.1007/978-1-4939-7318-7_14) - Awesome review of introducing all chromosome conformation capture assays.

- [Schmitt, A.D., Hu, M. and Ren, B., 2016\. **Genome-wide mapping and analysis of chromosome architecture.** Nature reviews Molecular cell biology, 17(12), p.743.](https://www.nature.com/articles/nrm.2016.104#ref85) - Awesome review of HiC-seq normalisation methods and some of the TADs calling approaches.

- [Rao, S.S., Huntley, M.H., Durand, N.C., Stamenova, E.K., Bochkov, I.D., Robinson, J.T., Sanborn, A.L., Machol, I., Omer, A.D., Lander, E.S. and Aiden, E.L., 2014\. **A 3D map of the human genome at kilobase resolution reveals principles of chromatin looping.** Cell, 159(7), pp.1665-1680.](https://www.sciencedirect.com/science/article/pii/S0092867414014974?via%3Dihub) - Highest resolution of HiC-seq data available, and includes an awesome video explaining the 3D genome.

## License

[![CC0](https://i.creativecommons.org/l/by-nc/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc/4.0/)

This work is licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License](https://creativecommons.org/licenses/by-nc/4.0/).

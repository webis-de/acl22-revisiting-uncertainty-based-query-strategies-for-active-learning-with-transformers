# Revisiting Uncertainty-based Query Strategies for Active Learning with Transformers

Accepted at ACL 2022 Findings.

## Summary

This repository contains the code to reproduce the paper 
"[Revisiting Uncertainty-based Query Strategies for Active Learning with Transformers](https://aclanthology.org/2022.findings-acl.172/)" (C. Schröder, A. Niekler and M. Potthast. 2022).

Large parts of the query strategies have been migrated into the [small-text library](https://github.com/webis-de/small-text).
Don't forget to check this out too if you're interested in active learning components *for both experiments and applications*.

## Installation

The installation is described in the [installation instructions](INSTALL.md). It is straightforward, except that 
you may need to make adjustments to install a Pytorch version that is compatible with your CUDA version.

# Usage

How to run this experiment (including configuration and inspecting obtained results)
is described in the [usage instructions](USAGE.md).

## Citation

If you wish to refer to the paper, it can be cited as follows:
```
@inproceedings{schroder-etal-2022-revisiting,
    title = "Revisiting Uncertainty-based Query Strategies for Active Learning with Transformers",
    author = {Schr{\"o}der, Christopher and Niekler, Andreas and Potthast, Martin},
    booktitle = "Findings of the Association for Computational Linguistics: ACL 2022",
    month = may,
    year = "2022",
    address = "Dublin, Ireland",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2022.findings-acl.172",
    doi = "10.18653/v1/2022.findings-acl.172",
    pages = "2194--2203",
    abstract = "Active learning is the iterative construction of a classification model through targeted labeling, enabling significant labeling cost savings. As most research on active learning has been carried out before transformer-based language models ({``}transformers{''}) became popular, despite its practical importance, comparably few papers have investigated how transformers can be combined with active learning to date. This can be attributed to the fact that using state-of-the-art query strategies for transformers induces a prohibitive runtime overhead, which effectively nullifies, or even outweighs the desired cost savings. For this reason, we revisit uncertainty-based query strategies, which had been largely outperformed before, but are particularly suited in the context of fine-tuning transformers. In an extensive evaluation, we connect transformers to experiments from previous research, assessing their performance on five widely used text classification benchmarks. For active learning with transformers, several other uncertainty-based approaches outperform the well-known prediction entropy query strategy, thereby challenging its status as most popular uncertainty baseline in active learning for text classification.",
}
```

## Acknowledgments

This research was partly funded by the Development Bank of Saxony (SAB) under project number 100335729.

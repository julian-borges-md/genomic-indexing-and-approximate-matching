# Genomic Indexing and Approximate Matching

[![Python 3.10+](https://img.shields.io/badge/python-3.10%2B-blue?style=flat-square&logo=python)](https://www.python.org/)
[![Johns Hopkins](https://img.shields.io/badge/Course-Johns_Hopkins_University-002D72?style=flat-square)](https://www.coursera.org/learn/dna-sequencing)
[![Specialization](https://img.shields.io/badge/Genomic_Data_Science-Bioinformatics-darkgreen?style=flat-square)](#)
[![ORCID](https://img.shields.io/badge/ORCID-0009--0001--9929--3135-a6ce39?style=flat-square&logo=orcid)](https://orcid.org/0009-0001-9929-3135)

> Johns Hopkins University — Genomic Data Science Specialization
> Module 2: Indexing, Boyer-Moore, and Approximate Matching
> Student: Julian Borges, MD

## Overview

Implementation of indexed and approximate matching algorithms for scalable read alignment in genomic data science. Extends Module 1's naive matching with sublinear-time indexing (Boyer-Moore, k-mer index) and pigeonhole-principle based approximate matching.

## Implemented Algorithms

| Algorithm | Description |
|---|---|
| Boyer-Moore | Bad character and good suffix rules for sublinear exact matching |
| K-mer Index | Hash-based indexing for rapid seed lookup |
| Pigeonhole Approximate Matching | Partitioned exact matching to find approximate hits |
| Subsequence Index | Subsequence-based indexing for flexible seed strategies |

## Key Concepts

- Preprocessing patterns and text for efficient search
- Trade-offs between index size, build time, and query speed
- Pigeonhole principle for reducing approximate matching to exact matching
- Benchmarking character comparisons across algorithms

## Technical Stack

`Python` · `Boyer-Moore` · `Hash Indexing` · `Algorithmic Complexity Analysis`

---

*Julian Borges, MD, MS · [ORCID](https://orcid.org/0009-0001-9929-3135) · [Academic CV](https://julian-borges-md.github.io/research-profile/)*

---

<div align="center">

**Frontier Translational Research Lab**

Department of Computer Science · Boston University · Harvard Medical School GCSRT Alumni

[![Lab Website](https://img.shields.io/badge/Lab-frontier--lab-002244?style=flat-square)](https://julian-borges-md.github.io/frontier-lab/)
[![BU CS](https://img.shields.io/badge/BU-Computer_Science-cc0000?style=flat-square)](https://www.bu.edu/cs/)
[![HMS](https://img.shields.io/badge/HMS-GCSRT_Alumni-a51c30?style=flat-square)](https://ghsm.hms.harvard.edu/education/global-clinical-scholars-research-training)
[![ORCID](https://img.shields.io/badge/ORCID-0009--0001--9929--3135-a6ce39?style=flat-square&logo=orcid&logoColor=white)](https://orcid.org/0009-0001-9929-3135)
[![CV](https://img.shields.io/badge/Academic_CV-research--profile-4f46e5?style=flat-square)](https://julian-borges-md.github.io/research-profile/)

*Julian Borges, MD, MS · jyborges@bu.edu*

</div>

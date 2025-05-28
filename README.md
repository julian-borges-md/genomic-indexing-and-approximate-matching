# Bioinformatics Module 2: Preprocessing, Indexing, and Approximate Matching  
**Specialization:** Genomic Data Science  
**Course:** Algorithms for DNA Sequencing  
**Institution:** Johns Hopkins University 
**Author:** Julian Borges (for personal documentation study)

# DNA Sequencing Algorithms – JHU Genomic Data Science Specialization

This project continues the exploration of algorithms and data structures to address the fundamental problem in genomics: **read alignment**.
So far, we’ve used naive exact matching — effective but slow, and incapable of finding approximate matches. In this module, we improve on both dimensions:

- **Speed** – via the Boyer-Moore algorithm and k-mer indexing  
- **Flexibility** – via approximate pattern matching with the pigeonhole principle


Combining Bad Character and Good Suffix Rules in Boyer-Moore
In practical applications of the Boyer-Moore algorithm, we don't rely on the bad character rule or the good suffix rule in isolation. Instead, we apply both rules simultaneously and take the maximum suggested shift from either. This approach ensures that we skip the largest number of alignments that are provably unnecessary, which significantly improves efficiency.

Rule Recap
Bad Character Rule: When a mismatch occurs, shift the pattern so that the mismatched text character aligns with its last occurrence in the pattern (if it exists). If it doesn't occur in the pattern, the pattern is shifted past the mismatched character.

Good Suffix Rule: When a mismatch follows a set of matched characters (a suffix), shift the pattern so that another occurrence of that suffix (or a compatible prefix) aligns in the pattern, or move the pattern completely past it if no match is found.

In genomic data processing, where sequences can be millions or billions of bases long, the efficiency gain from Boyer-Moore is not just theoretical—it’s essential.

## What This Project Covers

- **Boyer-Moore Algorithm**  
  Efficient preprocessing and skipping for fast exact matches
- **K-mer Index Construction**  
  Lookup tables for fast retrieval of k-length sequences in genomes
- **Ordered and Hash-Based Indexing**  
  Comparative performance analysis
- **Approximate Matching**  
  Using Hamming and Levenshtein distance
- **Pigeonhole Principle**  
  A strategy to reduce approximate matching to multiple exact matches

### Requirements

- Python 3.8+
- Jupyter Notebook (optional, for interactive exploration)
- No third-party packages required for core implementations

#### Project Structure

genomic_indexing_and_approximate_matching/
├── notebooks/
│ └── module2_analysis.ipynb # Jupyter notebook with explanations & examples
├── src/
│ ├── boyer_moore.py         # Full Boyer-Moore implementation
│ ├── kmer_index.py          # Index construction and search
│ ├── approximate_match.py   # Hamming and Edit distance functions
│ └── pigeonhole.py          # Approximate matching using pigeonhole principle
├── data/
│ └── [Optional genomic datasets]
├── tests/
│ └── [Unit tests for each algorithm]
├── requirements.txt         # Python package requirements
├── .gitignore
└── README.md                # This file

###### Disclaimer and Attribution

This repository is **not an official course resource**. All credit for the original course material goes to the instructors and creators of **Algorithms for DNA Sequencing**, offered via [Coursera](https://www.coursera.org/learn/dna-sequencing) and developed by the Johns Hopkins University.

This project is intended solely for **non-commercial, documentation and educational purposes** as part of my personal learning journey.

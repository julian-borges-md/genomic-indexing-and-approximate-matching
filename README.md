# genomic_indexing_and_approximate_matching
Bioinformatics - Genomic Data Science Specialization - The Johns Hoppkins University

This project continues the exploration of algorithms and data structures to address the fundamental problem in genomics: **read alignment**.
So far, we’ve used naive exact matching — effective but slow, and incapable of finding approximate matches. In this module, we improve on both dimensions:

- **Speed** – via the Boyer-Moore algorithm and k-mer indexing  
- **Flexibility** – via approximate pattern matching with the pigeonhole principle

The techniques here underlie real-world tools for genome-scale alignment, where both performance and tolerance for mismatches are essential.

# DNA Sequencing Algorithms – JHU Genomic Data Science Specialization

**Author:** Julian Borges MD
**Course:** Algorithms for DNA Sequencing - Module 2
**Institution:** Johns Hopkins University  

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

---

## Project Structure

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

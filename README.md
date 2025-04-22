# Compact-Math-Corpus

The **Compact Math Corpus (CM Corpus)** is a linguistically annotated dataset derived from three open-access mathematics textbooks. It was built to support research in Natural Language Processing (NLP), particularly in domain-specific understanding and reasoning tasks involving mathematical language.

## Corpus Composition

This repository includes data extracted and processed from the following textbooks:

1. **Abstract Algebra: Theory and Applications** – Tom Judson ([link](http://abstract.pugetsound.edu/))
2. **Linear Algebra** – Jim Hefferon ([link](https://hefferon.net/linearalgebra/))
3. **Discrete Mathematics: An Open Introduction** – Oscar Levin ([link](https://discrete.openmathbooks.org/))

All books are part of the [AIM Open Math Textbook Initiative](https://textbooks.aimath.org/) and are distributed under suitable open licenses.

## Linguistic Features Extracted

Each book was processed with `spaCy` using the `en_core_web_sm` model. Key outputs include:

- **CoNLL-U annotations**: Part-of-speech tags, lemmas, dependency relations.
- **Statistics**: Frequency distributions of UPOS tags and dependency labels.
- **Noun frequency lists**: High-frequency content words.
- **Adjective–Noun pairs**: To capture conceptual expressions (e.g., "normal subgroup").
- **Compound terms**: Based on syntactic dependencies and bigrams.

## Environmental Impact

To ensure low energy consumption and accessibility, we prioritized efficient tools such as `spaCy`’s small model (`en_core_web_sm`) over transformer-based alternatives. See our paper for details on the trade-offs in processing performance and output quality.

## Citation

If you use this corpus in your research, please cite: #########################

## Requirements

- Python 3.10+
- spaCy
- pandas
- tqdm
- PyMuPDF (`fitz`)
- pylatexenc

To install dependencies:

```bash
pip install -r requirements.txt

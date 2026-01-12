# arXiv-physics: A Large-Scale Physics Citation and Authorship Dataset (222k Papers)

> 🚀 **News:** This dataset has been officially adopted by **[RelBench](https://relbench.stanford.edu/datasets/rel-arxiv/)**! It serves as a core benchmark for evaluating end-to-end deep learning on relational databases.

## 📝 Introduction
**arXiv-physics** is a large-scale relational dataset curated from [arXiv](https://arxiv.org/), specifically focusing on the **Physics domain (2018-2023)**. Unlike generic text-only datasets, it is structured as a rich relational database designed for **Relational Deep Learning (RDL)**. 

It captures the complex evolution of scientific research through:
* **Citations:** Over 1.5M directed links modeling scientific influence.
* **Authorship:** Mapped paper-author relationships including ORCID identifiers.
* **Taxonomy:** Hierarchical physics categories for precise classification.
* 
## 📊 Dataset Statistics
The dataset is structured as a normalized relational database with 6 interconnected tables.

| # | Entity / Relationship | CSV File | Count | Description |
| :--- | :--- | :--- | :--- | :--- |
| 1 | **Papers** | `1Paper.csv` | 222,769 | Core metadata (Title, Abstract, Date, DOI) and the Primary Category |
| 2 | **Categories** | `2Category.csv` | 53 | Taxonomy of physics research areas |
| 3 | **Citations** | `3Citation.csv` | 1,595,687 | Directed reference links verified via Crossref API |
| 4 | **Paper-Category** | `4Paper_Category.csv` | 155,061 | Records of Secondary Categories only |
| 5 | **Authors** | `5Author.csv` | 143,691 | Unique researchers including ORCID identifiers |
| 6 | **Authorship** | `6Paper_Author.csv` | 616,585 | Many-to-many mappings between papers and authors |
| | **Total Records** | | **2,733,846** | **Total logical relational entries in the database** |

## 🏆 RelBench Integration
This dataset is a part of the **RelBench** suite. For standard tasks like `paper-citation` prediction, we recommend using the standard splits provided in the library:
- **GitHub:** [snap-stanford/relbench](https://github.com/snap-stanford/relbench)
- **Website:** [relbench.stanford.edu](https://relbench.stanford.edu/)

## 📥 Download
- **Raw Data:** [Google Drive](https://drive.google.com/drive/folders/1CfOAFXrrf6o9d5TMdlO5GHcIME4_9IZZ?usp=drive_link) .
- **Via Python:** Use `relbench.datasets.get_dataset("rel-arxiv")`.

## 🎓 Contributors
Contributed by **Tang Haiming, He Sirui, Li Mengjie, and Guo Zhimao** from the **National University of Singapore (NUS)**.

## 📜 Citation
If you use this dataset, please use the following BibTeX for proper attribution to the original authors:

```bibtex
@misc{arxiv_physics_dataset,
  author = {Tang, Haiming and He, Sirui and Li, Mengjie and Guo, Zhimao},
  title = {arXiv-physics: A Large-Scale Physics Citation and Authorship Dataset},
  year = {2024},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{[https://github.com/PKUTHM/arxiv-physics](https://github.com/PKUTHM/arxiv-physics)}}
}
```

## License
The metadata and dataset files are licensed under a [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). 

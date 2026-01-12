# arXiv-physics: A Large-Scale Physics Citation and Authorship Dataset (222k Papers)

> 🚀 **News:** This dataset has been officially adopted by **[RelBench](https://relbench.stanford.edu/datasets/rel-arxiv/)**! It serves as a core benchmark for evaluating end-to-end deep learning on relational databases.

## 📝 Introduction
**arXiv-physics** is a large-scale relational dataset curated from [arXiv](https://arxiv.org/), specifically focusing on the **Physics domain (2018-2023)**. Unlike generic text-only datasets, it is structured as a rich relational database designed for **Relational Deep Learning (RDL)**. 

It captures the complex evolution of scientific research through:
* **Citations:** Over 1.5M directed links modeling scientific influence.
* **Authorship:** Mapped paper-author relationships including ORCID identifiers.
* **Taxonomy:** Hierarchical physics categories for precise classification.

## 📊 Dataset Statistics
- **Number of papers:** 222,770
- **Number of citations:** 1,595,688
- **Number of authors:** 143,692
- **Paper-Author Relationships:** 616,586
- **Features:** arXiv_Code, Title, Abstract, Submission_Date, DOI, Name, ORCID.

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

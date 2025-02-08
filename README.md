# vs_dataset

## Overview

The dataset consists of microscopy images for developing models that predict virtual staining of biological samples.

## Original Source

This repository contains part of data from the **In Silico Labeling Dataset**:

- **Title:** In Silico Labeling Dataset  
- **Authors:** ([Original authors linked to this paper](https://doi.org/10.1016/j.cell.2018.03.040))  
- **Source:** [in-silico-labeling GitHub Repository](https://github.com/google/in-silico-labeling/blob/master/data.md)  
- **License:** [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)

This repository only contains the folders named ```scott_1_0``` corresponding to Condition A of the original dataset.
If you use this dataset in your research, you must follow the licensing requirements and properly attribute the original authors.

## Dataset structure

```bash
/vs_dataset  
  ├── train  
  │   └── scott_1_0/           # Training images  
  └── test  
      └── scott_1_0/           # Test images   
```

## How to Access the Data

To use the dataset in your project:

1. Clone this repository to your local machine.
2. Import the dataset into your machine learning framework of choice.
3. Train or evaluate your models using the dataset.

### Download via Command Line

To clone the repository and access the Cell Counting dataset:

```bash
git clone -b virtual_staining_dataset github.com/DeepTrackAI/vs_dataset
cd virtual_staining_dataset
```

---

## Attribution

This replication dataset is based on the original In Silico Labeling Dataset. When using this replication, please provide attribution as follows:

### Cite the original paper:
Christiansen E, Yang S, Ando D, Javaherian A, Skibinski G, Lipnick S, Mount E, O'Neil A, Shah K, Lee A, Goyal P, Fedus W, Poplin R, Esteva A, Berndl M, Rubin L, Nelson P, Finkbeiner S. In silico labeling: Predicting fluorescent labels in unlabeled images. Cell, 173(3): 792-803. 2018

BibTeX:

```bibtex
@article{christiansen2018isl,
  title={In silico labeling: predicting fluorescent labels in unlabeled images},
  author={CChristiansen, Eric M and Yang, Samuel J and Ando, D Michael and Javaherian, Ashkan and Skibinski, Gaia and Lipnick, Scott and Mount, Elliot and O’Neil, Alison and Shah, Kevan and Lee, Alicia K and Goyal, Piyush and Fedus, William and Poplin, Ryan and Esteva, Andre and Berndl, Marc and Rubin, Lee L and Nelson, Philip and Finkbeiner, Steven},
  journal={Cell},
  volume={173},
  number={3},
  pages={792--803},
  year={2018},
  publisher={Elsevier}
}
```

## License

This replication dataset is shared under the CC BY 4.0 License, following the original licensing terms.

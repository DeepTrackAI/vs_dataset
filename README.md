# Virtual Staining Dataset (vs_dataset)

## Overview

This DeepTrackAI repository replicates part of the **In Silico Labeling Dataset**, available from the [in-silico-labeling GitHub Repository](https://github.com/google/in-silico-labeling/blob/master/data.md) and described in [Christiansen et al, Cell, 2018](https://doi.org/10.1016/j.cell.2018.03.040).

These images were used for developing models that predict virtual staining of biological samples from brightfield images.

Out of the total dataset, this repository only contains the folders named `Rubin/scott_1_0` corresponding to human motor neurons, labeled as "Condition A" in the original dataset.  
This dataset comprises twenty-two pairs of brightfield images and their corresponding fluorescence images. Each pair includes spatially coregistered images (meaning that the brightfield and fluorescence images are matched pixel by pixel so that corresponding features appear in the same locations in both images), showcasing two fluorescent channels: Hoechst stain, which stains nuclei blue, and anti-TuJ1 stain, which stains neurons green. Notably, the brightfield images consist of a z-stack of thirteen images across different focal planes, offering a comprehensive view of the cellular structures.  
The filenames themselves include enough information to understand the contents of each image.

The dataset contains images corresponding to 25 fields of view, with 22 in the train folder and 3 in the test folder. For each field of view, a z-stack of 13 brightfield images, a fluorescence image, and the predicted fluorescence image are available.  
Each image is an RGB image with 8-bit per channel in PNG format. Brightfield images repeat the same information across all 3 channels.

- **Dataset Size**: 25 images (22 training + 3 test)
- **Image Size**: Various
- **Color**: RGB (brightfield)
- **Labels**: RGB (fluorescence)

---

## Original Source

- **Title:** In Silico Labeling Dataset  
- **Authors:** ([Original authors linked to this paper](https://doi.org/10.1016/j.cell.2018.03.040))  
- **Source:** [in-silico-labeling GitHub Repository](https://github.com/google/in-silico-labeling/blob/master/data.md)  
- **License:** [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)

If you use this dataset in your research, you must follow the licensing requirements and properly attribute the original authors.

---

## Dataset Structure

```bash
/vs_dataset  
  ├── train/          # Training images
  │               
  └── test/           # Test images        
```

## How to Access the Data

To use the dataset in your project:

1. Clone this repository to your local machine.
2. Import the dataset into your machine learning framework of choice.
3. Train or evaluate your models using the dataset.

### Download via Command Line

To clone the repository and access the dataset:

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
  author={Christiansen, Eric M and Yang, Samuel J and Ando, D Michael and Javaherian, Ashkan and Skibinski, Gaia and Lipnick, Scott and Mount, Elliot and O’Neil, Alison and Shah, Kevan and Lee, Alicia K and Goyal, Piyush and Fedus, William and Poplin, Ryan and Esteva, Andre and Berndl, Marc and Rubin, Lee L and Nelson, Philip and Finkbeiner, Steven},
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

# IF Images Croissant Dataset + DenseNet Embeddings Demo

Generate image embeddings from Croissant datasets using DenseNet and package results in RO-Crate format.

## What it does

1. Loads CM4AI immunofluorescence images from a Croissant dataset
2. Generates 1024-dimensional embeddings using pre-trained DenseNet121
3. Saves embeddings and metadata to TSV files
4. Creates an RO-Crate package for reproducible research

## Installation

```bash
pip install mlcroissant torch torchvision Pillow pandas numpy tqdm fairscape-cli
```

## Usage

1. Place `cm4ai_if_images_croissant.json` in the working directory
2. Run `jupyter notebook demo.ipynb`
3. Execute cells sequentially

## Outputs

- `./densenet_embeddings/image_embeddings.tsv` - 1024-dim embedding vectors
- `./densenet_embeddings/ro-crate-metadata.json` - Research object metadata

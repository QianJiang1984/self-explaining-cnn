# Self-Explaining Convolutional Networks via Attention Alignment with Human Saliency Maps

This repository contains the code and data-loading pipeline for our course project:

> **"Self-Explaining Convolutional Networks via Attention Alignment with Human Saliency Maps"**

The current version implements **Pair 1 (Data)**:

- Download and organize the SALICON dataset.
- Preprocess images and saliency maps.
- Provide a PyTorch `Dataset` + `DataLoader`.
- Generate sample visualizations of image / saliency / overlay.

Future work (Pair 2 and 3) will add the classification models and the attention-alignment training objective.

---

## Repository structure

```text
self_explaining_cnn/
  data/
    README.txt              # Instructions for downloading and placing SALICON
    train/
      images/               # TRAIN images (not tracked by git)
      saliency/             # TRAIN saliency maps (not tracked by git)
    val/
      images/               # VAL images
      saliency/             # VAL saliency maps
    test/
      images/               # TEST images (optional)
  samples/
    train_images.png        # Sample batch of RGB images
    train_saliency.png      # Sample batch of saliency maps (visualized)
    train_overlay.png       # Image + saliency overlay
  src/
    dataset.py              # ImageSaliencyDataset implementation
    debug_dataloader.py     # Sanity check for Dataset/DataLoader
    visualize_samples.py    # Saves sample images/saliency/overlays
  .gitignore
  README.md

# ECE 285 Homework 2

DCGAN for generating 64 x 64 RGB paintings from WikiArt. The notebook covers training, sample generation, and evaluation with FID and Inception Score.

## Run the notebook

1. Install the dependencies with `python -m pip install -r requirements.txt`. For GPU training, use a CUDA-enabled PyTorch and torchvision installation.
2. Download and extract [WikiArt](https://www.kaggle.com/datasets/steubk/wikiart) into `data/wikiart`. Set `data_dir` in the first cell if the images are in a different folder.
3. Open `ECE285_HW2.ipynb` in Jupyter and run the cells in order. The training cells run epoch 1, then resume for epochs 2 and 3. Set `run_dir` to a new folder for a fresh run.
4. Check `dcgan_results/run_01` for the checkpoints, sample grids, loss curves, and evaluation JSON. The final evaluation uses 5,000 generated images and 5,000 WikiArt images. The first evaluation downloads the pretrained Inception V3 weights.

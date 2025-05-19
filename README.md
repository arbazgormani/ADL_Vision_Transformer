# CIFAR-10 Classification with ResNet and Vision Transformers
Advanced Deep Learning project, implementation of vision transformers and cross ViT from scratch.

This project provides a PyTorch-based training pipeline for classifying CIFAR-10 images using either a standard ResNet-18 or custom Vision Transformer (ViT and CrossViT) models. It includes training, validation, testing, model checkpointing, and optional Weights & Biases (WandB) logging.

## Features

- Support for:
  - `ResNet-18` (predefined in `torchvision.models`)
  - Custom `ViT` (Vision Transformer)
  - Custom `CrossViT` (Cross-Attention Vision Transformer)
- CIFAR-10 dataset training and evaluation
- WandB logging integration
- Easy customization via command-line arguments
- Model checkpointing for best validation accuracy

## Project Structure

├── main.py # Main training script

├── vision_transformers.py # Contains ViT and CrossViT model implementations

├── utils.py # Utility functions (logging, transforms)

├── README.md # Project documentation


## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   
2. Create and activate a virtual environment (optional but recommended):
  ```bash
  python -m venv venv
  source venv/bin/activate  # On Windows: venv\Scripts\activate
  pip install torch torchvision wandb

3. Run the training script using to train resnet18 model:
  ```bash
  python main.py --model r18

4. To traing vision transformer:
  ```bash
  python main.py --model vit --epochs 20 --batch-size 128 --lr 0.001




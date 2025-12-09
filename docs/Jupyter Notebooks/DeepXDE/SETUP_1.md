## 🚀 Installation & Setup

### Option 1: Conda Environment - GPU Enabled PyTorch Backend (Recommended)
```bash
# Create and activate environment
conda create -n pytorch_xde python=3.9
conda activate pytorch_xde

# Install CUDA toolkit for GPU support
conda install -c conda-forge cudatoolkit=11.8

# Install PyTorch with CUDA 11.8
conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia

# Install remaining dependencies
pip install deepxde
pip install jupyter
conda install ipykernel
python -m ipykernel install --user --name=pytorch_xde

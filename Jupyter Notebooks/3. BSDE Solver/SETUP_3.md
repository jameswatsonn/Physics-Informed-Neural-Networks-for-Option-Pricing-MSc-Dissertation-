## 🚀 Installation & Setup

### Conda Environment - GPU Enabled TensorFlow Backend (Recommended)
```bash
# Create a new conda environment named 'tf-GPU-2' with Python 3.9
conda create --name tf-GPU-2 python=3.9

# Activate the newly created environment
conda activate tf-GPU-2

# Install NumPy version less than 2.0 via pip with forced reinstall
pip install "numpy<2" --force-reinstall

# Install CUDA Toolkit 11.2 and cuDNN 8.1.0 from conda-forge channel
conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0

# Install TensorFlow version less than 2.11 via pip
pip install "tensorflow<2.11"

# Install remaining dependencies
pip install jupyter
conda install ipykernel
python -m ipykernel install --user --name=tf-GPU-2

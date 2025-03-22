What i did to set up sam2 environment

# 1. Create a new conda environment with Python 3.10
conda create -n sam python=3.10 -y

# 2. Activate your new environment
conda activate sam

# 3. (Optional) Install PyTorch with CUDA (if you have a compatible GPU)
conda install pytorch torchvision torchaudio pytorch-cuda=12.1 -c pytorch -c nvidia -y


# 4. If you only need CPU support, use the following instead:
# conda install pytorch torchvision torchaudio cpuonly -c pytorch -y

# 5. Clone the repo and install or Install SAM2 from GitHub
git clone https://github.com/facebookresearch/sam2.git && cd sam2

pip install -e .
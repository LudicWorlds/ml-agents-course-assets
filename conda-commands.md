# Anaconda PowerShell Prompt Commands

```bash
# Create a new Conda environment with Python 3.10.12
conda create -n mlagents python=3.10.12

# Activate the environment
conda activate mlagents

# Install necessary packages
conda install numpy=1.23.5
pip3 install torch~=2.2.1 --index-url https://download.pytorch.org/whl/cu121

# Start Python to verify installation
python
import torch
import numpy
print(torch.__version__)
print(numpy.__version__)
exit()

# Clear the terminal (optional)
clear

# Change directory to ML-Agents folder
cd D:\Unity\ml-agents

# Install ML-Agents from the local source files
python -m pip install ./ml-agents-envs
python -m pip install ./ml-agents

# Check ML-Agents installation
mlagents-learn --help

# Start a training session for the Basic environment
mlagents-learn config/ppo/Basic.yaml --run-id=run1

# Force overwrite or resume previous run
mlagents-learn config/ppo/Basic.yaml --run-id=run1 --force
mlagents-learn config/ppo/Basic.yaml --run-id=run1 --resume
```

## Other Useful Commands

```bash
# Install PyTorch with CPU-only support (without CUDA)
pip3 install torch~=2.2.1 --index-url https://download.pytorch.org/whl/cpu

# Deactivate the current Conda environment
conda deactivate

# Remove a Conda environment and all its packages (replace "mlagents" with your environment name)
conda remove --name mlagents --all

# List all Conda environments available on your system
conda env list

# Display Conda environment information, including all available environments
conda info --envs
```

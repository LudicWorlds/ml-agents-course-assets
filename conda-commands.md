# Anaconda PowerShell Prompt Commands

conda create -n mlagents python=3.10.12
conda activate mlagents

conda install numpy=1.23.5
pip3 install torch~=2.2.1 --index-url https://download.pytorch.org/whl/cu121

python
import torch
import numpy
print(torch.__version__)
print(numpy.__version__)
exit()

clear

cd D:\Unity\ml-agents
python -m pip install ./ml-agents-envs
python -m pip install ./ml-agents

mlagents-learn --help
mlagents-learn config/ppo/Basic.yaml --run-id=run1

mlagents-learn config/ppo/Basic.yaml --run-id=run1 --force
mlagents-learn config/ppo/Basic.yaml --run-id=run1 --resume

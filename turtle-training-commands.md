# 'Turtle Agent' Training Commands

To train the 'TurtleAgent', launch the 'Anaconda PowerShell Prompt', and use the following commands:

```bash
# 1. Activate the environment
# NOTE: the environment should have been created in Part 1 of the tutorial series.
conda activate mlagents

# 2. Change directory to your 'Turtle Agent' Unity project folder
cd "D:\Unity\Turtle Agent"

# 3. Check ML-Agents installation
mlagents-learn --help

# 4. Run a training session
mlagents-learn --run-id=turtle1

# Force overwrite or resume previous run
mlagents-learn --run-id=turtle1 --force
mlagents-learn --run-id=turtle1 --resume
```
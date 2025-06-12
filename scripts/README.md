# RL-Optimised HVAC Control – Supplementary Package

This repository reproduces all experiments from  
**“Optimizing HVAC Energy Efficiency in Low-Energy Buildings:  
A Comparative Analysis of Reinforcement-Learning Control Strategies under Tehran Climate Conditions.”**

## Quick start
```bash
git clone https://github.com/your-org/hvac-rl-supplement.git
cd hvac-rl-supplement
conda env create -f environment.yml     # or mamba env create …
conda activate hvac_rl
git lfs pull                             # downloads heavy data
python scripts/train_rl.py --config configs/rl_config.yaml

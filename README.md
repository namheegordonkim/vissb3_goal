# Embodied AI Seminar: Goal-Driven Control and Curriculum Learning

## Installation

NOTE: if you already have last week's environment set up, you may not need to do any of the installation steps.

### Create a conda environment

```
conda create -y -n vissb3 python=3.10
conda activate vissb3
```

### Install JAX

Make sure to run this ***BEFORE*** other dependencies.

```
pip install jax[cuda12]
```

### Install other dependencies

Then install the requirements.

```
pip install -r requirements.txt
```

### Unlink the default installs

We will use a "poor man's fork" method and directly use `imitation`, `stable-baselines3`, and `brax` codebases as submodules. To avoid conflicts, we need to unlink the default installs.

```
pip uninstall -y imitation stable-baselines3 brax
```

### Run the code

Ensure that you can run the following command without any errors:

```
python enjoy_goal.py
```
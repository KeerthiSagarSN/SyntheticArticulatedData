# SyntheticArticulatedData
Procedurally generated articulated objects specified in Universal Robot Description Format (URDF), and rendered using Mujoco.

# Mujoco

Installation Steps here:
a. Download binaries and create a folder with name ".mujoco"
b. Place the mujoco210 folder into the previous folder
c. pip install mujoco-py
https://github.com/openai/mujoco-py?tab=readme-ov-file#install-mujoco

Setup:
```pip install -r requirements.txt```

Example generation:
```python3 generate_data.py --n 10 --dir ./test --obj microwave --masked --debug```

# PyBullet

Setup:
```pip install -r requirements-bullet.txt```

Example generation:
```python3 generate_data.py --n 10 --dir ./test --obj microwave --masked --debug --py-bullet```

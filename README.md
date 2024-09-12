# SyntheticArticulatedData
Procedurally generated articulated objects specified in Universal Robot Description Format (URDF), and rendered using Mujoco.


# Dependencies
a. pytorch (pip install torch)<br>
b. pyro (pip3 install pyro-ppl)<br>

# Mujoco

Installation Steps here:<br>
a. Download binaries and create a folder with name ".mujoco"<br>
b. Place the mujoco210 folder into the previous folder<br>
c. pip install mujoco-py<br>
https://github.com/openai/mujoco-py?tab=readme-ov-file#install-mujoco<br>

Please add following line to .bashrc:<br>
export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/home/YOUR_PC/.mujoco/mujoco210/bin<br>


Setup:
```pip install -r requirements.txt```

Example generation:
```python3 generate_data.py --n 10 --dir ./test --obj microwave --masked --debug```

Issues can be sorted by using this thread:<br>
https://github.com/openai/mujoco-py/issues/707

# PyBullet

Setup:
```pip install -r requirements-bullet.txt```

Example generation:
```python3 generate_data.py --n 10 --dir ./test --obj microwave --masked --debug --py-bullet```

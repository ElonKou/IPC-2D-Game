# Incremental Potential Contact (IPC) based 2D GAME

`Attention`: Thanks for XunZhan's great work, the [XunZhan version](https://github.com/XunZhan/IPC-2D-Game/fork) only compiles code succeed on old version of taichi(<= 0.7.31) and also doesn't match Mac M1, this version only fixed taichi-language bug.

## Install instruction
```bash
# download new verison taichi and run the code.
pip install taichi
python3 ipc2d.py
```

## Project Information
Incremental Potential Contact (hereinafter referred to as IPC), is the paper of SIGGRAPH 2020 and its simulation effect is very accurate and stable, which is worthy of in-depth understanding and research. However, the IPC source code is based on C + + and has many dependencies and puts emphasis on performance optimization. This results in a complex procedure for building up the environment and makes it difficult for beginners to learn. Therefore, this project uses Taichi programming language to realize the 2D IPC algorithm. And by using the TowerBlock style game, the accuracy of the algorithm is realized and verified.

## Features
- Implicit time step for calculating object trajectory and the system prevents intersection and reversal
- System Incremental Potential consists of: elastic potential energy, kinetic energy, gravitational potential energy and barrier potential energy
- Realize Barrier-augmented IP, use CCD to accelerate and avoid intersection
- System dynamically manages the included objects  


## Result
<img src="result.gif" width="300"  />  


## References

- [FEM Explicit Method](https://github.com/YuCrazing/Taichi/tree/master/fem_3d)
- [Incremental Potential Contact: Intersection - and Inversion - free, Large - Deformation Dynamics](https://ipc-sim.github.io)

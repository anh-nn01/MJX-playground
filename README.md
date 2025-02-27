# MJX-playground
Playground for MJX differentiable environments.


Test cases:
1. Basic shapes
2. MuJoCo reacher
3. MuJoCo Ant
4. SawyerXYZ (Meta-World)


## Potential errors, causes, and solutions:
1. `NotImplementedError: (mjtGeom.mjGEOM_CYLINDER, mjtGeom.mjGEOM_BOX) collisions not implemented.` <br>
   $\rightarrow$ <b> Cause </b>: The problem is because of MJX unimplemented collision handling of the `CYLINDER` and `BOX` geometries. <br>
   $\rightarrow$<b> Solution </b>: replace all geom `cylinder` with `capsule`
   

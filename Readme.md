In this exercise for the course Computational Models of Motion at ETH, we implemented FEM solver for a soft rigid body. The rigid body is controlled by pins at both ends and a minimum energy and force optimizer is implemented to achieve equilibrium state. A total energy objective is defined and minimized using Newtons method (second order Hessian method) for equilibrium conditions.  

# FEM, Soft Manipulation, and Control

Please find the assignment write-up on the course webpage or at the following link:
![Assignment Write-up](https://github.com/maturk/FEM_Soft_Body_Simulation/blob/master/CMM_SoftManipulation.pdf)

First demp illustrates the FEM solver at equilibrium for varying pin locations. Internal forces and energy within the mesh are minimized at equilibrium states. 

![FEM demo](https://user-images.githubusercontent.com/30566358/173822368-aaa0f918-eab2-4e27-ad4b-0f428836eb8c.gif)

The second demo illustrates how control of the soft body works. When the pin locations are moved, the soft body assumes minimum energy configuration. 

![Manipulator demo](https://user-images.githubusercontent.com/30566358/173823410-cdefbc59-55db-433d-8d75-7853459a5136.gif)

See code for implementation... 

---

Could use ./build.sh on Linux/MacOS

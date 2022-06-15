First Name: Matias
Last Name:  Turkulainen

Solution to Question 4: 

Please check exercise4IMG.pdf for proof of exercise 4.

![Exercise 4 proof](https://github.com/CMM-22/a4-maturk/blob/master/exercise4IMG.pdf)

Solution to Question 10:

Looking at the source code, optimization is done with GradientDescentLineSearch. If the optimization loss / cost function is non-convex, multiple solutions can exist if there are multiple local minima. The optimizer finds the first solution using gradient descent, and since the loss is at a local minimum here, it gets "stuck" and no longer updates the pose/controller.

Solution to Question 11:

A simple regularizer (often used in machine learning tasks) is the ridge regularizer along with the original L2 loss function (O). Since we desire the rotational components of the end pins to be vertical (i.e. at 90 degrees), I implement the ridge regularizer on the theta Left and theta Right components of U vector. I penalize angles that are not equal to 90 degrees with the following ridge regularizer:

regularizer = lambda *((u(theta_L)-90)^2 + (u(theta_R)-90)^2)

See code for implementation... 


Please find the assignment write-up on the course webpage.

---

Could use ./build.sh on Linux/MacOS

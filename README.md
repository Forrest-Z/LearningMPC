# LearningMPC
Learning based Model Prodictive Control for online iterative trajectory optimization for the F1/10 car 

The car is learning to improve its racing performance iteratively over laps.

Initial Sample Safe Set (Lap 1 and Lap 2) is collected using a PID path following controller.

Starting from Lap 3, control policies are generated by learning MPC. The MPC enforces the terminal state to be within a convex hull of a selected subset of samples. The sample safe set continously grows as more and more data is being collected along the way. The improvement of racing performance over laps is shown here below.

Lap 5 (Top speed 1.2 m/s)

![](media/lap5.gif)

Lap 25 (Top speed 3 m/s)

![](media/lap25.gif)

After Lap 60, it converges to an optimal policy (racing line and spped profile)

![](media/lap50.gif)


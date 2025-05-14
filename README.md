# Classical-Mechanics-Activity
In this project, I created a Mathematica notebook to simulate the motion of a particle under the influence of gravity in three different environments: vacuum, a gradual atmosphere, and an Earth-like atmosphere. The goal was to compare how air resistance affects the particle’s trajectory over time.

First, I set up the physical parameters — like mass, gravity, and initial velocities — and defined the drag coefficients for the two types of atmospheric resistance: linear and quadratic. The vacuum case is the simplest, since the particle only experiences gravity, so I used basic kinematics equations to describe its motion.

For the linear drag case, I used the known analytical solution for motion with a velocity-proportional drag force. The equations show how both horizontal and vertical velocities decrease exponentially due to the air resistance.

The quadratic drag case was more complex because it requires solving differential equations numerically. I used NDSolve in Mathematica to compute the motion over time, since there’s no simple analytical solution in this case. I also calculated the total velocity at each time step to apply the correct magnitude of the drag force.

Then I plotted the position components (x, y, z) over time for all three cases, both separately and in 3D. This helped visualize how the trajectory gets shorter and more curved as the drag force increases.

I also included plots for the kinetic, potential, and total mechanical energy to show how energy behaves in each case. In the vacuum case, the total energy stays constant, but with drag forces, the total energy decreases because some of it is dissipated by the air.

Finally, I made sure the numerical solutions were stable and accurate, especially in the quadratic drag case, by using careful settings in NDSolve and FindRoot.

Overall, this simulation helped me understand the impact of air resistance on projectile motion and how to model physical systems both analytically and numerically using Mathematica.

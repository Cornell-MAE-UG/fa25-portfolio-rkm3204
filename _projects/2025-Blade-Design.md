---
layout: project
title: MAE 4272 Wind Turbine Blade Design
description: Advanced CAD Project
technologies: [SolidWorks, MATLAB]
image: /assets/images/BigBlue.jpg
---

For MAE 4272, a lab-based class aimed to synthesize heat trasnfer and fluid mechanics, groups of students were tasked with designing a blade for a small-scale wind turbine experiment. The goal was to maximize aerodynamic power extraction while satisfying strict safety and operational constraints, including fixed rotor hardware, limited power dissipation, and a constant-angular-velocity operating requirement. This project emphasized applying aerodynamic theory to a realistic engineering system and validating predictions through experimental testing.

![Shaded rendering of earlier version]({{ "/assets/images/BladeDimensions.png" | relative_url }}){: .inline-image-r style="width: 400px"}

The blade was designed using blade element momentum (BEM) theory to target a specific tip-speed ratio and operating condition. Key design decisions included selecting a low-Reynolds-number airfoil (Selig 7075), implementing a tapered chord distribution, and applying a significant spanwise twist to maintain a near-optimal angle of attack along the blade. Prandtl tip-loss corrections were incorporated into the analytical model, and structural calculations were performed to verify that bending stresses at the blade root remained below material limits at the maximum allowable rotational speed. A MATLAB-based analysis tool was developed to predict power output and coefficient of performance prior to fabrication.

The fabricated blade was tested in the Big Blue wind tunnel using controlled torque-brake sweeps at multiple wind speeds. During testing, rotational speed, torque, and wind speed were recorded to generate full power curves and compute performance metrics such as mechanical power and coefficient of performance. The blade operated stably and safely across all test conditions, producing repeatable power curves with the expected characteristic behavior. Measured performance was lower than idealized model predictions, highlighting the impact of real-world losses such as tip effects, low-Reynolds-number aerodynamics, and manufacturing tolerances.

Below is a depiction of the resulting Coefficient of Power curves as a function of tip speed ratio:

![Photo of old radio]({{ "/assets/images/CpCurves.png" | relative_url }}){: .inline-image-l}

On an individual contribution level, I spearheaded modeling and post-processing analysis of the blade. Once other team members had determined the optimal blade geometry, I utilized SolidWorks to model the blade, projecting Selig 7075 airfoils onto rotated planes and lofting the sketches. Modeling this required close attention to the sizing constraints provided by course staff, ensuring that the blade would operate safely in the wind tunnel dimensions. A dimensioned depiction of this CAD model can be seen above in grey. After producing the design model, we continued to 3D print and test the blade. I assisted with experimental testing, operating the wind tunnel frequency to the outlined specifications. After experimentation, I formulated a MATLAB script to process the power output gained from the torque-sweeps. This helped the team visualize the performance of our blade, as we took to visualize the power outputs as a function of our experimental inputs. 
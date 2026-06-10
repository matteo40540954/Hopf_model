The main aim of our project was to generate virtual brains that emulates the altered connectivity of schizofrenic patients visual areas. Specifically, we wanted to investigate whether the visual areas of people with schizophrenia have a different bifurcation parameter compared to healthy controls.

To achieve this, we: 

1) Defined a control baseline: We used real MRI data to find the optimal bifurcation parameter that best describes a healthy population, using an evolutionary algorithm. We selected a = 0.175.
2) Localized simulation of the visual cortex: We chose the optimal bifurcation parameter that best describes patients' visual areas. We selected a = 0.453.
3) Patient vs. control comparison: A t-test was computed to compare patients' virtual brains against healthy virtual brains. 

THE HOPF MODEL 

For the class "Computational Neurology", we used a Hopf model. In this model, every brain region is modelled as an oscillator, and a bifurcation parameter "a" describes its oscillatory behavior: 

- If a < 0, Stable activity. If noise perturbs the oscillator, a small wave may appear but quickly dies out.
- If a > 0, Self-sustained oscillation. The brain region produces continuous oscillations on its own.
- If a = 0, The bifurcation point, sitting exactly between stability and sustained oscillation.

EVOLUTIONARY ALGORITHM 

To find the optimal bifurcation parameter for patients, we used an evolutionary algorithm. 
The process works as follows:

1) Random parameters are assigned to generate virtual brains.
2) These virtual brains are compared against real healthy MRI data.
3) Only the "fittest" virtual brains (those whose parameters most closely resemble the real MRI data) are selected.
4) The selected models produce "offspring," with small mutations introduced to slightly modify their parameters.
5) This selection process runs for 90 generations, after which the optimal parameters are identified.
 





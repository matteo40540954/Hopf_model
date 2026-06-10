In this project for the class "Computational Neurology" we use a Hopf model. 
According to this model every brain region is modelled as an oscillator and a parameter (e.g., the bifurcation parameter "a")
describes its oscillation. 
- If a < 0, there is a "stable" activity. In this state if noise hits our oscillator, it might show a tiny wave, but the wave quickly dies out.
- If a > 0, the brain becomes a self sustained oscillator. It produces continous oscillations on its own.
- If a = 0, bifurcation point between stability and sustained oscillation.  

The main aim of our project was to generate a virtual brain that emulates the altered connectivity of schizofrenic patients visual areas. In particular we want to 
investigate wether the visual areas of people with schizophrenia have a different bifurcation parameter compared to healthy control. 
In order to achieve this aim we: 

1) defined a control baseline: we used real  MRI data to find the optimal bifurcation parameter that best describes healthy poplulation using an evolutionary algorithm. The evolutionary alghorithm sets random parameters to generate virual brains and compares them against the healthy real data and in the end selects only the fittest, so the parameters of the virtual brains who resemble more the mri real data are selected. then these models haev their offsprings and some mutations are introduced, so the parameters are slightly modified and then selection continues for 90 generations and at the end we have the optimal parameters are selected (a= 0.175).
2) localized simulation of visual cortex:choose the optimal bifurcation parameter that best describes patients visual areas (a=0.453).  
3) patient Vs control: a t-test is computed to compare patients virual brains and healthy virtual brains.
4) 
...  

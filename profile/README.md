# Introduction to Wide-Angle-Team (WAT)

## What is WAT?

This is a github organization that contains theory and estimator code that are used for SPHEREx, but also are often used for other research projects, such as exploratory projects that are not 
officially part of the SPHEREx pipeline yet, as well as student projects. It is outside of the SPHEREx Github organization, which has stricter access control. 

## Repo organizations 

[A description of various repos go here]

[Questions to answer
1. Log-normal simulations + estimators: how they are connected to other repos in here
2. SFB code: what are the different SFB code? Theory code, estimator code? 
3. Which repos are obsolete, LogNormalSimulations is a continuation of some other repo?
4. Julia registry repo and how it's used? How and which repo is connected to the SPHEREx Pipeline.
5. Which repos are experimental and decoupled from the pipeline (e.g. SURF2024Window for Dennis Wu's SURF project).
]

## Entry Points

### Log-normal simulations + estimators

If you want to generate log-normal simulations and apply a power spectrum (or potentially a bispectrum estimator) to it, read this section. 

The code is written in julia, available here: https://github.com/Wide-Angle-Team/LogNormalSimulations
The README should be fairly self-explanatory, but may very well be incomplete (See sample yaml files for configuration files and available settings).
It mainly makes use of two packages: `LogNormalGalaxies.jl` and `MeasurePowerSpectra.jl`. They are both in the Wide-Angle-Team organization on github. With any luck, you will not need to interact directly with them, only with LogNormalSimulations.


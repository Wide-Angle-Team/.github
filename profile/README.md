# Introduction to Wide-Angle-Team (WAT)

## What is WAT?

This is a github organization that contains theory and estimator code that are used for SPHEREx, but also are often used for other research projects, such as exploratory projects that are not 
officially part of the SPHEREx pipeline yet, as well as student projects. It is outside of the SPHEREx Github organization, which has stricter access control. 

## Repo organizations 

There are essentially two types of repos: projects and packages.

All Julia packages end in `.jl` and projects don't.

### Packages
Julia packages end in `.jl`, they get registered in the `WATCosmologyJuliaRegistry` as a Julia registry so that it is convenient to use in projects. A Julia registry is similar to a conda channel. The most up-to-date documentation how to use the registry is in [LogNormalSimulations](https://github.com/Wide-Angle-Team/LogNormalSimulations).

`WATCosmologyJuliaLib` is a repo that contains several packages. Each subdirectory is its own Julia package. We combine them in one repo so as not to pollute the github organization. They individually registered in the `WATCosmologyJuliaRegistry`.

SFB code: Estimator code lives in `SphericalFourierBesselDecompositions-dev` and the public version in [SphericalFourierBesselDecompositions.jl](https://github.com/hsgg/SphericalFourierBesselDecompositions.jl), the theory code lives in `WATCosmologyJuliaLib/SFBPsiPhiModels`.

### Projects
These repos bring together several packages to run code and make plots for papers.

The most important one is `LogNormalSimulations` that connects the `LogNormalGalaxies.jl` code with the `MeasurePowerSpectra.jl` code, and it is used to run a bunch of such simulations.


## Entry Points

### Log-normal simulations + estimators

If you want to generate log-normal simulations and apply a power spectrum (or potentially a bispectrum estimator) to it, read this section. 

The code is written in julia, available here: [LogNormalSimulations](https://github.com/Wide-Angle-Team/LogNormalSimulations). 
The README should be fairly self-explanatory, but may very well be incomplete (See sample yaml files for configuration files and available settings).
It mainly makes use of two packages: [LogNormalGalaxies.jl](https://github.com/Wide-Angle-Team/LogNormalGalaxies.jl) and [MeasurePowerSpectra.jl](https://github.com/Wide-Angle-Team/MeasurePowerSpectra.jl). They are both in the Wide-Angle-Team organization on github. You should not need to interact directly with them, only with LogNormalSimulations.


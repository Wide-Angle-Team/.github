# Introduction to Wide-Angle-Team (WAT)

## What is WAT?

This is a github organization that contains theory and estimator code that are used for SPHEREx, but also are often used for other research projects, such as exploratory projects that are not 
officially part of the SPHEREx pipeline yet, as well as student projects. It is outside of the SPHEREx Github organization, which has stricter access control. 

## Repo organizations 

There are essentially two types of repos: Projects and Packages. 

Projects don't end with '.jl', while julia packages do (with some exceptions like `WATCosmologyJuliaLib` and `WATCosmologyJuliaRegistry`). 

### Packages
- All repos for Julia packages end in `.jl`. 
- `WATCosmologyJuliaLib`: A repo that contains several packages. Each subdirectory is its own Julia package. We combine them in one repo so as not to pollute the github organization.
- `WATCosmologyJuliaRegistry`: It registers the julia packages for easy installation as a Julia registry, so that it is convenient to use in projects. A Julia registry is similar to a conda channel.

The most up-to-date documentation on how to use the registry is in [LogNormalSimulations](https://github.com/Wide-Angle-Team/LogNormalSimulations).

SFB code: The estimator code lives in `SphericalFourierBesselDecompositions-dev` (this doesn't end in .jl yet since it's dev mode) and the public version in [SphericalFourierBesselDecompositions.jl](https://github.com/hsgg/SphericalFourierBesselDecompositions.jl), the theory code lives in `WATCosmologyJuliaLib/SFBPsiPhiModels`.

### Projects
Repos that don't end with '.jl' are usually individual project repos. These repos bring together several packages to run code and make plots for papers.

The most important one is `LogNormalSimulations` that connects the `LogNormalGalaxies.jl` code with the `MeasurePowerSpectra.jl` code, and it is used to run a bunch of such simulations. 


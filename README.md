# JGR2022

This repo contains the synthetic catalogs from simulations in the following paper:

- Shi, P., Wei, M., & Barbot, S. (2022). Contribution of Viscoelastic Stress to the Synchronization of Earthquake Cycles on Oceanic Transform Faults, Journal of Geophysical Research: Solid Earth


## Naming

- `w{x}`: barrier width (km)
- `ic{x}`: initial offset **C_{right}** in elastic models
- `icsync`, `icoffset`: synchronized/offset initial condition in viscoelastic models
- `dis{x}`: dislocation creep coefficient amplifier
- `dif{x}`: diffusion creep coefficient amplifer
- `eta{x}`: uniform linear viscosity (Pa s)
- `bgs{x}`: background strain rate under dislocation creep (1/s)
- `gs{x}`: grid size (m); *250 m* if without


## Contents

Each catalog JSON file has the following fields:

- `t`: time step corresponding `maxv` or `maxdϵ`
- `t1`: initial time of earthquakes in the *left* asperity
- `t2`: initial time of earthquakes in the *right* asperity
- `mw1`: moment magnitude of earthquakes in the *left* asperity
- `mw2`: moment magnitude of earthquakes in the *right* asperity
- `maxv1`: maximum slip velocity in the *left* asperity
- `maxv2`: maximum slip velocity in the *right* asperity
- `maxdϵ`: maximum strain rate norm in the mantle


## Other links

- [Simulation software](https://github.com/shipengcheng1230/Oetqf.jl)

- [To retrieve catalog based on slip velocity threshold](https://github.com/shipengcheng1230/Quaycle-Elastic.jl/blob/master/JGR2020/scripts/scanfunc.jl)
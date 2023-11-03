@def title = "Numerical Engine Room Talks"
@def tags = ["syntax", "code"]

# Numerical Engine Room Talks

<!--\fig{Numerical engine room}{assets/numerical\_engine\_room.png}-->
<!--![Numerical engine room](/assets/numerical\_engine\_room.png)-->
~~~
<div style="text-align:center;">
<img src="/assets/numerical-engine-room.png" style="width: 30%; padding: 0; margin: 0"/>
</div>
~~~

The *Numerical Engine Room Talks* are an interdisciplinary seminar series at the
intersection of numerical methods, algorithm development, and high-performance
computing. A particular focus in these talks is on the internals of the
"numerical engine room", i.e., on details such as implementation notes,
performance numbers, or specific corner cases. We invite our guest speakers
and the audience to engage in discussions at this level, to facilitate a
scientific exchange that goes beyond the polished results found in the
literature.

We host the Numerical Engine Room Talks on a semi-regular basis, approximately
once every month or two, via Zoom. If you are interested, please send an email to
[Michael](mailto:m.schlottke-lakemper@acom.rwth-aachen.de)
to be included in the regular announcement email.

Michael Schlottke-Lakemper, [RWTH Aachen University](https://lakemper.eu)\\
Gregor Gassner, [University of Cologne](https://www.mi.uni-koeln.de/NumSim)\\
Hendrik Ranocha, [Johannes Gutenberg University Mainz](https://ranocha.de)

---
[Arpit Babbar](https://www.math.tifrbng.res.in/people/arpit) (TIFR-CAM),
[Praveen Chandrashekar](http://cpraveen.github.io/) (TIFR-CAM)\\
**TrixiLW.jl: A high-order, single stage hyperbolic PDE solver using [Trixi.jl](https://github.com/trixi-framework/Trixi.jl/)**\\
*Friday, 13th November 2023, 1:00 PM CET*\\

TrixiLW.jl is a Lax-Wendroff (LW) PDE solver that accomplishes high-order accuracy
by doing a coupled temporal and spatial discretization in contrast to the method of lines
approach like that of [Trixi.jl](https://github.com/trixi-framework/Trixi.jl),
where a multi-stage ODE solver is used for temporal discretization following the
high-order spatial discretization. Lax-Wendroff (LW) schemes are friendly to the
modern memory-bound CPU as they evolve to the next time level in a single stage,
minimizing communication from RAM to cache in case of serial code and across nodes
in case of a parallel code.
Tenkai.jl is the Cartesian LW code used in our
[first](https://www.sciencedirect.com/science/article/pii/S0021999122004855) and 
[second](https://arxiv.org/abs/2305.10781) paper, which took design and optimization
inspiration from [Trixi.jl](https://github.com/trixi-framework/Trixi.jl). 
TrixiLW.jl was subsequently written to extend the LW discretization to curvilinear
grids using [Trixi.jl](https://github.com/trixi-framework/Trixi.jl) as a library.
The talk will begin by briefly discussing the optimization lessons Tenkai.jl took from
[Trixi.jl](https://github.com/trixi-framework/Trixi.jl) and then focus on how we
exploited Julia's multiple dispatch along with the modularity and generality of
[Trixi.jl](https://github.com/trixi-framework/Trixi.jl) to write TrixiLW.jl.

---
*[Benjamin Uekermann](https://github.com/uekerman) (University of Stuttgart)*\\
**preCICE – A General-Purpose Simulation Coupling Interface**\\
*Friday, 21st April 2023, 11am CET*\\

[preCICE](https://precice.org/) is an open-source coupling software for
partitioned multi-physics and multi-scale simulations. Thanks to the software's
library approach (the simulations call the coupling) and its high-level API,
only minimally-invasive changes are required to prepare an existing
(legacy) simulation software for coupling. Moreover, ready-to-use
adapters for many popular simulation software packages are available,
e.g. for OpenFOAM, SU2, CalculiX, FEniCS, and deal.II. For the actual
coupling, preCICE offers methods for fixed-point acceleration
(quasi-Newton acceleration), fully parallel communication (MPI or
TCP/IP), data mapping (radial-basis function interpolation), and
time interpolation (waveform relaxation). Today, although being an
academic software project at heart, preCICE is used by more than 100
research groups in both academia and industry.

---
*[Valentin Churavy](https://vchuravy.dev/) (MIT)*\\
**Compiler based automatic differentiation for scientific programs**\\
*Friday, 16th December 2022, 10am CET*\\

Automatic differentiation is a powerful technique in numerical computing. In this talk
we will explore the tradeoffs of implementing AD on different levels, and discuss automatic
differentiation for parallel programs and high-level programming languages. The particular
focus will be on Enzyme an AD framework that operates on the compiler level and supports
reverse and forward mode AD in a variety of languages such as Julia, C/C++, Fortran and others.

This talk is based on the paper "Scalable Automatic Differentiation of Multiple Parallel
Paradigms through Compiler Augmentation" by Moses et al. ([PDF](https://www.computer.org/csdl/proceedings-article/sc/2022/544400a859/1I0bT5ygZby), Winner of the Best Student Paper Award at SC22).

---
*[Deniz Bezgin](https://www.epc.ed.tum.de/aer/mitarbeiter-innen/cv-2/a-d/m-sc-deniz-bezgin/) (TU Munich), [Aaron Buhendwa](https://www.epc.ed.tum.de/aer/mitarbeiter-innen/cv-2/a-d/m-sc-aaron-buhendwa/) (TU Munich)*\\
**Differentiable Fluid Dynamics in JAX: Challenges and Perspectives**\\
*Friday, 26th August 2022, 10am CEST*\\

JAX-FLUIDS is a CFD solver written in Python, which uses the JAX framework to
enable automatic differentiation (AD). This allows one to easily create
applications for data-driven simulations or other optimization problems. The
talk is based on the recent preprint "JAX-FLUIDS: A fully-differentiable
high-order computational fluid dynamics solver for compressible two-phase
flows" [arXiv:2203.13760](https://arxiv.org/abs/2203.13760).

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
Hendrik Ranocha, [University of Hamburg](https://ranocha.de)

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

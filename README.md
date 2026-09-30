# Kartikeya Gangwar

Undergraduate Researcher in **Computational Mathematics & Scientific Machine Learning** at the Department of Mathematics, University of Delhi. *(Official / Academic Documents: Kartikey Singh)*.

Investigating the intersection of **geometric deep learning**, **numerical PDEs**, **high-dimensional stochastic control**, and **high-performance scientific computing**. Research emphasizes exact mathematical invariants (symplectic conservation, parameter null-space decoupling, hard boundary constraints) and bare-metal computational efficiency.

[![Portfolio](https://img.shields.io/badge/Portfolio-kartikeyagangwar.github.io-0284c7?style=flat-square&logo=google-chrome&logoColor=white)](https://kartikeyagangwar.github.io)
[![ORCID](https://img.shields.io/badge/ORCID-0009--0009--1973--7532-a6ce39?style=flat-square&logo=orcid&logoColor=white)](https://orcid.org/0009-0009-1973-7532)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-kartikey--singh-0077b5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kartikey-singh-2a3434329/)
[![Email](https://img.shields.io/badge/Email-kartikeysingh525%40protonmail.com-6d4aff?style=flat-square&logo=protonmail&logoColor=white)](mailto:kartikeysingh525@protonmail.com)
[![Zenodo](https://img.shields.io/badge/Zenodo-Preprints_%26_Datasets-0052cc?style=flat-square&logo=zenodo&logoColor=white)](https://zenodo.org/search?q=metadata.creators.person_or_org.name%3A%22Singh%2C%20Kartikey%22)

---

## Research Projects & Open-Source Code

### Scientific Machine Learning & Geometric Systems
- **[cpa-shnn](https://github.com/KartikeyaGangwar/cpa-shnn)** — Symplectic Hamiltonian Neural Networks for multi-body celestial mechanics. Formulates separable kinetic-Coriolis splitting and Arnold extended contact phase spaces across 6 chaotic gravitational systems, achieving up to $126.4\times$ Fourier error collapse.
- **[eit-neural-surrogate-inversion](https://github.com/KartikeyaGangwar/eit-neural-surrogate-inversion)** — Deep shape inversion in Electrical Impedance Tomography (EIT). Resolves Calderón logarithmic ill-posedness via stochastic directional JVP supervision on $\mathbb{S}^{63}$, bounding peak VRAM to $342.8\,\mathrm{MB}$ with a $56.8\times$ wall-clock speedup. *(Under review at IEEE Transactions on Computational Imaging; [DOI: 10.5281/zenodo.22096368](https://doi.org/10.5281/zenodo.22096368))*.
- **[pinn-fluid-formulations](https://github.com/KartikeyaGangwar/pinn-fluid-formulations)** — Formulation-induced failure modes in high-$Re$ incompressible fluid PINNs. Analyzes operator diffusion in continuous $\psi-\omega$ representations due to absence of discrete Thom stencils, and proves Helmholtz-Hodge projection recovery in $\psi-p$. *(Under review at Physics of Fluids; [DOI: 10.5281/zenodo.22979276](https://doi.org/10.5281/zenodo.22979276))*.

### The Adaptive Subspace (AS) Optimization Paradigm
- **[as-pinn](https://github.com/KartikeyaGangwar/as-pinn)** — Adaptive $N$-Subspace PINN. Autonomous parameter-space Adaptive Mesh Refinement (AMR) using vectorized per-sample Gram alignment profiling (`torch.func.vmap`) with exact zero-disruption cleavage invariance. Validated across 9 canonical PDEs with $725.6\times$ loss reduction on high-frequency Helmholtz.
- **[null-space-pinn](https://github.com/KartikeyaGangwar/null-space-pinn)** — Decoupling boundary-PDE gradient conflicts via orthogonal direct-sum parameter subspaces ($\Theta_0 \oplus \Theta_1$) blended with a $C^2$ Quintic Hermite seam operator. *([DOI: 10.5281/zenodo.22132799](https://doi.org/10.5281/zenodo.22132799))*.
- **[as-vit-multitask](https://github.com/KartikeyaGangwar/as-vit-multitask)** — Adaptive Subspace Vision Transformers. Tracks inter-task Gram matrix negative eigenvalues to dynamically route latent expert subspaces using Partition of Unity (PoU) gating, eliminating multi-task negative transfer on NYUv2.

### Stochastic Control, Financial PDEs & High-Performance Solvers
- **[Deep-EEP-PINN](https://github.com/KartikeyaGangwar/Deep-EEP-PINN)** — High-dimensional American basket option pricing up to $d=50$ assets (1,225 correlations). Computes diffusion operator via directional autograd trace contraction in $\mathcal{O}(d)$ linear complexity and $<3\,\mathrm{GB}$ VRAM, validated against 100K-path Longstaff-Schwartz Monte Carlo.
- **[PINN-Bayesian-Posterior-Fidelity](https://github.com/KartikeyaGangwar/PINN-Bayesian-Posterior-Fidelity)** — Diagnostic framework quantifying Bayesian posterior distortion under neural surrogate approximations using the 1-Wasserstein Bayesian Fidelity Ratio (BFR) normalized by empirical MCMC noise floors.
- **[lid-driven-cavity-cfd](https://github.com/KartikeyaGangwar/lid-driven-cavity-cfd)** — High-resolution 2D incompressible Navier-Stokes solver up to $Re=100,000$ ($1025 \times 1025$). Exact $\mathcal{O}(N^2 \log N)$ DST-I Poisson engine with ADI marching. *(Under review at Applied Mathematical Modelling; [DOI: 10.5281/zenodo.18312938](https://doi.org/10.5281/zenodo.18312938))*.
- **[BRSDK](https://github.com/KartikeyaGangwar/BRSDK)** — Real-time telemetry extraction framework operating inside the 2000Hz Vehicle Lua physics thread of BeamNG.drive/tech. Features pre-allocated static ring buffers, zero-allocation hot path, and RFC 8259 JSON metadata sidecars. *([DOI: 10.5281/zenodo.21729606](https://doi.org/10.5281/zenodo.21729606))*.

---

## Technical Stack

- **Languages:** Python (3.11+), C++20, Lua / LuaJIT, Bash, LaTeX
- **Deep Learning & Autograd:** PyTorch (custom autograd, `torch.func.vmap`, forward-mode AD, JVPs), JAX, CUDA
- **Scientific Computing & HPC:** NumPy, SciPy, OpenMP, CMake, Finite Element Method (FEM), Finite Difference Methods (ADI, Red-Black SOR), Symplectic Verlet Integration
- **Systems & Simulation:** Linux, Git/GitHub, Docker, BeamNG.tech JBeam Continuum Physics

---

## Contact & Identifiers

- **Portfolio:** [kartikeyagangwar.github.io](https://kartikeyagangwar.github.io)
- **ORCID:** [0009-0009-1973-7532](https://orcid.org/0009-0009-1973-7532)
- **Email:** [kartikeysingh525@protonmail.com](mailto:kartikeysingh525@protonmail.com)
- **LinkedIn:** [kartikey-singh-2a3434329](https://www.linkedin.com/in/kartikey-singh-2a3434329/)
- **Zenodo:** [Kartikey Singh on Zenodo](https://zenodo.org/search?q=metadata.creators.person_or_org.name%3A%22Singh%2C%20Kartikey%22)

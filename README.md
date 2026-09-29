# Kartikeya Gangwar

> **Undergraduate Researcher in Scientific Machine Learning (SciML), Symplectic Geometry & High-Performance Computing**  
> *Department of Mathematics, University of Delhi &bull; Advised by Prof. Vinay Kumar*  
> *(Official / Academic Documents: Kartikey Singh)*

[![Website](https://img.shields.io/badge/Portfolio-kartikeyagangwar.github.io-0284c7?style=flat-square&logo=google-chrome&logoColor=white)](https://kartikeyagangwar.github.io)
[![ORCID](https://img.shields.io/badge/ORCID-0009--0009--1973--7532-a6ce39?style=flat-square&logo=orcid&logoColor=white)](https://orcid.org/0009-0009-1973-7532)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-kartikey--singh-0077b5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kartikey-singh-2a3434329/)
[![Email](https://img.shields.io/badge/Email-kartikeysingh525%40protonmail.com-6d4aff?style=flat-square&logo=protonmail&logoColor=white)](mailto:kartikeysingh525@protonmail.com)
[![Zenodo](https://img.shields.io/badge/Zenodo-Preprints_%26_Datasets-0052cc?style=flat-square&logo=zenodo&logoColor=white)](https://zenodo.org/search?q=metadata.creators.person_or_org.name%3A%22Singh%2C%20Kartikey%22)

---

## 🔬 About & Research Vision

Undergraduate mathematical researcher investigating the intersection of **Scientific Machine Learning (SciML)**, **Symplectic Dynamical Systems**, **Inverse Problems**, and **High-Dimensional Stochastic PDEs**. Author of **10 research frameworks** (including 3 under review at **IEEE TCI**, **Physics of Fluids**, and **Applied Mathematical Modelling**) and **2 open-source scientific computing engines**.

Primary methodology emphasizes **structural mathematical invariants** (exact symplectic 2-form conservation, Arnold extended contact phase spaces, and B-spline sensitivity projections) coupled with **bare-metal computational efficiency** (custom autograd engines, `torch.func.vmap`, directional JVP projections, and zero-allocation streaming).

📄 **Documents:** [Download Academic CV (PDF)](https://kartikeyagangwar.github.io/Kartikeya_cv.pdf) &bull; [Download Industry Resume (PDF)](https://kartikeyagangwar.github.io/Kartikeya_Resume.pdf)

---

## 🏛️ Flagship Research Manuscripts & Preprints

### 1. Inverse Problems & Computational Imaging
- **[eit-neural-surrogate-inversion](https://github.com/KartikeyaGangwar/eit-neural-surrogate-inversion)** — *Derivative-Informed Neural Forward Surrogates with Directional Sensitivity Supervision for Shape Inversion in Electrical Impedance Tomography*  
  **Status:** **Under Review at IEEE Transactions on Computational Imaging (TCI)** &bull; **Authors:** **Kartikeya Gangwar** (Sole Author)  
  - Parameterized closed inclusion boundaries via 64D periodic cubic B-splines with mollified boundary-integral winding indicators.
  - Formulated **Stochastic Directional JVP Supervision** on $\mathbb{S}^{63}$, reducing backprop tangent branches from 64 to 1 per sample and bounding peak VRAM to $342.8\,\mathrm{MB}$.
  - Zero-online-FEM Levenberg–Marquardt delivers a **$56.8\times$ wall-clock speedup** ($35.6\,\mathrm{ms}$ vs $2.02\,\mathrm{s}$/step) with single-model mean IoU $0.8006$ (ensemble IoU $0.8235$) and $99.57\%$ noise robustness across 234 trials.  
  - **Preprint DOI:** [10.5281/zenodo.22096368](https://doi.org/10.5281/zenodo.22096368)

### 2. Theoretical Fluid Dynamics & Operator Conditioning
- **[pinn-fluid-formulations](https://github.com/KartikeyaGangwar/pinn-fluid-formulations)** — *Operator Conditioning and False Convergence in Physics-Informed Neural Networks for Incompressible Flows*  
  **Status:** **Under Review at Physics of Fluids (AIP Publishing)** `[MS #POF26-AR-14856]` &bull; **Authors:** **Kartikeya Gangwar** (Sole Author)  
  - Controlled regularized cavity benchmark ($Re=1000$); proved that continuous mesh-free PINNs lack discrete stencils for Thom's wall-vorticity condition, causing **False Convergence and Operator Diffusion** in $\psi$--$\omega$ models ($67.3\times$ residual drop while underpredicting corner eddies by $14.3\%$).
  - Proved retaining pressure $p$ in $\psi$--$p$ enforces an implicit elliptic Helmholtz–Hodge projection that restores operator conditioning ($14.2\%$ vs $2.8\%$ global velocity $L_2$ error).  
  - **Preprint DOI:** [10.5281/zenodo.22979276](https://doi.org/10.5281/zenodo.22979276)

- **[lid-driven-cavity-cfd](https://github.com/KartikeyaGangwar/lid-driven-cavity-cfd)** — *A High-Resolution Finite-Difference Framework for Steady Continuation and Finite-Window Unsteady Dynamics up to $Re = 100{,}000$ in 2D Lid-Driven Cavity Flows*  
  **Status:** **Under Review at Applied Mathematical Modelling (Elsevier)** &bull; **Authors:** **Kartikeya Gangwar** (Sole Author)  
  - Formulated an exact $\mathcal{O}(N^2 \log N)$ Discrete Sine Transform (DST-I) Poisson solver with vectorized ADI marching on $1025 \times 1025$ grids ($1.05\mathrm{M}$ nodes), eliminating iterative residual drift.
  - Maintained zero artificial viscosity ($\nu_{\text{art}} = 0$) for $Re \le 50,000$ via pure second-order central differencing; verified Batchelor's core vorticity theorem and ASME V&V 20 Richardson GCI ($0.48\%$).
  - Resolved periodic vortex shedding ($St=0.6249$) and finite-window spectral transitions up to $Re = 100,000$.  
  - **Datasets & DOI:** [10.5281/zenodo.18312938](https://doi.org/10.5281/zenodo.18312938)

### 3. Symplectic Geometry & Celestial Astrodynamics
- **[cpa-shnn](https://github.com/KartikeyaGangwar/cpa-shnn)** — *Causality-Preserving Adaptive Symplectic Hamiltonian Neural Networks for Multi-Body Gravitational Dynamics*  
  **Status:** Working Paper *(Target: Astronomy & Computing)* &bull; **Authors:** **Kartikeya Gangwar** (Lead Author), **Prof. Vinay Kumar** (Supervisor & Senior Author)  
  - Proved *Theorem 1* (Separable Symplectic Kinetic-Coriolis Decomposition, $\nabla_{\mathbf{z}}\cdot\mathbf{f}_\theta \equiv 0$) and *Theorem 2* (Arnold Extended Contact Phase Space $\mathbf{Z}_{\text{ext}} = (\mathbf{q}, t, \mathbf{p}, p_t)$, $\mathcal{K}_\theta \equiv 0$).
  - Benchmarked across 6 chaotic multi-body celestial systems (Binary Quasars, Restricted 6-Body, Sitnikov 5-Body), preserving energy to machine precision ($\Delta\mathcal{H} \le 10^{-4}\%$). Multi-scale Fourier features achieved up to a **$126.40\times$ error collapse** on gravitational saddle singularities.

---

## 🧬 The Adaptive Subspace (AS) Optimization Trilogy

Architect of the **Adaptive Subspace Paradigm** resolving gradient conflict across parameter manifolds:

1. **Act I: Algebraic Orthogonality — [null-space-pinn](https://github.com/KartikeyaGangwar/null-space-pinn)**  
   Decomposed the parameter manifold into orthogonal direct-sum subspaces ($\Theta = \Theta_0 \oplus \Theta_1$, $\mathcal{W}_0 \mathcal{W}_1^T = \mathbf{0}$) blended via a $C^2$ Quintic Hermite operator ($\psi(\xi) = 6\xi^5 - 15\xi^4 + 10\xi^3$). Proved structural gradient orthogonality ($\langle \nabla\mathcal{L}_{\mathrm{if}}, \nabla\mathcal{L}_{\mathrm{des}} \rangle \equiv 0$) on saturated domains.  
   *Preprint DOI: [10.5281/zenodo.22132799](https://doi.org/10.5281/zenodo.22132799)* &bull; *Target: Journal of Computational Physics (JCP)*

2. **Act II: Autonomous Parameter-Space AMR — [as-pinn](https://github.com/KartikeyaGangwar/as-pinn)**  
   Engineered autonomous domain decomposition via vectorized per-sample Gram alignment profiling ($\mathcal{G}_{ij} = \cos \angle(\mathbf{g}_i, \mathbf{g}_j)$ via `torch.func.vmap`) with exact zero-disruption cleavage invariance ($\|u^{(N+1)} - u^{(N)}\| = 0$). Attained **$725.6\times$ loss reduction** over standard PINNs, PCGrad, and CAGrad on high-frequency Helmholtz ($k=4\pi$).  
   *Target: SIAM Journal on Scientific Computing (SISC)*

3. **Act III: Latent Feature MoE — [as-vit-multitask](https://github.com/KartikeyaGangwar/as-vit-multitask)**  
   Resolved multi-task negative transfer in dense vision backbones (segmentation, depth, normals, edges) by tracking inter-task Gram matrix negative eigenvalues ($\lambda_{\min}(\mathcal{G}) < -\tau$) and dynamically cleaving dedicated latent expert subspaces using Partition of Unity (PoU) gating ($+5.84\%$ mean multi-task gain on NYUv2).  
   *Target: IEEE TPAMI / CVPR*

---

## 📈 High-Dimensional Stochastic PDEs & Systems Infrastructure

- **[Deep-EEP-PINN](https://github.com/KartikeyaGangwar/Deep-EEP-PINN)** — *Deep Early Exercise Premium PINN for High-Dimensional Free-Boundary Obstacle Problems*  
  Priced correlated American basket options up to **$d=50$ assets (1,225 correlations)**, breaking Bellman's Curse of Dimensionality ($N^d$) via Directional Autograd Hessian Trace Contraction in $\mathcal{O}(d)$ linear complexity ($<3\,\mathrm{GB}$ VRAM). Validated against 100,000-path Longstaff–Schwartz Monte Carlo and Crank–Nicolson PSOR ($0.37\%$ relative error).
- **[PINN-Bayesian-Posterior-Fidelity](https://github.com/KartikeyaGangwar/PINN-Bayesian-Posterior-Fidelity)** — Diagnostic framework quantifying neural surrogate induced Bayesian posterior distortion using the 1-Wasserstein Bayesian Fidelity Ratio ($\mathrm{BFR}$) normalized by empirical MCMC stochastic noise floors.
- **[BRSDK](https://github.com/KartikeyaGangwar/BRSDK)** — *High-Frequency In-Engine Telemetry Framework and Python SDK for Sim2Real Autonomous Vehicle Research in BeamNG*  
  Operates inside BeamNG's **2,000\,Hz soft-body physics thread** with zero dynamic Lua heap allocations during logging. Built an Apache Arrow columnar Python SDK (`brsdk`) with Polars and zero-copy DLPack interchange with PyTorch for offline reinforcement learning.  
  *Preprint DOI: [10.5281/zenodo.21729606](https://doi.org/10.5281/zenodo.21729606)* &bull; *Target: JOSS (2027)*

---

## 🛠️ Technical Stack & Toolchain

```
Mathematical Foundations │ Symplectic Geometry, Differential Forms, Lie Algebras, Optimal Transport (Wasserstein),
                         │ Sobolev Spaces, Free-Boundary Obstacle PDEs, Numerical Fluid Dynamics, Chaos Theory
Deep Learning & Autograd │ PyTorch (torch.func.vmap, forward-mode AD, JVP/VJP, custom autograd engines, HVP),
                         │ CUDA Acceleration, GPU Memory Profiling, JAX, HuggingFace
Scientific Computing    │ NumPy, SciPy, Finite Element Method (FEM / EIDORS), Finite Difference Schemes (ADI, Red-Black SOR),
                         │ Symplectic Runge-Kutta (RK4), L-BFGS (Strong-Wolfe), MCMC (Metropolis-Hastings)
Languages & Systems      │ Python (3.11+), C++20, Lua / LuaJIT, Bash, Git / GitHub, Linux (Debian/Ubuntu), LaTeX
Data & Infrastructure    │ Apache Arrow, Polars, BeamNG.tech JBeam Continuum Physics, Docker
```

---

## 📬 Contact & Links

- **Portfolio & Interactive Visuals:** [kartikeyagangwar.github.io](https://kartikeyagangwar.github.io)
- **ORCID:** [0009-0009-1973-7532](https://orcid.org/0009-0009-1973-7532)
- **GitHub:** [@KartikeyaGangwar](https://github.com/KartikeyaGangwar)
- **LinkedIn:** [linkedin.com/in/kartikey-singh-2a3434329](https://www.linkedin.com/in/kartikey-singh-2a3434329/)
- **Email:** [kartikeysingh525@protonmail.com](mailto:kartikeysingh525@protonmail.com)

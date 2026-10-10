# Kartikeya Gangwar
*(Officially documented name: Kartikey Singh)*

Independent researcher in computational mathematics and scientific machine learning, currently completing a B.Sc. (Honours) Mathematics at the University of Delhi. Invited peer reviewer for *Physics of Fluids* (AIP Publishing).

I build numerical solvers and computational systems from first principles. My work sits at the intersection of computational mathematics, geometric mechanics, and scientific machine learning. Rather than treating models as black boxes, I design computational architectures that respect the underlying mathematical structure—forcing algorithms to preserve geometric invariants, phase-space structure, and physical conservation laws.

When approaching complex or nonlinear dynamical systems, I look at the failure modes and extreme limits first. That is usually where naive approximations break down, where numerical diffusion creeps in, and where the true governing geometry reveals itself. Whether working on fluid turbulence, chaotic multi-body dynamics, high-dimensional stochastic PDEs, or foundation time-series architectures, the objective remains constant: building methods that hold up when conditions become extreme.

Outside of mathematical derivations and custom PyTorch/C++ routines, intellectual work cannot be separated from physical reality. Working with tractors and agriculture in my village, maintaining and driving machinery to understand mechanical thresholds, and daily heavy physical training keep my thinking grounded. Freehand pencil sketching trained my eye to understand continuous curvature, perspective, and spatial balance long before formalizing them into differential geometry.

The standard is straightforward: things must work under load—whether it is a mechanical engine, an athletic lift, or an algorithm. Everything I formulate is developed in the open with publicly archived code, manuscripts, and reproduction pipelines.

---

### Core Research & Codebases

| System | Focus | What It Actually Does | Venue / Status |
| :--- | :--- | :--- | :--- |
| **[Contact-SSM](https://github.com/KartikeyaGangwar/time-series-forecasting)** | Geometric Foundation Models | Embeds an odd-dimensional contact manifold $(2d+1)$ with Reeb vector dynamics into parallel associative prefix scans. Runs in $\mathcal{O}(L)$ on GPUs without the phase drift of Transformers or the dissipative decay of standard Mamba. | Target: Top-Tier ML / SIMODS |
| **[CHRONOS / SymPIN](https://github.com/KartikeyaGangwar/UG_R_proj)** | Celestial Astrodynamics | Recovers unknown non-integrable gravitational potentials from observational tracks. Enforces exact separable kinetic-potential decomposition, recovers all 5 Lagrange points with 100% stability match, and cuts Jacobi drift by $412\times$ via Poincaré-Sundman time stepping. | Working Paper (with Prof. Vinay Kumar) |
| **[EIT Neural Inversion](https://github.com/KartikeyaGangwar/eit-neural-surrogate-inversion)** | Calderón Inverse Problem | Parameterizes closed boundaries via 64D periodic cubic B-splines. Uses stochastic directional JVP supervision on $\mathbb{S}^{63}$ to drop backprop tangent branches from 64 to 1, cutting memory to $342.8\,\text{MB}$ and delivering a $56.8\times$ wall-clock speedup. | Under Review, *IEEE TCI* |
| **[Fluid PINN Formulations](https://github.com/KartikeyaGangwar/pinn-fluid-formulations)** | Incompressible Fluid Dynamics | Shows why continuous mesh-free PINNs suffer false convergence under streamfunction-vorticity ($\psi$--$\omega$) due to missing Thom wall stencils, and proves that keeping pressure in $\psi$--$p$ restores the elliptic Helmholtz-Hodge projection. | Under Review, *Physics of Fluids* |
| **[Extreme-$Re$ Cavity CFD](https://github.com/KartikeyaGangwar/lid-driven-cavity-cfd)** | Spectral Numerical Analysis | Direct DST-I Poisson solver running in $\mathcal{O}(N^2 \log N)$ without iterative residuals. Steady continuation to $Re=100,000$ on $1025^2$ grids with zero artificial viscosity up to $Re=50,000$. Verified by ASME V&V 20 Richardson extrapolation ($0.48\%$). | Under Review, *Emerald IJNMHFF* |
| **[Deep-EEP-PINN](https://github.com/KartikeyaGangwar/Deep-EEP-PINN)** | High-Dimensional Obstacle PDEs | Prices American basket options up to $d=50$ assets (1,225 correlations) via directional Hessian trace contractions in $\mathcal{O}(d)$ complexity ($<3\,\text{GB}$ VRAM). Absorbs maturity kinks into an analytical European baseline. | Working Paper / Zenodo |
| **[Adaptive Subspace (AS) Trilogy](https://github.com/KartikeyaGangwar/null-space-pinn)** | Multi-Task Optimization | Direct-sum parameter decomposition ($\Theta_0 \oplus \Theta_1$) with Quintic Hermite routing, extending from static null-space PINNs to autonomous parameter-space AMR (AS-PINN, $725\times$ lower loss) and dynamic vision transformers (AS-ViT). | Act I Under Review, *Elsevier JCP* |
| **[BRSDK v2.0.1](https://github.com/KartikeyaGangwar/BRSDK)** | Sim2Real Vehicle Dynamics | Hooks into BeamNG's 2,000 Hz soft-body physics loop to extract tire slip energy and dynamic damper velocities with zero dynamic Lua heap allocations. Includes an Apache Arrow / Polars Python SDK and DLPack PyTorch bindings. | Open-Source / Target: *JOSS* |

---

### Dissemination & Contact

- **Preprints & Datasets:** [Zenodo Archive](https://zenodo.org/search?q=metadata.creators.person_or_org.identifiers.identifier%3A%220009-0009-1973-7532%22)
- **Portfolio & Interactive Visuals:** [kartikeyagangwar.github.io](https://kartikeyagangwar.github.io)
- **ORCID:** [0009-0009-1973-7532](https://orcid.org/0009-0009-1973-7532)
- **Direct Mail:** [kartikeyagangwar@proton.me](mailto:kartikeyagangwar@proton.me)

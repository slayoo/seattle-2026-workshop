# hacking aerosol-cloud μ-physics modeling concepts in Python
### [mini-workshop @Uni. Washington Seattle, Jan 2026 (click for a flyer pdf)](https://raw.githubusercontent.com/slayoo/seattle-2026-workshop/main/flyer.pdf)

#### Speakers:
- [Sylwester Arabas (AGH.edu.pl)](https://open-atmos-krk.github.io/)
- [Emma Ware (UCDavis.edu)](https://emmaware.weebly.com/)

#### Synopsis: we're going to
- Code in a Pythonic way, and interactively explore (simple yet functional) models of diffusional and collisional growth of cloud droplets.
- Leverage Jupyter notebooks, the [Google Colab platform](https://colab.google/), and the Python scientific package ecosystem
- Focus on: 
  - moving-sectional/particle-based representation of cloud microphysics;
  - "SDM" Monte-Carlo algorithm for solving coagulation problems;
  - ODEs describing evolution of liquid particle sizes in a vertically displaced adiabatic parcel of humid air for modelling diffusional growth and the resultant phenomena of aerosol activarion and drop ripening.
- Outline the rationale behind, present the usage examples & encourage your contributions to the [PySDM](https://open-atmos.github.io/PySDM/) package

#### Notebooks:
- **Part 1**: size spectrum sampling using SciPy
  - [partial](https://github.com/slayoo/seattle-2026-workshop/tree/main/part_1_scipy_sampling_partial.ipynb)
  - [complete](https://github.com/slayoo/seattle-2026-workshop/tree/main/part_1_scipy_sampling_complete.ipynb)
- **Part 2**: SDM collisional growth Monte-Carlo algorithm in a box model (incl. validation against the Safranov-Golovin analytic solution to the Smoluchowski equation)
  - [partial](https://github.com/slayoo/seattle-2026-workshop/tree/main/part_2_SDM_partial.ipynb)      
  - [complete](https://github.com/slayoo/seattle-2026-workshop/tree/main/part_2_SDM_complete.ipynb)      
- **Part 3**: dimensional analysis using Pint (and PySDM.physics)
  - partial
  - [complete](https://github.com/slayoo/seattle-2026-workshop/blob/main/part_3_units_with_pint_and_pysdm_complete.ipynb)
- **Part 4**: condensational growth (incl. activation and ripening) in an adiabatic parcel model:
  - partial
  - [complete](https://github.com/slayoo/seattle-2026-workshop/tree/main/part_4_CCN_complete.ipynb)    
- **Part 5**: particle-based μ-physics simulations with diffusional & collisional processes using PySDM (box, parcel, single-column and beyond)
  - [PySDM documentation](https://open-atmos.github.io/PySDM)

#### Tools:
- [SciPy stats](https://docs.scipy.org/doc/scipy/reference/stats.html) for a library of probability distributions
- [Pint](https://pint.readthedocs.io/) for dimensional analysis and auto-labelling plots with units
- [SciPy ODE solvers](https://docs.scipy.org/doc/scipy/reference/integrate.html) for numerically integrating stiff ODE systems
- [Numba](https://numba.pydata.org/) for just-in-time compilation of Python code
- [PySDM](https://open-atmos.github.io/PySDM) for integrating Pint with SciPy ODE solvers and Numba, and for pre-built particle-based cloud-micropphysics modelling examples
- [open-atmos-jupyter-utils](https://pypi.org/project/open-atmos-jupyter-utils/) for embedding vector graphics and animations in Jupyter notebooks

### Further reading:
- [Shima et al. 2008 (arXiv)](https://doi.org/10.48550/arXiv.physics/0701103) / [Shima et al. 2009 (QJRMS)](https://doi.org/10.1002/qj.441): "_Super-Droplet Method for the Numerical Simulation of Clouds and Precipitation: a Particle-Based Microphysics Model Coupled with Non-hydrostatic Model_"
- [Arabas & Shima 2016 (arXiv)](https://doi.org/10.48550/arXiv.1608.08187) / [Arabas & Shima 2017 (NPG)](https://doi.org/10.5194/npg-24-535-2017): "_On the CCN [de]activation nonlinearities_"
- [Bartman et al. 2021 (JOSS)](https://doi.org/10.21105/joss.03219) & [de Jong, Singer et al. 2022 (JOSS)](https://doi.org/10.21105/joss.04968): JOSS papers on PySDM
- [Ware et al. 2025 (arXiv)](https://doi.org/10.48550/arXiv.2509.05536): "_Adaptive time-stepping for the Super-Droplet Method Monte Carlo collision-coalescence scheme_"

#### License: [Creative Commons Zero](https://creativecommons.org/public-domain/cc0/) (i.e. public domain)

#### Credits: materials composed by [Sylwester Arabas (AGH)](https://slayoo.github.io) and [Emma Ware (UCDavis)](https://emmaware.weebly.com/) with contributions from [Daria Klimaszewska (AGH)](https://github.com/thearia0/) & [Agnieszka Żaba (AGH)](https://github.com/AgnieszkaZaba)

#### Funding: European Union Erasmus+ Staff Mobility programme

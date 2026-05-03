# Optimizing Temporal Regularity of Noise-Induced Spikes in the FitzHugh-Nagumo Model

This project investigates **coherence resonance** in the stochastic FitzHugh-Nagumo neuron model, the phenomenon where intermediate noise intensity optimizes spike timing regularity.

## Key Finding

Unlike the classic coherence resonance expected in such systems, the coefficient of variation (CV) of inter-spike intervals did not show a clear minimum at intermediate noise levels. Instead, CV appeared to plateau rather than achieve a distinct optimal noise intensity for spike timing regularity. We attribute this to the fact
that our chosen parameter values are at some distance from the Hopf
bifurcation which causes coherence resonance to not have such a 
pronounced effect on dynamics.

## Project Structure

```
├── main.pdf            # Compiled research paper
├── README.md
├── requirements.txt    # Python dependencies
├── notebooks/         # Jupyter notebooks with simulation code
│   ├── stochastic_fhn_sim.ipynb
│   └── deterministic_fhn_sim.ipynb
├── figures/           # Generated figures
│   ├── cv_vs_sigma*.png
│   ├── spikecount_vs_sigma.png
│   ├── phase_plane_*.png
│   └── sample_trajectory.png
└── latex/             # LaTeX source for paper
    ├── main.tex
    └── references.bib
```

## Quick Start

```bash
# Install dependencies
pip install -r requirements.txt

# Run simulations
jupyter lab
```

Open `notebooks/stochastic_fhn_sim.ipynb` to explore the stochastic model and reproduce the coherence resonance results. The deterministic dynamics are in `notebooks/deterministic_fhn_sim.ipynb`.

## Academic Context

This work sits at the intersection of:
- **Dynamical systems** — phase plane analysis, nullclines, excitability
- **Stochastic processes** — Brownian motion, Ito calculus, Euler-Maruyama integration
- **Neuroscience** — action potentials, coherence resonance, spike-train statistics

See `main.pdf` for the full mathematical derivation and analysis.

## Why It Matters

### For Academic Researchers
- Demonstrates coherence resonance in a canonical excitable system
- Provides a template for combining analytical and numerical approaches to SDEs
- Extends classical phase-plane methods to stochastic settings

### For Industry
- **Neural interfaces**: Understanding how noise affects timing precision informs electrode placement and signal processing
- **Biosensors**: Noise-driven threshold crossings can be exploited for sensitive detection
- **Signal processing**: This work suggests that controlled randomness can sometimes improve — not degrade — system regularity

## License

MIT License — see `LICENSE` file.
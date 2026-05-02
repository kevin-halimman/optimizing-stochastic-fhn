# Optimizing Temporal Regularity of Noise-Induced Spikes in the FitzHugh-Nagumo Model

This project investigates **coherence resonance** in the stochastic FitzHugh-Nagumo neuron model — the phenomenon where intermediate noise intensity optimizes spike timing regularity.

## Key Finding

The coefficient of variation (CV) of inter-spike intervals exhibits a clear minimum at intermediate noise levels (~σ ≈ 0.15–0.25). This demonstrates that noise is not merely a source of irregularity — at the right intensity, it can **enhance** the temporal structure of neural signaling.

## Project Structure

```
├── notebooks/          # Jupyter notebooks with simulation code
│   ├── stochastic_fhn_sim.ipynb
│   └── deterministic_fhn_sim.ipynb
├── docs/
│   └── paper.pdf      # Full research paper
├── slides/
│   ├── slides_intro_stochastic_fhn.md
│   └── slides_intro_stochastic_fhn.pdf
└── figures/           # All figures from the study
```

## Quick Start

```bash
# Install dependencies
pip install -r requirements.txt

# Run simulations (open notebooks in Jupyter)
jupyter lab
```

## Academic Context

This work sits at the intersection of:
- **Dynamical systems** — phase plane analysis, nullclines, excitability
- **Stochastic processes** — Brownian motion, Ito calculus, Euler-Maruyama integration
- **Neuroscience** — action potentials, coherence resonance, spike-train statistics

See `docs/paper.pdf` for the full mathematical derivation and analysis.

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
# NeuralFoil-Core

NeuralFoil-Core is a lightweight fork of NeuralFoil, focused on a minimal runtime/core package with reduced dependencies.

## Upstream Credit

All core ideas and the original implementation come from NeuralFoil by Peter Sharpe and contributors.

- Upstream repository: https://github.com/peterdsharpe/NeuralFoil
- Author site: https://peterdsharpe.github.io
- Paper (preprint): https://arxiv.org/abs/2503.16323

This fork is made with appreciation for that work.

## Goal of This Fork

This repository targets a slim, practical core for integration use cases (such as AirfoilEditor):

- keep the neuralfoil runtime path clear and small
- avoid heavy optional ecosystems where possible
- reduce or remove dependency pressure from AeroSandbox-driven tooling

In short: keep the useful core, strip non-essential layers.

## Quick Example

The repository includes a runnable showcase script at [example.py](example.py).

What it demonstrates:

- builds a lightweight airfoil object from embedded coordinates
- fits CST/Kulfan parameters with [fit_cst](neuralfoil/cst.py)
- evaluates a polar through [get_aero_from_kulfan_parameters](neuralfoil/core_api.py)
- prints a formatted table of alpha, CL, CD, and CM

Run it from the repository root:

```bash
python example.py
```

Current script setup:

- alpha sweep from -3.0 to 13.0 deg in 0.5 deg steps
- Reynolds number: 600000
- Ncrit: 9.0


## License and Attribution

This project preserves upstream licensing and attribution requirements. See LICENSE and upstream notices for details.

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


## License and Attribution

This project preserves upstream licensing and attribution requirements. See LICENSE and upstream notices for details.

# CMG-PES Attitude Residual — Bounded Neuromorphic Control for Quadrotor Attitude Tracking

Six continuous coupled membrane-gate (CMG) units and an 18-weight online PES decoder form a bounded,
saturation-aware residual that augments a classical attitude controller — with exact recovery of the
baseline when disabled, and no change to the plant, sensing, or actuator interface.

> **Status:** Private (pre-publication). Submitted to the 2027 American Control Conference (ACC).
> The library here is complete and runnable; the full experiment/reproduction package (campaign
> scripts, pre-registration, certification reports) will be added upon acceptance. See
> [Citation](#citation).

## Overview

The residual reduces geometric-mean quaternion attitude-tracking error by 37.3% (Skydio X2) and 22.4%
(Crazyflie 2) over a bandwidth-tuned PD+feedforward baseline in MuJoCo simulation, with an explicit,
provable bound on its deviation from the baseline command and exact recovery of the baseline at zero
residual authority. The same bounded interface attaches without modification to five classical control
families beyond PD — LQR, backstepping, sliding-mode control, unconstrained MPC, and nonlinear MPC —
improving tracking for every family and platform tested, with no per-family retuning.

## Repository structure

```
.
├── Readme.md
├── CITATION.cff
├── requirements.txt        # TODO: pin exact versions used for the paper
└── gra_control/             # core library
    ├── math3d.py            # quaternion kinematics, shortest-path attitude error
    ├── gate.py               # the CMG-PES residual: encoding, PES decoder, saturation-aware gate
    └── platforms/            # X2 / CF2 model interfaces, torque limits, rotor allocation
```

## Requirements

- Python 3.x
- NumPy
- MuJoCo (simulation)
- Nengo (neuron/PES substrate)

TODO: pin exact versions in `requirements.txt` before making public.

## Usage / Reproducing results

The library (`gra_control`) implements the residual architecture and is directly importable. The
campaign scripts, pre-registration record, and the certification reports documenting every headline
number in the paper will be added here once the paper is accepted — this keeps the public release tied
to the reviewed, final version rather than an in-progress one.

## Data

Simulation-generated (MuJoCo); no external dataset. Run archives and the pre-registered analysis
scripts will be released alongside the full code upon acceptance.

## Citation

If you use this code, please cite the associated paper (see `CITATION.cff`); the BibTeX entry will be
added once the paper has a DOI.

## License

TODO: Choose a license (e.g. MIT, Apache-2.0, BSD-3-Clause) and add a `LICENSE` file. Until a license
is added, default copyright applies and others may not reuse the code.

## Contact

TODO: Name / email / lab / ORCID.

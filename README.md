# Neuromorphic Embodied AI

This repository contains research and development focused on Neuromorphic Embodied AI, organized into
the following core areas. Each project folder carries its own status (private/pre-publication vs.
public) — see that project's own README.

* **[`simulation-platforms/`](simulation-platforms/)** — Simulation platforms used to integrate
  neuromorphic sensing and control for embodied AI: ROS 2, Gazebo, NVIDIA Isaac Sim, MuJoCo, Basilisk,
  Quanser, and X-Plane.
  * [`xplane12-ehekatl-bwb/`](simulation-platforms/xplane12-ehekatl-bwb/) — X-Plane 12 controllers and
    the Ehekatl blended-wing-body aircraft.
* **[`closed-loop-control/`](closed-loop-control/)** — Core sensing & control algorithms exploring the
  spectrum of autonomy: conventional, hybrid, and fully neuromorphic closed-loop implementations,
  benchmarked against each other.
  * [`acc2027-cmg-pes-residual/`](closed-loop-control/acc2027-cmg-pes-residual/) — Bounded online
    neuromorphic (CMG-PES) residual for quadrotor attitude control; submitted to ACC 2027.
  * [`y6-coaxial-trirotor/`](closed-loop-control/y6-coaxial-trirotor/) — Spiking neural network control
    of a coaxial tri-rotor UAV in Nengo.
* **[`hardware-in-the-loop/`](hardware-in-the-loop/)** — Deployment pipelines that transition digital
  twins into physical applications: real-time testing interfaces and finalized project execution.
  * [`qcar2-lane-control/`](hardware-in-the-loop/qcar2-lane-control/) — Spiking neural network lane
    control on the Quanser QCar platform, simulation and hardware.

## Part of a three-pillar research portfolio

This is pillar 2 of 3: single-platform embodied systems applying neural/neuromorphic architectures to
real control problems, in simulation and hardware-in-the-loop.

1. **[Neural Networks & Learning](https://github.com/gandhico/Neural-Networks-and-Learning)** —
   architectures, learning rules, and benchmarks, independent of any one platform or application.
2. **Neuromorphic Embodied AI** (this repository) — quadrotors, ground vehicles, fixed-wing aircraft.
3. **Neuromorphic Multi-Agent Systems** — multi-vehicle and swarm extensions of this pillar. (Repository
   not yet public.)

Applied focus: aerospace, defense, and space.

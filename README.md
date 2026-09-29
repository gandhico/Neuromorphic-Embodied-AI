# Neuromorphic Embodied AI

This repository contains research and development focused on Neuromorphic Embodied AI. Projects are
listed flat below (one folder each) and grouped here by area — each carries its own status
(private/pre-publication vs. public) in its own README.

* **Closed-loop control algorithms** — conventional, hybrid, and fully neuromorphic implementations,
  benchmarked against each other.
  * [`online-pes-neuromorphic-residual-control/`](online-pes-neuromorphic-residual-control/) — Bounded
    online neuromorphic (CMG-PES) residual for quadrotor attitude control; submitted to ACC 2027.
  * [`y6-coaxial-trirotor/`](y6-coaxial-trirotor/) — Spiking neural network control of a coaxial
    tri-rotor UAV in Nengo.
* **Hardware-in-the-loop (HITL) / real-time testing** — deployment pipelines transitioning digital
  twins into physical applications.
  * [`qcar2-lane-control/`](qcar2-lane-control/) — Spiking neural network lane control on the Quanser
    QCar platform, simulation and hardware.
* **Simulation platforms** — environments used to integrate neuromorphic sensing and control: ROS 2,
  Gazebo, NVIDIA Isaac Sim, MuJoCo, Basilisk, Quanser, and X-Plane.
  * [`xplane12-ehekatl-bwb/`](xplane12-ehekatl-bwb/) — X-Plane 12 controllers and the Ehekatl
    blended-wing-body aircraft.

## Part of a three-pillar research portfolio

This is pillar 2 of 3: single-platform embodied systems applying neural/neuromorphic architectures to
real control problems, in simulation and hardware-in-the-loop.

1. **[Neural Networks & Learning](https://github.com/gandhico/Neural-Networks-and-Learning)** —
   architectures, learning rules, and benchmarks, independent of any one platform or application.
2. **Neuromorphic Embodied AI** (this repository) — quadrotors, ground vehicles, fixed-wing aircraft.
3. **Neuromorphic Multi-Agent Systems** — multi-vehicle and swarm extensions of this pillar. (Repository
   not yet public.)

Applied focus: aerospace, defense, and space.

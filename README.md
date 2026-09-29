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

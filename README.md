# Robotic Strawberry Harvesting with Robust Vision and Deep Reinforcement Learning-based Sim-to-Real Control

**[Paper (arXiv preprint)](https://arxiv.org/abs/2605.23863)** · **[PDF](https://arxiv.org/pdf/2605.23863)**

**Code, trained models, and supporting resources: Coming soon.**

## Overview

This project investigates a task-level, closed-loop robotic strawberry harvesting system that integrates **robust visual perception**, **simulation-trained deep reinforcement learning (DRL) control**, and **ROS-based execution** on a physical robotic manipulator. Strawberry harvesting serves as a real-world testbed for connecting target perception with reliable robot motion and physical interaction in cluttered environments.

The system brings together three components:

1. **Vision:** **HRAttnEdge-YOLO26-seg**, a modified YOLO26-seg instance-segmentation model incorporating a high-resolution P2 branch, segmentation-path attention, and edge-supervised prototype learning to address fruit segmentation in cluttered scenes.
2. **Learning-based control:** A target-conditioned **Proximal Policy Optimization (PPO)** controller, trained in **NVIDIA Isaac Lab** to generate joint-position commands for a **UR10e** robotic manipulator and transferred to the physical robot.
3. **Real-robot integration:** A **ROS-based execution framework** connecting vision-derived targets, the learned motion controller, and the robotic harvesting process for greenhouse evaluation.

The study examines how task-specific perception and simulation-trained control can work together in a physical harvesting system, including comparisons with a conventional inverse-kinematics-based motion-planning approach.

## Resources and release status

| Resource | Status |
| --- | --- |
| [Research preprint](https://arxiv.org/abs/2605.23863) | Available (arXiv) |
| Vision model implementation and configurations | Coming soon |
| PPO training and evaluation resources | Coming soon |
| ROS integration and deployment resources | Coming soon |
| Trained model and policy checkpoints | Release details to be announced |
| Demonstrations and additional supporting materials | To be announced |

The repository currently serves as the project's research landing page. Implementation and reproducibility materials will be added as they are prepared and approved for public release.

## Citation

If you refer to this work, please cite the available preprint:

```bibtex
@misc{bashir2026strawberryharvesting,
  title        = {Robotic Strawberry Harvesting with Robust Vision and Deep Reinforcement Learning-based Sim-to-Real Control},
  author       = {Bashir, Al and Chang, Shao-Yang and Ghose, Partho and Raj, Prem and Huang, Chen-Kang and Zahid, Azlan},
  year         = {2026},
  eprint       = {2605.23863},
  archivePrefix = {arXiv},
  primaryClass = {cs.RO},
  url          = {https://arxiv.org/abs/2605.23863}
}
```

The citation and repository resources will be updated when a newer manuscript or journal version becomes available.

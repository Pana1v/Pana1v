<div align="center">
  <img src="./assets/banner.svg" width="100%" alt="Banner"/>
</div>

<p align="center">
  <a href="https://panav.netlify.app"><img src="https://img.shields.io/badge/Portfolio-panav.netlify.app-111827?style=flat-square&logo=firefox&logoColor=white"/></a>
  <a href="https://panav.gitbook.io/robotics-handbook"><img src="https://img.shields.io/badge/Robotics_Handbook-GitBook-111827?style=flat-square&logo=gitbook&logoColor=white"/></a>
  <a href="https://www.linkedin.com/in/panavraaj/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:praajarpit@gmail.com"><img src="https://img.shields.io/badge/Email-Say_hi-8B0000?style=flat-square&logo=gmail&logoColor=white"/></a>
</p>

---

## About

I build software that lets mobile robots know where they are and decide what to do next: GPU-accelerated perception, 3D SLAM and localization, full autonomy stacks on ROS 2 and Nav2. Lately I've been working the other end too, fine-tuning vision-language-action policies and benchmarking what actually transfers to a real manipulator.

| When | Role | Where |
|---|---|---|
| Now | Robotics Engineer, Level II | [Eternal.ag](https://eternal.ag), Bangalore |
| 2025–26 | Robotics Software Apprentice | Origin (ex 10xConstruction.ai) |
| 2024 | Mobile Robotics Intern | Addverb Technologies |
| 2021–25 | B.Tech, EEE | IIT Patna |

---

## Selected work

### Robot Learning

**[openpi-DoRA](https://github.com/Pana1v)** · Weight-decomposed fine-tuning for π0.5. JAX/Flax overlay injecting DoRA into Physical Intelligence's policy, reimplemented for Gemma's einsum and FFN layers. Controlled DoRA-vs-LoRA sweeps across all four LIBERO suites: **92.0% vs 91.4%** average success at rank 8, winning 3 of 4.
`JAX` `Flax` `OpenPI` `LIBERO` `DoRA/LoRA`

**Intrinsic AI for Industry Challenge** · Solo entry, one week to deadline. Ground-truth policy at **285/300**, OpenCV baseline at 130/300, learned perception with ResNet18 and U-Net conditioned on TCP pose, port identity, board pose. Pushed ACT and SmolVLA under a tight data budget.

**LEAP** · Pick-and-place sequencing as asymmetric TSP with a cycle-aware heterogeneous GNN. CP-SAT Hamiltonian circuit formulation replacing MTZ gave **5–7×**; imitation-learned arc pruning to O(Nk) gave a further **17.5× at N=200**, 0.06% optimality gap. *BRAIn Lab, IIT Patna. Manuscript in prep.*

### Perception & Navigation

**[POLKA](https://github.com/Pana1v/polka)** · Multi-LiDAR fusion for ROS 2. Merges heterogeneous PointCloud2 and LaserScan sources in one composable node, replacing the usual relay/filter/merge chain. SE(3) IMU deskewing with per-source overrides, footprint exclusion, voxel downsampling, optional CUDA. Humble and Jazzy.
`C++17` `CUDA` `PCL` `Eigen3`

**GO-SLAM** · Full SLAM from scratch: GICP front-end, pose-graph back-end, loop closure. Custom Levenberg–Marquardt solvers for both, no external optimization libraries. Fed by deskewed LiDAR from Polka, benchmarked on KITTI.

**At Eternal** · GPU-accelerated SLAM + Nav2 stack under **40% CPU on Jetson Orin**, automated per-robot LiDAR↔IMU extrinsic calibration, CI/CD, parameter snapshots inside rosbags.

**At Origin** · Swerve motion model for Nav2 MPPI. Lower-latency collision monitor via composable nodes. Kidnapped-robot recovery using genetic algorithms plus ambiguity detection. Lichtblick, a TypeScript/ROS 2 viz interface that cut peak CPU **120% → 26%** versus Foxglove.

### Competition

**[ICRA BARN Challenge 2026](https://cs.gmu.edu/~xiao/Research/BARN_Challenge/BARN_Challenge26.html)** · Breadcrumb Explorer, built from scratch instead of tuning a baseline. Mapless, no SLAM, no laser odometry. An odom-frame breadcrumb memory marks trajectories *tasty* or *stale* so path selection improves across trials despite 270° coverage, wheel slip, and IMU drift. **0.3682/0.5 on first submission, highest by an Indian team since 2022.** 76% zero-shot across 300 Gazebo courses.

**ABU Robocon 2023–24** · Captain, 60+ member team. National Finals, one of two IITs to qualify, highest score among IIT teams in 2024. Custom PCBs for motor control and power, heterogeneous controllers (Cube Orange, Pi, ESP32), multi-bot coordination over ROS.

**ISRO Robotics Challenge (IRoC-U) 2024** · Founded and led IIT Patna's 35-student rover team, building a scratch-built lunar rover prototype. Owned mechanical, electronics, and software architecture end to end.

---

## Open source

[Nav2](https://github.com/ros-navigation/navigation2) · [PlotJuggler](https://github.com/facontidavide/PlotJuggler) · [AutonomousVehiclesBeginnerGuide](https://github.com/AtsushiSakai/AutonomousVehiclesBeginnerGuide) · [POLKA](https://github.com/Pana1v/polka) (creator) · [Robotics Handbook](https://panav.gitbook.io/robotics-handbook)

---

## Stack

<p>
  <img src="https://img.shields.io/badge/ROS_2-Humble_%7C_Jazzy-22314E?style=flat-square&logo=ros&logoColor=white" />
  <img src="https://img.shields.io/badge/Nav2-1C1C1C?style=flat-square&logo=ros&logoColor=white" />
  <img src="https://img.shields.io/badge/SLAM_%26_Localization-1C1C1C?style=flat-square" />
  <img src="https://img.shields.io/badge/Sensor_Fusion-1C1C1C?style=flat-square" />
  <img src="https://img.shields.io/badge/Behavior_Trees-1C1C1C?style=flat-square" />
  <img src="https://img.shields.io/badge/TF2-1C1C1C?style=flat-square" />
</p>
<p>
  <img src="https://img.shields.io/badge/C%2B%2B17-00599C?style=flat-square&logo=c%2B%2B&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white" />
</p>
<p>
  <img src="https://img.shields.io/badge/JAX-D9603B?style=flat-square" />
  <img src="https://img.shields.io/badge/Flax-4B8BBE?style=flat-square" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenPI_%CF%800.5-1C1C1C?style=flat-square" />
  <img src="https://img.shields.io/badge/LIBERO-1C1C1C?style=flat-square" />
  <img src="https://img.shields.io/badge/DoRA_%2F_LoRA-1C1C1C?style=flat-square" />
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white" />
</p>
<p>
  <img src="https://img.shields.io/badge/PCL-1C1C1C?style=flat-square" />
  <img src="https://img.shields.io/badge/Eigen3-1C1C1C?style=flat-square" />
  <img src="https://img.shields.io/badge/Gazebo-FF6F00?style=flat-square&logo=gazebo&logoColor=white" />
  <img src="https://img.shields.io/badge/Isaac_Sim-76B900?style=flat-square&logo=nvidia&logoColor=white" />
  <img src="https://img.shields.io/badge/Jetson_Orin-76B900?style=flat-square&logo=nvidia&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" />
  <img src="https://img.shields.io/badge/CMake-064F8C?style=flat-square&logo=cmake&logoColor=white" />
  <img src="https://img.shields.io/badge/ESP32-1C1C1C?style=flat-square&logo=espressif&logoColor=white" />
  <img src="https://img.shields.io/badge/KiCAD-314CB0?style=flat-square&logo=kicad&logoColor=white" />
</p>

---

## Recognition

🥇 Gold Medal, Inter IIT Tech Meet, JLR Chiplet Challenge for ADAS (2023) · 🏁 Highest Indian team score in ICRA BARN since 2022 · 🤖 Captain, ABU Robocon 2024 · 🚀 Founder, IIT Patna Rover Team (IRoC-U 2024) · 📐 Top 0.5% JEE Advanced 2021

---

<div align="center">

<img src="https://github-profile-trophy.vercel.app/?username=Pana1v&theme=matrix&no-frame=true&no-bg=true&column=7&margin-w=6&margin-h=6" />

<br/>

<img height="150" src="https://github-readme-stats.vercel.app/api?username=Pana1v&show_icons=true&hide_border=true&bg_color=0d1117&title_color=E6EDF3&text_color=9CA3AF&icon_color=E6EDF3" />
<img height="150" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Pana1v&layout=compact&langs_count=8&hide_border=true&bg_color=0d1117&title_color=E6EDF3&text_color=9CA3AF" />

<br/>

<img height="150" src="https://github-readme-streak-stats.herokuapp.com?user=Pana1v&hide_border=true&background=0D1117&ring=9CA3AF&fire=E6EDF3&currStreakLabel=E6EDF3&sideLabels=9CA3AF&dates=6B7280" />

<br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Pana1v&theme=github-compact&hide_border=true&bg_color=0D1117&color=E6EDF3&line=76B900&point=E6EDF3&area=true" width="98%" />

<br/>

<img src="https://raw.githubusercontent.com/Pana1v/Pana1v/output/snake.svg" width="98%" alt="contribution snake"/>

</div>

<p align="center"><sub>Open to conversations about mobile robot autonomy, VLA policies, and point clouds that refuse to align.</sub></p>

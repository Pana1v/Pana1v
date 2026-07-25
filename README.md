<div align="center">
  <img src="./assets/banner.svg" width="100%" alt="Panav Arpit Raaj"/>
</div>

<p align="center">
  <a href="https://panav.netlify.app"><img src="https://img.shields.io/badge/PORTFOLIO-1A1A1A?style=flat-square&labelColor=1A1A1A&color=1A1A1A"/></a>
  <a href="https://panav.gitbook.io/robotics-handbook"><img src="https://img.shields.io/badge/HANDBOOK-8B7355?style=flat-square&labelColor=8B7355&color=8B7355"/></a>
  <a href="https://www.linkedin.com/in/panavraaj/"><img src="https://img.shields.io/badge/LINKEDIN-4A4540?style=flat-square&labelColor=4A4540&color=4A4540"/></a>
  <a href="mailto:praajarpit@gmail.com"><img src="https://img.shields.io/badge/EMAIL-6B6560?style=flat-square&labelColor=6B6560&color=6B6560"/></a>
</p>

<br/>

## About

I build software that lets mobile robots know where they are and decide what to do next: GPU-accelerated perception, 3D SLAM and localization, full autonomy stacks on ROS 2 and Nav2. Lately I've been working the other end too, fine-tuning vision-language-action policies and benchmarking what actually transfers to a real manipulator.

<table>
<tr><td><b>Now</b></td><td>Robotics Engineer, Level II</td><td><a href="https://eternal.ag">Eternal.ag</a>, Bangalore</td></tr>
<tr><td><b>2025–26</b></td><td>Robotics Software Apprentice</td><td>Origin (ex 10xConstruction.ai)</td></tr>
<tr><td><b>2024</b></td><td>Mobile Robotics Intern</td><td>Addverb Technologies</td></tr>
<tr><td><b>2021–25</b></td><td>B.Tech, Electrical & Electronics</td><td>IIT Patna</td></tr>
</table>

<br/>

## Selected work

<h3><sub>◼</sub> Robot Learning</h3>

**[openpi-DoRA](https://github.com/Pana1v)** &nbsp;·&nbsp; Weight-decomposed fine-tuning for π0.5. JAX/Flax overlay injecting DoRA into Physical Intelligence's policy, reimplemented for Gemma's einsum and FFN layers. Controlled DoRA-vs-LoRA sweeps across all four LIBERO suites: **92.0% vs 91.4%** average success at rank 8, winning 3 of 4.
<sub>`JAX` `Flax` `OpenPI` `LIBERO` `DoRA/LoRA`</sub>

**Intrinsic AI for Industry Challenge** &nbsp;·&nbsp; Solo entry, one week to deadline. Ground-truth policy at **285/300**, OpenCV baseline at 130/300, learned perception with ResNet18 and U-Net conditioned on TCP pose, port identity, board pose. Pushed ACT and SmolVLA under a tight data budget.
<sub>`ACT` `SmolVLA` `ResNet18` `U-Net`</sub>

**LEAP** &nbsp;·&nbsp; Pick-and-place sequencing as asymmetric TSP with a cycle-aware heterogeneous GNN. CP-SAT Hamiltonian circuit formulation replacing MTZ gave **5–7×**; imitation-learned arc pruning to O(Nk) gave a further **17.5× at N=200**, 0.06% optimality gap. *BRAIn Lab, IIT Patna. Manuscript in prep.*
<sub>`CP-SAT` `GNN` `Combinatorial Optimization`</sub>

<h3><sub>◼</sub> Perception & Navigation</h3>

**[POLKA](https://github.com/Pana1v/polka)** &nbsp;·&nbsp; Multi-LiDAR fusion for ROS 2. Merges heterogeneous PointCloud2 and LaserScan sources in one composable node, replacing the usual relay/filter/merge chain. SE(3) IMU deskewing with per-source overrides, footprint exclusion, voxel downsampling, optional CUDA. Humble and Jazzy.
<sub>`C++17` `CUDA` `PCL` `Eigen3`</sub>

**GO-SLAM** &nbsp;·&nbsp; Full SLAM from scratch: GICP front-end, pose-graph back-end, loop closure. Custom Levenberg–Marquardt solvers for both, no external optimization libraries. Fed by deskewed LiDAR from Polka, benchmarked on KITTI.
<sub>`ROS 2` `GICP` `Pose Graph Optimization` `KITTI`</sub>

**At Eternal** &nbsp;·&nbsp; GPU-accelerated SLAM and Nav2 stack under **40% CPU on Jetson Orin**, automated per-robot LiDAR↔IMU extrinsic calibration, CI/CD, parameter snapshots inside rosbags.

**At Origin** &nbsp;·&nbsp; Swerve motion model for Nav2 MPPI. Lower-latency collision monitor via composable nodes. Kidnapped-robot recovery using genetic algorithms plus ambiguity detection. Lichtblick, a TypeScript/ROS 2 viz interface that cut peak CPU **120% → 26%** versus Foxglove.

<h3><sub>◼</sub> Competition</h3>

**[ICRA BARN Challenge 2026](https://cs.gmu.edu/~xiao/Research/BARN_Challenge/BARN_Challenge26.html)** &nbsp;·&nbsp; Breadcrumb Explorer, built from scratch instead of tuning a baseline. Mapless, no SLAM, no laser odometry. An odom-frame breadcrumb memory marks trajectories *tasty* or *stale* so path selection improves across trials despite 270° coverage, wheel slip, and IMU drift. **0.3682/0.5 on first submission, highest by an Indian team since 2022.** 76% zero-shot across 300 Gazebo courses.

**ABU Robocon 2023–24** &nbsp;·&nbsp; Captain, 60+ member team. National Finals, one of two IITs to qualify, highest score among IIT teams in 2024. Custom PCBs for motor control and power, heterogeneous controllers (Cube Orange, Pi, ESP32), multi-bot coordination over ROS.

**ISRO Robotics Challenge (IRoC-U) 2024** &nbsp;·&nbsp; Founded and led IIT Patna's 35-student rover team, building a scratch-built lunar rover prototype. Owned mechanical, electronics, and software architecture end to end.

<br/>

## Achievements

- **Gold Medal**, Inter IIT Tech Meet, Jaguar Land Rover Chiplet Challenge for ADAS (2023)
- **Highest score by an Indian team** in the ICRA BARN Challenge since the benchmark began in 2022
- **Captain**, ABU Robocon 2024, highest score among IIT teams at National Finals
- **Founder**, IIT Patna Rover Team, ISRO Robotics Challenge 2024
- **Top 0.5%**, JEE Advanced 2021 · **Rank 8 (Karnataka)**, NSTSE 2020

<br/>

## Open source

- **[POLKA](https://github.com/Pana1v/polka)** · creator, multi-LiDAR fusion node for ROS 2
- **[Nav2](https://github.com/ros-navigation/navigation2)** · contributor, ROS 2 Navigation stack
- **[PlotJuggler](https://github.com/facontidavide/PlotJuggler)** · contributor, ROS time-series visualization
- **[AutonomousVehiclesBeginnerGuide](https://github.com/AtsushiSakai/AutonomousVehiclesBeginnerGuide)** · contributor
- **[Robotics Handbook](https://panav.gitbook.io/robotics-handbook)** · an evolving reference on ROS 2, Nav2, SLAM, sensor fusion

<br/>

## Stack

<p>
<img src="https://img.shields.io/badge/ROS_2-Humble_|_Jazzy-F5F1E8?style=flat-square&labelColor=1A1A1A&color=E8E2D5" />
<img src="https://img.shields.io/badge/Nav2-F5F1E8?style=flat-square&labelColor=1A1A1A&color=E8E2D5" />
<img src="https://img.shields.io/badge/SLAM-&_Localization-F5F1E8?style=flat-square&labelColor=1A1A1A&color=E8E2D5" />
<img src="https://img.shields.io/badge/Sensor_Fusion-F5F1E8?style=flat-square&labelColor=1A1A1A&color=E8E2D5" />
<img src="https://img.shields.io/badge/Behavior_Trees-F5F1E8?style=flat-square&labelColor=1A1A1A&color=E8E2D5" />
<img src="https://img.shields.io/badge/TF2-F5F1E8?style=flat-square&labelColor=1A1A1A&color=E8E2D5" />
</p>

<p>
<img src="https://img.shields.io/badge/C++17-F5F1E8?style=flat-square&labelColor=1A1A1A&color=E8E2D5" />
<img src="https://img.shields.io/badge/Python-F5F1E8?style=flat-square&labelColor=1A1A1A&color=E8E2D5" />
<img src="https://img.shields.io/badge/CUDA-F5F1E8?style=flat-square&labelColor=1A1A1A&color=E8E2D5" />
<img src="https://img.shields.io/badge/TypeScript-F5F1E8?style=flat-square&labelColor=1A1A1A&color=E8E2D5" />
<img src="https://img.shields.io/badge/Bash-F5F1E8?style=flat-square&labelColor=1A1A1A&color=E8E2D5" />
</p>

<p>
<img src="https://img.shields.io/badge/JAX-F5F1E8?style=flat-square&labelColor=8B7355&color=EFE7D8" />
<img src="https://img.shields.io/badge/Flax-F5F1E8?style=flat-square&labelColor=8B7355&color=EFE7D8" />
<img src="https://img.shields.io/badge/PyTorch-F5F1E8?style=flat-square&labelColor=8B7355&color=EFE7D8" />
<img src="https://img.shields.io/badge/OpenPI_π0.5-F5F1E8?style=flat-square&labelColor=8B7355&color=EFE7D8" />
<img src="https://img.shields.io/badge/LIBERO-F5F1E8?style=flat-square&labelColor=8B7355&color=EFE7D8" />
<img src="https://img.shields.io/badge/DoRA_|_LoRA-F5F1E8?style=flat-square&labelColor=8B7355&color=EFE7D8" />
<img src="https://img.shields.io/badge/OpenCV-F5F1E8?style=flat-square&labelColor=8B7355&color=EFE7D8" />
</p>

<p>
<img src="https://img.shields.io/badge/PCL-F5F1E8?style=flat-square&labelColor=4A4540&color=E8E2D5" />
<img src="https://img.shields.io/badge/Eigen3-F5F1E8?style=flat-square&labelColor=4A4540&color=E8E2D5" />
<img src="https://img.shields.io/badge/Gazebo-F5F1E8?style=flat-square&labelColor=4A4540&color=E8E2D5" />
<img src="https://img.shields.io/badge/Isaac_Sim-F5F1E8?style=flat-square&labelColor=4A4540&color=E8E2D5" />
<img src="https://img.shields.io/badge/Jetson_Orin-F5F1E8?style=flat-square&labelColor=4A4540&color=E8E2D5" />
<img src="https://img.shields.io/badge/Docker-F5F1E8?style=flat-square&labelColor=4A4540&color=E8E2D5" />
<img src="https://img.shields.io/badge/GitHub_Actions-F5F1E8?style=flat-square&labelColor=4A4540&color=E8E2D5" />
<img src="https://img.shields.io/badge/CMake-F5F1E8?style=flat-square&labelColor=4A4540&color=E8E2D5" />
<img src="https://img.shields.io/badge/ESP32-F5F1E8?style=flat-square&labelColor=4A4540&color=E8E2D5" />
<img src="https://img.shields.io/badge/KiCAD-F5F1E8?style=flat-square&labelColor=4A4540&color=E8E2D5" />
</p>

<br/>

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=Pana1v&show_icons=true&hide_border=true&hide_title=true&bg_color=00000000&text_color=A9A196&icon_color=C4B59B&ring_color=C4B59B" />
  <img height="150" src="https://github-readme-stats.vercel.app/api?username=Pana1v&show_icons=true&hide_border=true&hide_title=true&bg_color=00000000&text_color=4A4540&icon_color=8B7355&ring_color=8B7355" alt="GitHub stats" />
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=Pana1v&layout=compact&langs_count=8&hide_border=true&hide_title=true&bg_color=00000000&text_color=A9A196" />
  <img height="150" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Pana1v&layout=compact&langs_count=8&hide_border=true&hide_title=true&bg_color=00000000&text_color=4A4540" alt="Top languages" />
</picture>

<br/>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com?user=Pana1v&hide_border=true&background=00000000&stroke=2A2622&ring=C4B59B&fire=C4B59B&currStreakNum=F5F1E8&currStreakLabel=C4B59B&sideNums=A9A196&sideLabels=A9A196&dates=6B6560" />
  <img height="150" src="https://streak-stats.demolab.com?user=Pana1v&hide_border=true&background=00000000&stroke=DDD5C7&ring=8B7355&fire=8B7355&currStreakNum=1A1A1A&currStreakLabel=8B7355&sideNums=4A4540&sideLabels=4A4540&dates=6B6560" alt="Contribution streak" />
</picture>

</div>

<br/>

<p align="center"><sub>Open to conversations about mobile robot autonomy, VLA policies, and point clouds that refuse to align.</sub></p>

<div align="center">
  <img src="./assets/banner.svg" width="100%" alt="Panav Arpit Raaj"/>
</div>

<p align="center">
  <a href="https://panav.netlify.app"><img src="https://img.shields.io/badge/PORTFOLIO-FFFFFF?style=flat-square&labelColor=000000&color=000000" alt="PORTFOLIO"/></a>
  <a href="https://panav.gitbook.io/robotics-handbook"><img src="https://img.shields.io/badge/HANDBOOK-FFFFFF?style=flat-square&labelColor=000000&color=000000" alt="HANDBOOK"/></a>
  <a href="https://www.linkedin.com/in/panavraaj/"><img src="https://img.shields.io/badge/LINKEDIN-FFFFFF?style=flat-square&labelColor=000000&color=000000" alt="LINKEDIN"/></a>
  <a href="mailto:praajarpit@gmail.com"><img src="https://img.shields.io/badge/EMAIL-FFFFFF?style=flat-square&labelColor=000000&color=000000" alt="EMAIL"/></a>
</p>

<br/>

## About

I build software that lets mobile robots know where they are and decide what to do next: GPU-accelerated perception, 3D SLAM and localization, full autonomy stacks on ROS 2 and Nav2. Lately I've been working the other end too, fine-tuning vision-language-action policies and benchmarking what actually transfers to a real manipulator.

<table>
<tr><td><b>Now</b></td><td>Robotics Engineer, Level II</td><td><a href="https://eternal.ag">Eternal.ag</a>, Bangalore</td></tr>
<tr><td><b>2025–26</b></td><td>Robotics Software Apprentice</td><td>Origin (ex 10xConstruction.ai)</td></tr>
<tr><td><b>2024</b></td><td>Mobile Robotics Intern</td><td>Addverb Technologies</td></tr>
<tr><td><b>2021–25</b></td><td>B.Tech, Electrical &amp; Electronics</td><td>IIT Patna</td></tr>
</table>

<br/>

## Selected work

<img src="./assets/h-robot-learning.svg" height="26" alt="Robot Learning"/>

<table>
<tr>
<td width="250"><img src="https://panav.netlify.app/projects/openpi-dora-motion.gif" width="240" alt="openpi-DoRA"/></td>
<td>

**[openpi-DoRA](https://github.com/Pana1v)** &nbsp;·&nbsp; Weight-decomposed fine-tuning for π0.5. JAX/Flax overlay injecting DoRA into Physical Intelligence's policy, reimplemented for Gemma's einsum and FFN layers. Controlled DoRA-vs-LoRA sweeps across all four LIBERO suites: **92.0% vs 91.4%** average success at rank 8, winning 3 of 4.

<sub>`JAX` `Flax` `OpenPI` `LIBERO` `DoRA/LoRA`</sub>

</td>
</tr>
</table>

<table>
<tr>
<td width="250"><img src="https://panav.netlify.app/writing/intrinsic-challenge-views.png" width="240" alt="Intrinsic AI for Industry Challenge"/></td>
<td>

**Intrinsic AI for Industry Challenge** &nbsp;·&nbsp; Solo entry, one week to deadline. Ground-truth policy at **285/300**, OpenCV baseline at 130/300, learned perception with ResNet18 and U-Net conditioned on TCP pose, port identity, board pose. Pushed ACT and SmolVLA under a tight data budget.

<sub>`ACT` `SmolVLA` `ResNet18` `U-Net`</sub>

</td>
</tr>
</table>

**LEAP** &nbsp;·&nbsp; Pick-and-place sequencing as asymmetric TSP with a cycle-aware heterogeneous GNN. CP-SAT Hamiltonian circuit formulation replacing MTZ gave **5–7×**; imitation-learned arc pruning to O(Nk) gave a further **17.5× at N=200**, 0.06% optimality gap. *BRAIn Lab, IIT Patna. Manuscript in prep.*
<sub>`CP-SAT` `GNN` `Combinatorial Optimization`</sub>

<br/>

<img src="./assets/h-perception.svg" height="26" alt="Perception and Navigation"/>

**[POLKA](https://github.com/Pana1v/polka)** &nbsp;·&nbsp; Multi-LiDAR fusion for ROS 2. Merges heterogeneous PointCloud2 and LaserScan sources in one composable node, replacing the usual relay/filter/merge chain. SE(3) IMU deskewing with per-source overrides, footprint exclusion, voxel downsampling, optional CUDA. Humble and Jazzy.
<sub>`C++17` `CUDA` `PCL` `Eigen3`</sub>

<table>
<tr>
<td width="250"><img src="https://panav.netlify.app/projects/go-slam.png" width="240" alt="GO-SLAM"/></td>
<td>

**GO-SLAM** &nbsp;·&nbsp; Full SLAM from scratch: GICP front-end, pose-graph back-end, loop closure. Custom Levenberg–Marquardt solvers for both, no external optimization libraries. Fed by deskewed LiDAR from Polka, benchmarked on KITTI.

<sub>`ROS 2` `GICP` `Pose Graph Optimization` `KITTI`</sub>

</td>
</tr>
</table>

**At Eternal** &nbsp;·&nbsp; GPU-accelerated SLAM and Nav2 stack under **40% CPU on Jetson Orin**, automated per-robot LiDAR↔IMU extrinsic calibration, CI/CD, parameter snapshots inside rosbags.

<table>
<tr>
<td width="250"><img src="./assets/lichtblick.png" width="240" alt="Lichtblick"/></td>
<td>

**At Origin** &nbsp;·&nbsp; Swerve motion model for Nav2 MPPI. Lower-latency collision monitor via composable nodes. Kidnapped-robot recovery using genetic algorithms plus ambiguity detection. Lichtblick, a TypeScript/ROS 2 viz interface that cut peak CPU **120% → 26%** versus Foxglove.

</td>
</tr>
</table>

<br/>

<img src="./assets/h-competition.svg" height="26" alt="Competition"/>

<table>
<tr>
<td width="250"><img src="https://panav.netlify.app/projects/barn-motion.gif" width="240" alt="ICRA BARN Challenge 2026"/></td>
<td>

**[ICRA BARN Challenge 2026](https://cs.gmu.edu/~xiao/Research/BARN_Challenge/BARN_Challenge26.html)** &nbsp;·&nbsp; Breadcrumb Explorer, built from scratch instead of tuning a baseline. Mapless, no SLAM, no laser odometry. An odom-frame breadcrumb memory marks trajectories *tasty* or *stale* so path selection improves across trials despite 270° coverage, wheel slip, and IMU drift. **0.3682/0.5 on first submission, highest by an Indian team since 2022.** 76% zero-shot across 300 Gazebo courses.

</td>
</tr>
</table>

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
<img src="https://img.shields.io/badge/ROS_2-Humble_|_Jazzy-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/Nav2-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/SLAM_&_Localization-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/Sensor_Fusion-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/Behavior_Trees-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/TF2-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
</p>

<p>
<img src="https://img.shields.io/badge/C++17-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/Python-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/CUDA-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/TypeScript-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/Bash-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
</p>

<p>
<img src="https://img.shields.io/badge/JAX-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/Flax-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/PyTorch-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/OpenPI_π0.5-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/LIBERO-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/DoRA_|_LoRA-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/OpenCV-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
</p>

<p>
<img src="https://img.shields.io/badge/PCL-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/Eigen3-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/Gazebo-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/Isaac_Sim-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/Jetson_Orin-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/Docker-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/GitHub_Actions-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/CMake-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/ESP32-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
<img src="https://img.shields.io/badge/KiCAD-FFFFFF?style=flat-square&labelColor=000000&color=000000" />
</p>

<br/>

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=Pana1v&show_icons=true&hide_border=true&hide_title=true&bg_color=00000000&text_color=FFFFFF&icon_color=FFFFFF&ring_color=FFFFFF" />
  <img height="150" src="https://github-readme-stats.vercel.app/api?username=Pana1v&show_icons=true&hide_border=true&hide_title=true&bg_color=00000000&text_color=000000&icon_color=000000&ring_color=000000" alt="GitHub stats" />
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=Pana1v&layout=compact&langs_count=8&hide_border=true&hide_title=true&bg_color=00000000&text_color=FFFFFF" />
  <img height="150" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Pana1v&layout=compact&langs_count=8&hide_border=true&hide_title=true&bg_color=00000000&text_color=000000" alt="Top languages" />
</picture>

<br/>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com?user=Pana1v&hide_border=true&background=00000000&stroke=FFFFFF&ring=FFFFFF&fire=FFFFFF&currStreakNum=FFFFFF&currStreakLabel=FFFFFF&sideNums=FFFFFF&sideLabels=FFFFFF&dates=FFFFFF" />
  <img height="150" src="https://streak-stats.demolab.com?user=Pana1v&hide_border=true&background=00000000&stroke=000000&ring=000000&fire=000000&currStreakNum=000000&currStreakLabel=000000&sideNums=000000&sideLabels=000000&dates=000000" alt="Contribution streak" />
</picture>

</div>

<br/>

<p align="center"><sub>Open to conversations about mobile robot autonomy, VLA policies, and point clouds that refuse to align.</sub></p>

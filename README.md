<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&height=170&color=0a0a0a&text=Panav%20Arpit%20Raaj&fontSize=58&fontColor=ff1f3d&fontAlign=50&fontAlignY=42&desc=PERCEPTION%20%C2%B7%20SLAM%20%C2%B7%20NAVIGATION%20%C2%B7%20ROBOT%20LEARNING&descSize=14&descAlign=50&descAlignY=60&descColor=cccccc" width="100%" alt="Panav Arpit Raaj"/>
</div>

<p align="center">
  <a href="mailto:praajarpit@gmail.com">praajarpit@gmail.com</a> &nbsp;·&nbsp; <a href="mailto:panav.raaj@hotmail.com">panav.raaj@hotmail.com</a>
</p>

<p align="center">
  <a href="https://panav.netlify.app"><img src="https://img.shields.io/badge/PORTFOLIO-PANAV.NETLIFY.APP-FFFFFF?style=for-the-badge&labelColor=0a0a0a&color=0a0a0a" alt="Portfolio: panav.netlify.app"/></a>
  <a href="https://panav.gitbook.io/robotics-handbook"><img src="https://img.shields.io/badge/HANDBOOK-FFFFFF?style=for-the-badge&labelColor=0a0a0a&color=0a0a0a" alt="HANDBOOK"/></a>
  <a href="https://pana1v.substack.com"><img src="https://img.shields.io/badge/SUBSTACK-FFFFFF?style=for-the-badge&labelColor=0a0a0a&color=0a0a0a" alt="SUBSTACK"/></a>
  <a href="https://www.linkedin.com/in/panavraaj/"><img src="https://img.shields.io/badge/LINKEDIN-FFFFFF?style=for-the-badge&labelColor=0a0a0a&color=0a0a0a" alt="LINKEDIN"/></a>
  <a href="mailto:praajarpit@gmail.com"><img src="https://img.shields.io/badge/EMAIL-FFFFFF?style=for-the-badge&labelColor=0a0a0a&color=0a0a0a" alt="praajarpit@gmail.com"/></a>
</p>

<br/>

## About

Robotics Engineer. I build perception, SLAM, navigation, and robot-learning systems: ROS 2, Nav2, CUDA pointclouds, JAX and PyTorch VLAs. Based in Bangalore at Eternal.ag; previously Addverb (mobile robotics intern) and Origin (sweep motion models, Nav2 MPPI). B.Tech EEE, IIT Patna.

Projects and writing: [panav.netlify.app](https://panav.netlify.app).

<br/>

## Selected work

<table>
<tr>
<td width="260"><img src="https://panav.netlify.app/projects/openpi-dora-motion.gif" width="240" alt="openpi-DoRA"/></td>
<td>

**[openpi-DoRA](https://github.com/Pana1v/openpi-dora)** · DoRA fine-tuning for pi0.5 in JAX/Flax, reimplemented for Gemma einsum and FFN layers. DoRA vs LoRA across all four LIBERO suites: 92.0% vs 91.4% at rank 8, winning 3 of 4.

<sub>`JAX` `Flax` `OpenPI` `LIBERO` `DoRA/LoRA`</sub>

</td>
</tr>
</table>

<table>
<tr>
<td width="260"><img src="https://panav.netlify.app/writing/intrinsic-challenge-views.png" width="240" alt="Intrinsic AI for Industry Challenge"/></td>
<td>

**Intrinsic AI for Industry Challenge** · Solo entry, one week. Ground-truth policy 285/300, OpenCV baseline 130/300, learned perception with ResNet18 and U-Net on TCP, port and board pose. ACT and SmolVLA under a tight data budget. [Write-up ↗](https://substack.com/@panav1/p-198501217)

<sub>`ACT` `SmolVLA` `ResNet18` `U-Net`</sub>

</td>
</tr>
</table>

<table>
<tr>
<td width="260"><img src="https://panav.netlify.app/projects/ego-hamer-compare.jpg" width="240" alt="Egocentric data pipeline"/></td>
<td>

**Egocentric Data Pipeline** · First-person video to annotated robot-learning sequences. HaMeR and WiLoR hand tracking and MANO pose, FastFoundationStereo depth at 9x real-time, automated segmentation and prelabelling. Hand tracking $0.30 per video hour; prelabelling $7.00 to $0.80 per hour.

<sub>`HaMeR` `WiLoR` `MANO` `FoundationStereo` `VLMs`</sub>

</td>
</tr>
</table>

<table>
<tr>
<td width="260"><img src="https://panav.netlify.app/projects/gnn-pipeline.svg" width="240" alt="LEAP"/></td>
<td>

**LEAP** · Pick-and-place as asymmetric TSP with a cycle-aware heterogeneous GNN. CP-SAT Hamiltonian circuit replacing MTZ gave 5-7x; arc pruning to O(Nk) added 17.5x at N=200, 0.06% optimality gap. BRAIn Lab, IIT Patna. Manuscript in prep.

<sub>`CP-SAT` `GNN` `Combinatorial Optimization`</sub>

</td>
</tr>
</table>

<table>
<tr>
<td width="260"><img src="https://panav.netlify.app/projects/go-slam.png" width="240" alt="GO-SLAM"/></td>
<td>

**[GO-SLAM](https://github.com/Pana1v/go-slam)** · SLAM from scratch: GICP front-end, pose-graph back-end, loop closure. Custom Levenberg-Marquardt solvers, no external optimization libraries. Fed by deskewed LiDAR from Polka, benchmarked on KITTI.

<sub>`ROS 2` `GICP` `Pose Graph Optimization` `KITTI`</sub>

</td>
</tr>
</table>

<table>
<tr>
<td width="260" align="center"><img src="https://img.shields.io/badge/AT_ETERNAL-FFFFFF?style=for-the-badge&labelColor=0a0a0a&color=0a0a0a" alt="At Eternal"/></td>
<td>

**At Eternal** · GPU-accelerated SLAM and navigation on Nav2 for AgTech: 40% CPU on Jetson Orin, CUDA pointcloud processing and deskewing at 40 ms latency, automated per-robot extrinsic calibration (LiDAR-to-IMU, LiDAR-to-LiDAR), CI with rosbag parameter snapshots.

</td>
</tr>
</table>

<table>
<tr>
<td width="260"><img src="https://panav.netlify.app/gallery/origin.jpg" width="240" alt="At Origin"/></td>
<td>

**At Origin** · Swerve motion model for Nav2 MPPI, lower-latency composable collision monitor, kidnapped-robot recovery with genetic algorithms plus ambiguity detection. Lichtblick, a TypeScript/ROS 2 viz interface: peak CPU 120% to 26% vs Foxglove.

</td>
</tr>
</table>

<table>
<tr>
<td width="260"><img src="https://panav.netlify.app/projects/barn-motion.gif" width="240" alt="ICRA BARN Challenge 2026"/></td>
<td>

**[ICRA BARN Challenge 2026](https://cs.gmu.edu/~xiao/Research/BARN_Challenge/BARN_Challenge26.html)** · Breadcrumb Explorer, built from scratch - no SLAM, no laser odometry. Odom-frame breadcrumb memory marks trajectories tasty or stale, improving path selection across trials despite 270 degree coverage, wheel slip, IMU drift. 0.3682/0.5 first submission, highest by an Indian team since 2022. 76% zero-shot across 300 Gazebo courses.

</td>
</tr>
</table>

<table>
<tr>
<td width="260"><img src="https://panav.netlify.app/gallery/robocon-2024.jpg" width="240" alt="ABU Robocon 2024, IIT Patna"/></td>
<td>

**ABU Robocon 2023-24** · Captain, 60+ team. National Finals; one of two IITs to qualify, highest score among IIT teams in 2024. Custom motor-control and power PCBs, heterogeneous controllers (Cube Orange, Pi, ESP32), multi-bot ROS coordination.

</td>
</tr>
</table>

<table>
<tr>
<td width="260"><img src="https://panav.netlify.app/gallery/isro-rover.jpg" width="240" alt="IRoC-U 2024 rover"/></td>
<td>

**ISRO Robotics Challenge 2024** · Founded and led IIT Patna's 35-student rover team; scratch-built lunar rover prototype, mechanical, electronics and software end to end.

</td>
</tr>
</table>

<br/>

## Achievements

- Gold Medal, Inter IIT Tech Meet, Jaguar Land Rover Chiplet Challenge for ADAS (2023)
- Highest score by an Indian team, ICRA BARN Challenge since 2022
- Captain, ABU Robocon 2024, highest score among IIT teams at National Finals
- Founder, IIT Patna Rover Team, ISRO Robotics Challenge 2024
- Top 0.5%, JEE Advanced 2021 · Rank 8, Karnataka, NSTSE 2020

<p align="center">
  <img src="https://panav.netlify.app/gallery/inter-iit-gold.jpg" height="160" alt="Inter IIT Tech gold medal"/>
  <img src="https://panav.netlify.app/projects/robocon-robot.jpg" height="160" alt="Robocon robot"/>
  <img src="https://panav.netlify.app/gallery/addverb.jpg" height="160" alt="At Addverb"/>
</p>

<br/>

## Writing

<table>
<tr>
<td width="260"><img src="https://panav.netlify.app/writing/deskew-cover.jpg" width="240" alt="To deskew LiDAR data or not?"/></td>
<td>

**[To deskew LiDAR data or not?](https://pana1v.substack.com/p/to-deskew-lidar-data-or-not)** · Why and when deskewing point clouds matters, compared against GLIM, rko_lio and LIO-SAM on public datasets.

**[A Journey Through the Intrinsic AI for Industry Challenge](https://substack.com/@panav1/p-198501217)** · Exhausting classical approaches first to dodge the data wall in imitation learning.

**[The Robotics Handbook](https://panav.gitbook.io/robotics-handbook)** · Living field guide: kinematics, SLAM, controls, perception.

</td>
</tr>
</table>

<br/>

## Open source

- POLKA, creator, multi-LiDAR fusion node for ROS 2
- Nav2, contributor
- PlotJuggler, contributor
- AutonomousVehicleControlBeginnersGuide, contributor
- Robotics Handbook, evolving reference on ROS 2, Nav2, SLAM, sensor fusion

<br/>

## Stack

<p>
<img src="https://img.shields.io/badge/ROS_2-Humble_|_Jazzy-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/Nav2-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/SLAM_&_Localization-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/Sensor_Fusion-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/Behavior_Trees-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/TF2-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
</p>

<p>
<img src="https://img.shields.io/badge/C%2B%2B17-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/Python-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/CUDA-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/TypeScript-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/Bash-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
</p>

<p>
<img src="https://img.shields.io/badge/JAX-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/Flax-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/PyTorch-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/OpenPI_pi0.5-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/LIBERO-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/DoRA_|_LoRA-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/OpenCV-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
</p>

<p>
<img src="https://img.shields.io/badge/PCL-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/Eigen3-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/Gazebo-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/Isaac_Sim-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/Jetson_Orin-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/Docker-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/GitHub_Actions-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/CMake-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/ESP32-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
<img src="https://img.shields.io/badge/KiCAD-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" />
</p>

<br/>

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=Pana1v&show_icons=true&hide_border=true&hide_title=true&bg_color=00000000&text_color=FFFFFF&icon_color=ff1f3d&ring_color=ff1f3d" />
  <img height="160" src="https://github-readme-stats.vercel.app/api?username=Pana1v&show_icons=true&hide_border=true&hide_title=true&bg_color=00000000&text_color=000000&icon_color=ff1f3d&ring_color=ff1f3d" alt="GitHub stats" />
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=Pana1v&layout=compact&langs_count=8&hide_border=true&hide_title=true&bg_color=00000000&text_color=FFFFFF" />
  <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Pana1v&layout=compact&langs_count=8&hide_border=true&hide_title=true&bg_color=00000000&text_color=000000" alt="Top languages" />
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com?user=Pana1v&hide_border=true&background=00000000&stroke=FFFFFF&ring=ff1f3d&fire=ff1f3d&currStreakNum=FFFFFF&currStreakLabel=FFFFFF&sideNums=FFFFFF&sideLabels=FFFFFF&dates=FFFFFF" />
  <img height="160" src="https://streak-stats.demolab.com?user=Pana1v&hide_border=true&background=00000000&stroke=000000&ring=ff1f3d&fire=ff1f3d&currStreakNum=000000&currStreakLabel=000000&sideNums=000000&sideLabels=000000&dates=000000" alt="Contribution streak" />
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-activity-graph.vercel.app/graph?username=Pana1v&hide_border=true&bg_color=00000000&color=ff1f3d&line=ff1f3d&point=ff1f3d&title_color=FFFFFF&area=true&area_color=ff1f3d" />
  <img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=Pana1v&hide_border=true&bg_color=00000000&color=ff1f3d&line=ff1f3d&point=ff1f3d&title_color=000000&area=true&area_color=ff1f3d" alt="Contribution activity" />
</picture>

</div>

<br/>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=Pana1v&style=for-the-badge&label=PROFILE+VIEWS&color=0a0a0a" alt="Profile views"/>
  <a href="https://github.com/Pana1v?tab=followers"><img src="https://img.shields.io/github/followers/Pana1v?style=for-the-badge&label=FOLLOWERS&labelColor=0a0a0a&color=0a0a0a" alt="Followers"/></a>
  <a href="https://github.com/Pana1v/polka"><img src="https://img.shields.io/github/stars/Pana1v/polka?style=for-the-badge&label=POLKA%20STARS&labelColor=0a0a0a&color=0a0a0a" alt="POLKA stars"/></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/BASED_IN-BANGALORE,_IN-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" alt="Based in Bangalore"/>
  <img src="https://img.shields.io/badge/OPEN_TO-COLLABORATION_&_CONVERSATION-FFFFFF?style=flat-square&labelColor=0a0a0a&color=0a0a0a" alt="Open to collaboration"/>
</p>

<p align="center"><sub>Open to conversations about mobile robot autonomy, VLA policies, and point clouds that refuse to align. More at <a href="https://panav.netlify.app">panav.netlify.app</a>.</sub></p>

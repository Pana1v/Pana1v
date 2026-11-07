<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&height=200&color=000000&text=Panav%20Arpit%20Raaj&fontSize=60&fontColor=FFFFFF&fontAlign=50&fontAlignY=40&desc=PERCEPTION%20%C2%B7%20SLAM%20%C2%B7%20NAVIGATION%20%C2%B7%20ROBOT%20LEARNING&descSize=15&descAlign=50&descAlignY=62" width="100%" alt="Panav Arpit Raaj"/>
</div>

<p align="center">
  <a href="https://panav.netlify.app"><b>panav.netlify.app</b></a> &nbsp;·&nbsp; <a href="mailto:praajarpit@gmail.com">praajarpit@gmail.com</a> &nbsp;·&nbsp; <a href="mailto:panav.raaj@hotmail.com">panav.raaj@hotmail.com</a>
</p>

<p align="center">
  <a href="https://panav.netlify.app"><img src="https://img.shields.io/badge/PORTFOLIO-PANAV.NETLIFY.APP-FFFFFF?style=flat-square&labelColor=000000&color=000000" alt="Portfolio: panav.netlify.app"/></a>
  <a href="https://panav.gitbook.io/robotics-handbook"><img src="https://img.shields.io/badge/HANDBOOK-FFFFFF?style=flat-square&labelColor=000000&color=000000" alt="HANDBOOK"/></a>
  <a href="https://pana1v.substack.com"><img src="https://img.shields.io/badge/SUBSTACK-FFFFFF?style=flat-square&labelColor=000000&color=000000" alt="SUBSTACK"/></a>
  <a href="https://www.linkedin.com/in/panavraaj/"><img src="https://img.shields.io/badge/LINKEDIN-FFFFFF?style=flat-square&labelColor=000000&color=000000" alt="LINKEDIN"/></a>
  <a href="mailto:praajarpit@gmail.com"><img src="https://img.shields.io/badge/EMAIL-FFFFFF?style=flat-square&labelColor=000000&color=000000" alt="praajarpit@gmail.com"/></a>
</p>

<br/>

## About

I write autonomy stacks for robots that make decisions in unpredictable places: warehouses, farms, construction sites. That means GPU-accelerated perception, 3D SLAM and localization, and full navigation stacks on ROS 2 and Nav2. Lately I've been working the other end too, fine-tuning vision-language-action policies and building data pipelines for robot learning.

Projects, writing and the full work history live on **[panav.netlify.app](https://panav.netlify.app)**.

<table>
<tr><td><b>Now</b></td><td>Robotics Engineer, Level II</td><td><a href="https://eternal.ag">Eternal.ag</a>, Bangalore</td></tr>
<tr><td><b>2025–26</b></td><td>Robotics Software Apprentice</td><td>Origin (ex 10xConstruction.ai)</td></tr>
<tr><td><b>2024</b></td><td>Mobile Robotics Intern</td><td>Addverb Technologies</td></tr>
<tr><td><b>2021–25</b></td><td>B.Tech, Electrical &amp; Electronics</td><td>IIT Patna</td></tr>
</table>

<br/>

## Selected work

<img src="https://img.shields.io/badge/ROBOT_LEARNING-FFFFFF?style=for-the-badge&labelColor=000000&color=000000" alt="Robot Learning"/>

<table>
<tr>
<td width="250"><img src="https://panav.netlify.app/projects/openpi-dora-motion.gif" width="240" alt="openpi-DoRA"/></td>
<td>

**[openpi-DoRA](https://github.com/Pana1v/openpi-dora)** &nbsp;·&nbsp; Weight-decomposed fine-tuning for π0.5. JAX/Flax overlay injecting DoRA into Physical Intelligence's policy, reimplemented for Gemma's einsum and FFN layers. Controlled DoRA-vs-LoRA sweeps across all four LIBERO suites: **92.0% vs 91.4%** average success at rank 8, winning 3 of 4.

<sub>`JAX` `Flax` `OpenPI` `LIBERO` `DoRA/LoRA`</sub>

</td>
</tr>
</table>

<table>
<tr>
<td width="250"><img src="https://panav.netlify.app/writing/intrinsic-challenge-views.png" width="240" alt="Intrinsic AI for Industry Challenge"/></td>
<td>

**Intrinsic AI for Industry Challenge** &nbsp;·&nbsp; Solo entry, one week to deadline. Ground-truth policy at **285/300**, OpenCV baseline at 130/300, learned perception with ResNet18 and U-Net conditioned on TCP pose, port identity, board pose. Pushed ACT and SmolVLA under a tight data budget. [Write-up ↗](https://substack.com/@panav1/p-198501217)

<sub>`ACT` `SmolVLA` `ResNet18` `U-Net`</sub>

</td>
</tr>
</table>

<table>
<tr>
<td width="250"><img src="https://panav.netlify.app/projects/ego-hamer-compare.jpg" width="240" alt="Egocentric data pipeline"/></td>
<td>

**Egocentric Data Pipeline** &nbsp;·&nbsp; Turns long first-person videos into structured, annotated sequences for robot learning. HaMeR and WiLoR for hand tracking and MANO pose, FastFoundationStereo for depth at **9× real-time**, automated segmentation and prelabelling for task, subtask, difficulty and venue. Hand tracking at **$0.30 per video hour**, prelabelling cut from **$7.00 to $0.80 per hour**. 

<sub>`HaMeR` `WiLoR` `MANO` `FoundationStereo` `VLMs`</sub>

</td>
</tr>
</table>

<table>
<tr>
<td width="250"><img src="https://panav.netlify.app/projects/gnn-pipeline.svg" width="240" alt="LEAP"/></td>
<td>

**LEAP** &nbsp;·&nbsp; Pick-and-place sequencing as asymmetric TSP with a cycle-aware heterogeneous GNN. CP-SAT Hamiltonian circuit formulation replacing MTZ gave **5–7×**; imitation-learned arc pruning to O(Nk) gave a further **17.5× at N=200**, 0.06% optimality gap. *BRAIn Lab, IIT Patna. Manuscript in prep.*

<sub>`CP-SAT` `GNN` `Combinatorial Optimization`</sub>

</td>
</tr>
</table>

<br/>

<img src="https://img.shields.io/badge/PERCEPTION_%26_NAVIGATION-FFFFFF?style=for-the-badge&labelColor=000000&color=000000" alt="Perception and Navigation"/>

<table>
<tr>
<td width="250"><img src="https://panav.netlify.app/projects/polka-scan-merge.gif" width="240" alt="POLKA merging LiDAR scans"/></td>
<td>

**[POLKA](https://github.com/Pana1v/polka)** &nbsp;·&nbsp; Multi-LiDAR fusion for ROS 2. Merges heterogeneous PointCloud2 and LaserScan sources in one composable node, replacing the usual relay/filter/merge chain. SE(3) IMU deskewing with per-source overrides, footprint exclusion, voxel downsampling, optional CUDA. Humble and Jazzy.

<sub>`C++17` `CUDA` `PCL` `Eigen3`</sub>

</td>
</tr>
</table>

<table>
<tr>
<td width="250"><img src="https://panav.netlify.app/projects/go-slam.png" width="240" alt="GO-SLAM"/></td>
<td>

**[GO-SLAM](https://github.com/Pana1v/go-slam)** &nbsp;·&nbsp; Full SLAM from scratch: GICP front-end, pose-graph back-end, loop closure. Custom Levenberg–Marquardt solvers for both, no external optimization libraries. Fed by deskewed LiDAR from Polka, benchmarked on KITTI.

<sub>`ROS 2` `GICP` `Pose Graph Optimization` `KITTI`</sub>

</td>
</tr>
</table>

<table>
<tr>
<td width="250" align="center"><img src="https://img.shields.io/badge/AT_ETERNAL-FFFFFF?style=for-the-badge&labelColor=000000&color=000000" alt="At Eternal"/></td>
<td>

**At Eternal** &nbsp;·&nbsp; Architecting a GPU-accelerated SLAM and navigation stack on Nav2 for AgTech, under **40% CPU on Jetson Orin**. CUDA pointcloud processing and deskewing node bringing pipeline latency to **40 ms**. Automated per-robot extrinsic calibration (LiDAR-to-IMU, LiDAR-to-LiDAR) and CI with parameter snapshots in rosbags.

</td>
</tr>
</table>

<table>
<tr>
<td width="250"><img src="https://panav.netlify.app/gallery/origin.jpg" width="240" alt="At Origin"/></td>
<td>

**At Origin** &nbsp;·&nbsp; Swerve motion model for Nav2 MPPI. Lower-latency collision monitor via composable nodes. Kidnapped-robot recovery using genetic algorithms plus ambiguity detection. Lichtblick, a TypeScript/ROS 2 viz interface that cut peak CPU **120% → 26%** versus Foxglove.

</td>
</tr>
</table>

<br/>

<img src="https://img.shields.io/badge/COMPETITION-FFFFFF?style=for-the-badge&labelColor=000000&color=000000" alt="Competition"/>

<table>
<tr>
<td width="250"><img src="https://panav.netlify.app/projects/barn-motion.gif" width="240" alt="ICRA BARN Challenge 2026"/></td>
<td>

**[ICRA BARN Challenge 2026](https://cs.gmu.edu/~xiao/Research/BARN_Challenge/BARN_Challenge26.html)** &nbsp;·&nbsp; Breadcrumb Explorer, built from scratch instead of tuning a baseline. Mapless, no SLAM, no laser odometry. An odom-frame breadcrumb memory marks trajectories *tasty* or *stale* so path selection improves across trials despite 270° coverage, wheel slip, and IMU drift. **0.3682/0.5 on first submission, highest by an Indian team since 2022.** 76% zero-shot across 300 Gazebo courses.

</td>
</tr>
</table>

<table>
<tr>
<td width="250"><img src="https://panav.netlify.app/gallery/robocon-2024.jpg" width="240" alt="ABU Robocon 2024, IIT Patna"/></td>
<td>

**ABU Robocon 2023–24** &nbsp;·&nbsp; Captain, 60+ member team. National Finals, one of two IITs to qualify, highest score among IIT teams in 2024. Custom PCBs for motor control and power, heterogeneous controllers (Cube Orange, Pi, ESP32), multi-bot coordination over ROS.

</td>
</tr>
</table>

<table>
<tr>
<td width="250"><img src="https://panav.netlify.app/gallery/isro-rover.jpg" width="240" alt="IRoC-U 2024 rover"/></td>
<td>

**ISRO Robotics Challenge (IRoC-U) 2024** &nbsp;·&nbsp; Founded and led IIT Patna's 35-student rover team, building a scratch-built lunar rover prototype. Owned mechanical, electronics, and software architecture end to end.

</td>
</tr>
</table>

<br/>

## Achievements

- **Gold Medal**, Inter IIT Tech Meet, Jaguar Land Rover Chiplet Challenge for ADAS (2023)
- **Highest score by an Indian team** in the ICRA BARN Challenge since the benchmark began in 2022
- **Captain**, ABU Robocon 2024, highest score among IIT teams at National Finals
- **Founder**, IIT Patna Rover Team, ISRO Robotics Challenge 2024
- **Top 0.5%**, JEE Advanced 2021 · **Rank 8 (Karnataka)**, NSTSE 2020

<p align="center">
  <img src="https://panav.netlify.app/gallery/inter-iit-gold.jpg" height="160" alt="Inter IIT Tech gold medal"/>
  <img src="https://panav.netlify.app/projects/robocon-robot.jpg" height="160" alt="Robocon robot"/>
  <img src="https://panav.netlify.app/gallery/addverb.jpg" height="160" alt="At Addverb"/>
</p>

<br/>

## Writing

<table>
<tr>
<td width="250"><img src="https://panav.netlify.app/writing/deskew-cover.jpg" width="240" alt="To deskew LiDAR data or not?"/></td>
<td>

**[To deskew LiDAR data or not?](https://pana1v.substack.com/p/to-deskew-lidar-data-or-not)** &nbsp;·&nbsp; Why and when deskewing point clouds matters, tested on public datasets, and how Polka does it compared with GLIM, rko_lio and LIO-SAM.

**[A Journey Through the Intrinsic AI for Industry Challenge](https://substack.com/@panav1/p-198501217)** &nbsp;·&nbsp; The final week before the deadline: exhausting classical approaches first to dodge the data wall in imitation learning.

**[The Robotics Handbook](https://panav.gitbook.io/robotics-handbook)** &nbsp;·&nbsp; A living field guide, from kinematics and SLAM to controls and perception.

</td>
</tr>
</table>

<br/>

## Open source

- **[POLKA](https://github.com/Pana1v/polka)** · creator, multi-LiDAR fusion node for ROS 2
- **[Nav2](https://github.com/ros-navigation/navigation2)** · contributor, ROS 2 Navigation stack
- **[PlotJuggler](https://github.com/facontidavide/PlotJuggler)** · contributor, ROS time-series visualization
- **[AutonomousVehicleControlBeginnersGuide](https://github.com/ShisatoYano/AutonomousVehicleControlBeginnersGuide)** · contributor, path planning, SLAM and localization examples
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
  <img height="160" src="https://github-readme-stats.vercel.app/api?username=Pana1v&show_icons=true&hide_border=true&hide_title=true&bg_color=00000000&text_color=000000&icon_color=000000&ring_color=000000" alt="GitHub stats" />
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=Pana1v&layout=compact&langs_count=8&hide_border=true&hide_title=true&bg_color=00000000&text_color=FFFFFF" />
  <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Pana1v&layout=compact&langs_count=8&hide_border=true&hide_title=true&bg_color=00000000&text_color=000000" alt="Top languages" />
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com?user=Pana1v&hide_border=true&background=00000000&stroke=FFFFFF&ring=FFFFFF&fire=FFFFFF&currStreakNum=FFFFFF&currStreakLabel=FFFFFF&sideNums=FFFFFF&sideLabels=FFFFFF&dates=FFFFFF" />
  <img height="160" src="https://streak-stats.demolab.com?user=Pana1v&hide_border=true&background=00000000&stroke=000000&ring=000000&fire=000000&currStreakNum=000000&currStreakLabel=000000&sideNums=000000&sideLabels=000000&dates=000000" alt="Contribution streak" />
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-activity-graph.vercel.app/graph?username=Pana1v&hide_border=true&bg_color=00000000&color=FFFFFF&line=FFFFFF&point=FFFFFF&title_color=FFFFFF&area=true&area_color=FFFFFF" />
  <img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=Pana1v&hide_border=true&bg_color=00000000&color=000000&line=000000&point=000000&title_color=000000&area=true&area_color=000000" alt="Contribution activity" />
</picture>

</div>

<br/>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=Pana1v&style=for-the-badge&label=PROFILE+VIEWS&color=000000" alt="Profile views"/>
  <a href="https://github.com/Pana1v?tab=followers"><img src="https://img.shields.io/github/followers/Pana1v?style=for-the-badge&label=FOLLOWERS&labelColor=000000&color=000000" alt="Followers"/></a>
  <a href="https://github.com/Pana1v/polka"><img src="https://img.shields.io/github/stars/Pana1v/polka?style=for-the-badge&label=POLKA%20STARS&labelColor=000000&color=000000" alt="POLKA stars"/></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/BASED_IN-BANGALORE,_IN-FFFFFF?style=flat-square&labelColor=000000&color=000000" alt="Based in Bangalore"/>
  <img src="https://img.shields.io/badge/OPEN_TO-COLLABORATION_&_CONVERSATION-FFFFFF?style=flat-square&labelColor=000000&color=000000" alt="Open to collaboration"/>
  <img src="https://img.shields.io/badge/ASK_ME_ABOUT-NAV2_·_SLAM_·_VLA-FFFFFF?style=flat-square&labelColor=000000&color=000000" alt="Ask me about"/>
</p>

<p align="center"><sub>Open to conversations about mobile robot autonomy, VLA policies, and point clouds that refuse to align. More at <a href="https://panav.netlify.app">panav.netlify.app</a>.</sub></p>

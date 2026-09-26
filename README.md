<div align="center">

# Xinyu Jiang · 江鑫宇

**Robotics & Embodied AI** — perception, manipulation, and sim-to-real
医疗机器人 · 具身智能 · 感知与操作

[Website](https://Jxy-yxJ.github.io/en/) · [CV](https://Jxy-yxJ.github.io/en/cv/) · [LinkedIn](https://www.linkedin.com/in/xinyu-jiang-a00b17402) · [Email](mailto:jiaoxiangyue3@gmail.com)

</div>

---

## About · 关于

I build and evaluate robotic systems for the physical world. My current work is
medical manipulation in simulation: perceiving a patient from RGB-D data,
localizing a clinical target, planning collision-aware motion, and validating
the result against independent data instead of self-asserted assumptions. I
care about honest evaluation — every number in my repositories is traceable to a
script and a result file, and I report where a method still falls short.

我在仿真中构建并评估真实世界可用的机器人系统，目前聚焦医疗操作：从 RGB-D 感知患者、
定位临床目标、规划带碰撞约束的运动，并用独立数据验证结果，而不是自说自话。我在意
诚实的评估——仓库里的每个数字都能追溯到脚本与结果文件，也会如实报告方法的不足。

## Featured Projects · 精选项目

### RoboECG — autonomous robotic ECG electrode placement
A UR3 perceives a supine patient's chest from an overhead depth camera, locates
the six precordial electrodes (V1–V6) from clinical rules, presses them onto the
skin, and checks its own work — in Isaac Sim. It fills the execution gap left by
prior work that only detects or predicts electrode positions.

- **6/6** first-attempt placements · **0.14–0.36 mm** contact error · **≥ 33 mm** min clearance
- Target localization **6.08 mm** mean over 360 placements (60 held-out scenes), robust across 11 configurations (body scale 0.90–1.10, arm 60–90°, breathing ±8 mm, camera ±4 cm)
- Validated against independent data: 25 statistical-shape torsos and 120 measured electrodes (PhysioNet/CinC 2007)

`Python · Isaac Sim · UR3 · depth perception` → [Code](https://github.com/Jxy-yxJ/RoboECG)

### Robotic Thyroid Scanning in Isaac Sim
A simulation reproduction of the coarse-localization stage of an autonomous
thyroid-ultrasound system: RGB-D perception (MediaPipe), depth-fused target
localization, and collision-aware UR3 motion planning at the paper's camera
geometry.

- **0.70 mm** end-effector reach error with **≥ 2.26 cm** guaranteed body clearance
- Depth fusion improves target localization by **25%** (6.23 → 4.67 cm) across 7 camera/pose perturbations
- **40** simulator-free unit tests + CI, with a reproducibility map and an honest paper-vs-reproduction analysis

`Python · Isaac Sim · UR3 · RGB-D · MediaPipe` → [Code](https://github.com/Jxy-yxJ/robotic-thyroid-scanning-isaac-sim) · [Demo](https://github.com/Jxy-yxJ/robotic-thyroid-scanning-isaac-sim/blob/main/media/m4_reach.gif)

### MemoryGuard — bounded active memory maintenance
Long-horizon agents act on remembered object locations that silently go stale.
MemoryGuard treats memory as something to be actively maintained under a bounded
budget: before acting, it decides whether to verify, verifies with a grounded
signal, refreshes on staleness, then acts.

- Detector-agnostic verify → update → act loop under a bounded revisit budget
- Key finding: a strong vision-language model detects staleness **6/6** but makes the correct update only **3/6** — detection is not maintenance

`Python · embodied agents · memory` → [Code](https://github.com/Jxy-yxJ/MemoryGuard) · [Project page](https://jxy-yxj.github.io/MemoryGuard/)

## More · 更多

- **EgoGlove** — egocentric hand-intelligence layer: wearable + vision infrastructure for human–robot interaction in embodied AI. → [Code](https://github.com/Jxy-yxJ/EgoGlove)
- **ARIS** — lightweight, framework-free skills for autonomous ML research: cross-model review loops and idea discovery. → [Code](https://github.com/Jxy-yxJ/Auto-claude-code-research-in-sleep)
- **oh-my-context** — cross-device, cross-model context synchronization for agents. → [Code](https://github.com/Jxy-yxJ/oh-my-context)

## GitHub

<div align="center">

<img width="98%" src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Jxy-yxJ&theme=github_dark" alt="GitHub profile summary" />

<br/>

<img height="160" src="https://streak-stats.demolab.com/?user=Jxy-yxJ&theme=github-dark&hide_border=true" alt="GitHub streak" />

</div>

## Contact · 联系

- Website: [Jxy-yxJ.github.io](https://Jxy-yxJ.github.io/en/)
- CV: [jxy-yxj.github.io/en/cv](https://Jxy-yxJ.github.io/en/cv/)
- LinkedIn: [xinyu-jiang-a00b17402](https://www.linkedin.com/in/xinyu-jiang-a00b17402)
- Email: [jiaoxiangyue3@gmail.com](mailto:jiaoxiangyue3@gmail.com)

<sub>Photographer and drummer in the indie band 巧克力文件岛.</sub>

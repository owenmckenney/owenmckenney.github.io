---
layout: default
title: Owen McKenney
---

<!-- HERO (layout preserved; text still editable as Markdown) -->
<table style="width:100%; border-spacing:0; border-collapse:separate;">
  <tr>
    <td style="width:63%; padding:2.5%; vertical-align:middle;" markdown="1">

<p class="name" style="text-align:center;">Owen McKenney</p>

Hey there! I'm Owen, a 4th year undergraduate researcher at the
[University of Virginia](https://engineering.virginia.edu/department/mechanical-and-aerospace-engineering),
where I am pursuing a B.S. in Mechanical Engineering with a minor in Computer Science.
I am originally from Charlottesville, Virginia and have spent much of my time at UVA conducting research in the bio-inspired robotics field.
Outside of school, I spend a lot of my free time hiking and camping in the
[Blue Ridge Mountains](https://www.gettyimages.com/photos/blue-ridge-mountains-virginia?servicecontext=srp-related)
and honing my cooking skills.

<p style="text-align:center;">
  <a href="mailto:hph2ax@virginia.edu">Email</a> /
  <a href="https://www.linkedin.com/in/owenmckenney/">LinkedIn</a> /
  <a href="https://orcid.org/0009-0003-5218-5473">ORCID</a>
</p>

    </td>

    <td style="width:37%; padding:2.5%; vertical-align:middle;">
      <a href="images/IMG_1266.png">
        <img
          src="images/IMG_1266.png"
          alt="profile photo"
          style="width:70%; aspect-ratio:1/1; object-fit:cover; border-radius:50%;"
        >
      </a>
    </td>
  </tr>
</table>


## Research Experience and Interests

I currently conduct research under the direction of
[Dr. Hilary Bart-Smith](https://engineering.virginia.edu/faculty/hilary-bart-smith)
and Dr. Joseph Zhu and have been doing so since Fall 2023.
My work here has mainly focused on developing control strategies for bio-inspired swimming platforms, including a significant amount of work with the lab's
[Tunabot](https://www.science.org/doi/full/10.1126/scirobotics.aax4615)
and [Mantabot](https://www.mdpi.com/2226-4310/3/3/20) robotic vehicles.
I also had the opportunity to conduct research under the direction of
[Dr. Sarah Sun](https://engineering.virginia.edu/faculty/ye-sarah-sun)
during Spring 2025 where I built a simulation environment for motion planning for use in EEG-controlled robotic manipulation.
I am very interested in the design and control of bio-inspired systems and believe that manueverable, efficient, low-cost, novel robots will eventually become commonplace for navigating adverse environments and completing tasks not suited for traditional robotics.

**I am actively searching for PhD programs for this upcoming 2025 application cycle! I am specifically interested in universities with labs working on bio-inspired and novel robotics.**

**My motivation:** Biological systems embody millions of years of optimization, and I see immense potential in drawing from these principles to advance robotics in both fundamental and applied domains.
I aim to advance robotic efficiency and adaptability through the co-design of bio-inspired morphology and control, treating physical design and computation as a unified system to achieve intelligent behavior.
I seek to accomplish this by pairing rigorous theoretical modeling that captures key robot behaviors with computation driven sensing and control that allow robots to leverage their morphology for efficient, adaptive behavior.


## Selected Research Projects

<!-- Project 1 -->
<table style="width:100%; border:0px; border-spacing:0px 10px; border-collapse:separate; margin-right:auto; margin-left:auto;">
  <tr>
    <td style="padding:8px; width:35%; vertical-align:top;">
      <div style="position: relative; width: 100%; height: 0; padding-bottom: 56.25%;">
        <!-- NOTE: ensure images/tunabot_turning.jpg exists (your original HTML referenced it) -->
        <img src="images/tunabot_turning.jpg" style="position:absolute; top:0; left:0; width:100%; height:100%;">
        <video width="100%" height="100%" muted autoplay loop playsinline
               style="position:absolute; top:0; left:0; width:100%; height:100%;">
          <source src="images/tunabot_turning.mp4" type="video/mp4">
          Your browser does not support the video tag.
        </video>
      </div>
    </td>

    <td style="padding:8px; width:65%; vertical-align:top;" markdown="1">
### Tunabot Turning Control

I developed a single-actuator turning and control strategy for a tuna-inspired swimming vehicle, Tunabot.
Frequency asymmetry between the left and right half-strokes of the full path of the tailbeat cycle was introduced, leading to a turn.
Scaling laws for tangential velocity \(V\), turning radius \(r\), and turning rate \(\omega\) were developed to model the behavior of the vehicle based on the base flapping frequency \(f\) and asymmetric frequency difference \(\Delta f\).

\[
r(f, \Delta f) = c_{2} \left(
  \frac{
    f_{1}^{2}(f_{1} - \Delta f) + (f_{1} - \Delta f)^{2} f_{1}
  }{
    f_{1}^{2}(f_{1} - \Delta f) - (f_{1} - \Delta f)^{2} f_{1}
  }
\right)
\]

<p style="text-align:center;">
  <a href="https://iopscience.iop.org/article/10.1088/1748-3190/adf67a">Read my publication here!</a>
</p>
    </td>
  </tr>
</table>


<!-- Project 2 -->
<table style="width:100%; border:0px; border-spacing:0px 10px; border-collapse:separate; margin-right:auto; margin-left:auto;">
  <tr>
    <td style="padding:8px; width:35%; vertical-align:top;">
      <div style="position: relative; width: 100%; height: 0; padding-bottom: 56.25%;">
        <img src="images/mantabot.png"
             alt="Mantabot"
             style="position:absolute; top:0; left:0; width:100%; height:100%; object-fit:cover;">
      </div>
    </td>

    <td style="padding:8px; width:65%; vertical-align:top;" markdown="1">
### Mantabot Autonomous Navigation

I implemented a vison and IMU based path planning strategy for a manta-inspired swimming vehicle, Mantabot.
Paths to ArUco tags were generated using onboard cameras and tracked using pure-pursuit coupled with PID control.
I also redesigned the circuitry and control PCB for the vehicle (see Technical Work section).

\[
\delta = \arctan\!\left(\frac{2L \sin(\alpha)}{l_d}\right), ~~~~ u(t) = K_p e(t) + K_i \int_{0}^{t} e(\tau)\, d\tau + K_d \frac{de(t)}{dt}
\]

<p style="text-align:center;">
  Work in progress.
</p>
    </td>
  </tr>
</table>


<!-- Project 3 -->
<table style="width:100%; border:0px; border-spacing:0px 10px; border-collapse:separate; margin-right:auto; margin-left:auto;">
  <tr>
    <td style="padding:8px; width:35%; vertical-align:top;">
      <div style="position: relative; width: 100%; height: 0; padding-bottom: 56.25%;">
        <!-- NOTE: ensure images/ur5_demo.jpg exists (your original HTML referenced it) -->
        <img src="images/ur5_demo.jpg" style="position:absolute; top:0; left:0; width:100%; height:100%;">
        <video width="100%" height="100%" muted autoplay loop playsinline
               style="position:absolute; top:0; left:0; width:100%; height:100%;">
          <source src="images/ur5_demo.mp4" type="video/mp4">
          Your browser does not support the video tag.
        </video>
      </div>
    </td>

    <td style="padding:8px; width:65%; vertical-align:top;" markdown="1">
### Robotic Manipulation Simulation Environment

I created a simulation environment for a Universal Robotics' UR5 using Python coupled with ROS2 and MoveIt for control and motion planning.
A camera was used to capture the actual workspace and mirror objects into the simulation, enabling accurate pick-and-place.
Software will be used to carry out electroencephalogram (EEG) robotic manipulation testing with human participants.

\[
\begin{bmatrix}
x_c \\
y_c \\
z_c
\end{bmatrix}
=
\begin{bmatrix}
r_{11} & r_{12} & r_{13} & t_x \\
r_{21} & r_{22} & r_{23} & t_y \\
r_{31} & r_{32} & r_{33} & t_z
\end{bmatrix}
\begin{bmatrix}
x_w \\
y_w \\
z_w \\
1
\end{bmatrix}
\]

<p style="text-align:center;">
  Work in progress.
  <a href="files/ur5_sim.pdf" download="ur5_sim.pdf">See a documentation file of the work I did here.</a>
</p>
    </td>
  </tr>
</table>


## Publications

1. **McKenney, O.**, Zhu, J., Han, T., Bart-Smith, H. (2025). Development of a turning control strategy for a bio-inspired underwater vehicle. **Bioinspiration & Biomimetics,** 20(5), 056004.


## Conferences & Presentations

1. **McKenney, O.**, Zhu, J, Bart-Smith, H. (2025). Bending Underwater: Turning and control of a tethered, tuna-inspired underwater vehicle. Oral presentation at SICB 2025 Annual Conference  
2. **McKenney, O.**, Zhu, J, Bart-Smith, H. (2024). Stability and maneuverability control in Tunabot platform with quantitative analysis of swimming dynamics. Oral presentation at ONR MURI review attended by collaborators from Lehigh, Harvard, and Princeton University


## Teaching

- Teaching Assistant, **MAE 4501 Special Topics: Robotic Manipulators**, Fall 2025


## Selected Technical Work

[Download a portfolio of selected technical work here.](files/Owen-McKenney-Technical-Portfolio.pdf)


## Personal Computational Projects

### Double Pendulum Simulation

[Read more about my derivations and computation here](https://iopscience.iop.org/article/10.1088/1748-3190/adf67a)


<footer>
  <p style="text-align:right; font-size:small;">
    This website is built based on the template from
    <a href="https://github.com/jonbarron/jonbarron_website">Jon Barron</a>
    with further formatting used from
    <a href="https://github.com/tianjunhan/tianjunhan.github.io">Tianjun Han</a>.
  </p>
</footer>

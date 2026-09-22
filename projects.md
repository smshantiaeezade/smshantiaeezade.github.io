---
layout: default
title: Projects
permalink: /projects/
---

<section class="projects-index-hero">

  <p class="eyebrow">Projects</p>

  <h1>Research & engineering work</h1>

  <p>
    Selected projects spanning precision mechatronics, control systems,
    system identification, machining dynamics, and experimental engineering.
  </p>

</section>


<section class="featured-project-index">

  <!-- ASPE -->

  <a class="project-index-card"
     href="{{ '/projects/aspe-student-challenge/' | relative_url }}">

    <div class="project-index-image project-index-image-technical">

      <img
        src="{{ '/assets/images/projects/aspe-student-challenge/aspe-challenge-day.png' | relative_url }}"
        alt="ASPE Student Challenge experimental work">

    </div>

    <div class="project-index-content">

      <p class="project-index-kicker">
        Precision motion control · System identification · Experimental mechatronics
      </p>

      <div class="project-index-title">

        <h2>
          ASPE Student Challenge 2025:
          Musical Record Manufacturing
        </h2>

        <span aria-hidden="true">→</span>

      </div>

      <p class="project-index-summary">
        Developed and experimentally validated the motion-control strategy for a precision record-manufacturing system, including stage characterization, feedback control, trajectory filtering, gain scheduling, and real-time LabVIEW implementation. Team OSU won 1st place in the 2025 ASPE Student Challenge.
      </p>

    </div>

  </a>


  <!-- FMM -->

  <a class="project-index-card"
     href="{{ '/projects/feed-modulated-milling/' | relative_url }}">

    <div class="project-index-image project-index-image-technical">

      <img
        src="{{ '/assets/images/projects/feed-modulated-milling/fmm-cirp-stability.png' | relative_url }}"
        alt="Feed Modulated Milling chatter-stability results">

    </div>

    <div class="project-index-content">

      <p class="project-index-kicker">
        Machining dynamics · Chatter mitigation · Adaptive control
      </p>

      <div class="project-index-title">

        <h2>
          Feed Modulated Milling (FMM)
        </h2>

        <span aria-hidden="true">→</span>

      </div>

      <p class="project-index-summary">
        Developed a spindle-synchronized feed-modulation approach for modifying cutting-edge engagement and regenerative dynamics using existing machine-tool feed drives. The work combines process mechanics, stability prediction, adaptive control, real-time implementation, and experimental validation.
      </p>

    </div>

  </a>


  <!-- VCA -->

  <a class="project-index-card"
     href="{{ '/projects/voice-coil-actuator/' | relative_url }}">

    <div class="project-index-image project-index-image-photo">

      <img
        src="{{ '/assets/images/projects/voice-coil-actuator/vca-setup.png' | relative_url }}"
        alt="Planar voice-coil actuator experimental setup">

    </div>

    <div class="project-index-content">

      <p class="project-index-kicker">
        Precision positioning · Embedded control · System identification
      </p>

      <div class="project-index-title">

        <h2>
          Planar Voice-Coil Actuator:
          Precision Positioning & Friction Modeling
        </h2>

        <span aria-hidden="true">→</span>

      </div>

      <p class="project-index-summary">
        Characterized and controlled a planar voice-coil actuator for precision positioning using experimental system identification, embedded control, sensing and instrumentation, and nonlinear friction modeling. The identified model achieved 90.75% agreement with experimental data.
      </p>

    </div>

  </a>

</section>

<section class="selected-robotics-project">

  <div class="selected-robotics-heading">

    <p class="eyebrow">Selected Robotics Project</p>

    <h2>Robot programming & experimental implementation</h2>

  </div>


  <a class="project-index-card project-index-card-secondary"
     href="{{ '/projects/armpi-robotic-writing/' | relative_url }}">

  <div class="project-index-image project-index-image-photo project-index-image-armpi">

  <img
    src="{{ '/assets/images/projects/armpi-writing/armpi-writing-preview.png' | relative_url }}"
    alt="ArmPi robot with a marker mounted for robotic writing">

</div>


    <div class="project-index-content">

      <p class="project-index-kicker">
        Course Project · Robotics · Trajectory Generation · Raspberry Pi
      </p>

      <div class="project-index-title">

        <h2>
          ArmPi Robotic Writing:
          Trajectory Generation & Experimental Implementation
        </h2>

        <span aria-hidden="true">→</span>

      </div>

      <p class="project-index-summary">
        Implemented a robotic writing system using Raspberry Pi, Python, and MATLAB.
        Generated letter trajectories, tuned the writing height experimentally, and
        executed pen-up/pen-down waypoint sequences while addressing marker stability
        and vibration during physical writing.
      </p>

    </div>

  </a>

</section>



<section id="additional-engineering-projects"
         class="projects-section">
    <h2>Additional Engineering Projects</h2>

    <div class="project-grid">

      <article class="project-small-card">

  <video
    class="small-project-video"
    controls
    preload="metadata"
    playsinline
    muted>

    <source
      src="/assets/videos/projects/robot-gripper/gripper-simulation.mp4"
      type="video/mp4">

    Your browser does not support the video tag.

  </video>

  <div class="small-project-type">
    Team Course Project
  </div>

  <h3>Mechanical Robot Gripper Redesign</h3>

  <p>
    Redesigned and analyzed a mechanical robot-gripper concept to improve force transmission and mechanical advantage. Siemens NX simulations were developed to evaluate linkage motion, end-effector kinematics, velocity, acceleration, and the effects of incorporating a two-stage gear train.
  </p>

  <div class="tag-list">
    <span>Siemens NX</span>
    <span>Mechanism Design</span>
    <span>Kinematic Analysis</span>
    <span>Mechanical Advantage</span>
    <span>Gear Trains</span>
  </div>

</article>





    <article class="project-small-card">

  <a
    href="/assets/images/projects/additional-projects/microgripper-comsol.png"
    target="_blank"
    rel="noopener noreferrer">

    <img
  class="small-project-image"
  src="/assets/images/projects/additional-projects/microgripper-comsol.png"
  alt="COMSOL multiphysics model, mesh, displacement, and stress results for an electrothermal MEMS microgripper">

  </a>

  <div class="small-project-type">
    Team Course Project
  </div>

  <h3>Electrothermal MEMS Microgripper Validation</h3>

  <p>
  Reproduced and analyzed a published Au–polysilicon electrothermal microgripper
  (Pasumarthy et al., 2015) in COMSOL Multiphysics. Built and meshed the 3-D model
  and evaluated coupled thermo-mechanical behavior, including thermally induced
  displacement and stress, to compare the simulated response with the published results.
</p>

  <div class="tag-list">
    <span>COMSOL</span>
    <span>Multiphysics</span>
    <span>MEMS</span>
    <span>Finite Element Analysis</span>
    <span>Electrothermal Actuation</span>
  </div>

</article>





      <article class="project-small-card">

  <a
    href="/assets/images/projects/additional-projects/optimization-algorithms.png"
    target="_blank"
    rel="noopener noreferrer">

    <img
      class="small-project-image"
      src="/assets/images/projects/additional-projects/optimization-algorithms.png"
      alt="Genetic algorithm convergence and optimized geometric packing solution">

  </a>

  <div class="small-project-type">
    Course Project
  </div>

  <h3>Numerical Optimization Algorithm Implementations</h3>

  <p>
    Implemented and evaluated numerical optimization methods in MATLAB and Python, including gradient-based and population-based approaches. Applied methods such as genetic algorithms, particle swarm optimization, and simulated annealing to numerical and engineering optimization problems while examining convergence and solution quality.
  </p>

  <div class="tag-list">
    <span>MATLAB</span>
    <span>Python</span>
    <span>Optimization</span>
    <span>Genetic Algorithms</span>
    <span>Particle Swarm Optimization</span>
    <span>Simulated Annealing</span>
  </div>

</article>

    </div>
  </section>

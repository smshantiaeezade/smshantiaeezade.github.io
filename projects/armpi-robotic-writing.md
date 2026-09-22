---
layout: default
title: ArmPi Robotic Writing
permalink: /projects/armpi-robotic-writing/
---

<div class="project-detail-container">

  <a class="project-back-link"
     href="{{ '/projects/' | relative_url }}">
    ← All projects
  </a>

  <article class="project-card armpi-project">

    <h3>ArmPi Robotic Writing: Trajectory Generation & Experimental Implementation</h3>

    <div class="project-meta">
      Course Project · Robotics · Trajectory Generation · Raspberry Pi
    </div>


    <section class="armpi-intro">

      <h4>The Project</h4>

      <p>
        This project developed and experimentally implemented a robotic writing
        system using an ArmPi robot. Letter trajectories were generated in MATLAB
        and executed through a pen-up/pen-down waypoint sequence, while writing
        height, motion timing, and the physical pen setup were tuned experimentally.
      </p>

      <p>
        A Raspberry Pi was used as part of the robot-control platform, with Python
        used for motion execution and experimental tuning. The final system
        successfully wrote “OSU” on paper despite practical limitations associated
        with marker stability, robot vibration, and contact with the writing surface.
      </p>

    </section>



<section class="armpi-system-workflow">

  <div class="armpi-section-heading">
    <span>System Workflow</span>
    <h4>From physical setup to final writing</h4>
  </div>

  <div class="armpi-flowchart">

    <div class="armpi-flow-node armpi-flow-node-setup">
      <span class="armpi-flow-number">01</span>
      <strong>Pen Setup</strong>
      <small>Stabilize marker in the gripper</small>
    </div>


    <div class="armpi-flow-branches">

      <div class="armpi-flow-node">
        <span class="armpi-flow-number">02</span>
        <strong>Height Tuning</strong>
        <small>Determine reachable writing height</small>
      </div>

      <div class="armpi-flow-node">
        <span class="armpi-flow-number">03</span>
        <strong>Trajectory Generation</strong>
        <small>Generate O, S, U waypoints in MATLAB</small>
      </div>

    </div>


    <div class="armpi-flow-node">
      <span class="armpi-flow-number">04</span>
      <strong>Motion Execution</strong>
      <small>Pen-up, pen-down, waypoint following</small>
    </div>


    <div class="armpi-flow-node armpi-flow-node-result">
      <span class="armpi-flow-number">05</span>
      <strong>Final Writing</strong>
      <small>Robot writes “OSU” on paper</small>
    </div>

  </div>

</section>

<section class="armpi-stage">

  <div class="armpi-stage-header">

    <span>01–02</span>

    <div>
      <h4>Physical Setup & Writing-Height Tuning</h4>
      <p>
        Establishing stable marker contact was the first practical requirement
        before trajectory execution could be tested reliably.
      </p>
    </div>

  </div>


  <div class="armpi-stage-grid">

    <div class="armpi-stage-text">

      <h5>Marker setup</h5>

      <p>
        The original plan was to grip the marker directly, but paper contact caused
        the marker either to slip or tilt about the grip point. After software-side
        adjustments were insufficient, the marker was taped to one gripper finger
        to provide support at more than one location and keep its height fixed.
      </p>

      <h5>Writing-height tuning</h5>

      <p>
        A Python script moved the marker to a test point, hovered above the paper,
        and performed a pen-down motion at a selected height. The writing height was
        reduced iteratively until reliable contact was achieved while remaining
        within the robot's reachable workspace.
      </p>

    </div>


    <div class="armpi-stage-media armpi-setup-figure">

      <img
        src="/assets/images/projects/armpi-writing/armpi-pen-setup.png"
        alt="Marker attached to the ArmPi gripper for stable writing">

      <p class="media-caption">
        Final marker mounting arrangement used to improve stability during paper contact.
      </p>

    </div>

  </div>

</section>

<div class="armpi-height-visuals">

  <figure class="armpi-wide-figure armpi-flowchart-figure">

    <img
      src="/assets/images/projects/armpi-writing/armpi-height-tuning-flowchart.png"
      alt="Iterative writing-height tuning procedure for the ArmPi robot">

    <figcaption>
      Iterative procedure used to determine reliable marker contact with the paper.
    </figcaption>

  </figure>


  <figure class="armpi-wide-figure armpi-contact-figure">

    <img
      src="/assets/images/projects/armpi-writing/armpi-height-tuning-result.png"
      alt="Marker position before and after writing-height tuning">

    <figcaption>
      Marker position before and after iterative writing-height tuning.
    </figcaption>

  </figure>

</div>


<section class="armpi-stage">

  <div class="armpi-stage-header">

    <span>03</span>

    <div>

      <h4>Trajectory Generation</h4>

      <p>
        Letter geometry was converted into smooth, uniformly sampled waypoints
        suitable for robot execution.
      </p>

    </div>

  </div>


  <div class="armpi-stage-grid">

    <div class="armpi-stage-text">

      <p>
        Each letter was defined in a normalized coordinate system before being
        scaled and shifted to the robot workspace. The letter O was modeled as an
        oval, S was generated by fitting a spline through approximately nine
        control points, and U was constructed using two vertical segments connected
        by a semicircular arc.
      </p>

      <p>
        Dense reference paths were then resampled at approximately uniform
        distances along arc length to obtain a fixed number of executable
        waypoints. The final experiments used 20 waypoints per letter.
      </p>

    </div>


    <figure class="armpi-stage-media armpi-trajectory-figure">

      <img
        src="/assets/images/projects/armpi-writing/armpi-trajectories.png"
        alt="Generated O, S, and U trajectories with uniformly resampled waypoints">

      <figcaption>
        Dense reference trajectories and the 20 resampled waypoints used for each letter.
      </figcaption>

    </figure>

  </div>

</section>


<section class="armpi-stage">

  <div class="armpi-stage-header">

    <span>04</span>

    <div>

      <h4>Motion Execution</h4>

      <p>
        Each letter was executed as a continuous stroke using a fixed writing pose
        and experimentally tuned writing height.
      </p>

    </div>

  </div>



  <div class="armpi-motion-layout">

    <div class="armpi-motion-sequence">

      <div>Move to first waypoint</div>
      <span>↓</span>

      <div>Pen down</div>
      <span>↓</span>

      <div class="armpi-motion-active">
        Follow stroke waypoints
      </div>
      <span>↓</span>

      <div>Pen up</div>
      <span>↓</span>

      <div>Move to next letter</div>

    </div>


    <div class="armpi-stage-text">

      <p>
        The robot first moved above the initial waypoint, lowered the marker to the
        calibrated writing height, and followed the stroke waypoints. After each
        letter, the marker was lifted before moving to the start of the next letter
        to avoid unwanted marks.
      </p>

      <p>
        After completing the full word, the robot returned to its home position.
      </p>

    </div>

  </div>

</section>


<section class="armpi-result-section">

  <div class="armpi-stage-header">

    <span>05</span>

    <div>

      <h4>Experimental Result</h4>

      <p>
        The complete trajectory-generation and motion-execution workflow was
        validated on the physical ArmPi system.
      </p>

    </div>

  </div>


<div class="armpi-result-grid">

  <figure class="armpi-result-panel">

    <video
      class="armpi-demo-video"
      controls
      preload="metadata"
      playsinline>

      <source
        src="/assets/videos/projects/armpi-writing/armpi-writing-demo.mp4"
        type="video/mp4">

      Your browser does not support the video tag.

    </video>

    <figcaption class="media-caption">
      ArmPi executing the generated waypoint sequence to write “OSU.” Video shown at 7× the actual writing speed.
    </figcaption>

  </figure>

  <figure class="armpi-result-panel armpi-result-panel--image">

    <img
      class="armpi-result-image"
      src="/assets/images/projects/armpi-writing/armpi-final-writing.png"
      alt="Experimental OSU writing produced by the ArmPi robot">

    <figcaption class="media-caption">
      Final writing result produced on paper.
    </figcaption>

  </figure>

</div>


  <p class="armpi-result-summary">
    The robot successfully followed the generated trajectories and produced the
    intended “OSU” writing. Residual vibration remained visible in the written
    lines, but the overall writing procedure was successfully implemented.
  </p>

</section>


<section class="armpi-results">

  <h4>Experimental Parameters</h4>

  <div class="armpi-parameter-grid">

    <div>
      <span>Waypoints / letter</span>
      <strong>20</strong>
    </div>

    <div>
      <span>Writing height</span>
      <strong>4.4 cm</strong>
    </div>

    <div>
      <span>Hover height</span>
      <strong>7 cm</strong>
    </div>

    <div>
      <span>X–Y motion time</span>
      <strong>1800 ms</strong>
    </div>

    <div>
      <span>Z motion time</span>
      <strong>800 ms</strong>
    </div>

  </div>

</section>


<section class="armpi-technical-section">

  <h4>Experimental Challenges & Adjustments</h4>

  <ul class="project-contribution-list">

    <li>
      <strong>Marker stability:</strong>
      paper-contact forces caused slipping or tilting in the original gripping
      configuration, leading to the supported marker mount used in the final tests.
    </li>

    <li>
      <strong>Robot vibration:</strong>
      writing motion produced noticeable vibration, which was reduced by lowering
      motion speed, using fewer waypoints, and selecting a workspace region closer
      to the robot base.
    </li>

    <li>
      <strong>Contact sensitivity:</strong>
      incorrect writing height could cause the marker to lose contact or become
      stuck, making iterative height tuning necessary before executing the final
      trajectory.
    </li>

  </ul>

</section>


<section class="project-skills">

  <h4>Skills & Tools</h4>

  <div class="tag-list">
    <span>Robotics</span>
    <span>Raspberry Pi</span>
    <span>Python</span>
    <span>MATLAB</span>
    <span>Trajectory Generation</span>
    <span>Waypoint Planning</span>
    <span>Robot Manipulation</span>
    <span>Experimental Tuning</span>
    <span>Motion Execution</span>
    <span>Experimental Testing</span>
  </div>

</section>

  </article>

</div>
---
layout: default
title: Projects
permalink: /projects/
---

<div class="projects-container">

  <section class="projects-hero">
    <h1>Projects</h1>

    <p class="projects-lead">
      Selected research and engineering projects in control systems, precision mechatronics, machining dynamics, and advanced manufacturing.
    </p>

    <p>
      My project work combines modeling, simulation, experimental system identification, control design, and hardware implementation. The projects below are organized by technical depth and relevance rather than chronology.
    </p>
  </section>

  <section class="projects-section">
    <h2>Featured Research Projects</h2>


  <!--------- ASPE 2025 Student Challenge ---------------->
<article class="project-card project-featured aspe-project">

  <h3>ASPE Student Challenge 2025: Musical Record Manufacturing</h3>

  <div class="project-meta">
    Precision Motion Control · System Identification · Experimental Mechatronics
  </div>

  <div class="project-award">
    <div class="project-award-label">Award</div>

    <div>
      <strong>1st Place — Team OSU</strong><br>
      12th ASPE Student Challenge, ASPE 40th Annual Meeting (2025)
    </div>
  </div>


  <div class="aspe-main-grid">

    <!-- LEFT SIDE -->
    <div class="aspe-text-column">

      <section class="aspe-overview-text">

  <h4>The Challenge</h4>

  <p>
    The 2025 ASPE Student Challenge tasked teams with manufacturing a playable music record on an acrylic disc using a diamond cutting tool and an air-bearing spindle.
  </p>

  <p>
    A voice-coil-actuated flexure stage had to maintain accurate low-speed motion for spiral groove spacing while reproducing higher-frequency audio content. Meeting these requirements required precision assembly, sensor calibration, system identification, feedback control, trajectory and signal processing, and real-time implementation.
  </p>

</section>


      <section class="aspe-role">

  <h4>My Role & Engineering Impact</h4>

  <ul class="project-contribution-list">

    <li>
      <strong>Characterized the X-stage dynamics</strong> using sine-sweep FRF testing and model fitting. Measurements at multiple stage positions identified a resonance shift of approximately 17.5–19 Hz, providing the dynamic models used for subsequent control design.
    </li>

    <li>
      <strong>Achieved approximately 1 Hz tracking bandwidth with 17 dB gain margin and 83° phase margin</strong> by designing a lead-integrator feedback controller with a 10 Hz low-pass filter and resonance-notch filtering.
    </li>

    <li>
      <strong>Compensated position-dependent dynamics across five spatial regions</strong> using inverse disturbance-FRF filtering and gain scheduling, while developing resonance-aware low-speed trajectories to reduce excitation of the dominant structural mode.
    </li>

    <li>
      <strong>Implemented the real-time control system in LabVIEW and NI myRIO</strong> and supported integration, alignment, experimental testing, and hardware debugging through the final competition.
    </li>

  </ul>

</section>
    </div>


    <!-- RIGHT SIDE: ALL MEDIA -->
    <div class="aspe-media-column">

      <figure class="aspe-media-item">

        <video
          class="project-video"
          controls
          preload="metadata"
          playsinline
          onloadedmetadata="this.volume=0.4"
          poster="/assets/images/projects/aspe-student-challenge/aspe-video-poster.png">

          <source
            src="/assets/videos/projects/aspe-student-challenge/aspe-demo.mp4"
            type="video/mp4">

          Your browser does not support the video tag.

        </video>

        <figcaption>
          Team OSU's record-manufacturing system during experimental testing and the ASPE competition.
        </figcaption>

      </figure>


      <figure class="aspe-media-item">

        <a href="/assets/images/projects/aspe-student-challenge/aspe-control-trajectory.png"
           target="_blank"
           rel="noopener noreferrer">

          <img
            src="/assets/images/projects/aspe-student-challenge/aspe-control-trajectory.png"
            alt="Feedback control architecture, tracking performance, and low-speed trajectory filtering developed for the ASPE Student Challenge">

        </a>

        <figcaption>
          Feedback control architecture, tracking validation, and resonance-aware trajectory filtering. Click to enlarge.
        </figcaption>

      </figure>


      <figure class="aspe-media-item">

        <a href="/assets/images/projects/aspe-student-challenge/aspe-challenge-day.png"
           target="_blank"
           rel="noopener noreferrer">

          <img
            src="/assets/images/projects/aspe-student-challenge/aspe-challenge-day.png"
            alt="Stage alignment, record cutting, and microscope inspection during the ASPE Student Challenge">

        </a>

        <figcaption>
          Stage alignment, record-cutting tests, and microscope inspection of the manufactured grooves. Click to enlarge.
        </figcaption>

      </figure>

    </div>

  </div>

  <!-- Skills -->
<section class="project-skills aspe-full-width-skills">

  <h4>Skills & Tools</h4>

  <div class="tag-list">
    <span>System Identification</span>
    <span>Frequency-Response Analysis</span>
    <span>Feedback Control</span>
    <span>Trajectory Filtering</span>
    <span>LabVIEW</span>
    <span>NI myRIO</span>
    <span>Voice-Coil Actuation</span>
    <span>Precision Motion</span>
    <span>Experimental Testing</span>
  </div>

</section>


<!-- External link -->
<div class="project-links">

  <a href="https://aspe.net/2025-student-challenge/"
     target="_blank"
     rel="noopener noreferrer">
    Official ASPE Challenge
  </a>

</div>

</article>







  <!--------- Feed Modulated Milling ---------------->
    <article class="project-card project-featured fmm-project">

  <h3>Feed Modulated Milling (FMM)</h3>

  <div class="project-meta">
    M.Sc. Thesis Research · Machining Dynamics · Chatter Mitigation · Adaptive Control
  </div>

  <div class="fmm-thesis-box">

    <div class="fmm-thesis-label">
      Research
    </div>

    <div>
      <strong>M.Sc. Thesis — Oregon State University</strong><br>
      Low-Frequency Feed Modulation Assisted Milling for Chatter Avoidance
    </div>

  </div>


  <div class="fmm-main-grid">

    <!-- =====================================================
         LEFT COLUMN
         ===================================================== -->

    <div class="fmm-text-column">

      <section class="fmm-overview">

  <h4>The Challenge & Approach</h4>

  <p>
  Regenerative chatter is an unstable vibration that can arise during milling, limiting how aggressively material can be removed while degrading surface finish and tool life.
</p>

  <p>
    Feed Modulated Milling (FMM) addresses this limitation using the machine tool's existing X/Y feed drives. Small circular motions are superimposed on the nominal feed and synchronized with spindle rotation to actively control the chip load and engagement of individual cutting edges.
  </p>

  <p>
  By adjusting the modulation frequency, amplitude, and phase, FMM redistributes chip load and can selectively change the engagement of individual cutting edges. This modifies the regenerative dynamics and shifts the chatter-stability boundary without requiring a specialized cutter or an additional actuator.
</p>

</section>


     <section class="fmm-role">

  <h4>My Research & Engineering Contributions</h4>

  <ul class="project-contribution-list">

    <li>
      <strong>Developed the mechanics of Feed Modulated Milling</strong> to control individual cutting-edge engagement using micro-scale circular feed motions synchronized with spindle rotation, enabling on-demand modification of the milling process without changing the cutting tool.
    </li>

    <li>
      <strong>Developed and experimentally validated chatter-stability prediction methods for FMM</strong>, including a semi-discrete time-domain formulation that captures modulation-dependent engagement and regenerative delays that are not represented accurately by conventional frequency-domain approximations.
    </li>

    <li>
      <strong>Developed a real-time adaptive chatter-suppression algorithm</strong> that automatically identifies stabilizing feed-modulation amplitude and phase from measured machining response, removing the need to preselect modulation parameters from an exact process model.
    </li>

    <li>
      <strong>Implemented the approach through the machine tool's existing feed drives</strong>, integrating process modeling, signal processing, adaptive control, and experimental machining into a software-based strategy that does not require an additional vibration actuator.
    </li>

  </ul>

</section>


      <div class="fmm-impact-box">

  <div class="fmm-impact-label">
    Research Impact
  </div>

  <div class="fmm-impact-main">
    <strong>Up to ~3× higher milling productivity potential</strong>
  </div>

  <p>
    Simulation and experimental results showed that FMM can substantially expand chatter-free operating limits by actively controlling cutting-edge engagement using micro-scale feed-drive motions.
  </p>

</div>

    </div>


    <!-- =====================================================
         RIGHT COLUMN — MEDIA
         ===================================================== -->

    <div class="fmm-media-column">


      <!-- Working principle animation -->

      <figure class="fmm-media-item">

        <video
          class="fmm-animation"
          autoplay
          loop
          muted
          playsinline
          preload="metadata">

          <source
            src="/assets/videos/projects/feed-modulated-milling/fmm-principle.mp4"
            type="video/mp4">

          Your browser does not support the video tag.

        </video>

        <figcaption>
          Working principle of Feed Modulated Milling. Small circular feed motions redistribute chip thickness and change cutting-edge engagement.
        </figcaption>

      </figure>


      <!-- CIRP published result -->

      <figure class="fmm-media-item">

        <a
          href="/assets/images/projects/feed-modulated-milling/fmm-cirp-stability.png"
          target="_blank"
          rel="noopener noreferrer">

          <img
            src="/assets/images/projects/feed-modulated-milling/fmm-cirp-stability.png"
            alt="Published Feed Modulated Milling stability lobe and experimental chatter stabilization results">

        </a>

        <figcaption>
          Published chatter-stability results showing how feed modulation reshapes the milling stability limits. Click to enlarge.
        </figcaption>

      </figure>


      <!-- Published adaptive-control architecture -->

      <figure class="fmm-media-item">

        <a
          href="/assets/images/projects/feed-modulated-milling/fmm-adaptive-control.png"
          target="_blank"
          rel="noopener noreferrer">

          <img
            src="/assets/images/projects/feed-modulated-milling/fmm-adaptive-control.png"
            alt="Adaptive Feed Modulated Milling control architecture">

        </a>

        <figcaption>
          Adaptive FMM architecture for automatically adjusting the feed-modulation parameters from measured process response. Click to enlarge.
        </figcaption>

      </figure>

    </div>

  </div>


  <!-- =====================================================
       SKILLS — FULL WIDTH
       ===================================================== -->

  <section class="project-skills fmm-full-width-skills">

    <h4>Skills & Tools</h4>

    <div class="tag-list">

      <span>MATLAB</span>
      <span>Simulink</span>
      <span>Machining Dynamics</span>
      <span>Regenerative Chatter</span>
      <span>Stability Lobe Analysis</span>
      <span>Semi-Discretization</span>
      <span>Time-Domain Simulation</span>
      <span>Adaptive Control</span>
      <span>Signal Processing</span>
      <span>System Identification</span>
      <span>Impact Testing</span>
      <span>FRF Analysis</span>
      <span>Cutting-Force Modeling</span>
      <span>Cutting-Coefficient Identification</span>
      <span>CNC Machining</span>
      <span>Experimental Validation</span>

    </div>

  </section>


  <!-- =====================================================
       RELATED PUBLICATIONS
       ===================================================== -->

  <section class="fmm-publications">

  <h4>Related Publications</h4>

  <div class="fmm-publication-list">

    <a
      class="fmm-publication-item fmm-publication-link"
      href="https://doi.org/10.1016/j.cirp.2025.04.057"
      target="_blank"
      rel="noopener noreferrer">

      <strong>
        Low frequency feed modulation assisted milling for chatter avoidance
      </strong>

      <span>
        CIRP Annals, Vol. 74, Issue 1, pp. 535–539, 2025
      </span>

      <span class="publication-doi">
        DOI / Publication ↗
      </span>

    </a>


    <a
      class="fmm-publication-item fmm-publication-link"
      href="https://www.scopus.com/pages/publications/105031776907"
      target="_blank"
      rel="noopener noreferrer">

      <strong>
        Low Frequency Feed Modulation for Tool Eccentricity Cancellation and Chatter Avoidance in Milling
      </strong>

      <span>
        Proceedings of the 40th Annual Meeting of the American Society for Precision Engineering (ASPE), 2025
      </span>

      <span class="publication-doi">
        View in Scopus ↗
      </span>

    </a>

  </div>

</section>

</article>





<article class="project-card project-featured vca-project">

  <h3>Planar Voice-Coil Actuator: Precision Positioning & Friction Modeling</h3>

  <div class="project-meta">
    B.Sc. Thesis · System Identification · Precision Motion Control · Embedded Control · Friction Modeling
  </div>


  <!-- =====================================================
       THESIS INFORMATION
       ===================================================== -->

  <div class="vca-thesis-box">

  <div class="vca-thesis-label">
    RESEARCH
  </div>

  <div>
    <strong>B.Sc. Thesis — University of Tehran</strong><br>
    Precision Positioning of a Planar Voice-Coil Actuator
  </div>

</div>


  <!-- =====================================================
       MAIN TWO-COLUMN SECTION
       ===================================================== -->

  <div class="vca-main-grid">


    <!-- ================= LEFT COLUMN ================= -->

    <div class="vca-text-column">

      <section class="vca-overview">

        <h4>The Challenge & Approach</h4>

        <p>
          Precision positioning requires accurate motion despite sensor limitations, actuator dynamics, and nonlinear effects such as friction. This project focused on a planar voice-coil actuator (VCA), a direct-drive linear actuator suited to compact precision-motion applications.
        </p>

        <p>
          An experimental control platform was developed around the existing actuator by integrating position sensing, embedded control hardware, and a servo amplifier. The actuator dynamics were characterized experimentally, a dynamic model was identified, and a digital feedback controller was developed for precision positioning.
        </p>

        <p>
          The platform was later extended to a microliter syringe application, where the added mechanism introduced significant nonlinear friction. This motivated experimental friction characterization and development of a nonlinear friction model to better reproduce the physical system behavior.
        </p>

      </section>


      <!-- =====================================================
           CONTRIBUTIONS
           ===================================================== -->

      <section class="vca-role">

        <h4>My Research & Engineering Contributions</h4>

        <ul class="project-contribution-list">

          <li>
            <strong>Identified the actuator dynamics with 90.75% agreement with experimental data</strong> using chirp excitation, force-constant characterization, and MATLAB-based system identification.
          </li>

          <li>
            <strong>Achieved zero overshoot, less than 0.5 s settling time, and near-zero steady-state error</strong> in experimental positioning tests by designing and implementing a discrete feedback controller.
          </li>

          <li>
            <strong>Integrated the sensing, instrumentation, and 1 kHz embedded control platform</strong> using a magnetic position encoder, STM32 microcontroller, and servo-amplifier current drive for real-time position measurement and actuator control.
          </li>

          <li>
            <strong>Characterized and modeled nonlinear friction for a microliter syringe application</strong> using constant-velocity experiments, Stribeck-curve identification, Generalized Maxwell-Slip modeling, and experimental validation.
          </li>

        </ul>

      </section>


      <!-- =====================================================
           PERFORMANCE BOX
           ===================================================== -->

      <div class="vca-impact-box">

        <div class="vca-impact-label">
          Control Performance
        </div>

        <div class="vca-impact-main">
          <strong>0% overshoot · &lt;0.5 s settling time</strong>
        </div>

        <p>
          Experimental positioning tests achieved fast closed-loop motion with near-zero steady-state error.
        </p>

      </div>

    </div>


    <!-- ================= RIGHT COLUMN ================= -->

    <div class="vca-media-column">


      <!-- Chirp experiment -->

      <figure class="vca-media-item">

        <video
          class="vca-video"
          controls
          preload="metadata"
          playsinline
          onloadedmetadata="this.volume=0.6">

          <source
            src="/assets/videos/projects/voice-coil-actuator/vca-chirp.mp4"
            type="video/mp4">

          Your browser does not support the video tag.

        </video>

        <figcaption>
          Experimental chirp excitation used for dynamic system identification of the planar VCA.
        </figcaption>

      </figure>


      <!-- Physical setup -->

      <figure class="vca-media-item vca-setup-media">

        <a
          href="/assets/images/projects/voice-coil-actuator/vca-setup.png"
          target="_blank"
          rel="noopener noreferrer">

          <img
            src="/assets/images/projects/voice-coil-actuator/vca-setup.png"
            alt="Planar voice-coil actuator experimental setup">

        </a>

        <figcaption>
          Planar voice-coil actuator experimental platform used for positioning and control experiments. Click to enlarge.
        </figcaption>

      </figure>


      <!-- Control validation -->

      <figure class="vca-media-item">

        <a
          href="/assets/images/projects/voice-coil-actuator/vca-control-result.png"
          target="_blank"
          rel="noopener noreferrer">

          <img
            src="/assets/images/projects/voice-coil-actuator/vca-control-result.png"
            alt="Experimental closed-loop positioning response of the planar voice-coil actuator">

        </a>

        <figcaption>
          Experimental closed-loop positioning response used to validate the digital controller. Click to enlarge.
        </figcaption>

      </figure>


      <!-- Friction model validation -->

      <figure class="vca-media-item">

        <a
          href="/assets/images/projects/voice-coil-actuator/vca-friction-validation.png"
          target="_blank"
          rel="noopener noreferrer">

          <img
            src="/assets/images/projects/voice-coil-actuator/vca-friction-validation.png"
            alt="Experimental and simulated response comparison using the nonlinear friction model">

        </a>

        <figcaption>
          Experimental and simulated responses used to validate the nonlinear friction model. Click to enlarge.
        </figcaption>

      </figure>

    </div>

  </div>


  <!-- =====================================================
       SKILLS
       ===================================================== -->

  <section class="project-skills vca-full-width-skills">

    <h4>Skills & Tools</h4>

    <div class="tag-list">

      <span>MATLAB</span>
      <span>Simulink</span>
      <span>STM32</span>
      <span>Embedded Control</span>
      <span>System Identification</span>
      <span>Digital Control</span>
      <span>Precision Positioning</span>
      <span>Voice-Coil Actuation</span>
      <span>Magnetic Encoder</span>
      <span>Sensor Integration</span>
      <span>Experimental Modeling</span>
      <span>Friction Modeling</span>
      <span>Stribeck Friction</span>
      <span>Generalized Maxwell-Slip Model</span>
      <span>Experimental Validation</span>

    </div>

  </section>


  <!-- =====================================================
       RELATED PUBLICATION
       ===================================================== -->

  <section class="vca-publications">

    <h4>Related Publication</h4>

    <div class="vca-publication-list">

      <a
        class="vca-publication-item vca-publication-link"
        href="https://ieeexplore.ieee.org/document/10025221/"
        target="_blank"
        rel="noopener noreferrer">

        <strong>
          Optimal Design and Control of a Planar Voice-Coil Actuator for Micropositioning Applications
        </strong>

        <span>
          2022 10th RSI International Conference on Robotics and Mechatronics (ICRoM), pp. 439–444
        </span>

        <span class="vca-publication-doi">
          View IEEE Publication ↗
        </span>

      </a>

    </div>

  </section>

</article>





  <section class="projects-section">
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

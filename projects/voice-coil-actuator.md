---
layout: default
title: Planar Voice-Coil Actuator
permalink: /projects/voice-coil-actuator/
---

<div class="project-detail-container">

  <a class="project-back-link"
     href="{{ '/projects/' | relative_url }}">
    ← All projects
  </a>

  <article id="voice-coil-actuator"
           class="project-card project-featured vca-project">


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


  <!-- =====================================================
       MAIN TWO-COLUMN SECTION
       ===================================================== -->

  <div class="vca-main-grid">


    <!-- ================= LEFT COLUMN ================= -->

    <div class="vca-text-column">


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
          <strong>near-zero steady-state error · 0% overshoot · &lt;0.5 s settling time</strong>
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

</div>
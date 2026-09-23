---
layout: default
title: ASPE Student Challenge 2025
permalink: /projects/aspe-student-challenge/
---

<div class="project-detail-container">

  <a class="project-back-link"
     href="{{ '/projects/' | relative_url }}">
    ← All projects
  </a>

  <article id="aspe-student-challenge"
           class="project-card project-featured aspe-project">


  <!--------- ASPE 2025 Student Challenge ---------------->

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

  <section class="aspe-overview-text aspe-overview-lead">

  <h4>The Challenge</h4>

  <p>
    The 2025 ASPE Student Challenge tasked teams with manufacturing a playable music record on an acrylic disc using a diamond cutting tool and an air-bearing spindle.
  </p>

  <p>
    A voice-coil-actuated flexure stage had to maintain accurate low-speed motion for spiral groove spacing while reproducing higher-frequency audio content. Meeting these requirements required precision assembly, sensor calibration, system identification, feedback control, trajectory and signal processing, and real-time implementation.
  </p>

</section>


<figure class="aspe-media-item">

        <video
        class="project-video"
        controls
        preload="metadata"
        onloadedmetadata="this.volume=0.4">

          <source
            src="/assets/videos/projects/aspe-student-challenge/aspe-demo.mp4"
            type="video/mp4">

          Your browser does not support the video tag.

        </video>

        <figcaption>
          Team OSU's record-manufacturing system during experimental testing and the ASPE competition.
        </figcaption>

      </figure>


  <div class="aspe-main-grid">

    <!-- LEFT SIDE -->
    <div class="aspe-text-column">



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
<section class="project-related-links">

  <h4>Challenge Link</h4>

  <div class="project-links">

    <a href="https://aspe.net/2025-student-challenge/"
       target="_blank"
       rel="noopener noreferrer">
      Official ASPE Challenge ↗
    </a>

  </div>

</section>

</article>

</div>
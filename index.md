---
layout: default
title: Home
permalink: /
image: /assets/images/profile.jpeg
---

<div class="home-container">

  <!-- =====================================================
       HERO
       ===================================================== -->

  <section class="home-hero" aria-labelledby="home-title">

    <div class="home-hero-copy">

      <p class="eyebrow">
        Ph.D. Student · Oregon State University
      </p>

      <h1 id="home-title">
        Seyed Mahmood Shantiaeezade
      </h1>

      <p class="home-hero-role">
        Mechatronics, control systems, precision engineering, and advanced manufacturing
      </p>

      <p class="home-hero-lead">
        I develop and experimentally validate control methods for precision mechatronic and manufacturing systems using dynamic modeling, system identification, real-time control, and hardware experiments.
      </p>

      <p class="home-hero-context">
        Graduate Research Assistant in the Manufacturing Process Control Laboratory, with research spanning precision motion, machining dynamics, vibration control, adaptive control, and experimental mechatronic systems.
      </p>

      <div class="hero-actions">

        <a class="button button-primary"
           href="{{ '/projects/' | relative_url }}">
          View selected work
        </a>

        <a class="button button-secondary"
           href="{{ '/publications/' | relative_url }}">
          Publications
        </a>

        {% if site.cv_url %}
          <a class="button button-secondary"
             href="{{ site.cv_url | relative_url }}"
             target="_blank"
             rel="noopener noreferrer">
            View CV
          </a>
        {% endif %}

      </div>

    </div>


    <figure class="home-hero-photo">

      <img
        src="{{ '/assets/images/profile.jpeg' | relative_url }}"
        alt="Portrait of Seyed Mahmood Shantiaeezade"
        class="profile-photo">

    </figure>

  </section>


  <!-- =====================================================
       SELECTED WORK
       ===================================================== -->

  <section class="home-section" aria-labelledby="selected-work-title">

    <div class="section-heading-row">

      <div>
        <p class="eyebrow">Selected Work</p>
        <h2 id="selected-work-title">
          Engineering systems, modeled through experiment
        </h2>
      </div>

      <a class="text-link"
         href="{{ '/projects/' | relative_url }}">
        View all projects →
      </a>

    </div>


    <div class="selected-work-grid">

      <!-- ASPE -->

      <article class="work-preview">

        <a class="work-preview-media"
           href="{{ '/projects/aspe-student-challenge/' | relative_url }}">

          <img
            src="{{ '/assets/images/projects/aspe-student-challenge/aspe-challenge-day.png' | relative_url }}"
            alt="ASPE Student Challenge record-manufacturing system"
            loading="lazy">

        </a>

        <div class="work-preview-body">

          <p class="work-kicker">
            Precision motion control · System identification · Experimental mechatronics
          </p>

          <h3>
            <a href="{{ '/projects/aspe-student-challenge/' | relative_url }}">
              ASPE Student Challenge 2025
            </a>
          </h3>

          <p>
            Characterized the stage dynamics and developed the feedback-control, trajectory-filtering, gain-scheduling, and LabVIEW implementation for a precision record-manufacturing system. The final controller achieved approximately 1 Hz tracking bandwidth with 17 dB gain margin and 83° phase margin; Team OSU won 1st place.
          </p>

          <a class="text-link"
             href="{{ '/projects/aspe-student-challenge/' | relative_url }}">
            View project →
          </a>

        </div>

      </article>


      <!-- FMM -->

      <article class="work-preview">

        <a class="work-preview-media"
           href="{{ '/projects/feed-modulated-milling/' | relative_url }}">

          <img
            src="{{ '/assets/images/projects/feed-modulated-milling/fmm-cirp-stability.png' | relative_url }}"
            alt="Feed Modulated Milling chatter-stability results"
            loading="lazy">

        </a>

        <div class="work-preview-body">

          <p class="work-kicker">
            Machining dynamics · Chatter mitigation · Adaptive control
          </p>

          <h3>
            <a href="{{ '/projects/feed-modulated-milling/' | relative_url }}">
              Feed Modulated Milling (FMM)
            </a>
          </h3>

          <p>
            M.Sc. thesis research on spindle-synchronized micro feed motions that modify cutting-edge engagement and regenerative dynamics. The work combines process mechanics, chatter-stability prediction, adaptive parameter tuning, feed-drive implementation, and experimental validation, with up to ~3× higher milling productivity potential.
          </p>

          <a class="text-link"
             href="{{ '/projects/feed-modulated-milling/' | relative_url }}">
            View project →
          </a>

        </div>

      </article>


      <!-- VCA -->

      <article class="work-preview">

        <a class="work-preview-media"
           href="{{ '/projects/voice-coil-actuator/' | relative_url }}">

          <img
            src="{{ '/assets/images/projects/voice-coil-actuator/vca-setup.png' | relative_url }}"
            alt="Planar voice-coil actuator experimental setup"
            loading="lazy">

        </a>

        <div class="work-preview-body">

          <p class="work-kicker">
            Precision positioning · Embedded control · System identification
          </p>

          <h3>
            <a href="{{ '/projects/voice-coil-actuator/' | relative_url }}">
              Planar Voice-Coil Actuator
            </a>
          </h3>

          <p>
            B.Sc. thesis work on experimental system identification, sensing and instrumentation, digital control, and nonlinear friction modeling. The identified model achieved 90.75% agreement with experiments; closed-loop positioning achieved zero overshoot, &lt;0.5 s settling time, and near-zero steady-state error.
          </p>

          <a class="text-link"
             href="{{ '/projects/voice-coil-actuator/' | relative_url }}">
            View project →
          </a>

        </div>

      </article>

    </div>

  </section>


  <!-- =====================================================
       RESEARCH FOCUS
       ===================================================== -->

  <section class="home-section" aria-labelledby="research-focus-title">

    <div class="section-heading-row">

      <div>
        <p class="eyebrow">Research Focus</p>

        <h2 id="research-focus-title">
          From physical dynamics to validated control
        </h2>
      </div>

    </div>


    <div class="focus-grid">

      <article class="focus-item">
        <h3>Precision motion & mechatronic systems</h3>
        <p>
          Motion generation, sensing, actuator dynamics, feed-drive systems, embedded control, and experimental implementation.
        </p>
      </article>

      <article class="focus-item">
        <h3>System identification & control</h3>
        <p>
          FRF-based characterization, model identification, feedback control, adaptive control, and real-time validation on physical systems.
        </p>
      </article>

      <article class="focus-item">
        <h3>Vibration & machining dynamics</h3>
        <p>
          Regenerative chatter, stability analysis, cutting-process dynamics, structural testing, and vibration mitigation.
        </p>
      </article>

      <article class="focus-item">
        <h3>Adaptive & learning-based manufacturing control</h3>
        <p>
          Online optimization, adaptive and iterative-learning concepts, and model-light strategies for uncertain manufacturing processes.
        </p>
      </article>

    </div>

  </section>


  <!-- =====================================================
       PUBLICATIONS / RECOGNITION
       ===================================================== -->

  <section class="home-section" aria-labelledby="evidence-title">

    <div class="section-heading-row">

      <div>
        <p class="eyebrow">Highlights</p>
        <h2 id="evidence-title">Publications & awards</h2>
      </div>

    </div>


    <div class="evidence-list">

      <article class="evidence-row">

        <div class="evidence-meta">
          2025 · Award
        </div>

        <div>

          <h3>
            <a href="{{ '/projects/aspe-student-challenge/' | relative_url }}">
              1st Place — ASPE Student Challenge →
            </a>
          </h3>

          <p>
            Team OSU · 12th ASPE Student Challenge, ASPE 40th Annual Meeting.
          </p>

        </div>

      </article>


      <article class="evidence-row">

        <div class="evidence-meta">
          2025 · CIRP Annals
        </div>

        <div>
          <h3>
            <a href="https://doi.org/10.1016/j.cirp.2025.04.057"
               target="_blank"
               rel="noopener noreferrer">
              Low frequency feed modulation assisted milling for chatter avoidance ↗
            </a>
          </h3>
        </div>

      </article>


      <article class="evidence-row">

        <div class="evidence-meta">
          2025 · MM Science Journal
        </div>

        <div>
          <h3>
            <a href="https://doi.org/10.17973/MMSJ.2025_12_2025157"
               target="_blank"
               rel="noopener noreferrer">
              Adaptive Tool Eccentricity Compensation Using Machine Tool Feed Drives ↗
            </a>
          </h3>
        </div>

      </article>

    </div>

  </section>


  <!-- =====================================================
       EDUCATION / CURRENT ROLE
       ===================================================== -->

  <section class="home-section" aria-labelledby="background-title">

    <div class="section-heading-row">

      <div>
        <p class="eyebrow">Background</p>
        <h2 id="background-title">Education & current role</h2>
      </div>

    </div>


    <div class="background-grid">

      <div class="education-list">


        <!-- PhD -->

        <div class="education-item">

          <span class="education-icon education-icon-current"
                aria-hidden="true">

            <svg viewBox="0 0 24 24">
              <path d="M2.5 9 12 4l9.5 5L12 14 2.5 9Z"></path>
              <path d="M6 11.2v5.1c2.8 2.2 9.2 2.2 12 0v-5.1"></path>
              <path d="M21.5 9v6"></path>
            </svg>

          </span>

          <div>
            <div class="education-degree">
              Ph.D. in Mechatronics, Robotics, and Automation Engineering
            </div>

            <div class="education-school">
              Oregon State University · 2025–present
            </div>
          </div>

        </div>


        <!-- MSc -->

        <div class="education-item">

          <span class="education-icon education-icon-completed"
                aria-hidden="true">

            <svg viewBox="0 0 24 24">
              <path d="M2.5 9 12 4l9.5 5L12 14 2.5 9Z"></path>
              <path d="M6 11.2v5.1c2.8 2.2 9.2 2.2 12 0v-5.1"></path>
              <path d="M21.5 9v6"></path>
            </svg>

          </span>

          <div>
            <div class="education-degree">
              M.Sc. in Mechanical Engineering
            </div>

            <div class="education-school">
              Oregon State University · 2023–2025
            </div>
          </div>

        </div>


        <!-- BSc -->

        <div class="education-item">

          <span class="education-icon education-icon-completed"
                aria-hidden="true">

            <svg viewBox="0 0 24 24">
              <path d="M2.5 9 12 4l9.5 5L12 14 2.5 9Z"></path>
              <path d="M6 11.2v5.1c2.8 2.2 9.2 2.2 12 0v-5.1"></path>
              <path d="M21.5 9v6"></path>
            </svg>

          </span>

          <div>
            <div class="education-degree">
              B.Sc. in Mechanical Engineering
            </div>

            <div class="education-school">
              University of Tehran · 2018–2023
            </div>
          </div>

        </div>

      </div>


      <div class="current-role-block">

        <p class="eyebrow">Current Role</p>

        <h3>Graduate Research Assistant</h3>

        <p class="current-role-org">
          Manufacturing Process Control Laboratory · Oregon State University
        </p>

        <p>
          Research centered on dynamic modeling, system identification, precision motion, machining-process stability, adaptive control, and experimental validation.
        </p>

      </div>

    </div>

  </section>

</div>
---
layout: default
title: Feed Modulated Milling
permalink: /projects/feed-modulated-milling/
---

<div class="project-detail-container">

  <a class="project-back-link"
     href="{{ '/projects/' | relative_url }}">
    ← All projects
  </a>

  <article id="feed-modulated-milling"
           class="project-card project-featured fmm-project">


<!--------- Feed Modulated Milling ---------------->

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

</div>
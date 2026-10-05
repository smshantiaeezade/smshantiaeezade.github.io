---
layout: default
title: Botanist
permalink: /projects/botanist/
---

<div class="project-detail-container">

  <a class="project-back-link"
     href="{{ '/projects/' | relative_url }}">
    ← All projects
  </a>

  <article id="botanist"
           class="project-card project-featured botanist-project">

    <h1>Botanist: Leaf Disease Classification with Transfer Learning</h1>

    <div class="project-meta">
      Course Project · Computer Vision · Deep Learning · PyTorch
    </div>

    <div class="botanist-project-box">

  <div class="botanist-project-label">
    COURSE PROJECT
  </div>

  <div>
    <strong>38-Class Plant-Leaf Image Classification</strong><br>
    50,000 labeled images · ResNet50 · EfficientNet-B4
  </div>

</div>

<section class="botanist-overview">

  <h4>The Problem &amp; Dataset</h4>

  <p>
    The Botanist project addressed a 38-class plant-leaf image-classification
    problem using 50,000 labeled images. The dataset contained substantial
    variation in lighting, background, scale, orientation, color, texture, and
    visible leaf damage, with some classes sharing very similar visual features.
  </p>

  <p>
    The data were divided using a stratified 80/20 split, producing 40,000
    training images and 10,000 validation images while preserving the class
    distribution. Because the dataset was imbalanced across the 38 labels,
    evaluation considered both overall accuracy and class-specific error patterns.
  </p>

</section>


<figure class="botanist-lead-media">

  <a
    href="/assets/images/projects/botanist/botanist-dataset-overview.png"
    target="_blank"
    rel="noopener noreferrer">

    <img
      src="/assets/images/projects/botanist/botanist-dataset-overview.png"
      alt="Botanist dataset examples, augmented leaf images, and class distribution">

  </a>

  <figcaption>
    Dataset overview showing representative leaf images, training augmentation,
    and the class distribution across the 38 labels. Click to enlarge.
  </figcaption>

</figure>


<section class="botanist-section">

  <h4>Model Development</h4>

  <p>
    Transfer learning was used instead of training convolutional networks from
    scratch. Pretrained ResNet50 and EfficientNet-B4 models were adapted to the
    38-class task by replacing their classifier layers and then fine-tuning
    selected deeper feature-extraction layers.
  </p>

  <div class="botanist-pipeline">

    <div class="botanist-pipeline-step">
      <span>01</span>
      <strong>Transfer Learning</strong>
      <small>ResNet50 + EfficientNet-B4</small>
    </div>

    <div class="botanist-pipeline-step">
      <span>02</span>
      <strong>Staged Fine-Tuning</strong>
      <small>Classifier first, deeper layers later</small>
    </div>

    <div class="botanist-pipeline-step">
      <span>03</span>
      <strong>Lighting Augmentation</strong>
      <small>Brightness, contrast, saturation &amp; color</small>
    </div>

    <div class="botanist-pipeline-step">
      <span>04</span>
      <strong>Soft-Voting Ensemble</strong>
      <small>50% ResNet50 + 50% EfficientNet-B4</small>
    </div>

    <div class="botanist-pipeline-step">
      <span>05</span>
      <strong>Multi-Scale TTA</strong>
      <small>Probability averaging across center crops</small>
    </div>

  </div>

</section>


<section class="botanist-section">

  <h4>Diagnostics &amp; Model Iteration</h4>

  <p>
    Validation errors were examined rather than relying only on aggregate
    accuracy. Grad-CAM was used to inspect which image regions influenced
    ResNet50 predictions, while brightness statistics were compared between
    correctly classified and misclassified validation images. The analysis
    suggested that lighting and dark regions could contribute to some errors,
    motivating stronger lighting-oriented augmentation during later ResNet50
    fine-tuning.
  </p>

  <div class="project-media-grid project-media-grid--two botanist-diagnostics-grid">

    <figure class="project-media">

      <a
        href="/assets/images/projects/botanist/botanist-gradcam.png"
        target="_blank"
        rel="noopener noreferrer">

        <img
          src="/assets/images/projects/botanist/botanist-gradcam.png"
          alt="Grad-CAM visualization for a Botanist ResNet50 prediction">

      </a>

      <figcaption>
        Grad-CAM visualization used to inspect which image regions influenced a
        ResNet50 prediction.
      </figcaption>

    </figure>


    <figure class="project-media">

      <a
        href="/assets/images/projects/botanist/botanist-brightness.png"
        target="_blank"
        rel="noopener noreferrer">

        <img
          src="/assets/images/projects/botanist/botanist-brightness.png"
          alt="Brightness distributions for correct and misclassified Botanist validation images">

      </a>

      <figcaption>
        Mean-brightness distributions for correctly classified and misclassified
        validation images used during error analysis.
      </figcaption>

    </figure>

  </div>

</section>


<section class="botanist-section">

  <h4>Performance</h4>

  <div class="botanist-metric-box">

    <div class="botanist-metric-label">
      FINAL TEST ACCURACY
    </div>

    <div class="botanist-metric-value">
      99.58%
    </div>

    <p>
      The final submitted pipeline combined transfer learning, data augmentation,
      a 50/50 probability-level ensemble, and multi-scale center-crop
      test-time augmentation.
    </p>

  </div>


  <div class="botanist-table-wrap">

    <table class="botanist-results-table">

      <thead>
        <tr>
          <th>Model / Setting</th>
          <th>Validation Accuracy</th>
          <th>Errors</th>
        </tr>
      </thead>

      <tbody>

        <tr>
          <td>ResNet50</td>
          <td>99.11%</td>
          <td>89</td>
        </tr>

        <tr>
          <td>EfficientNet-B4</td>
          <td>97.84%</td>
          <td>216</td>
        </tr>

        <tr>
          <td>50/50 Soft-Voting Ensemble</td>
          <td>99.43%</td>
          <td>57</td>
        </tr>

        <tr class="botanist-best-row">
          <td>Ensemble + Multi-Scale TTA</td>
          <td><strong>99.54%</strong></td>
          <td><strong>46</strong></td>
        </tr>

      </tbody>

    </table>

  </div>

  <p>
    Probability-level ensembling improved validation accuracy from the best
    individual-model result of 99.11% to 99.43%. Multi-scale center-crop TTA
    improved it further to 99.54%, reducing the remaining validation errors from
    57 to 46. Horizontal-flip TTA was also evaluated but slightly reduced
    validation accuracy and was therefore not used in the final submission.
  </p>


  
<section class="botanist-section">

  <h4>Class-Level Performance</h4>

  <div class="botanist-confusion-layout">

    <div class="botanist-confusion-text">

      <p>
        Overall accuracy was supplemented with class-level analysis because the
        dataset was imbalanced and several leaf classes were visually similar.
        The focused normalized confusion matrix shows that predictions for the
        examined classes were concentrated primarily along the diagonal, while
        the remaining errors were limited to a small number of class pairs.
      </p>

      <p>
        This analysis helped identify where the final ensemble still struggled
        despite its high overall validation accuracy.
      </p>

    </div>


    <figure class="project-media botanist-confusion-media">

      <a
        href="/assets/images/projects/botanist/botanist-confusion-matrix.png"
        target="_blank"
        rel="noopener noreferrer">

        <img
          src="/assets/images/projects/botanist/botanist-confusion-matrix.png"
          alt="Focused normalized confusion matrix for the final Botanist ensemble model">

      </a>

      <figcaption>
        Focused normalized confusion matrix for the best ensemble model.
        Click to enlarge.
      </figcaption>

    </figure>

  </div>

</section>

</section>



<section class="project-skills botanist-skills">

  <h4>Skills &amp; Tools</h4>

  <div class="tag-list">

    <span>Python</span>
    <span>PyTorch</span>
    <span>Computer Vision</span>
    <span>Transfer Learning</span>
    <span>ResNet50</span>
    <span>EfficientNet-B4</span>
    <span>Data Augmentation</span>
    <span>Ensemble Learning</span>
    <span>Test-Time Augmentation</span>
    <span>Grad-CAM</span>
    <span>Model Diagnostics</span>
    <span>Error Analysis</span>

  </div>

</section>

  </article>

</div>
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <!-- Meta tags for social media banners, these should be filled in appropriatly as they are your "business card" -->
  <!-- Replace the content tag with appropriate information -->
  <meta name="description" content="DESCRIPTION META TAG">
  <meta property="og:title" content="SOCIAL MEDIA TITLE TAG"/>
  <meta property="og:description" content="SOCIAL MEDIA DESCRIPTION TAG TAG"/>
  <meta property="og:url" content="URL OF THE WEBSITE"/>
  <!-- Path to banner image, should be in the path listed below. Optimal dimenssions are 1200X630-->
  <meta property="og:image" content="static/image/your_banner_image.png" />
  <meta property="og:image:width" content="1200"/>
  <meta property="og:image:height" content="630"/>


  <meta name="twitter:title" content="TWITTER BANNER TITLE META TAG">
  <meta name="twitter:description" content="TWITTER BANNER DESCRIPTION META TAG">
  <!-- Path to banner image, should be in the path listed below. Optimal dimenssions are 1200X600-->
  <meta name="twitter:image" content="static/images/your_twitter_banner_image.png">
  <meta name="twitter:card" content="summary_large_image">
  <!-- Keywords for your paper to be indexed by-->
  <meta name="keywords" content="KEYWORDS SHOULD BE PLACED HERE">
  <meta name="viewport" content="width=device-width, initial-scale=1">

  <h1>
  <div class="center">
  <title>Improving Robustness to Model Inversion Attacks via Sparse Coding Architectures</title>
  <link rel="icon" type="image/x-icon" href="static/images/favicon.ico">
  <link href="https://fonts.googleapis.com/css?family=Google+Sans|Noto+Sans|Castoro"
  rel="stylesheet">
  </div>
  </h1>
  <link rel="stylesheet" href="static/css/bulma.min.css">
  <link rel="stylesheet" href="static/css/bulma-carousel.min.css">
  <link rel="stylesheet" href="static/css/bulma-slider.min.css">
  <link rel="stylesheet" href="static/css/fontawesome.all.min.css">
  <link rel="stylesheet"
  href="https://cdn.jsdelivr.net/gh/jpswalsh/academicons@1/css/academicons.min.css">
  <link rel="stylesheet" href="static/css/index.css">

  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
  <script src="https://documentcloud.adobe.com/view-sdk/main.js"></script>
  <script defer src="static/js/fontawesome.all.min.js"></script>
  <script src="static/js/bulma-carousel.min.js"></script>
  <script src="static/js/bulma-slider.min.js"></script>
  <script src="static/js/index.js"></script>
</head>
<body>


  <section class="hero">
    <div class="hero-body">
      <div class="container is-max-desktop">
        <div class="columns is-centered">
          <div class="column has-text-centered">
            <h1 class="title is-1 publication-title">Improving Robustness to Model Inversion Attacks via Sparse Coding Architectures</h1>
            <div class="is-size-5 publication-authors">
              <!-- Paper authors -->
              <span class="author-block">
                <a href="https://sayantondibbo.github.io/" target="_blank">Sayanton Dibbo</a><sup>ψ, *</sup>,</span>
                <span class="author-block">
                  <a href="https://www.adambreuer.com/" target="_blank">Adam Breuer</a><sup>ψ</sup>,</span>
                  <span class="author-block">
                    <a href="https://scholar.google.com/citations?user=gyFa3X0AAAAJ&hl=en" target="_blank">Juston Moore</a><sup>*</sup>,
                  </span>
              <span class="author-block">
                    <a href="https://scholar.google.com/citations?user=cTWaSg8AAAAJ&hl=en" target="_blank">Micahel Teti</a><sup>*</sup>
                  </span>
                  </div>

                  <div class="is-size-5 publication-authors">
                    <span class="author-block"><sup>ψ</sup>Dartmouth College<br><sup>*</sup>Los Alamos National Laboratory<br>Acccepted @ European Conference on Computer Vision (ECCV 2024)</span>
                  </div>

                  <div class="column has-text-centered">
                    <div class="publication-links">
                         <!-- Arxiv PDF link -->
                      <span class="link-block">
                        <a href="./assets/files/ECCV24.pdf" target="_blank"
                        class="external-link button is-normal is-rounded is-dark">
                        <span class="icon">
                          <i class="fas fa-file-pdf"></i>
                        </span>
                        <span>Paper</span>
                      </a>
                    </span>

                    <!-- Supplementary PDF link -->
                    <span class="link-block">
                      <a href="./assets/files/ECCV_Supplementary.pdf" target="_blank"
                      class="external-link button is-normal is-rounded is-dark">
                      <span class="icon">
                        <i class="fas fa-file-pdf"></i>
                      </span>
                      <span>Supplementary</span>
                    </a>
                  </span>

                  <!-- Github link -->
                  <span class="link-block">
                    <a href="https://github.com/SayantonDibbo/SCA" target="_blank"
                    class="external-link button is-normal is-rounded is-dark">
                    <span class="icon">
                      <i class="fab fa-github"></i>
                    </span>
                    <span>Code</span>
                  </a>
                </span>

                <!-- ArXiv abstract Link -->
                <span class="link-block">
                  <a href="https://arxiv.org/abs/2403.14772" target="_blank"
                  class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                    <i class="ai ai-arxiv"></i>
                  </span>
                  <span>arXiv</span>
                </a>
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>


<!-- Teaser video-->
<section class="hero teaser">
  <div class="container is-max-desktop">
    <div class="hero-body">
      
      <i>
      <h3 class="subtitle has-text-centered">
        The first study of neural network architectures that are robust to model inversion (MI) attacks, where a novel sparse coding-based architecture, SCA, is developed that outperforms state-of-the-art defenses against MI attacks.
      </h3></i>
    </div>
  </div>
</section>
<!-- End teaser video -->

<!-- Paper abstract -->
<section class="section hero is-light">
  <div class="container is-max-desktop">
    <div class="columns is-centered has-text-centered">
      <div class="column is-four-fifths">
        <h2 class="title is-3">Abstract</h2>
        <div class="content has-text-justified">
          
          <p>
Recent model inversion attack algorithms permit adversaries to reconstruct a neural network's private training data just by repeatedly querying the network and inspecting its outputs. In this work, we develop a novel network architecture that leverages sparse-coding layers to obtain superior robustness to this class of attacks. Three decades of computer science research has studied sparse coding in the context of image denoising, object recognition, and adversarial misclassification settings, but to the best of our knowledge, its connection to state-of-the-art privacy vulnerabilities remains unstudied. However, sparse coding architectures suggest an advantageous means to defend against model inversion attacks because they allow us to control the amount of irrelevant private information encoded in a network's intermediate representations in a manner that can be computed efficiently during training and that is known to have little effect on classification accuracy. Specifically, compared to networks trained with a variety of state-of-the-art defenses, our sparse-coding architectures maintain comparable or higher classification accuracy while degrading state-of-the-art training data reconstructions by factors of 1.1 to 18.3 across a variety of reconstruction quality metrics (PSNR, SSIM, FID). This performance advantage holds across 5 datasets ranging from CelebA faces to medical images and CIFAR-10, and across various state-of-the-art SGD-based and GAN-based inversion attacks, including Plug-&-Play attacks. We provide a cluster-ready PyTorch codebase to promote research and standardize defense evaluations. Interested? Please complete the following  <a href="https://forms.gle/Xf3VJMhf1CnGHVMW7">brief survey </a> for additional information or resources for this project.
            </p>
        </div>
      </div>
    </div>
  </div>
</section>
<!-- End paper abstract -->

<!--BibTex citation -->
  <section class="section" id="BibTeX">
    <div class="container is-max-desktop content">
      <h2 class="title">BibTeX</h2>
      <pre><code>@inproceedings{dibbo2025improving,
  title={Improving robustness to model inversion attacks via sparse coding architectures},
  author={Dibbo, Sayanton V and Breuer, Adam and Moore, Juston and Teti, Michael},
  booktitle={European Conference on Computer Vision},
  pages={117--136},
  year={2025},
  organization={Springer}
}</code></pre>
    </div>
</section>
<!--End BibTex citation -->


<!-- Image carousel -->
<section class="hero is-small">
  <div class="hero-body">
    <div class="container">
      <div id="results-carousel" class="carousel results-carousel">
       <div class="item">
        <!-- Your image here -->
        <img src="./assets/img/teaser_example_11.png" alt="Multi-layer Sparse Coding Network"/>
        <h2 class="subtitle has-text-centered">
          Overview of the Proposed Sparse Coding Architecture that can show more robustness against privacy attacks.
        </h2>
      </div>
      <div class="item">
        <!-- Your image here -->
        <img src="./assets/img/teaser_example_2.png" alt="SCA Performance on CelebA Dataset"/>
        <h2 class="subtitle has-text-centered">
          Qualitative Comparisons in CelebA Dataset among Original vs. Reconstructed Images in SOTA Defenses and our Proposed SCA.
        </h2>
      </div>
      <div class="item">
        <!-- Your image here -->
        <img src="./assets/img/teaser_example_10.png" alt="SCA Performance on Medical MNIST Dataset"/>
        <h2 class="subtitle has-text-centered">
          Qualitative Comparisons Medical MNIST Dataset among Original vs. Reconstructed Images in SOTA Defenses and our Proposed SCA.
       </h2>
     </div>
     <div class="item">
        <!-- Your image here -->
        <img src="./assets/img/teaser_example_12.png" alt="UMap Representations Comparisons"/>
        <h2 class="subtitle has-text-centered">
          UMap 2D projections of input images’ features by class after 2 linear layers, 2
conv. layers, or 2 sparse-coded layers on MNIST (top) & Fashion MNIST (bottom).
       </h2>
     </div>
  </div>
</div>
</div>
</section>
<!-- End image carousel -->




<!-- Survey -->
<section class="section hero is-light">
  <div class="container is-max-desktop">
    <div class="columns is-centered has-text-centered">
      <div class="column is-four-fifths">
        <h2 class="title is-3">Abstract</h2>
        <div class="content has-text-justified">
          
          <p>
Interested? Please Complete the Following Brief Survey for additional Info or Resources for this Project
            <a href="https://forms.gle/Xf3VJMhf1CnGHVMW7" target="_blank"
                  class="external-link button is-normal is-rounded is-dark">
        </div>
      </div>
    </div>
  </div>
</section>
<!-- End survey -->









  <footer class="footer">
  <div class="container">
    <div class="columns is-centered">
      <div class="column is-8">
        <div class="content">

          <p>
            This page was built using the <a href="https://github.com/eliahuhorwitz/Academic-project-page-template" target="_blank">Academic Project Page Template</a> which was adopted from the <a href="https://nerfies.github.io" target="_blank">Nerfies</a> project page.
            You are free to borrow the of this website, we just ask that you link back to this page in the footer. <br> This website is licensed under a <a rel="license"  href="http://creativecommons.org/licenses/by-sa/4.0/" target="_blank">Creative
            Commons Attribution-ShareAlike 4.0 International License</a>.
          </p>

        </div>
      </div>
    </div>
  </div>
</footer>

<!-- Statcounter tracking code -->
  
<!-- You can add a tracker to track page visits by creating an account at statcounter.com -->

    <!-- End of Statcounter Code -->

  </body>
  </html>

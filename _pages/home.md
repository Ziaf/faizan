---
layout: single
permalink: /
---

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<style>
 /* Original CSS remains unchanged */

/* === Full Width Overrides === */
/* Override ALL width limitations in theme and template */
body,
.initial-content,
#main,
.page,
.splash,
.archive,
.archive__item,
.masthead__inner-wrap,
.greedy-nav,
.page__related,
.page__content,
.page__inner-wrap,
.page__footer,
.pagination,
.layout--single,
.layout--splash,
.layout--home,
.layout--archive,
.layout--categories,
.layout--tags,
.layout--posts,
.layout--search,
.toc,
.sidebar,
.author__avatar,
.author__content,
.author__urls-wrapper,
.feature__wrapper,
.feature__item,
.post-grid,
header,
footer {
  max-width: 100% !important;
  width: 100% !important;
  margin-left: auto !important;
  margin-right: auto !important;
}

/* Override container width */
.container {
  max-width: 100% !important;
  width: 100% !important;
  padding-left: 3% !important;
  padding-right: 3% !important;
  box-sizing: border-box !important;
}

/* Make header content full width */
.header-section {
  width: 100% !important;
  max-width: 100% !important;
}

.header-content {
  width: 100% !important;
  max-width: 100% !important;
}

/* Make content sections fill width */
.section,
.grid-container,
.card,
.news-container,
.publication-item,
.skills-container {
  width: 100% !important;
  max-width: 100% !important;
}

/* Full width grid items */
.grid-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)) !important;
  width: 100% !important;
}

/* Reset any float properties that might affect layout */
.layout--single .page,
.layout--single #main,
.layout--home .page,
.layout--archive .page,
.layout--categories .page,
.layout--tags .page,
.archive__item,
.archive__item-teaser {
  float: none !important;
}

/* Fix for Jekyll navigation and header */
.masthead,
.masthead__menu,
.masthead__menu-item,
.greedy-nav {
  width: 100% !important;
  max-width: 100% !important;
}

/* Override specific breakpoints */
@media (min-width: 64em) {
  .layout--single .page,
  .layout--archive .page,
  #main,
  .archive,
  .archive__item-teaser {
    float: none !important;
    width: 100% !important;
    padding-right: 0 !important;
  }
  
  .sidebar {
    float: none !important;
    width: 100% !important;
    margin-right: 0 !important;
  }
  
  .masthead__inner-wrap {
    max-width: 100% !important;
    padding-left: 3% !important;
    padding-right: 3% !important;
  }
  
  .page__related {
    float: none !important;
    width: 100% !important;
  }
}

@media (min-width: 80em) {
  .layout--single .page,
  #main,
  .archive__item-teaser {
    width: 100% !important;
    padding-right: 0 !important;
  }
  
  /* Ensure container remains full width at large screens */
  .container {
    max-width: 100% !important;
    padding-left: 3% !important;
    padding-right: 3% !important;
  }
}

/* Responsive adjustments */
@media (max-width: 992px) {
  .container {
    padding-left: 2% !important;
    padding-right: 2% !important;
  }
}

@media (max-width: 768px) {
  .container {
    padding-left: 1.5% !important;
    padding-right: 1.5% !important;
  }
}

/* Override Jekyll defaults */
.layout--single .page__content,
.layout--home .page__content,
.page__inner-wrap {
  width: 100% !important;
  max-width: 100% !important;
  float: none !important;
}

/* Ensure no content overflow */
body {
  overflow-x: hidden !important;
  max-width: 100vw !important;
}
</style>

<!-- Header Section -->
<div class="header-section">
  <div class="container">
    <div class="header-content">
      <div class="profile-info">
        <h1 class="profile-name">Faizanuddin Ansari</h1>
        <p class="subtitle"><strong>Ph.D. Fellow</strong> | <em>Machine Learning & AI Research</em> | <em>he/him</em></p>
        <p class="contact-info"><i class="fas fa-envelope"></i> faizanuddin_r@isical.ac.in</p>
        
        <div class="social-links">
          <a href="mailto:faizanuddin_r@isical.ac.in" class="social-link" title="Email"><i class="fas fa-envelope"></i></a>
          <a href="#" class="social-link" title="CV"><i class="fas fa-file-alt"></i></a>
          <a href="https://github.com/" class="social-link" title="GitHub"><i class="fab fa-github"></i></a>
          <a href="https://scholar.google.com/" class="social-link" title="Google Scholar"><i class="fas fa-graduation-cap"></i></a>
          <a href="https://orcid.org/0009-0009-5517-8846" class="social-link" title="ORCID"><i class="fab fa-orcid"></i></a>
          <a href="https://medium.com/" class="social-link" title="Medium"><i class="fab fa-medium"></i></a>
        </div>
        
        <div class="quote-section" onmouseover="showRandomQuote()" onmouseout="resetQuote()">
          <div id="quote-heading">Ilham 🕊️ (hover for inspiration)</div>
          <div id="random-quote"></div>
        </div>
      </div>
      
      <div class="profile-image">
        <img src="assets/images/avtar.png" alt="Faizanuddin Ansari">
      </div>
    </div>
  </div>
</div>

<!-- Main Content -->
<div class="container">
  <!-- About Section -->
  <section class="section animate-up">
    <h2 class="section-title">About Me</h2>
    <p>I'm a <strong>Ph.D. fellow</strong> at the <a href="https://www.isical.ac.in" target="_blank" style="color: var(--primary-color); text-decoration: none; font-weight: 500;">Indian Statistical Institute (ISI), Kolkata</a>, working under the supervision of <a href="https://www.isical.ac.in/~swagatam.das/" target="_blank" style="color: var(--primary-color); text-decoration: none; font-weight: 500;">Prof. Swagatam Das</a> in the <a href="https://www.isical.ac.in/~ecsu/?q=node/1" target="_blank" style="color: var(--primary-color); text-decoration: none; font-weight: 500;">Electronics and Communication Sciences Unit (ECSU)</a>.</p>
    <p>Most real-world datasets are far from ideal—they're imbalanced, biased, or simply too small to learn from effectively — and that's exactly where I come in. My doctoral research focuses on building <strong>resilient deep learning models</strong> to solve challenges around <strong>class imbalance</strong>, <strong>long-tailed distributions</strong>, <strong>bias mitigation</strong>, and <strong>fairness</strong>.</p>
    
    <div class="grid-container">
      <div class="card">
        <h3 class="card-title"><i class="fas fa-flask"></i> Research Focus</h3>
        <p>My work focuses on designing algorithms that tackle real-world data challenges such as class imbalance, long-tailed distributions, bias mitigation, and fairness in machine learning. I develop novel techniques to ensure AI systems perform reliably even when trained on imperfect data.</p>
      </div>
      
      <div class="card">
        <h3 class="card-title"><i class="fas fa-graduation-cap"></i> Education</h3>
        <p><strong>Ph.D. in Machine Learning</strong><br>Indian Statistical Institute, Kolkata<br>Advisor: Prof. Swagatam Das</p>
        <p><strong>M.Tech in Computer Science and Engineering</strong><br>Specialization: Software Engineering<br>Aligarh Muslim University (AMU)</p>
        <p><strong>B.Tech in Computer Engineering</strong><br>Zakir Husain College of Engineering & Technology, AMU</p>
      </div>
    </div>
  </section>
  
  <!-- News Section -->
  <section class="section animate-up">
    <h2 class="section-title">Latest News</h2>
    <div class="news-container">
      <table class="news-table">
        <thead>
          <tr>
            <th>📅 Date</th>
            <th>🗞️ News</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><strong>May 2024</strong></td>
            <td>
              Presented my research (poster) at <strong>IEEE ISBI 2024</strong>, Athens, Greece.
            </td>
          </tr>
          <tr>
            <td><strong>May 2024</strong></td>
            <td>
              Our work <a href="https://ieeexplore.ieee.org/document/10555431" target="_blank" style="color: var(--accent-color); text-decoration: none; font-weight: 500;">CCO: A Cluster Core-based Oversampling Technique for Improved Class-Imbalanced Learning</a> has been published in <a href="https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=7433297" target="_blank" style="color: var(--primary-color); text-decoration: none; font-weight: 500;">IEEE TETCI</a>.
            </td>
          </tr>
          <tr>
            <td><strong>February 2024</strong></td>
            <td>
              (Poster) Paper on <strong>Mo2E: Mixture of Two Experts for Class-Imbalanced Learning from Medical Images</strong> accepted at <a href="https://biomedicalimaging.org/2024/" target="_blank" style="color: var(--accent-color); text-decoration: none;">IEEE ISBI 2024</a>. <a href="https://ieeexplore.ieee.org/document/10635212" target="_blank" style="color: var(--primary-color); text-decoration: none;">[View Paper]</a>
            </td>
          </tr>
          <tr>
            <td><strong>April 2023</strong></td>
            <td>
              (Oral & Poster) Paper on <strong>Handling Class Imbalance by Estimating Minority Class Statistics</strong> accepted at <a href="https://2023.ijcnn.org/" target="_blank" style="color: var(--accent-color); text-decoration: none;">IEEE IJCNN 2023</a>. <a href="https://ieeexplore.ieee.org/document/10191975/" target="_blank" style="color: var(--primary-color); text-decoration: none;">[View Paper]</a>
            </td>
          </tr>
        </tbody>
      </table>
    </div>
  </section>
  
  <!-- Publications Section -->
  <section class="section animate-up">
    <h2 class="section-title">Selected Publications</h2>
    
    <div class="publication-item">
      <h3 class="publication-title">CCO: A Cluster Core-based Oversampling Technique for Improved Class-Imbalanced Learning</h3>
      <p class="publication-authors">Faizanuddin Ansari, Swagatam Das</p>
      <p class="publication-venue">IEEE Transactions on Emerging Topics in Computational Intelligence (TETCI), 2024</p>
      <div class="publication-links">
        <a href="https://ieeexplore.ieee.org/document/10555431" class="pub-link" target="_blank"><i class="fas fa-external-link-alt"></i> View Paper</a>
        <a href="#" class="pub-link"><i class="fas fa-code"></i> Code</a>
        <a href="#" class="pub-link"><i class="fas fa-file-pdf"></i> PDF</a>
      </div>
    </div>
    
    <div class="publication-item">
      <h3 class="publication-title">Mo2E: Mixture of Two Experts for Class-Imbalanced Learning from Medical Images</h3>
      <p class="publication-authors">Faizanuddin Ansari, Swagatam Das</p>
      <p class="publication-venue">IEEE International Symposium on Biomedical Imaging (ISBI), 2024</p>
      <div class="publication-links">
        <a href="https://ieeexplore.ieee.org/document/10635212" class="pub-link" target="_blank"><i class="fas fa-external-link-alt"></i> View Paper</a>
        <a href="#" class="pub-link"><i class="fas fa-code"></i> Code</a>
        <a href="#" class="pub-link"><i class="fas fa-file-pdf"></i> PDF</a>
      </div>
    </div>
    
    <div class="publication-item">
      <h3 class="publication-title">Handling Class Imbalance by Estimating Minority Class Statistics</h3>
      <p class="publication-authors">Faizanuddin Ansari, Swagatam Das</p>
      <p class="publication-venue">IEEE International Joint Conference on Neural Networks (IJCNN), 2023</p>
      <div class="publication-links">
        <a href="https://ieeexplore.ieee.org/document/10191975/" class="pub-link" target="_blank"><i class="fas fa-external-link-alt"></i> View Paper</a>
        <a href="#" class="pub-link"><i class="fas fa-code"></i> Code</a>
        <a href="#" class="pub-link"><i class="fas fa-file-pdf"></i> PDF</a>
      </div>
    </div>
  </section>
  
  <!-- Research Interests & Skills -->
  <section class="section animate-up">
    <h2 class="section-title">Research Interests & Skills</h2>
    
    <div class="grid-container">
      <div class="card">
        <h3 class="card-title"><i class="fas fa-brain"></i> Research Areas</h3>
        <div class="skills-container">
          <span class="skill-tag">Machine Learning</span>
          <span class="skill-tag">Deep Learning</span>
          <span class="skill-tag">Class Imbalance</span>
          <span class="skill-tag">Long-tailed Distributions</span>
          <span class="skill-tag">Bias Mitigation</span>
          <span class="skill-tag">Fairness in ML</span>
          <span class="skill-tag">Medical Image Analysis</span>
          <span class="skill-tag">Computer Vision</span>
        </div>
      </div>
      
      <div class="card">
        <h3 class="card-title"><i class="fas fa-code"></i> Technical Skills</h3>
        <div class="skills-container">
          <span class="skill-tag">Python</span>
          <span class="skill-tag">PyTorch</span>
          <span class="skill-tag">TensorFlow</span>
          <span class="skill-tag">Scikit-learn</span>
          <span class="skill-tag">Data Analysis</span>
          <span class="skill-tag">Statistical Methods</span>
          <span class="skill-tag">Computer Vision</span>
          <span class="skill-tag">Research & Publication</span>
        </div>
      </div>
    </div>
  </section>
  
  <!-- Contact Section -->
  <section class="section animate-up">
    <h2 class="section-title">Contact Me</h2>
    <p>If you're interested in my research or potential collaborations, feel free to reach out!</p>
    
    <div class="grid-container">
      <div class="card">
        <h3 class="card-title"><i class="fas fa-map-marker-alt"></i> Location</h3>
        <p>Electronics and Communication Sciences Unit (ECSU)<br>Indian Statistical Institute<br>Kolkata, India</p>
      </div>
      
      <div class="card">
        <h3 class="card-title"><i class="fas fa-envelope"></i> Email</h3>
        <p>faizanuddin_r@isical.ac.in</p>
        
        <div class="contact-form">
          <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
            <div class="form-group">
              <label for="name">Name</label>
              <input type="text" id="name" name="name" class="form-control" placeholder="Your name" required>
            </div>
            
            <div class="form-group">
              <label for="email">Email</label>
              <input type="email" id="email" name="_replyto" class="form-control" placeholder="Your email" required>
            </div>
            
            <div class="form-group">
              <label for="message">Message</label>
              <textarea id="message" name="message" class="form-control" placeholder="Your message" required></textarea>
            </div>
            
            <button type="submit" class="btn">Send Message</button>
          </form>
        </div>
      </div>
    </div>
  </section>
</div>

<!-- Footer -->
 <footer> <div class="container"><p>&copy; 2025 Faizanuddin Ansari. All rights reserved.</p> </div> </footer> 

<!-- Scripts -->
<script>
  // Quote functionality
  const quotes = [
    `فَإِنَّ مَعَ العُسرِ يُسرًا <br><em>"So, surely with hardship comes ease." (Qur'an 94:5)</em>`,
    `إِنَّ ٱللَّهَ مَعَ ٱلصَّبِرِينَ <br><em>"I will be with those who have patience." (Qur'an 2:153)</em>`,
    `لَا يُكَلِّفُ اللَّهُ نَفْسًا إِلَّا وُسْعَهَا <br><em>"Allah does not burden a soul beyond that it can bear." (Qur'an 2:286)</em>`,
  ];

  function showRandomQuote() {
    const randomQuote = quotes[Math.floor(Math.random() * quotes.length)];
    document.getElementById('random-quote').innerHTML = `<p>${randomQuote}</p>`;
  }

  function resetQuote() {
    document.getElementById('random-quote').innerHTML = "";
  }
  
  // Animation on scroll
  document.addEventListener('DOMContentLoaded', function() {
    const animatedElements = document.querySelectorAll('.animate-up');
    
    function checkIfInView() {
      animatedElements.forEach(element => {
        const elementPosition = element.getBoundingClientRect().top;
        const windowHeight = window.innerHeight;
        
        if (elementPosition < windowHeight - 100) {
          element.classList.add('show');
        }
      });
    }
    
    // Initial check
    setTimeout(checkIfInView, 300);
    
    // Check on scroll
    window.addEventListener('scroll', checkIfInView);
  });
</script>

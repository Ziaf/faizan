---
layout: single
permalink: /
---

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<style>
   :root {
    --primary-color: #1a73e8;
    --secondary-color: #34495e;
    --accent-color: #8e44ad;
    --light-bg: #f8f9fa;
    --dark-bg: #2c3e50;
    --text-color: #333;
    --light-text: #666;
    --border-color: #eaecef;
    --card-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    --transition-speed: 0.3s;
  }
  
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: var(--text-color);
    background: #fff;
    overflow-x: hidden;
  }
  
  /*.container {
  max-width: 100% !important;
  width: 100% !important;
  padding-left: 3% !important;
  padding-right: 3% !important;
  box-sizing: border-box !important;
}*/
  .container {
  max-width: 100% !important;
  width: 100% !important;
  padding-left: 10% !important;
  padding-right: 10% !important;
  box-sizing: border-box !important;
}
  
  /* Header Styles */
  .header-section {
    background: linear-gradient(135deg, #ffffff 0%, #f8f9fa 100%);
    padding: 40px 0;
    border-bottom: 1px solid var(--border-color);
    position: relative;
    overflow: hidden;
    margin-bottom: 50px;
  }
  
  .header-content {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 40px;
  } 
  
  .profile-info {
    flex: 2;
  }
  
  .profile-image {
    flex: 1;
    text-align: right;
    position: relative;
  }
  
  .profile-image img {
    width: 220px;
    height: 220px;
    object-fit: cover;
    border-radius: 12px;
    box-shadow: var(--card-shadow);
    transition: transform var(--transition-speed);
  }
  
  .profile-image img:hover {
    transform: scale(1.03);
  }
  
  .profile-name {
    font-size: 2.8rem;
    font-weight: 700;
    margin-bottom: 10px;
    color: var(--dark-bg);
    line-height: 1.2;
  }
  
  .subtitle {
    font-size: 1.2rem;
    color: var(--light-text);
    margin-bottom: 15px;
    font-weight: 500;
  }
  
  .contact-info {
    margin-bottom: 20px;
    font-size: 1rem;
  }
  
  .social-links {
    display: flex;
    gap: 15px;
    margin-top: 25px;
  }
  
  .social-link {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 40px;
    height: 40px;
    background-color: var(--light-bg);
    border-radius: 50%;
    color: var(--secondary-color);
    transition: all var(--transition-speed);
    text-decoration: none;
    font-size: 1.2rem;
  }
  
  .social-link:hover {
    background-color: var(--primary-color);
    color: white;
    transform: translateY(-3px);
  }
  
  /* Quote Section */
  .quote-section {
    margin-left: 20px;
    padding: 10px 20px;
    border-left: 3px solid var(--primary-color);
    color: var(--light-text);
    font-style: italic;
    cursor: pointer;
    transition: all var(--transition-speed);
  }
  
  .quote-section:hover {
    background-color: rgba(26, 115, 232, 0.05);
  }
  
  #quote-heading {
    font-weight: 600;
    color: var(--primary-color);
    margin-bottom: 5px;
  }
  
  #random-quote {
    min-height: 60px;
    line-height: 1.5;
  }
  
  /* Main Content */
  .section {
    margin-bottom: 60px;
  }
  
  .section-title {
    font-size: 1.8rem;
    margin-bottom: 25px;
    color: var(--dark-bg);
    position: relative;
    padding-bottom: 10px;
    border-bottom: 2px solid var(--border-color);
  }
  
  .section-title::after {
    content: '';
    position: absolute;
    bottom: -2px;
    left: 0;
    width: 60px;
    height: 2px;
    background-color: var(--primary-color);
  }
  
  .grid-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
    margin-top: 30px;
  }
  
  .card {
    background-color: white;
    border-radius: 10px;
    padding: 25px;
    box-shadow: var(--card-shadow);
    transition: all var(--transition-speed);
    height: 100%;
    border: 1px solid var(--border-color);
  }
  
  .card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
  }
  
  .card-title {
    font-size: 1.3rem;
    margin-bottom: 15px;
    color: var(--secondary-color);
    display: flex;
    align-items: center;
    gap: 10px;
  }
  
  .card-title i {
    color: var(--primary-color);
  }
  
  /*  Section */
  .news-container {
    max-height: 600px;
    overflow-y: auto;
    border: 1px solid var(--border-color);
    border-radius: 10px;
    box-shadow: var(--card-shadow);
  }
  
  .news-table {
    width: 100%;
    border-collapse: collapse;
  }
  
  .news-table thead {
    position: sticky;
    top: 0;
    z-index: 1;
  }
  
  .news-table th, .news-table td {
    padding: 15px 20px;
    text-align: left;
    border-bottom: 1px solid var(--border-color);
  }
  
  .news-table th {
    background-color: var(--light-bg);
    color: var(--secondary-color);
    font-weight: 600;
  }
  
  .news-table tr:nth-child(even) {
    background-color: #f9f9f9;
  }
  
  .news-table tr:hover {
    background-color: rgba(26, 115, 232, 0.05);
  }
  
  /* Publication Section */
  .publication-item {
    margin-bottom: 25px;
    padding-bottom: 25px;
    border-bottom: 1px solid var(--border-color);
  }
  
  .publication-item:last-child {
    border-bottom: none;
  }
  
  .publication-title {
    font-size: 1.2rem;
    font-weight: 600;
    margin-bottom: 10px;
    color: var(--secondary-color);
  }
  
  .publication-authors {
    font-style: italic;
    margin-bottom: 8px;
    color: var(--light-text);
  }
  
  .publication-venue {
    margin-bottom: 12px;
    color: var(--accent-color);
    font-weight: 500;
  }
  
  .publication-links {
    display: flex;
    gap: 15px;
    flex-wrap: wrap;
  }
  
  .pub-link {
    display: inline-flex;
    align-items: center;
    gap: 5px;
    padding: 6px 12px;
    background-color: var(--light-bg);
    border-radius: 4px;
    color: var(--secondary-color);
    text-decoration: none;
    font-size: 0.9rem;
    transition: all var(--transition-speed);
  }
  
  .pub-link:hover {
    background-color: var(--primary-color);
    color: white;
  }
  
  /* Skills Section */
  .skills-container {
    display: flex;
    flex-wrap: wrap;
    gap: 15px;
    margin-top: 20px;
  }
  
  .skill-tag {
    padding: 8px 16px;
    background-color: var(--light-bg);
    border-radius: 50px;
    color: var(--secondary-color);
    font-size: 0.95rem;
    transition: all var(--transition-speed);
    cursor: default;
  }
  
  .skill-tag:hover {
    background-color: var(--primary-color);
    color: white;
    transform: translateY(-3px);
  }
  
  /* Contact Form */
  .form-group {
    margin-bottom: 20px;
  }
  
  .form-group label {
    display: block;
    margin-bottom: 8px;
    color: var(--secondary-color);
    font-weight: 500;
  }
  
  .form-control {
    width: 100%;
    padding: 12px 15px;
    border: 1px solid var(--border-color);
    border-radius: 5px;
    font-size: 1rem;
    transition: all var(--transition-speed);
  }
  
  .form-control:focus {
    outline: none;
    border-color: var(--primary-color);
    box-shadow: 0 0 0 3px rgba(26, 115, 232, 0.2);
  }
  
  textarea.form-control {
    min-height: 150px;
    resize: vertical;
  }
  
  .btn {
    display: inline-block;
    padding: 12px 25px;
    background-color: var(--primary-color);
    color: white;
    border: none;
    border-radius: 5px;
    font-size: 1rem;
    font-weight: 500;
    cursor: pointer;
    transition: all var(--transition-speed);
    text-align: center;
  }
  
  .btn:hover {
    background-color: #0d62d0;
    transform: translateY(-2px);
  }
  
  /* Footer */
 /* footer {
    background-color: var(--light-bg);
    padding: 30px 0;
    text-align: center;
    color: var(--light-text);
    border-top: 1px solid var(--border-color);
    margin-top: 60px;
  }*/
  
  /* Animation for elements */
  .animate-up {
    opacity: 0;
    transform: translateY(30px);
    transition: all 0.8s ease;
  }
  
  .animate-up.show {
    opacity: 1;
    transform: translateY(0);
  }
  
  /* Responsive */
  @media (max-width: 992px) {
    .header-content {
      flex-direction: column-reverse;
      text-align: center;
    }
    
    .profile-image {
      text-align: center;
      margin-bottom: 30px;
    }
    
    .social-links {
      justify-content: center;
    }
    
    .quote-section {
      margin: 30px auto 0;
      max-width: 500px;
    }
  }
  
  @media (max-width: 768px) {
    .profile-name {
      font-size: 2.2rem;
    }
    
    .section-title {
      font-size: 1.6rem;
    }
    
    .news-container {
      overflow-x: visible;
    }
    
    .publication-links {
      flex-direction: column;
      gap: 10px;
    }
    
    .pub-link {
      width: fit-content;
    }
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
 <!-- <footer> <div class="container"><p>&copy; 2025 Faizanuddin Ansari. All rights reserved.</p> </div> </footer> -->

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

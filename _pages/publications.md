---
layout: single
title: "Publications"
permalink: /publications/
---
<style>
  :root {
    --bg-color: #ffffff;
    --card-bg: #ffffff;
    --text-color: #1c1c1c;
    --border-color: #e0e0e0;
    --highlight: #2980b9;
    --hover-bg: #f5f5f5;
    --card-shadow: rgba(0, 0, 0, 0.1);
    --tag-bg: #e9f2fa;
    --tag-text: #2980b9;
  }

  @media (prefers-color-scheme: dark) {
    :root {
      --bg-color: #121212;
      --card-bg: #1e1e1e;
      --text-color: #e0e0e0;
      --border-color: #2c2c2c;
      --highlight: #4da6ff;
      --hover-bg: #1f1f1f;
      --card-shadow: rgba(0, 0, 0, 0.3);
      --tag-bg: #253544;
      --tag-text: #4da6ff;
    }
  }

  .publications-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
    font-family: 'Segoe UI', Arial, sans-serif;
    color: var(--text-color);
  }

  .pub-controls {
    display: flex;
    flex-wrap: wrap;
    gap: 15px;
    margin-bottom: 30px;
    align-items: center;
  }

  .pub-search {
    flex-grow: 1;
    padding: 12px 16px;
    font-size: 16px;
    border: 1px solid var(--border-color);
    border-radius: 8px;
    background-color: var(--card-bg);
    color: var(--text-color);
    transition: all 0.3s ease;
  }

  .pub-search:focus {
    outline: none;
    border-color: var(--highlight);
    box-shadow: 0 0 0 2px rgba(41, 128, 185, 0.2);
  }

  .filter-group {
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
  }

  .filter-btn {
    padding: 8px 16px;
    border: 1px solid var(--border-color);
    border-radius: 20px;
    background-color: var(--card-bg);
    color: var(--text-color);
    cursor: pointer;
    transition: all 0.3s ease;
    font-size: 14px;
  }

  .filter-btn:hover, .filter-btn.active {
    background-color: var(--highlight);
    color: white;
  }

  .pub-year-divider {
    font-size: 22px;
    font-weight: 700;
    margin: 40px 0 20px;
    color: var(--highlight);
    display: flex;
    align-items: center;
  }

  .pub-year-divider::after {
    content: "";
    flex-grow: 1;
    height: 1px;
    background-color: var(--border-color);
    margin-left: 15px;
  }

  .pub-card {
    display: flex;
    gap: 24px;
    padding: 24px;
    margin-bottom: 24px;
    background-color: var(--card-bg);
    border-radius: 12px;
    box-shadow: 0 4px 12px var(--card-shadow);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    position: relative;
    overflow: hidden;
  }

  .pub-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px var(--card-shadow);
  }

  .pub-image-container {
    flex-shrink: 0;
    position: relative;
    width: 200px;
    margin-top: 5px;
  }

  .pub-image {
    width: 200px;
    height: 150px;
    object-fit: cover;
    border-radius: 8px;
    border: 1px solid var(--border-color);
    transition: transform 0.3s ease;
  }

  .pub-image:hover {
    transform: scale(1.03);
  }

  .pub-content {
    flex-grow: 1;
    display: flex;
    flex-direction: column;
  }

  .pub-title {
    font-size: 20px;
    font-weight: 600;
    margin-bottom: 8px;
    color: var(--text-color);
    line-height: 1.4;
  }

  .pub-authors {
    font-size: 15px;
    margin-bottom: 12px;
    color: var(--text-color);
  }

  .pub-venue {
    font-style: italic;
    font-size: 14px;
    margin-bottom: 16px;
    color: var(--text-color);
    opacity: 0.85;
  }

  .pub-abstract {
    font-size: 15px;
    line-height: 1.6;
    margin-bottom: 16px;
    position: relative;
    color: var(--text-color);
    opacity: 0.9;
  }

  .pub-abstract-full {
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.5s ease;
  }

  .pub-abstract-toggle {
    display: inline-block;
    color: var(--highlight);
    cursor: pointer;
    font-weight: 500;
    user-select: none;
    margin-bottom: 16px;
  }

  .pub-abstract-toggle:hover {
    text-decoration: underline;
  }

  .pub-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    margin-bottom: 16px;
  }

  .pub-tag {
    padding: 4px 10px;
    border-radius: 16px;
    font-size: 12px;
    font-weight: 500;
    background-color: var(--tag-bg);
    color: var(--tag-text);
  }

  .pub-links {
    display: flex;
    gap: 12px;
    margin-top: auto;
  }

  .pub-link {
    display: inline-flex;
    align-items: center;
    padding: 8px 16px;
    border-radius: 6px;
    background-color: var(--highlight);
    color: white;
    text-decoration: none;
    font-size: 14px;
    font-weight: 500;
    transition: all 0.2s ease;
  }

  .pub-link:hover {
    opacity: 0.9;
    transform: translateY(-2px);
  }

  .pub-link i {
    margin-right: 6px;
  }

  .pub-secondary-link {
    background-color: transparent;
    border: 1px solid var(--highlight);
    color: var(--highlight);
  }

  .pub-secondary-link:hover {
    background-color: var(--highlight);
    color: white;
  }

  @media (max-width: 768px) {
    .pub-card {
      flex-direction: column;
    }
    
    .pub-image-container {
      width: 100%;
      margin-bottom: 16px;
    }
    
    .pub-image {
      width: 100%;
      height: auto;
      aspect-ratio: 4/3;
    }
  }

  .no-results {
    text-align: center;
    padding: 40px;
    font-size: 18px;
    color: var(--text-color);
    opacity: 0.7;
  }

  .highlight-animation {
    animation: highlight-pulse 2s infinite;
  }

  @keyframes highlight-pulse {
    0% { box-shadow: 0 4px 12px var(--card-shadow); }
    50% { box-shadow: 0 4px 20px var(--highlight); }
    100% { box-shadow: 0 4px 12px var(--card-shadow); }
  }
</style>

<div class="publications-container">
  <div class="pub-controls">
    <input type="text" id="pubSearch" class="pub-search" placeholder="Search by title, author, or keywords...">
    <div class="filter-group">
      <button class="filter-btn active" data-year="all">All Years</button>
      <button class="filter-btn" data-year="2025">2025</button>
      <button class="filter-btn" data-year="2024">2024</button>
      <button class="filter-btn" data-year="2023">2023</button>
    </div>
  </div>

  <div id="publicationsContainer">
    <!-- Publications will be dynamically inserted here -->
  </div>
</div>

<script>
// Publication data
const publications = [
  {
    year: 2025,
    image: "assets/publications/mot_diag.png",
    title: "Force of Attraction-Based Distribution Calibration for Enhancing Minority Class Representation",
    authors: "Mondal, P., Ansari, F., Das, S., &amp; Shamsolmoali, P.",
    venue: "2025 International Joint Conference on Neural Networks (IJCNN). IEEE.",
    abstract: "Imbalanced image datasets pose significant challenges for developing robust classifiers, particularly when certain classes are heavily underrepresented. To tackle this issue, we propose Density-Driven Attraction (DDA) Oversampling, a novel technique designed to improve class representation in the latent space. Our approach begins by projecting images into disentangled latent representations, ensuring clear separation between classes and precise identification of subclasses. At the core of this method is the Density-Driven Attraction Force (DDAF), a mechanism inspired by gravitational forces. DDAF quantifies the attraction between components of well-represented and underrepresented classes, adjusting the attraction based on the density of each component. This process recalibrates the distributions of underrepresented classes by leveraging their strongest attractions, effectively simulating the natural principles of mass attraction. Extensive classification experiments on six multiclass imbalanced datasets demonstrate that DDA Oversampling outperforms existing state-of-the-art methods, resulting in more accurate and balanced class distributions.",
    paperLink: "https://ieeexplore.ieee.org/",
    paperText: "Available Soon",
    tags: ["Class Imbalance", "Neural Networks", "Image Classification", "Density-Driven Attraction"]
  },
  {
    year: 2025,
    image: "assets/publications/goldilock.png",
    title: "The Goldilocks Principle: Achieving Just Right Boundary Fidelity for Long-Tailed Classification",
    authors: "Ansari, F., Panigrahi, A., &amp; Das, S.",
    venue: "IEEE Transactions on Emerging Topics in Computational Intelligence",
    abstract: "This study addresses the challenges of learning from long-tailed class imbalances in deep neural networks, particularly for image recognition. Long-tailed class imbalances occur when a dataset's class distribution is highly skewed, with a few head classes containing many instances and numerous tail classes having fewer instances. This imbalance becomes problematic when traditional classification methods, especially deep learning models, prioritize accuracy in the more frequent classes, neglecting the less common ones. Furthermore, these methods struggle to maintain consistent boundary fidelity—decision boundaries that are sharp enough to distinguish classes yet smooth enough to generalize well. Hard boundaries, often caused by overfitting tail classes, amplify intra-class variations, while overly soft boundaries blur distinctions between classes, reducing classification accuracy. We propose a dual-branch network with a shared feature extractor to overcome these challenges. This network uses instance and median samplers for head and medium classes and a reverse sampler for tail classes. Additionally, we implement a specialized loss function as a feature regularizer to reduce the model's sensitivity to irrelevant intra-class variations during classification. This loss function dynamically modulates feature representation alignment, promoting cohesive intra-class structures and clear inter-class separations. To achieve this, our framework incorporates two key components: Dual-Branch Sampler-Guided Mixup (DBSGM) and Adaptive Class-Aware Feature Regularizer (ACFR), which work together to balance class representation and refine decision boundaries. Integrating DBSGM and ACFR during training helps shape decision boundaries that align with class semantics. To ensure class boundaries are appropriately defined, we propose the temperature-adaptive supervised contrastive loss (TASCL) within the ACFR module, achieving the right balance between smoothness and sharpness. Our single-stage, end-to-end framework demonstrates significant performance improvements, offering a promising solution to the challenges of long-tailed class imbalances in deep learning.",
    paperLink: "https://ieeexplore.ieee.org/",
    paperText: "Available Soon",
    tags: ["Long-Tailed Classification", "Boundary Fidelity", "Deep Learning", "Image Recognition"]
  },
  {
    year: 2024,
    image: "assets/publications/skin_fairness.jpg",
    title: "Algorithmic Fairness in Lesion Classification by Mitigating Class Imbalance and Skin Tone Bias",
    authors: "Ansari, F., Chakraborti, T., &amp; Das, S.",
    venue: "International Conference on Medical Image Computing and Computer-Assisted Intervention, 373–382. Springer Nature Switzerland Cham.",
    abstract: "Deep learning models have shown considerable promise in the classification of skin lesions. However, a notable challenge arises from their inherent bias towards dominant skin tones and the issue of imbalanced class representation. This study introduces a novel data augmentation technique designed to address these limitations. Our approach harnesses contextual information from the prevalent class to synthesize various samples representing minority classes. Using a mixup-based algorithm guided by an adaptive sampler, our method effectively tackles bias and class imbalance issues. The adaptive sampler dynamically adjusts sampling probabilities based on the network's meta-set performance, enhancing overall accuracy. Our research demonstrates the efficacy of this approach in mitigating skin tone bias and achieving robust lesion classification across a spectrum of diverse skin colors from two distinct benchmark datasets, offering promising implications for improving dermatological diagnostic systems.",
    paperLink: "https://link.springer.com/chapter/10.1007/978-3-031-72378-0_35",
    paperText: "Paper",
    tags: ["Algorithmic Fairness", "Skin Lesion Classification", "Medical Imaging", "Bias Mitigation"]
  },
  {
    year: 2024,
    image: "assets/publications/cco_oversampling.jpg",
    title: "CCO: A cluster core-based oversampling technique for improved class-imbalanced learning",
    authors: "Mondal, P., Ansari, F., &amp; Das, S.",
    venue: "IEEE Transactions on Emerging Topics in Computational Intelligence",
    abstract: "Supervised classification problems from the real world typically face a challenge characterized by the scarcity of samples in one or more target classes compared to the rest of the majority classes. In response to such class imbalance, we propose an oversampling technique based on clustering, aiming to populate the minority class with synthetic samples. This approach capitalizes on the notion of \"Cluster Cores,\" representing locally dense regions within clusters. These Cluster Cores act as central, densely crowded areas that capture intricate topological properties of the corresponding clusters, especially in complex datasets with a non-convex spatial orientation in the feature space. By concentrating on these high-density regions, our clustering-based oversampling technique generates synthetic samples within the convex hull region of minority class instances in the formed clusters. This strategy ensures the creation of points that align with the data space and considers each minority instance within a specific cluster, thereby averting the problems encountered due to the generation of artificial samples by mere linear combination of the minority class data points, as is encountered in SMOTE (Synthetic Minority Oversampling Technique)-based algorithms. To assess the efficacy of our proposal, we conducted experimental comparisons against several cutting-edge algorithms, considering an array of evaluation metrics on well-known datasets used in the literature for both binary and multi-class classification. Additionally, we undertook a detailed ablation study, scrutinized existing algorithms in our context, delineated their strengths and limitations, and contemplated potential research directions in this domain.",
    paperLink: "https://ieeexplore.ieee.org/document/10555431",
    paperText: "Paper",
    tags: ["Cluster Core Oversampling", "Class Imbalance", "Classification", "Synthetic Samples"]
  },
  {
    year: 2024,
    image: "assets/publications/mo2e_experts.jpg",
    title: "Mo2E: Mixture of Two Experts for Class-Imbalanced Learning from Medical Images",
    authors: "Ansari, F., Bhattacharya, A., Saha, B., &amp; Das, S.",
    venue: "2024 IEEE International Symposium on Biomedical Imaging (ISBI), 1–5. IEEE.",
    abstract: "Class imbalance in the medical image dataset is almost inherent due to the limited availability of clinical data for certain diseases and patient populations. Under-represented classes in the training set affect the classification task because the classifier tends to learn more from the majority classes, which are more common in the dataset and ignore data from the minority classes. To mitigate this issue, we propose a method to learn using two different convolutional neural network-based experts; such experts try to learn boundaries within the head classes, between the head and tail classes, and within the tail classes. During expert training, we integrate the MixUp regularization method to augment imbalanced data, employing distinct data sampling strategies for more effective mixing compared to random selection in traditional MixUp. During the inference phase, we combine the logits of the different experts based on their expertise in the corresponding classes. This way, we can improve the accuracy of the head and tail classes. Experiments using highly imbalanced and long-tailed datasets demonstrate the effectiveness of the suggested framework.",
    paperLink: "https://ieeexplore.ieee.org/document/10635212",
    paperText: "Paper",
    tags: ["Medical Imaging", "Mixture of Experts", "Class Imbalance", "CNN"]
  },
  {
    year: 2023,
    image: "assets/publications/minority_statistics.jpg",
    title: "Handling class imbalance by estimating minority class statistics",
    authors: "Ansari, F., Das, S., &amp; Shamsolmoali, P.",
    venue: "2023 International Joint Conference on Neural Networks (IJCNN), 1–8. IEEE.",
    abstract: "The problem of class imbalance arises in machine learning due to the unequal class-specific distribution of data, where most samples belong to one class, and only a few represent the others. To tackle this issue, one paradigm is to use oversampling techniques that synthesize artificial samples of the minority class using the convex combination of the minority class samples taken in some specialized way for different methods. Existing methods do not take into account any information regarding the actual distribution of the minority class, which leads to inconsistencies between the generated distribution and the actual distribution that the minority class might have. In this paper, we propose a parametrization-based method that tries to estimate the statistics of the minority class samples using the statistics of the nearby classes. Using the different hyperparameters, we can control the distribution such that it may approximate the original distribution. Experiments using synthetic and real-world benchmark datasets demonstrate the usefulness of our techniques across multiple metrics.",
    paperLink: "https://ieeexplore.ieee.org/document/10191975",
    paperText: "Paper",
    tags: ["Minority Class Statistics", "Neural Networks", "Oversampling", "Class Imbalance"]
  }
];

function renderPublications(filteredPubs) {
  const container = document.getElementById('publicationsContainer');
  container.innerHTML = '';
  
  if (filteredPubs.length === 0) {
    container.innerHTML = '<div class="no-results">No publications found matching your search criteria.</div>';
    return;
  }
  
  // Group by year
  const pubsByYear = {};
  filteredPubs.forEach(pub => {
    if (!pubsByYear[pub.year]) {
      pubsByYear[pub.year] = [];
    }
    pubsByYear[pub.year].push(pub);
  });
  
  // Sort years in descending order
  const sortedYears = Object.keys(pubsByYear).sort((a, b) => b - a);
  
  // Render publications by year
  sortedYears.forEach(year => {
    const yearDivider = document.createElement('div');
    yearDivider.className = 'pub-year-divider';
    yearDivider.textContent = year;
    container.appendChild(yearDivider);
    
    pubsByYear[year].forEach(pub => {
      const pubCard = document.createElement('div');
      pubCard.className = 'pub-card';
      pubCard.dataset.year = pub.year;
      
      // Create shortened abstract (first 150 characters)
      const shortAbstract = pub.abstract.substring(0, 200) + '...';
      
      pubCard.innerHTML = `
        <div class="pub-image-container">
          <img src="${pub.image}" alt="${pub.title}" class="pub-image">
        </div>
        <div class="pub-content">
          <h2 class="pub-title">${pub.title}</h2>
          <div class="pub-authors">${pub.authors}</div>
          <div class="pub-venue">${pub.venue}</div>
          <div class="pub-abstract">
            <div class="pub-abstract-preview">${shortAbstract}</div>
            <div class="pub-abstract-full" id="abstract-${sortedYears.indexOf(year)}-${pubsByYear[year].indexOf(pub)}">${pub.abstract}</div>
            <span class="pub-abstract-toggle" data-target="abstract-${sortedYears.indexOf(year)}-${pubsByYear[year].indexOf(pub)}">Read more</span>
          </div>
          <div class="pub-tags">
            ${pub.tags.map(tag => `<span class="pub-tag">${tag}</span>`).join('')}
          </div>
          <div class="pub-links">
            <a href="${pub.paperLink}" target="_blank" class="pub-link"><i class="fas fa-scroll"></i>${pub.paperText}</a>
            <a href="#" class="pub-link pub-secondary-link cite-link" data-index="${sortedYears.indexOf(year)}-${pubsByYear[year].indexOf(pub)}"><i class="fas fa-quote-right"></i>Cite</a>
          </div>
        </div>
      `;
      container.appendChild(pubCard);
    });
  });
  
  // Add toggle functionality for abstracts
  document.querySelectorAll('.pub-abstract-toggle').forEach(toggle => {
    toggle.addEventListener('click', function() {
      const targetId = this.getAttribute('data-target');
      const abstractElement = document.getElementById(targetId);
      
      if (this.textContent === 'Read more') {
        abstractElement.style.maxHeight = abstractElement.scrollHeight + 'px';
        this.textContent = 'Read less';
      } else {
        abstractElement.style.maxHeight = '0';
        this.textContent = 'Read more';
      }
    });
  });
  
  // Add citation functionality
  document.querySelectorAll('.cite-link').forEach(link => {
    link.addEventListener('click', function(e) {
      e.preventDefault();
      const indices = this.getAttribute('data-index').split('-');
      const year = sortedYears[parseInt(indices[0])];
      const pubIndex = parseInt(indices[1]);
      const pub = pubsByYear[year][pubIndex];
      
      // Create citation text in different formats
      alert(`Citation copied to clipboard: ${pub.authors} (${pub.year}). ${pub.title}. ${pub.venue}`);
      
      // Highlight the publication card temporarily
      const card = this.closest('.pub-card');
      card.classList.add('highlight-animation');
      setTimeout(() => {
        card.classList.remove('highlight-animation');
      }, 2000);
    });
  });
}

// Filter publications by year and search term
function filterPublications() {
  const searchTerm = document.getElementById('pubSearch').value.toLowerCase();
  const activeYearBtn = document.querySelector('.filter-btn.active');
  const yearFilter = activeYearBtn.getAttribute('data-year');
  
  const filtered = publications.filter(pub => {
    // Filter by year if not "all"
    const yearMatch = yearFilter === 'all' || pub.year.toString() === yearFilter;
    
    // Filter by search term
    const searchMatch = searchTerm === '' || 
      pub.title.toLowerCase().includes(searchTerm) ||
      pub.authors.toLowerCase().includes(searchTerm) ||
      pub.abstract.toLowerCase().includes(searchTerm) ||
      pub.tags.some(tag => tag.toLowerCase().includes(searchTerm));
    
    return yearMatch && searchMatch;
  });
  
  renderPublications(filtered);
}

// Set up event listeners
document.addEventListener('DOMContentLoaded', function() {
  // Initialize with all publications
  renderPublications(publications);
  
  // Search input event
  document.getElementById('pubSearch').addEventListener('input', filterPublications);
  
  // Year filter buttons
  document.querySelectorAll('.filter-btn').forEach(btn => {
    btn.addEventListener('click', function() {
      document.querySelectorAll('.filter-btn').forEach(b => b.classList.remove('active'));
      this.classList.add('active');
      filterPublications();
    });
  });
});
</script>

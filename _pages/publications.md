---
layout: single
title: "Publications"
permalink: /publications/
---
<style>
  :root {
    --bg-color: #ffffff;
    --text-color: #1c1c1c;
    --border-color: #e0e0e0;
    --highlight: #2980b9;
    --hover-bg: #f5f5f5;
  }

  @media (prefers-color-scheme: dark) {
    :root {
      --bg-color: #121212;
      --text-color: #e0e0e0;
      --border-color: #2c2c2c;
      --highlight: #4da6ff;
      --hover-bg: #1f1f1f;
    }
  }

  .pub-section {
    padding: 24px;
    background-color: var(--bg-color);
    border: 1px solid var(--border-color);
    border-radius: 12px;
    margin-top: 30px;
  }

  .pub-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 16px;
  }

  .pub-search {
    padding: 6px 12px;
    font-size: 14px;
    border: 1px solid var(--border-color);
    border-radius: 6px;
    background-color: var(--bg-color);
    color: var(--text-color);
  }

  .pub-table-wrapper {
    max-height: 800px;
    overflow-y: auto;
    overflow-x: auto;
    border-radius: 8px;
    position: relative;
  }

  .pub-table {
    width: 100%;
    border-collapse: separate;
    border-spacing: 0;
    font-family: 'Segoe UI', sans-serif;
    font-size: 15px;
    line-height: 1.6;
    color: var(--text-color);
    background-color: var(--bg-color);
    table-layout: fixed;
  }

  .pub-table thead th {
    background-color: var(--hover-bg);
    position: sticky;
    top: 0;
    z-index: 10;
    border-bottom: 2px solid var(--border-color);
  }

  .pub-table th, .pub-table td {
    padding: 14px;
    text-align: left;
    border-bottom: 1px solid var(--border-color);
    vertical-align: top;
  }

  .pub-table tr:hover {
    background-color: var(--hover-bg);
    transition: background-color 0.3s ease;
  }

  .pub-image {
    width: 180px;
    height: 120px;
    object-fit: cover;
    border-radius: 6px;
    border: 1px solid var(--border-color);
    background-color: #fff;
  }

  details summary {
    cursor: pointer;
    color: var(--highlight);
    font-weight: 500;
    margin-top: 8px;
  }

  .pub-link a {
    color: var(--highlight);
    text-decoration: none;
    font-weight: 500;
  }

  .pub-link a:hover {
    text-decoration: underline;
  }

  @media (max-width: 768px) {
    .pub-image {
      width: 100%;
      height: auto;
    }

    .pub-table td, .pub-table th {
      padding: 10px;
    }
  }
</style>
<div class="pub-section">
  <div class="pub-header">
    <input type="text" id="pubSearch" class="pub-search" placeholder="Search by keyword...">
  </div>
  <div class="pub-table-wrapper">
    <table class="pub-table" id="pubTable">
      <thead style="position: sticky; top: 0; z-index: 2; background-color: var(--hover-bg);">
        <tr>
          <th style="width: 20%;">Visual Insight</th>
          <th style="width: 60%;">Paper</th>
          <th style="width: 12%;">Link</th>
        </tr>
      </thead>
      <tbody>
    <tr>
      <td style="white-space: nowrap; padding: 10px;">2025</td>
      <td><img src="assets/publications/mot_diag.png" alt="Thumbnail" class="pub-image"></td>
      <td>
        Mondal, P., Ansari, F., Das, S., & Shamsolmoali, P. (2025). <strong>Force of Attraction-Based Distribution Calibration for Enhancing Minority Class Representation.</strong> 
        <em>2025 International Joint Conference on Neural Networks (IJCNN)</em>. IEEE.
          <details style="margin-top: 8px;">
            <summary style="cursor: pointer; color: #2980b9;">Abstract</summary>
            <p style="margin-top: 6px;">
        Imbalanced image datasets pose significant challenges for developing robust classifiers, particularly when certain classes are heavily underrepresented. To tackle this issue, we propose Density-Driven Attraction (DDA) Oversampling, a novel technique designed to improve class representation in the latent space. Our approach begins by projecting images into disentangled latent representations, ensuring clear separation between classes and precise identification of subclasses. At the core of this method is the Density-Driven Attraction Force (DDAF), a mechanism inspired by gravitational forces. DDAF quantifies the attraction between components of well-represented and underrepresented classes, adjusting the attraction based on the density of each component. This process recalibrates the distributions of underrepresented classes by leveraging their strongest attractions, effectively simulating the natural principles of mass attraction. Extensive classification experiments on six multiclass imbalanced datasets demonstrate that DDA Oversampling outperforms existing state-of-the-art methods, resulting in more accurate and balanced class distributions.     
  </p>
   </details> 
      </td>
      <td><a href="https://ieeexplore.ieee.org/" target="_blank"><span><i class="fas fa-scroll"></i>Available Soon</span></a></td>
    </tr>
    <tr>
      <td style="white-space: nowrap; padding: 10px;">2025</td>
      <td><img src="assets/publications/goldilock.png" alt="Thumbnail" class="pub-image"></td>
      <td>
        Ansari, F., Panigrahi, A., & Das, S. (2024). <strong>The Goldilocks Principle: Achieving Just Right Boundary Fidelity for Long-Tailed Classification.</strong> 
        <em>IEEE Transactions on Emerging Topics in Computational Intelligence</em>.         
        <details style="margin-top: 8px;">
            <summary style="cursor: pointer; color: #2980b9;">Abstract</summary>
            <p style="margin-top: 6px;">
        This study addresses the challenges of learning from long-tailed class imbalances in deep neural networks, particularly for image recognition. Long-tailed class imbalances occur when a dataset's class distribution is highly skewed, with a few head classes containing many instances and numerous tail classes having fewer instances. This imbalance becomes problematic when traditional classification methods, especially deep learning models, prioritize accuracy in the more frequent classes, neglecting the less common ones. 
Furthermore, these methods struggle to maintain consistent boundary fidelity—decision boundaries that are sharp enough to distinguish classes yet smooth enough to generalize well. Hard boundaries, often caused by overfitting tail classes, amplify intra-class variations, while overly soft boundaries blur distinctions between classes, reducing classification accuracy.
We propose a dual-branch network with a shared feature extractor to overcome these challenges. This network uses instance and median samplers for head and medium classes and a reverse sampler for tail classes. Additionally, we implement a specialized loss function as a feature regularizer to reduce the model's sensitivity to irrelevant intra-class variations during classification. This loss function dynamically modulates feature representation alignment, promoting cohesive intra-class structures and clear inter-class separations. To achieve this, our framework incorporates two key components: Dual-Branch Sampler-Guided Mixup (DBSGM) and Adaptive Class-Aware Feature Regularizer (ACFR), which work together to balance class representation and refine decision boundaries.
Integrating DBSGM and ACFR during training helps shape decision boundaries that align with class semantics. To ensure class boundaries are appropriately defined, we propose the temperature-adaptive supervised contrastive loss (TASCL) within the ACFR module, achieving the right balance between smoothness and sharpness. Our single-stage, end-to-end framework demonstrates significant performance improvements, offering a promising solution to the challenges of long-tailed class imbalances in deep learning. 
            </p>
          </details> 
      </td>
      <td><a href="https://ieeexplore.ieee.org/" target="_blank"><span><i class="fas fa-scroll"></i>Available Soon</span></a></td>
    </tr>
    <tr>
      <td style="white-space: nowrap; padding: 10px;">2024</td>
      <td><img src="assets/publications/skin_fairness.jpg" alt="Thumbnail" class="pub-image"></td>
      <td>
        Ansari, F., Chakraborti, T., & Das, S. (2024). <strong>Algorithmic Fairness in Lesion Classification by Mitigating Class Imbalance and Skin Tone Bias.</strong> 
        <em>International Conference on Medical Image Computing and Computer-Assisted Intervention</em>, 373–382. Springer Nature Switzerland Cham.
         <details style="margin-top: 8px;">
            <summary style="cursor: pointer; color: #2980b9;">Abstract</summary>
            <p style="margin-top: 6px;">
Deep learning models have shown considerable promise in the classification of skin lesions. However, a notable challenge arises from their inherent bias towards dominant skin tones and the issue of imbalanced class representation. This study introduces a novel data augmentation technique designed to address these limitations. Our approach harnesses contextual information from the prevalent class to synthesize various samples representing minority classes. Using a mixup-based algorithm guided by an adaptive sampler, our method effectively tackles bias and class imbalance issues. The adaptive sampler dynamically adjusts sampling probabilities based on the network’s meta-set performance, enhancing overall accuracy. Our research demonstrates the efficacy of this approach in mitigating skin tone bias and achieving robust lesion classification across a spectrum of diverse skin colors from two distinct benchmark datasets, offering promising implications for improving dermatological diagnostic systems.
        </p>
          </details> 
      </td>
      <td><a href="https://link.springer.com/chapter/10.1007/978-3-031-72378-0_35" target="_blank"><span><i class="fas fa-scroll"></i>Paper</span></a></td>
    </tr>
    <tr>
      <td style="white-space: nowrap; padding: 10px;">2024</td>
      <td><img src="assets/publications/cco_oversampling.jpg" alt="Thumbnail" class="pub-image"></td>
      <td>
        Mondal, P., Ansari, F., & Das, S. (2024). <strong>CCO: A cluster core-based oversampling technique for improved class-imbalanced learning.</strong> 
        <em>IEEE Transactions on Emerging Topics in Computational Intelligence</em>.
                         <details style="margin-top: 8px;">
            <summary style="cursor: pointer; color: #2980b9;">Abstract</summary>
            <p style="margin-top: 6px;">
        Supervised classification problems from the real world typically face a challenge characterized by the scarcity of samples in one or more target classes compared to the rest of the majority classes. In response to such class imbalance, we propose an oversampling technique based on clustering, aiming to populate the minority class with synthetic samples. This approach capitalizes on the notion of “Cluster Cores,” representing locally dense regions within clusters. These Cluster Cores act as central, densely crowded areas that capture intricate topological properties of the corresponding clusters, especially in complex datasets with a non-convex spatial orientation in the feature space. By concentrating on these high-density regions, our clustering-based oversampling technique generates synthetic samples within the convex hull region of minority class instances in the formed clusters. This strategy ensures the creation of points that align with the data space and considers each minority instance within a specific cluster, thereby averting the problems encountered due to the generation of artificial samples by mere linear combination of the minority class data points, as is encountered in SMOTE (Synthetic Minority Oversampling Technique)-based algorithms. To assess the efficacy of our proposal, we conducted experimental comparisons against several cutting-edge algorithms, considering an array of evaluation metrics on well-known datasets used in the literature for both binary and multi-class classification. Additionally, we undertook a detailed ablation study, scrutinized existing algorithms in our context, delineated their strengths and limitations, and contemplated potential research directions in this domain.
           </p>
          </details>
      </td>
      <td><a href="https://ieeexplore.ieee.org/document/10555431" target="_blank"><span><i class="fas fa-scroll"></i>Paper</span></a></td>
    </tr>
    <tr>
      <td style="white-space: nowrap; padding: 10px;">2024</td>
      <td><img src="assets/publications/mo2e_experts.jpg" alt="Thumbnail" class="pub-image"></td>
      <td>
        Ansari, F., Bhattacharya, A., Saha, B., & Das, S. (2024). <strong>Mo2E: Mixture of Two Experts for Class-Imbalanced Learning from Medical Images.</strong> 
        <em>2024 IEEE International Symposium on Biomedical Imaging (ISBI)</em>, 1–5. IEEE.
                         <details style="margin-top: 8px;">
            <summary style="cursor: pointer; color: #2980b9;">Abstract</summary>
            <p style="margin-top: 6px;">
        Class imbalance in the medical image dataset is almost inherent due to the limited availability of clinical data for certain diseases and patient populations. Under-represented classes in the training set affect the classification task because the classifier tends to learn more from the majority classes, which are more common in the dataset and ignore data from the minority classes. To mitigate this issue, we propose a method to learn using two different convolutional neural network-based experts; such experts try to learn boundaries within the head classes, between the head and tail classes, and within the tail classes. During expert training, we integrate the MixUp regularization method to augment imbalanced data, employing distinct data sampling strategies for more effective mixing compared to random selection in traditional MixUp. During the inference phase, we combine the logits of the different experts based on their expertise in the corresponding classes. This way, we can improve the accuracy of the head and tail classes. Experiments using highly imbalanced and long-tailed datasets demonstrate the effectiveness of the suggested framework.
           </p>
          </details>
      </td>
      <td><a href="https://ieeexplore.ieee.org/document/10635212" target="_blank"><span><i class="fas fa-scroll"></i>Paper</span></a></td>
    </tr>
    <tr>
      <td style="white-space: nowrap; padding: 10px;">2023</td>
      <td><img src="assets/publications/minority_statistics.jpg" alt="Thumbnail" class="pub-image"></td>
      <td>
        Ansari, F., Das, S., & Shamsolmoali, P. (2023). <strong>Handling class imbalance by estimating minority class statistics.</strong> 
        <em>2023 International Joint Conference on Neural Networks (IJCNN)</em>, 1–8. IEEE.
         <details style="margin-top: 8px;">
            <summary style="cursor: pointer; color: #2980b9;">Abstract</summary>
            <p style="margin-top: 6px;">
             The problem of class imbalance arises in machine learning due to the unequal class-specific distribution of data, where most samples belong to one class, and only a few represent the others. To tackle this issue, one paradigm is to use oversampling techniques that synthesize artificial samples of the minority class using the convex combination of the minority class samples taken in some specialized way for different methods. Existing methods do not take into account any information regarding the actual distribution of the minority class, which leads to inconsistencies between the generated distribution and the actual distribution that the minority class might have. In this paper, we propose a parametrization-based method that tries to estimate the statistics of the minority class samples using the statistics of the nearby classes. Using the different hyperparameters, we can control the distribution such that it may approximate the original distribution. Experiments using synthetic and real-world benchmark datasets demonstrate the usefulness of our techniques across multiple metrics.
            </p>
          </details>
      </td>
      <td><a href="https://ieeexplore.ieee.org/document/10191975" target="_blank"><span><i class="fas fa-scroll"></i>Paper</span></a></td>
    </tr>
  </tbody>
    </table>
  </div>
</div>

<script>
  document.getElementById('pubSearch').addEventListener('input', function () {
    const filter = this.value.toLowerCase();
    const rows = document.querySelectorAll('#pubTable tbody tr');
    rows.forEach(row => {
      row.style.display = row.innerText.toLowerCase().includes(filter) ? '' : 'none';
    });
  });
</script>


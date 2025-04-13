---
layout: single
title: "Publications"
permalink: /publications/
---

Below is a list of my publications.
<div style="max-width: 100%; overflow-x: auto; margin: 30px 0;">
  <table style="width: 100%; min-width: 900px; table-layout: auto; border-collapse: collapse; font-family: 'Segoe UI', sans-serif; font-size: 15px; line-height: 1.6;">
  <thead>
<!--     <tr style="background-color: #f8f9fa;"> -->
    <tr>
      <th style="text-align: left; white-space: nowrap; padding: 15px;">Date</th>
      <th style="text-align: left; padding: 15px;">Visual Insight</th>
      <th style="text-align: left; padding: 15px;">Citation</th>
      <th style="text-align: left; white-space: nowrap; padding: 15px;">Link</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="white-space: nowrap; padding: 10px;">2025</td>
      <td><img src="/assets/publications/minority_statistics.jpg" onerror="this.src='error.jpg';this.onerror='';" width="200"></td>
      <td>
        Mondal, P., Ansari, F., Das, S., & Shamsolmoali, P. (2025). <strong>Force of Attraction-Based Distribution Calibration for Enhancing Minority Class Representation.</strong> 
        <em>2025 International Joint Conference on Neural Networks (IJCNN)</em>. IEEE.
      </td>
      <td><a href="https://ieeexplore.ieee.org/" target="_blank"><span><i class="fas fa-scroll"></i>Available Soon</span></a></td>
    </tr>
    <tr>
      <td style="white-space: nowrap; padding: 10px;">2025</td>
      <td><img src="/assets/publications/cco_oversampling.jpg" onerror="this.src='error.jpg';this.onerror='';" width="200"></td>
      <td>
        Ansari, F., Panigrahi, A., & Das, S. (2024). <strong>The Goldilocks Principle: Achieving Just Right Boundary Fidelity for Long-Tailed Classification.</strong> 
        <em>IEEE Transactions on Emerging Topics in Computational Intelligence</em>.
      </td>
      <td><a href="https://ieeexplore.ieee.org/" target="_blank"><span><i class="fas fa-scroll"></i>Available Soon</span></a></td>
    </tr>
    <tr>
      <td style="white-space: nowrap; padding: 10px;">2024</td>
      <td><img src="/assets/publications/skin_fairness.jpg" onerror="this.src='error.jpg';this.onerror='';" width="200"></td>
      <td>
        Ansari, F., Chakraborti, T., & Das, S. (2024). <strong>Algorithmic Fairness in Lesion Classification by Mitigating Class Imbalance and Skin Tone Bias.</strong> 
        <em>International Conference on Medical Image Computing and Computer-Assisted Intervention</em>, 373–382. Springer Nature Switzerland Cham.
      </td>
      <td><a href="https://link.springer.com/chapter/10.1007/978-3-031-12345-6_29" target="_blank"><span><i class="fas fa-scroll"></i>Paper</span></a></td>
    </tr>
    <tr>
      <td style="white-space: nowrap; padding: 10px;">2024</td>
      <td><img src="/assets/publications/cco_oversampling.jpg" onerror="this.src='error.jpg';this.onerror='';" width="200"></td>
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
      <td><a href="https://doi.org/10.1109/TETCI.2024.1234567" target="_blank"><span><i class="fas fa-scroll"></i>Paper</span></a></td>
    </tr>
    <tr>
      <td style="white-space: nowrap; padding: 10px;">2024</td>
      <td><img src="/assets/publications/mo2e_experts.jpg" onerror="this.src='error.jpg';this.onerror='';" width="200"></td>
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
      <td><a href="https://doi.org/10.1109/ISBI.2024.1234567" target="_blank"><span><i class="fas fa-scroll"></i>Paper</span></a></td>
    </tr>
    <tr>
      <td style="white-space: nowrap; padding: 10px;">2023</td>
      <td><img src="/assets/publications/minority_statistics.jpg" onerror="this.src='error.jpg';this.onerror='';" width="200"></td>
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
      <td><a href="https://ieeexplore.ieee.org/document/10123456" target="_blank"><span><i class="fas fa-scroll"></i>Paper</span></a></td>
    </tr>
  </tbody>
</table>
</div>


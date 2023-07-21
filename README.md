# Simple-similar-image-search-tutorial

### Similar image retrival

Drawing inspiration from Fréchet inception distance[1], I have implemented an algorithm for retrieving similar images based on feature distance. Leveraging Inception V3[2] as the feature extractor, I utilized the Euclidean distance to gauge the dissimilarity between features.

Following [1], feature extraction occurred at the final average pooling layer, while extracting features from other layers is possible. 

--- 

### Dataset

For the experiments, I randomly selected 500 samples from the wild category images in Animal Faces-HQ (AFHQ)[3]. These images showcase diverse wildlife, including lions, tigers, and wolves.

--- 

### Results
**A query image**

<img src="https://github.com/DonghweeYoon/Simple-similar-image-search-tutorial/assets/28053711/90736961-2cac-4d0a-8a92-207f6f4a58a7" alt="query" width="200"/>

<br/>
<br/>

**N nearest neighbors sorted by the feature distance (Ascending order)**

![image](https://github.com/DonghweeYoon/Simple-similar-image-search-tutorial/assets/28053711/d57a85cb-1470-4e46-9780-76ac3c8454a0)

<br/>

**N Random samples**

![image](https://github.com/DonghweeYoon/Simple-similar-image-search-tutorial/assets/28053711/0ff35c9b-baee-4995-91d2-cde65973255f)

<br/>

**N farthest samples (Descending order)**

![image](https://github.com/DonghweeYoon/Simple-similar-image-search-tutorial/assets/28053711/5fa8397b-5f79-45d8-89e4-c0de04024c74)

<br/>

--- 

**References**

[1] Heusel, M., Ramsauer, H., Unterthiner, T., Nessler, B., & Hochreiter, S. (2017). Gans trained by a two time-scale update rule converge to a local nash equilibrium. Advances in neural information processing systems, 30.

[2] Szegedy, C., Vanhoucke, V., Ioffe, S., Shlens, J., & Wojna, Z. (2016). Rethinking the inception architecture for computer vision. In Proceedings of the IEEE conference on computer vision and pattern recognition (pp. 2818-2826).

[3] Choi, Y., Uh, Y., Yoo, J., & Ha, J. W. (2020). Stargan v2: Diverse image synthesis for multiple domains. In Proceedings of the IEEE/CVF conference on computer vision and pattern recognition (pp. 8188-8197).

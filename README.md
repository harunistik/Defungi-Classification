# Microscobic Fungal Classification

In this project, we used the Defungi dataset, which contains 5 classes and 9,114 images. Due to class imbalance, we applied data augmentation (random flips/rotations, zoom, color jitter) with higher probability/intensity for minority classes to improve generalization.
Below are sample images from the dataset.

### Samples From Dataset
<table>
  <tr>
    <td><img src="data/train/TSH/H1_100a_1.jpg" width="180" alt="TSH"><br/><em>TSH</em></td>
    <td><img src="data/train/SHC/H5_101a_1.jpg" width="180" alt="SHC"><br/><em>SHC</em></td>
    <td><img src="data/train/GMA/H3_10a_10.jpg" width="180" alt="GMA"><br/><em>GMA</em></td>
  </tr>
  <tr>
    <td><img src="data/train/BBH/H6_10a_1.jpg" width="180" alt="BBH"><br/><em>BBH</em></td>
    <td><img src="data/train/BASH/H2_104b_1.jpg" width="180" alt="BASH"><br/><em>BASH</em></td>
  </tr>
</table>

## Models Used
- ResNet50 — residual network baseline
- Inception v3 — multi-branch convolutional model
- VGG16 — classic CNN baseline

We evaluate using accuracy and macro-averaged F1, along with per-class precision and recall. We also include a normalized confusion matrix to visualize class-wise errors and the impact of class imbalance.


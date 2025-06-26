# 🧮 **Multi-Object-Counting with Density Map**

This repository provides a **PyTorch-based implementation** for single and multi-class object counting and size estimation using deep learning. The project includes model architectures, dataset generation scripts, and evaluation tools for benchmarking object counting and size estimation tasks.

---

## 🗂️ **Dataset: MOCSE13**

- **MOCSE13** is a synthetic dataset generated using Unity, containing images of 13 different objects (fruits and vegetables).
- The dataset includes **ground truth annotations** for object counts and sizes.
- 📥 **Download**: [Dropbox Link](https://www.dropbox.com/sh/8nqyj6ycgr7jltl/AACfmgH7eU-OT4FDrrC9luyma?dl=0)
- 🛠️ **Custom datasets** (new object types) can be generated upon request.

### 📁 **Dataset Structure**

- `dataset/ground_truth/`: **Ground truth density maps and annotations**
- `dataset/train_data/`, `dataset/test_data/`: **Training and testing images**
- `dataset/annotations.xml`: **XML file with detailed annotations**

---

## 🧠 **Model Architectures**

The repository supports various deep learning backbones for object counting and size estimation, including:

- 🏗️ **VGG** (with/without batch normalization)
- 🏢 **ResNet**
- 🌀 **Inception**
- 🔀 **ShuffleNet**
- 🧩 **MCNN, SANet, CFFNet, CSRNet, TEDNet, and more**

Model definitions are located in `backbones_NN/`.

---

## 🛠️ **Main Scripts**

- `multi_channels_counting.py`: **Multi-class object counting**
- `multi_channels_size_estination.py`: **Multi-class size estimation**
- `single_channel_counting.py`: **Single-class object counting**
- `single_channel_size_estimation.py`: **Single-class size estimation**
- `generate_density_map.py`: **Generate density maps from annotations**
- `Individual object size retrieval.py`: **Retrieve individual object sizes**

---

## 🚀 **How to Use**

1. 📝 **Modify data paths and parameters** in the scripts as needed.
2. ▶️ **Train or test a model** using:
   ```bash
   python3 single_channel_counting.py
   # or
   python3 multi_channels_counting.py
   ```
   Replace with the appropriate script for your task.

3. 🔍 **Inference**: Use `inference.ipynb` for running inference and visualizing results.

---


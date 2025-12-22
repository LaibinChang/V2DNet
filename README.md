# From Visibility to Detection: Saliency-Guided Underwater Image Restoration with Hierarchical Dual-Branch Refinement

## 📌 Introduction
Underwater salient object detection (USOD) plays a vital role in many marine vision tasks, yet remains challenging due to severe visual degradation and complex scene variability. The quality degradation of raw underwater images (caused by selective absorption and medium scattering) makes it challenging to perform object detection directly. One conceivable approach involves first removing visual disturbances through underwater image enhancement, followed by salient object detection. However, such a sequential design separates low-level restoration from high-level perception, leading to semantic inconsistency that makes the restoration results unfavorable for detection and may even introduce additional noise. To address this, we propose V2DNet, a unified network that jointly optimizes visual restoration and salient object detection. Unlike physics-guided approaches that rely on handcrafted priors and iterative optimization, V2DNet adopts a semantic-driven learning paradigm, wherein high-level saliency semantics guide image restoration while restored visual cues reciprocally enhance saliency perception. Specifically, V2DNet first employs a hierarchical dual-branch initialization, in which a self-calibrated decoder predicts the saliency mask and a mask-aware restoration module reconstructs the image content. After that, a saliency-guided refinement module with cross-level modulation is used to improve the structural fidelity and semantic consistency. Extensive experiments show that V2DNet outperforms existing state-of-the-art methods in both quantitative and qualitative evaluations across multiple benchmarks.

<img width="1619" height="542" alt="image" src="https://github.com/user-attachments/assets/0ea26c0b-36d3-4708-a292-4233a57b7f61" />

## 🌊 Requirement
* Python 3.9
* CUDA 11.8
* matplotlib==2.2.2
albumentations==0.4.5
scipy==1.4.1
scikit_image==0.17.2
torch==1.6.0
tqdm==4.46.1
progress==1.5
numpy==1.18.1
torchvision==0.6.0
opencv_python_headless==4.2.0.34
Pillow==8.3.2
scikit_learn==1.0
skimage==0.0
tensorboardX==2.4

## 🚀 Training
```bash
bash scripts/train.sh
```

## 🧪 Testing
```bash
bash scripts/test.sh
```

## 📖 Paper Info & Status
> **Title**: From Visibility to Detection: Saliency-Guided Underwater Image Restoration with Hierarchical Dual-Branch Refinement  
> **Authors**: Laibin Chang, Yuxin Wang, Kui Jiang, Shaodong Wang, Bo Du  
> **Status**: Under Review  
> **Code**: The code will be released after the paper is accepted.

---
## 📝 Notes
* ❓ If you have any questions, please feel free to contact us at **[changlb666@whu.edu.cn](mailto:changlb666@whu.edu.cn)**.
* 🌐 I am open to collaboration and welcome inquiries from anyone interested in my research. Please find us at **[https://laibinchang.github.io/](https://laibinchang.github.io/)**.

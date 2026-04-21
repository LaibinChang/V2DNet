# UniV2D: Bridging Visual Restoration and Semantic Perception for Underwater Salient Object Detection

## 📌 Introduction
Underwater salient object detection (USOD) plays a vital role in marine vision tasks but remains fundamentally challenging due to severe visual degradation, such as selective absorption and medium scattering. Conventional pipelines typically adopt a sequential "enhance-then-detect" paradigm. However, isolating low-level visual restoration from high-level semantic perception often leads to semantic inconsistency, where the restored images may not be optimal for detection and can even introduce task-irrelevant noise. To break this sequential bottleneck, we propose UniV2D, a Unified Vision-to-Detection Network that jointly optimizes visual restoration and salient object detection within a mutually beneficial framework. Unlike traditional methods that rely on disjointed pipelines or rigid physical priors, UniV2D introduces a semantic-driven learning paradigm: high-level saliency semantics actively guide the restoration process, while the restored visual cues reciprocally enhance saliency perception. Specifically, UniV2D features a hierarchical dual-branch architecture. It first employs a self-calibrated decoder to predict initial saliency masks alongside a mask-aware restoration module to reconstruct image content. Subsequently, a saliency-guided refinement module equipped with cross-level modulation is utilized to align structural fidelity with semantic consistency. Extensive experiments across multiple benchmarks demonstrate that UniV2D significantly outperforms state-of-the-art methods in both quantitative and qualitative evaluations, establishing a new standard for joint underwater perception.

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
> **Title**: UniV2D: Bridging Visual Restoration and Semantic Perception for Underwater Salient Object Detection
> **Authors**: Laibin Chang, Yunke Wang, Xu Zhang, Kui Jiang, Chang Xu, and Bo Du
> **Status**: Under Review
> **Code**: The code will be released after the paper is accepted.

---
## 📝 Notes
* ❓ If you have any questions, please feel free to contact us at **[changlb666@whu.edu.cn](mailto:changlb666@whu.edu.cn)**.
* 🌐 I am open to collaboration and welcome inquiries from anyone interested in my research. Please visit **[https://laibinchang.github.io/](https://laibinchang.github.io/)** for our latest updates.

# 🔥 PyTorch Marathon

A structured, hands-on run through PyTorch, from tensors to deployed models. I'm using it to refresh my PyTorch skills and to strengthen my deep learning fundamentals.

> **Course:** [PyTorch for Deep Learning (Zero To Mastery) by Daniel Bourke](https://www.udemy.com/course/pytorch-for-deep-learning/)
> **Approach:** Code along, then re-implement from scratch, then write down what I learned.

---

## 🎯 Objectives

- **Refresh PyTorch.** Get fluent again with tensors, autograd, `nn.Module`, `Dataset`/`DataLoader` and the training loop.
- **Strengthen DL fundamentals.** Understand *why* things work: loss functions, optimizers, activations, overfitting and regularization, CNNs, transfer learning and Vision Transformers.
- **Write production-minded code.** Move from notebooks to modular, reusable Python scripts.
- **Build a reference repo.** Keep clean notebooks, notes and mini-projects I can come back to later.

---

## 🗺️ Roadmap

| #  | Module                          | Key Topics                                                           | Status |
|----|---------------------------------|----------------------------------------------------------------------|:------:|
| 00 | PyTorch Fundamentals            | Tensors, shapes, dtypes, devices, indexing, matrix ops               | ⬜ |
| 01 | PyTorch Workflow                | Data → model → loss/optimizer → training loop → evaluate → save/load | ⬜ |
| 02 | Neural Network Classification   | Binary & multi-class classification, non-linearity, metrics          | ⬜ |
| 03 | Computer Vision                 | `torchvision`, FashionMNIST, CNNs (TinyVGG), confusion matrix        | ⬜ |
| 04 | Custom Datasets                 | `ImageFolder`, custom `Dataset` classes, data augmentation           | ⬜ |
| 05 | Going Modular                   | Turning notebooks into scripts: `data_setup`, `engine`, `train.py`   | ⬜ |
| 06 | Transfer Learning               | Pretrained models (EfficientNet), feature extraction, fine-tuning    | ⬜ |
| 07 | Experiment Tracking             | TensorBoard, comparing models, data and epochs                       | ⬜ |
| 08 | Paper Replicating               | Replicating the Vision Transformer (ViT) paper from scratch          | ⬜ |
| 09 | Model Deployment                | Gradio demo, Hugging Face Spaces, speed vs. performance trade-offs   | ⬜ |

**Legend:** ⬜ Not started · 🟨 In progress · ✅ Done

---

## 📁 Repository Structure

```
pytorch-marathon/
├── notebooks/            # Code-along + from-scratch notebooks, one per module
│   ├── 00_pytorch_fundamentals.ipynb
│   ├── 01_pytorch_workflow.ipynb
│   └── ...
├── going_modular/        # Reusable scripts built in module 05 onwards
│   ├── data_setup.py
│   ├── engine.py
│   ├── model_builder.py
│   ├── train.py
│   └── utils.py
├── exercises/            # Course exercises + extra-curricular solutions
├── notes/                # Concept notes and "explain it simply" write-ups
├── projects/             # Milestone projects (e.g. FoodVision Mini/Big)
├── models/               # Saved model weights (git-ignored if large)
├── data/                 # Datasets (git-ignored)
├── requirements.txt
└── README.md
```

---

## ⚙️ Setup

```bash
# Clone the repo
git clone https://github.com/Krishna-yadu-048/pytorch-marathon.git
cd pytorch-marathon

# Create and activate a virtual environment
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

**Core dependencies:** `torch`, `torchvision`, `torchinfo`, `numpy`, `pandas`, `matplotlib`, `scikit-learn`, `torchmetrics`, `tensorboard`, `gradio`, `tqdm`

> 💡 For GPU support, install the PyTorch build that matches your CUDA version from [pytorch.org](https://pytorch.org/get-started/locally/).

Check that everything works:

```python
import torch
print(torch.__version__)
print("CUDA available:", torch.cuda.is_available())
```

---

## 🧠 How I'm Running This Marathon

1. **Watch, then code along.** Follow each lesson in a notebook.
2. **Rebuild from memory.** Re-implement the key pieces without looking (training loop, model class, dataset class).
3. **Do the exercises.** Complete each module's exercises and extra-curriculars.
4. **Write it down.** Add a short note to `notes/` that explains the concept in my own words.
5. **Commit daily.** Small, consistent commits to track progress.

---

## 📝 Key Learnings Log

A running list of insights, gotchas and "aha" moments.

| Date | Module | Learning |
|------|--------|----------|
| — | — | — |

---

## 🚀 Milestone Projects

- [ ] **FashionMNIST classifier**: CNN trained from scratch (Module 03)
- [ ] **FoodVision Mini**: pizza / steak / sushi classifier on custom data (Modules 04–07)
- [ ] **ViT from scratch**: Vision Transformer paper replication (Module 08)
- [ ] **FoodVision Big**: deployed Gradio app on Hugging Face Spaces (Module 09)

---

## 📚 Resources

- 🎓 [Course on Udemy](https://www.udemy.com/course/pytorch-for-deep-learning/)
- 📖 [Learn PyTorch for Deep Learning (online book)](https://www.learnpytorch.io/)
- 💻 [Course GitHub repo](https://github.com/mrdbourke/pytorch-deep-learning)
- 📘 [Official PyTorch Docs](https://pytorch.org/docs/stable/index.html)
- 🧪 [PyTorch Tutorials](https://pytorch.org/tutorials/)

---

## 🙏 Acknowledgements

Course content and materials by [Daniel Bourke](https://github.com/mrdbourke) / [Zero To Mastery](https://zerotomastery.io/). This repo holds my personal learning notes and implementations.

---

<p align="center"><i>One tensor at a time. 🏃‍♂️🔥</i></p>
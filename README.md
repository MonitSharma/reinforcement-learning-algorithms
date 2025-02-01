# Deep Learning Learning Journey 🚀

This repo is dedicated to my journey through deep learning, primarily following the excellent resource [Understanding Deep Learning](https://udlbook.github.io/udlbook/) by Simon J.D. Prince. Along the way, I'll also experiment with accelerating certain computations using Apple's GPU capabilities. 

## 📌 Overview

This repository serves as:
- A structured collection of notes, exercises, and implementations based on **Understanding Deep Learning**.
- A playground for experimenting with different deep learning concepts and architectures.
- An exploration of Apple's **Metal Performance Shaders (MPS)** for GPU acceleration in deep learning.

## 🏗️ Structure

The repo is structured as follows:

```
📂 deep-learning-journey
│── 📜 README.md          # This file
│── 📂 notebooks          # Jupyter notebooks covering concepts from the book
│── 📂 experiments        # Custom implementations and explorations
│── 📂 apple-gpu-tests    # Code snippets using Apple's GPU for acceleration
│── 📂 datasets           # Sample datasets used in the experiments
│── 📂 models             # Saved model checkpoints
```

## 🚀 Topics Covered

✔️ Fundamentals of deep learning
✔️ Training and optimization techniques
✔️ Regularization and generalization
✔️ Deep architectures and representation learning
✔️ Probabilistic models and uncertainty in deep learning
✔️ Exploring GPU acceleration using Apple MPS

## 🖥️ Running the Code

1. **Clone the repo:**
   ```bash
   git clone https://github.com/monitsharma/deep-learning.git
   cd deep-learning-journey
   ```
2. **Create a virtual environment:**
   ```bash
   python3 -m venv env
   source env/bin/activate  # On Windows, use `env\Scripts\activate`
   ```
3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
4. **Run Jupyter Notebooks:**
   ```bash
   jupyter notebook
   ```

## 🚀 Using Apple GPU for Acceleration

For Mac users with Apple Silicon (M1/M2/M3+), deep learning models can leverage Metal Performance Shaders (MPS) for acceleration:

```python
import torch
import torch.backends.mps as mps

device = torch.device("mps" if torch.backends.mps.is_available() else "cpu")
print(f"Using device: {device}")
```

If MPS is not available, the code will fall back to CPU.

## 📌 Resources

- [Understanding Deep Learning](https://udlbook.github.io/udlbook/)
- [PyTorch MPS Backend](https://pytorch.org/docs/stable/notes/mps.html)
- [Metal Performance Shaders](https://developer.apple.com/documentation/metalperformanceshaders)

## 📌 Future Plans

🔹 Complete all exercises and implementations from **Understanding Deep Learning**  
🔹 Optimize select parts of the code using **Apple Metal GPU Acceleration**  
🔹 Explore alternative deep learning frameworks for performance comparison  
🔹 Share insights through blog posts and discussions  

Please cite this work :

```bash
   @book{prince2023understanding,
        author = "Simon J.D. Prince",
        title = "Understanding Deep Learning",
        publisher = "The MIT Press",
        year = 2023,
        url = "http://udlbook.com"
    }
```


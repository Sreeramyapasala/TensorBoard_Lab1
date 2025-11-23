# TensorBoard Lab 1 – Custom Version

## Overview
This repository contains my customized version of the TensorBoard Lab from the MLOps course.  
I completed **one lab** as required in the assignment and made several modifications so it is **not identical** to the original notebook.

---

## Modifications I Made

- **Changed the synthetic dataset**
  - Original: linear function `y = 0.5 * x + 2 + noise`
  - Modified: non-linear quadratic function  
    `y = 0.8 * (x ** 2) + 0.3 * x + 1.5 + noise`

- **Modified the model architecture**
  - Added an explicit input layer  
    `keras.layers.Input(shape=(1,))`
  - Changed hidden layers to:
    - Dense(32, activation='relu')
    - Dense(16, activation='relu')
    - Dense(1)

- **Changed optimizer**
  - Original: SGD  
  - Modified: Adam with learning_rate=0.05

- **Added a Matplotlib visualization**
  - Plotted training loss and validation loss curves

- **Added explanations + markdown cells**
  - Explained the dataset
  - Explained model design
  - Explained TensorBoard tabs (Scalars, Graphs)
  - Added training observations

---

## TensorBoard Components Used

- **Scalars:** Tracked training and validation loss  
- **Graphs:** Viewed model structure  
- **Histograms:** Observed weight distribution  
- **Debugger (basic):** Viewed alerts summary




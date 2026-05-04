# Action Recognition using CNN + LSTM

## Project Overview
A deep learning model that recognizes 30 human actions from video clips
using MobileNetV2 as CNN backbone and stacked LSTM for temporal modeling.

## Dataset
UCF50 — 30 selected action classes

## Model Architecture
- CNN Backbone : MobileNetV2 (pretrained on ImageNet)
- Temporal      : Stacked LSTM (128 → 64 units)
- Input         : 20 frames at 64x64 per video
- Output        : 30 action classes (softmax)

## Results
| Metric         | Value  |
|----------------|--------|
| Test Accuracy  | 77.92%  |
| Val Loss       | 1.1375  |
| Epochs ran     | 100     |

## How to Run
1. Open the notebook on Kaggle
2. Enable GPU T4 in Settings
3. Run all cells in order

## Libraries Used
TensorFlow, Keras, OpenCV, NumPy, Matplotlib, Seaborn, Scikit-learn

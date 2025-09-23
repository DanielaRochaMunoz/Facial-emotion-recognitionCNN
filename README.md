# Facial Emotion Recognition Model

Convolutional Neural Network (CNN) trained with **30,000 images** to detect facial expressions and classify emotions in real time.

---

## Main Features
- Trained with a diverse dataset of emotions (**happiness, sadness, anger, surprise, etc.**).
- Implemented in **Keras + TensorFlow**, optimized with augmentation techniques.
- Achieved **75% validation accuracy**.
- Integrated with **OpenAI API** for contextual responses.

---

## Installation & Training

### 1. Clone repository
```bash
git clone <repo-cnn>
cd repo-cnn
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Train model
```bash
python train.py
```

### 4. Test model
```bash
python predict.py --image test.jpg
```

---

## Model Architecture
- **Convolutions** → feature extraction.
- **Pooling** → dimensionality reduction.
- **Fully Connected Layers** → classification.
- **Softmax** → multiclass output.

---

## Integration
This model is connected to **EmoCare’s backend (NestJS)**, which:
- Processes the detected emotion.  
- Calls the **OpenAI API** to generate empathetic responses.  
- Returns the personalized response to the **React Native frontend**.  

---

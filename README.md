# Text Generation using Recurrent Long Short-Term Memory (LSTM) Network

A deep learning project that generates human-like text using a Recurrent Neural Network (RNN) with Long Short-Term Memory (LSTM). The model is trained on a large text dataset at the character level and learns sequential patterns to generate new text based on a user-provided seed.

---

## 📌 Project Overview

Text generation is a Natural Language Processing (NLP) task where a model predicts the next character in a sequence based on previously seen characters. In this project, an LSTM network is trained on a large corpus of text to learn language patterns and generate realistic text one character at a time.

The model uses TensorFlow and Keras for training and inference. After training, users can provide a starting phrase (seed text), and the model generates new text by predicting one character at a time.

---

## 🚀 Features

- Character-level text generation using LSTM
- Automatic vocabulary creation from dataset
- Character-to-index and index-to-character encoding
- Sequence generation using TensorFlow Dataset API
- Embedding layer for dense character representation
- LSTM-based sequence modeling
- Configurable text generation temperature
- User-defined seed text
- Random text generation after training

---

## 🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas

---

## 📂 Dataset

The project uses a CSV file containing textual data.

Dataset format:

| Column |
|---------|
| text |

All text samples are merged into a single corpus after:

- Removing missing values
- Converting text to lowercase

---

## ⚙️ Project Workflow

### 1. Load Dataset

- Read CSV dataset
- Remove null values
- Merge all text into one corpus
- Convert text to lowercase

---

### 2. Text Preprocessing

- Create vocabulary of unique characters
- Character encoding
- Integer encoding of text
- Generate input-target sequences
- Shuffle dataset
- Batch dataset for training

---

### 3. Model Architecture

The model consists of:

- Embedding Layer
- LSTM Layer
- Dense Output Layer

Architecture:

```
Input Characters
       │
       ▼
Embedding Layer
       │
       ▼
LSTM Layer (128 Units)
       │
       ▼
Dense Layer
       │
       ▼
Predicted Next Character
```

---

## 📊 Model Configuration

| Parameter | Value |
|------------|--------|
| Sequence Length | 100 |
| Embedding Dimension | 64 |
| LSTM Units | 128 |
| Batch Size | 64 |
| Optimizer | Adam |
| Loss Function | Sparse Categorical Crossentropy |
| Epochs | 20 |

---

## 🧠 Training

The model is trained using character sequences where:

- Input = First 100 characters
- Target = Next 100 characters shifted by one position

The network learns to predict the next character in the sequence.

---

## ✨ Text Generation

After training, the model generates text using:

- Seed text provided by the user
- Temperature sampling for controlling randomness
- Character-by-character prediction

Temperature values:

| Temperature | Output |
|--------------|--------|
| 0.2 | Very predictable |
| 0.5 | Less random |
| 0.8 | Balanced |
| 1.0 | Creative |
| >1.0 | Highly random |

---

## 📁 Project Structure

```
Text-Generation-LSTM/
│
├── train.csv
├── text_generation_lstm.ipynb
├── README.md
└── requirements.txt
```

---

## ▶️ How to Run

### Clone Repository

```bash
git clone https://github.com/your-username/Text-Generation-LSTM.git
```

### Install Dependencies

```bash
pip install tensorflow pandas numpy
```

### Run

Open the notebook:

```
text_generation_lstm.ipynb
```

Run all cells sequentially.

---

## 📈 Sample Output

Input Seed:

```
The
```

Generated Text:

```
The uster mp fo haveun fre anth to wasicore s mprmalitrsall win a f r pens. tmilerin inthentin s vistha as. in fout wr pres bla an ivo “ithe bed o, ase tay s fed ste “trinsppove a atond d s.
```

The generated text becomes more coherent with larger datasets, longer training, and hyperparameter tuning.

---

## 🔮 Future Improvements

- Word-level text generation
- Multi-layer LSTM architecture
- Bidirectional LSTM
- GRU-based text generation
- Transformer-based language models
- Model checkpointing
- Beam search decoding
- Web interface using Flask or Streamlit
- Fine-tuning on domain-specific datasets

---

## 📚 Learning Outcomes

Through this project, the following concepts were explored:

- Natural Language Processing (NLP)
- Character-level language modeling
- Recurrent Neural Networks (RNN)
- Long Short-Term Memory (LSTM)
- Text preprocessing
- Sequence generation
- Embedding layers
- TensorFlow Dataset API
- Deep learning model training
- Probabilistic text generation

---

## 👩‍💻 Author

**Pallavi Buddhana**

B.Tech Electronics and Communication Engineering

Interested in Artificial Intelligence, Machine Learning, and Software Development.

---
```

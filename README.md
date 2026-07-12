# Text Generation using Recurrent LSTM

A deep learning project that generates human-like text using a Recurrent Long Short-Term Memory (LSTM) network. The model is trained on a large text corpus at the character level and learns sequential patterns to predict the next character, enabling it to generate new text from a given seed.

---

## 📌 Project Overview

This project demonstrates character-level text generation using a Recurrent Neural Network (RNN) with Long Short-Term Memory (LSTM). The model is trained on textual data to learn language patterns and generate coherent text one character at a time.

The project is implemented using TensorFlow and Keras, with preprocessing techniques such as character encoding and sequence generation.

---

## 🚀 Features

- Character-level text generation
- Text preprocessing and encoding
- Character-to-index and index-to-character mapping
- Sequence creation using TensorFlow Dataset API
- Embedding layer for character representation
- LSTM-based sequence modeling
- Adjustable temperature for controlling randomness
- User-defined seed text generation
- Trained model saved for future inference

---

## 🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas

---

## 📂 Dataset

The model is trained on a CSV dataset containing textual data.

Preprocessing steps include:

- Removing missing values
- Converting text to lowercase
- Creating character vocabulary
- Encoding characters into integer indices
- Generating fixed-length sequences

---

## ⚙️ Workflow

### 1. Load Dataset

- Read CSV file
- Merge all text into a single corpus
- Convert text to lowercase

### 2. Text Preprocessing

- Create vocabulary
- Character encoding
- Generate input-target sequences
- Shuffle and batch the dataset

### 3. Build LSTM Model

The architecture consists of:

- Embedding Layer
- LSTM Layer
- Dense Output Layer

```
Input Text
     │
     ▼
Embedding Layer
     │
     ▼
LSTM Layer
     │
     ▼
Dense Layer
     │
     ▼
Next Character Prediction
```

### 4. Train Model

The model learns to predict the next character in a sequence using Sparse Categorical Crossentropy loss and the Adam optimizer.

### 5. Generate Text

After training, users can provide a starting string (seed text), and the model generates new text character by character.

---

## 📊 Model Configuration

| Parameter | Value |
|-----------|-------|
| Sequence Length | 100 |
| Embedding Dimension | 64 |
| LSTM Units | 128 |
| Batch Size | 64 |
| Optimizer | Adam |
| Loss Function | Sparse Categorical Crossentropy |
| Epochs | 20 |

---

## 📁 Project Structure

```
text-generation-using-recurrent-LSTM/
│
├── README.md
├── char_maps.pkl
├── text_generation_using_recurrent_LSTM (3).ipynb
└── text_lstm_model.keras
```

---

## ▶️ How to Run

### Clone Repository

```bash
git clone https://github.com/pallavi0120/text-generation-using-recurrent-LSTM.git
```

### Install Dependencies

```bash
pip install tensorflow numpy pandas
```

### Run the Notebook

Open:

```
text_generation_using_recurrent_LSTM (3).ipynb
```

Run all cells sequentially to:

- Load the dataset
- Train the LSTM model
- Generate new text

---

## 📈 Sample Output

**Input Seed**

```
The
```

**Generated Text**

```
The uster mp fo haveun fre anth to wasicore s mprmalitrsall win a f r pens. tmilerin inthentin s vistha as. in fout wr pres bla an ivo "ithe bed o, ase tay s fed ste trinsppove a atond d s.
```

---

## 🔮 Future Improvements

- Word-level text generation
- Multi-layer LSTM architecture
- Bidirectional LSTM
- GRU implementation
- Transformer-based language models
- Model checkpointing
- Streamlit or Flask web application
- Fine-tuning on custom datasets

---

## 📚 Learning Outcomes

This project helped in understanding:

- Natural Language Processing (NLP)
- Character-level language modeling
- Recurrent Neural Networks (RNN)
- Long Short-Term Memory (LSTM)
- Text preprocessing
- Sequence generation
- TensorFlow Dataset API
- Deep learning model training
- Probabilistic text generation

---

## 👩‍💻 Author

**Pallavi Buddhana**

B.Tech Electronics and Communication Engineering

Interested in Artificial Intelligence, Machine Learning, and Software Development.

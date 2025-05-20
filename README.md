
# 🧠 English to Hindi Neural Machine Translation using Seq2Seq (LSTM)

This repository contains a sequence-to-sequence (seq2seq) neural machine translation (NMT) model using TensorFlow/Keras. The model is trained to translate English sentences into Hindi using parallel sentence data.

## 📁 Dataset

- CSV file with two columns:
  - `English` (source sentences)
  - `Hindi` (target translations)

## 📚 Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Scikit-learn (for train/test split)
- Google Colab

## 🛠️ How It Works

1. **Data Loading**  
   Load the English–Hindi sentence pairs from a CSV file.

2. **Preprocessing**  
   - Tokenize and index each word in English and Hindi.
   - Filter out long sentences (> 20 words).
   - Create vocabulary mappings.

3. **Sequence Preparation**  
   Use custom generators to prepare:
   - Encoder input
   - Decoder input
   - Decoder target (one-hot)

4. **Model Architecture**  
   - **Encoder**: Embedding + LSTM layers
   - **Decoder**: Embedding + LSTM + Dense (softmax)
   - Uses `categorical_crossentropy` loss and `adam` optimizer.

5. **Training**  
   Trained for 50 epochs with a batch size of 256.

## 🧪 Output

After training, the model can be used to translate new English sentences into Hindi. A decoding function can be added to generate predictions from test data.

## 🚀 Usage

- Mount Google Drive in Google Colab.
- Upload the dataset to Colab or Google Drive.
- Run the training cell to build and train the model.

## 🔮 Future Improvements

- Add attention mechanism
- Subword tokenization using SentencePiece or Byte Pair Encoding
- Use pre-trained embeddings

## ✍️ Author

- Aleena Roy


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
  <h1>Fine-Tuning mBART-50 for English to Urdu Translation</h1>
  <p>This repository contains code for fine-tuning the mBART-50 model for English to Urdu translation using personalized data. The process involves data preparation, model training, and evaluation.</p>

  <h2>Introduction</h2>
  <p>In this project, we fine-tune the mBART-50 model to translate English text into Urdu. We utilize personalized data and guide users through each step of the process, from data preparation to model input. The fine-tuning process is conducted using 2 T4 GPUs for efficient training.</p>

  <h2>Getting Started</h2>
  <ol>
    <li>Install the required libraries:
      <pre><code>pip install datasets</code></pre>
      <pre><code>pip install transformers[torch]</code></pre>
      <pre><code>pip install accelerate -U</code></pre>
    </li>
    <li>Clone this repository:
      <pre><code>git clone &lt;https://github.com/umairaziz999/BERT-Style-LLM-Assignment.git&gt;</code></pre>
    </li>
    <li>Run the notebook <code>LLM_Assignment.ipynb</code> in a Jupyter environment or any compatible environment.</li>
  </ol>

  <h2>Data Preparation</h2>
  <p>We utilize the "opus100" dataset from Hugging Face, containing English and Urdu text samples. The dataset is preprocessed and divided into training and validation sets. The data is then formatted into CSV files for ease of handling.</p>

  <h2>Model Training</h2>
  <p>The model used for fine-tuning is the mBART-50 model, which is loaded and trained on the personalized data. The training process is managed using the <code>Seq2SeqTrainer</code> from the Hugging Face <code>transformers</code> library.</p>

  <h2>Evaluation</h2>
  <p>The trained model is evaluated using validation data to assess its translation performance. Training and validation loss curves are plotted to visualize the training progress and model performance.</p>

  <h2>Testing</h2>
  <p>Users can test the trained model on custom prompts to translate English text into Urdu. The model's responses are generated using the <code>text2text-generation</code> pipeline from the <code>transformers</code> library.</p>

  <h2>Results</h2>
  <p>The fine-tuned mBART-50 model demonstrates promising performance in translating English to Urdu text. The evaluation metrics and sample translations are provided in the notebook.</p>

  <h2>License</h2>
  <p>This project is licensed under the <a href="LICENSE">MIT License</a>.</p>
</body>
</html>

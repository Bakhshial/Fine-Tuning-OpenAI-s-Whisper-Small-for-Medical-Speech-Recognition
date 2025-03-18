# Fine-Tuning-OpenAI-s-Whisper-Small-for-Medical-Speech-Recognition

This repository contains the code and resources for fine-tuning OpenAI’s Whisper-small model for medical speech recognition. The goal of this project is to improve transcription accuracy for medical-related audio data, such as doctor-patient conversations, medical reports, and dictations. The fine-tuned model is designed to handle domain-specific terminology and improve the overall performance of automatic speech recognition (ASR) in the healthcare domain.

### 𝐊𝐞𝐲 𝐅𝐞𝐚𝐭𝐮𝐫𝐞𝐬

    𝐅𝐢𝐧𝐞-𝐓𝐮𝐧𝐢𝐧𝐠: Adapting OpenAI’s Whisper-small model to the medical domain using a specialized dataset.
    
    𝐃𝐚𝐭𝐚 𝐏𝐫𝐞𝐩𝐫𝐨𝐜𝐞𝐬𝐬𝐢𝐧𝐠: Preparing medical audio datasets, including resampling audio files and tokenizing transcriptions.
    
    𝐌𝐨𝐝𝐞𝐥 𝐓𝐫𝐚𝐢𝐧𝐢𝐧𝐠: Fine-tuning the model with a custom training loop and evaluating performance using Word Error Rate (WER).
    
   𝐃𝐞𝐩𝐥𝐨𝐲𝐦𝐞𝐧𝐭: Creating a user-friendly interface using Gradio to test the fine-tuned model.
    
    𝐇𝐮𝐠𝐠𝐢𝐧𝐠 𝐅𝐚𝐜𝐞 𝐈𝐧𝐭𝐞𝐠𝐫𝐚𝐭𝐢𝐨𝐧: Saving and sharing the fine-tuned model on Hugging Face Hub for easy access.


### Installation

    pip install datasets[audio] transformers accelerate evaluate jiwer tensorboard gradio

### Usage
𝟏. 𝐅𝐢𝐧𝐞-𝐓𝐮𝐧𝐢𝐧𝐠 𝐭𝐡𝐞 𝐌𝐨𝐝𝐞𝐥

The fine-tuning process is documented in the provided Colab notebook (Fine_Tuning_Whisper.ipynb). The notebook includes:

    GPU setup and environment configuration.
    
    Loading and preprocessing the medical ASR dataset.
    
    Feature extraction and tokenization.
    
    Model training and evaluation.

𝟐. 𝐓𝐞𝐬𝐭𝐢𝐧𝐠 𝐭𝐡𝐞 𝐌𝐨𝐝𝐞𝐥 𝐰𝐢𝐭𝐡 𝐆𝐫𝐚𝐝𝐢𝐨
Once the model is fine-tuned, you can deploy it using Gradio. Run the cell on colab to launch the interface


### Results
The fine-tuned model achieves improved transcription accuracy for medical-related audio data. The Word Error Rate (WER) is used as the primary evaluation metric.

### Contributing
Contributions are welcome! If you’d like to contribute to this project, please follow these steps:

### Fork the repository.

Create a new branch for your feature or bugfix.

Submit a pull request with a detailed description of your changes.

### License
This project is licensed under the Apachi 2.0. See the LICENSE file for details.

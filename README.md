# **Medical AI Chatbot Using LLaMA 2 with PEFT, LoRA, and QLoRA**

## **Project Overview**  
This project involves developing a **Medical AI Chatbot** that utilizes **LLaMA 2**, a state-of-the-art language model, to provide recommendations and precautions for medical symptoms. It focuses on fine-tuning the base model with **Parameter-Efficient Fine-Tuning (PEFT)** techniques like **LoRA (Low-Rank Adaptation)** and **QLoRA (Quantized Low-Rank Adaptation)** to ensure efficient training on limited computational resources.

---

## **Features**  
- Provides **recommendations** and **precautions** based on user input.  
- Handles **medical terms** and **abbreviations** effectively.  
- Optimized for training and inference on resource-constrained environments (e.g., Google Colab).  

---

## **Dataset**  
- **Source:** [AI Medical Chatbot Dataset](https://www.kaggle.com/datasets/yousefsaeedian/ai-medical-chatbot/data)  
- **Key Statistics:**  
  - Total Records: 228,722  
  - Unique Patients: 246,006  
  - Unique Doctors: 242,150  
- **Features Used:** `Description`, `Patient`, `Doctor`  

---

## **Model Architecture**  
- **Base Model:** [LLaMA 2](https://huggingface.co/meta-llama)  
- **Fine-Tuning Methods:**  
  - **PEFT:** Enabled efficient adaptation by fine-tuning only specific layers.  
  - **LoRA:** Reduced memory usage by adding low-rank matrices for parameter updates.  
  - **QLoRA:** Combined quantization with low-rank updates for even greater efficiency.  

---

## **Implementation Steps**  
1. **Environment Setup:** Install required libraries like `transformers`, `peft`, and `bitsandbytes`.  
2. **Dataset Preprocessing:** Clean and tokenize medical descriptions.  
3. **Model Fine-Tuning:** Fine-tune LLaMA 2 using LoRA and QLoRA.  
4. **Inference:** Generate recommendations for given medical symptoms.  
5. **Evaluation:** Validate performance with evaluation metrics and sample predictions.  

---

## **Requirements**  
- **Hardware:**  
  - Minimum: 8 GB RAM, GPU-enabled Colab environment.  
  - Recommended: 16 GB RAM for faster training.  

- **Python Libraries:**  
  - `transformers`  
  - `datasets`  
  - `peft`  
  - `bitsandbytes`  
  - `torch`  

To install dependencies:  
```bash
pip install transformers datasets peft bitsandbytes torch
```

---

## **Usage**  
1. Clone this repository:  
   ```bash
   git clone(https://github.com/Daniyal-DS/AI-Medical-Chatbot)
   cd Medical-AI-Chatbot
   ```
2. Open the Jupyter Notebook:  
   ```bash
   jupyter notebook Medical_Ai_Chatbot.ipynb
   ```
3. Upload the dataset and follow the notebook steps for training and inference.

---

## **Results**  
- **Validation Accuracy:** [89%]    
- **Sample Output:**  
  - **Input:** *"Patient experiencing shortness of breath and chest pain."*  
  - **Output:** *"Recommended Specialist: Cardiologist. Precautions: Avoid strenuous activities, consult immediately."*

---

## **Challenges and Solutions**  
- **Limited Computational Resources:** Addressed with LoRA and QLoRA to optimize GPU usage.  
- **Handling Medical Jargon:** Used domain-specific tokenization for accurate text understanding.  

---

## **Files in the Repository**  
- **`medical_ai_chatbot.ipynb`**: Jupyter Notebook containing the code.  
- **`dataset/`**: Folder for uploading the Kaggle dataset.  
- **`images/`**: Includes screenshots and architecture diagrams.  
- **`README.md`**: Project documentation file.  

---

## **Future Work**  
- Integrate chatbot into a web or mobile application.  
- Expand dataset with more medical conditions for broader coverage.  

---

## **Contributors**  
- **Daniyal Haider**
-  [GitHub Profile](https://github.com/Daniyal-DS) | [LinkedIn Profile](https://www.linkedin.com/in/daniyal-haider83/) 
- **Mohsin Raza** 
-  [GitHub Profile](https://github.com/mohsinraza2999)
  

---

## **License**  
This project is licensed under the MIT License. See the `LICENSE` file for more details.  

---

Let me know if you’d like to customize any part of this README!

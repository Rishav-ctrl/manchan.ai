# WriterAI - The Script Generation LLM

WriterAI is a custom-trained Large Language Model (LLM) designed to generate high-quality, easy-to-understand educational scripts. It specializes in breaking down complex technical topics into simple, engaging content. 

Currently optimized for **Nepali, Hindi, and English**, this model is fine-tuned to mirror the clear and engaging teaching style of "Rishav Explains."

## 🏗️ Project Architecture

This is a full-stack AI application divided into three main microservices:

* **`/ai_engine`**: The core machine learning environment. Contains PyTorch and Hugging Face Transformers code for LoRA fine-tuning and inference.
* **`/backend`**: A Nest.js server that securely handles API requests, user authentication, subscription tiers (NPR 1000/mo), and communication with the AI engine.
* **`/frontend`**: A sleek Next.js user interface for content creators to generate, edit, and manage their scripts.

## 🚀 Getting Started (Local Development)

### 1. AI Engine Setup (Python)
Navigate to the AI engine directory and activate the virtual environment:
```bash
cd ai_engine
python -m venv venv
venv\Scripts\activate  # On Windows
pip install -r requirements.txt
```
### 2. Backend Setup (Nest.js)
```bash
cd backend
npm install
npm run start:dev
```
### 3. Frontend Setup (Next.js)
```bash
cd frontend
npm install
npm run dev
```

### 4. 🧠 Model Training (Coming Soon)
Details on dataset formatting (.jsonl), LoRA weight adapters, and evaluation metrics will be documented here as the model reaches Phase 2 of training.




















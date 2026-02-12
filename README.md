# Bilingual AI Customer Support (FR/EN)

An end-to-end AI pipeline that processes customer messages in French or English:
1) Detects the message language (FR/EN)
2) Classifies the message category
3) Detects urgency level
4) Generates a suggested reply in the same language
5) Supports human validation before sending

Capstone AI project focused on NLP, classification, and intelligent response generation.

---

## Key Features
- Language detection at input (FR/EN)
- Automatic message classification
- Urgency detection (urgent / non-urgent)
- Response generation aligned with the customer language
- Human validation before final response

---

## Architecture (high-level)

Input message  
→ Language Detection  
→ Category Classifier  
→ Urgency Detector  
→ Response Generator (same language)  
→ Human Validation  
→ Final Response

---

## Tech Stack
- Python
- Machine Learning / NLP (scikit-learn, Transformers)
- Language detection (fastText or langdetect)
- Pandas / NumPy
- Optional API: FastAPI

---

## Project Structure (planned)

bilingual-ai-customer-support/
│
├── README.md  
├── requirements.txt  
├── src/
│   ├── main.py
│   ├── language_detect.py
│   ├── category_classifier.py
│   ├── urgency_detector.py
│   └── response_generator.py
│
├── data/
└── assets/

---

## How to Run (example)

Create environment:

python -m venv .venv

Activate environment:

Windows:
.venv\Scripts\activate

Mac/Linux:
source .venv/bin/activate

Install dependencies:

pip install -r requirements.txt

Run example:

python -m src.main --text "The room wasn't clean and comfortable"

Expected output:
Language detected: EN  
Category: Complaint  
Urgency: High  
Suggested reply generated.

---

## Dataset
Customer message datasets in French and English will be used.

If datasets are private:
- Provide download instructions
- Explain preprocessing steps
- Describe labeling

---

## Evaluation Plan
- Classification accuracy and F1-score
- Urgency detection precision/recall
- Error analysis for improvement

---

## Future Improvements
- Transformer fine-tuning
- Better urgency detection
- API deployment
- Demo interface

---

## Author
Abdelkhalek Aksil  
AI Student – La Cité Collégiale  
Montreal, Canada  
Email: aksilabdelkhalek@gmail.com

# 🍎🍊🥭🍈 Fruit Grading System

An AI-based fruit grading system for agricultural and food quality analysis.
Built using CNN (Convolutional Neural Networks) and Machine Learning.

## 👥 Contributors
- **Bhavna** — Apple freshness classifier + Apple grading logic
- **Tasmiya** — Fruit type classifier + Orange/Mango/Guava grading + Master pipeline

## 🎯 Objective
Automatically classify and grade fruits based on:
1. **Fruit Type Detection** — Identify which fruit it is
2. **Freshness Detection** — Fresh or Rotten (via CNN)
3. **Quality Analysis** — Based on physical features
4. **Grade Assignment** — A (Best), B (Good), C (Fair), D (Bad)

## 🍱 Supported Fruits
| Fruit | Freshness CNN | Quality Grading |
|---|---|---|
| 🍎 Apple | ✅ Done | ✅ Done |
| 🍊 Orange | ✅ Done | ✅ Done |
| 🥭 Mango | ✅ Done | ✅ Done |
| 🍈 Guava | ✅ Done | ✅ Done |

## 🔄 Workflow
Input Image
↓
Fruit Type Classifier (CNN)
↓
Freshness Classifier (CNN per fruit)
↓
Quality Analysis
↓
Final Grade: A / B / C / D
## 📊 Grade System
| Grade | Meaning | Condition |
|---|---|---|
| A | Best | Fresh + excellent quality |
| B | Good | Fresh + good quality |
| C | Fair | Fresh + poor quality OR slightly rotten |
| D | Bad | Rotten + very poor quality |

## 🗂️ Project Structure
fruit-grading-system/
├── notebooks/
│   └── apple_freshness.ipynb        # Bhavna's apple CNN
├── tasmiya-work/
│   ├── apple_grade_fix.ipynb        # Fixed Grade D logic
│   ├── fruit-type-classifier/
│   │   └── fruit_type_classifier.ipynb
│   ├── orange-grading/
│   │   └── orange_grading.ipynb
│   ├── mango-grading/
│   │   └── mango_grading.ipynb
│   ├── guava-grading/
│   │   └── guava_grading.ipynb
│   └── master-pipeline/
│       └── master_pipeline.ipynb
├── models/
│   ├── apple_freshness_model.h5
│   ├── fruit_type_classifier.keras
│   ├── orange_freshness_model.keras
│   ├── mango_freshness_model.keras
│   └── guava_freshness_model.keras
└── datasets/
├── apple_quality/
└── fruits360/


## 🛠️ Tech Stack
- Python 3.12
- TensorFlow / Keras
- OpenCV
- Pandas
- Matplotlib
- Jupyter Notebook

## 🚀 Future Improvements
- YOLO real-time fruit detection
- Surface defect analysis
- Web app interface
- Mobile app integration
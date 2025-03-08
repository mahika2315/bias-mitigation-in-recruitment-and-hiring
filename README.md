# ⚖️ Recruitment Bias Mitigation Tool

## 📌 Overview
The **Recruitment Bias Mitigation Tool** is a **Streamlit-based application** that enables users to analyze and mitigate bias in recruitment datasets. It provides insights into demographic parity difference and equalized odds difference and applies bias mitigation using **Fairlearn's ExponentiatedGradient** method.

## ✨ Features
- 📊 **Upload a recruitment dataset** (CSV format)
- 🎯 **Select target and sensitive attributes** for bias analysis
- 🏆 **Evaluate bias metrics** (such as Demographic Parity Difference, Equalized Odds Difference)
- 🏗️ **Apply bias mitigation** using Fairlearn
- 📈 **Visualizations**: Confusion Matrix and ROC Curve
- 💾 **Download results** after analysis and mitigation

## 🛠️ Installation
To run this project locally, follow these steps:

### 1️⃣ Clone the Repository
```sh
git clone https://github.com/mripradhan/bias-mitigation-tool.git
cd bias-mitigation-tool
```

### 2️⃣ Install Dependencies
Create a virtual environment (optional but recommended):
```sh
python -m venv env
source env/bin/activate  # On Windows use: env\Scripts\activate
```
Then, install the required libraries:
```sh
pip install -r requirements.txt
```

Create a `.env` file and add your API key:
```sh
GROQ_API_KEY="yourapikey"' > .env
```

### 3️⃣ Run the Streamlit App
```sh
streamlit run biasmitigation.py
```

## 📂 Project Structure
```
📁 bias-mitigation-tool/
│-- 📄 biasmitigation.py      # Main Streamlit application
│-- 📄 requirements.txt       # List of dependencies
│-- 📄 README.md              # Documentation
```

## 🏗️ How to Use
1. **Upload your dataset**: Select a CSV file containing recruitment-related data.
2. **Select columns**: Choose a sensitive attribute (e.g., gender, race) and a target column (e.g., hired or not).
3. **Analyze bias**: The tool computes bias metrics and visualizes results.
4. **Mitigate bias**: Apply Fairlearn's ExponentiatedGradient method to reduce bias.
5. **Download results**: Save the processed predictions for further evaluation.

## 🔍 Bias Metrics Explained
- **Demographic Parity Difference**: Measures if different groups have equal selection rates.
- **Equalized Odds Difference**: Measures if predictions are equally accurate across groups.

## 🛠️ Technologies Used
- **Python** 🐍
- **Streamlit** 📊
- **Fairlearn** ⚖️
- **scikit-learn** 🤖
- **Matplotlib & Seaborn** 📈

## 📜 License
This project is licensed under the **MIT License**.

## 🤝 Contributing
Contributions are welcome! Feel free to fork this repo, open issues, or submit pull requests.

---
🚀 **Empower ethical AI in recruitment with this bias mitigation tool!**


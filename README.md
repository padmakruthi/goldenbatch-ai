# GoldenBatch AI

GoldenBatch AI is an intelligent batch-processing and predictive analytics platform designed for pharmaceutical manufacturing. The system leverages machine learning to predict the quality of pharmaceutical tablets before production begins, allowing for real-time optimization of manufacturing settings to reduce waste and energy consumption.

## 🚀 Overview

The platform provides a data-driven approach to manufacturing, shifting from reactive quality testing to proactive quality assurance. By analyzing input parameters such as pressure, temperature, and material composition, the system predicts critical quality attributes and recommends optimal machine configurations.

### Key Features

* **Predictive Analytics:** Uses an XGBoost machine learning model to forecast tablet quality (e.g., hardness, dissolution) based on pre-run parameters.
* **Role-Based Access Control (RBAC):** Tailored interfaces and permissions for three distinct user levels:
* **Operators:** Input batch data and receive real-time production guidance.
* **Engineers:** Perform deep-dive analysis into machine performance and model outputs.
* **Managers:** Oversee production trends, quality compliance, and operational efficiency.


* **Sustainability Tracking:** Built-in carbon footprint monitoring to track and reduce energy usage during the manufacturing process.
* **Real-time Messaging:** Integrated communication tools for seamless collaboration between plant floor staff and management.

## 🛠️ Tech Stack

* **Backend:** FastAPI (Python)
* **Machine Learning:** XGBoost, Scikit-learn
* **Database:** SQLite
* **Frontend:** Modern UI with real-time data visualization
* **Deployment:** Render

## 💻 Getting Started

### Prerequisites

* Python 3.9+
* Pip (Python package manager)

### Installation

1. **Clone the repository:**
```bash
git clone https://github.com/your-username/goldenbatch-ai.git
cd goldenbatch-ai

```


2. **Create a virtual environment:**
```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

```


3. **Install dependencies:**
```bash
pip install -r requirements.txt

```


4. **Run the application:**
```bash
uvicorn main:app --reload

```


The application will be available at `http://127.0.0.1:8000`.

## ⚙️ How It Works

1. **Data Input:** Operators enter raw material specs and machine set-points into the FastAPI-powered interface.
2. **ML Inference:** The XGBoost model processes the data against historical batch records stored in SQLite.
3. **Optimization:** The system outputs a "Quality Score" and suggests adjustments to parameters (like compression force) to ensure the batch meets regulatory standards.
4. **Monitoring:** Energy consumption is calculated per batch, providing a transparent view of the environmental impact of production.

---

**Live Demo:** [https://goldenbatch-ai.onrender.com/app](https://goldenbatch-ai.onrender.com/app)

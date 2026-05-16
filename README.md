# 🌿 PlantGuard AI - Smart Greenhouse Management & Disease Detection

An advanced cloud-integrated Smart Agriculture ecosystem that unifies IoT telemetry simulation, deep-learning computer vision, and an intelligent Gemini-powered RAG knowledge engine.

🚀 **[Try it on Google Colab](https://colab.research.google.com/drive/19Y6sAc2wNiBi3heTw1LHLU6ITEFgAu7D?usp=sharing#scrollTo=uvtTlmhxzDyT)**

---

## 📖 System Overview
This project implements a comprehensive Smart Agriculture solution that combines IoT data monitoring, Artificial Intelligence (AI), and a user-friendly interface. The system allows greenhouse managers to monitor environmental conditions, identify plant diseases using computer vision, and access research data instantly.

---

## 🛠️ Technical Stack & Libraries
The system is built using Python and integrates the following cloud services and libraries:

* **Google Gemini API (`google.generativeai`):** Functions as the system's "Brain" for Natural Language Processing (NLP), powering the RAG (Retrieval-Augmented Generation) search engine to summarize agricultural articles and driving the intelligent Chatbot assistant.
* **Firebase Realtime Database (`firebase`):** Acts as the cloud storage backend, storing historical IoT sensor data (Temperature, Humidity, Soil) and holding the Inverted Index and article metadata for the search engine.
* **NLTK (Natural Language Toolkit):** Used for text preprocessing, Tokenization, and Stop-words removal to optimize the search engine's accuracy.
* **OpenCV & Pillow (`cv2`, `PIL`):** Performs advanced image processing using HSV color masking to detect specific disease symptoms (e.g., White for Powdery Mildew, Yellow for Chlorosis).
* **Transformers (HuggingFace):** Utilizes the `umutbozdag/plant-identity` model to classify and verify the plant species before analysis.

---

## 📂 System Modules
| Module | Core Implementation |
| :--- | :--- |
| **Cloud Telemetry Backend** | Manages live sync and data retrieval from Firebase Realtime Database. |
| **Diagnostic Vision Engine** | Processes plant images using OpenCV color masking and HuggingFace models. |
| **AI RAG Router** | Builds the Inverted Index and queries Google Gemini API for expert medical insights. |

---

## 📊 Installation & Quickstart

To run this project locally or in your environment, clone the repository and install the dependencies:

```bash
# Clone the repository
git clone [https://github.com/ShonAzulay/Cloud-computing-2026-ant-group.git](https://github.com/ShonAzulay/Cloud-computing-2026-ant-group.git)

# Install required packages
pip install google-generativeai firebase-admin nltk opencv-python transformers pillow

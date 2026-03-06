# ⚖️ The Standoff: Local AI Negotiation Simulator

The Standoff is a privacy-first, fully local AI negotiation simulator built with Python and Gradio. It allows professionals, founders, and students to pressure-test their negotiation strategies against a highly customizable AI opponent. 

Because it runs entirely on your local machine using **Ollama**, your contract clauses, negotiation tactics, and business logic never leave your computer—no API keys, no cloud processing, and zero privacy risks.

## ✨ Features
* **100% Local & Private:** Powered by Ollama. Your sensitive contract clauses stay on your hard drive.
* **Customizable Opponent Engine:** Define the AI's exact persona, tone, and organization.
* **Strict Strategic Constraints:** Program the AI's underlying logic by setting its Win/Lose Interests, Situational Leverage, BATNA (Best Alternative to a Negotiated Agreement), and absolute Walk-Away Conditions.
* **Focused Context:** Paste specific, problematic clauses to keep the AI highly responsive and focused on the exact terms in dispute.

## 🛠️ Prerequisites
Before running The Standoff, you need two things installed on your system:
1. **Python 3.8+** (Anaconda/JupyterLab recommended)
2. **Ollama:** The engine that runs the local AI models. Download it from [ollama.com](https://ollama.com/)

## 🚀 Installation & Setup

**1. Install Python Dependencies**
Open your terminal or Jupyter Notebook and install the required libraries:
```bash
pip install gradio ollama
```

**2. Download the AI Model**
This project uses **Llama 3.1 (8B)** by default, which requires about 5GB of storage and runs smoothly on standard laptops. Open your terminal and run:
```bash
ollama run llama3.1:8b
```
*Note: Once it says "success", type `/bye` to exit the prompt. Ensure the Ollama application remains running in your system tray/background.*

## 💻 Running the Simulator

If you are using JupyterLab or a Jupyter Notebook:
1. Open the `.ipynb` file or paste the Python code into a new cell.
2. Run the cell.
3. The simulator will automatically launch in a new, dedicated tab in your default web browser (usually at `http://127.0.0.1:7860`).

## 🎯 How to Use
The interface is split into two sections: **Configuration (Left)** and **The Arena (Right)**.

1. **Engine & Contract:** Paste the exact text of the clauses you want to dispute. 
2. **Personas:** Define who you are and who the AI is playing (e.g., "Harvard MBA, risk-averse").
3. **Opponent's Constraints:** This is the secret sauce. Tell the AI what it actually wants behind the scenes. Define its BATNA and the strict Walk-Away conditions it must not compromise on.
4. **Negotiate:** Type your opening move in the chat interface on the right and see if you can break the opponent's defenses.

## 🛑 Stopping the Application
* **Close the App:** Interrupt the kernel in your Jupyter Notebook (click the "Stop" square).
* **Free up RAM:** If you want to unload the AI model from your computer's memory, open your terminal and type:
  ```bash
  ollama stop llama3.1:8b
  ```

## 🤖 Acknowledgments
This project was developed with code assistance and debugging support from **Gemini 3.1 Pro**.

## 📄 License
This project is licensed under the MIT License. Feel free to fork, modify, and improve!

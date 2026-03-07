# ⚖️ The Standoff: Local AI Negotiation Simulator

The Standoff is a privacy-first, fully local AI negotiation simulator built with Python and Gradio. It allows professionals, founders, and students to pressure-test their negotiation strategies against a highly customizable AI opponent. 

Because it runs entirely on your local machine using **Ollama**, your contract clauses, negotiation tactics, and business logic never leave your computer—no API keys, no cloud processing, and zero privacy risks.

## ✨ Features
* **100% Local & Private:** Powered by Ollama. Your sensitive contract clauses stay on your hard drive.
* **Customizable Opponent Engine:** Define the AI's exact persona, tone, and organization.
* **Strict Strategic Constraints:** Program the AI's underlying logic by setting its Interests, Situational Leverage, BATNA (Best Alternative to a Negotiated Agreement), and absolute Walk-Away Conditions.
* **Lightweight & Fast:** Designed to use specific text snippets rather than heavy PDF files to ensure near-instant AI response times.

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
This project uses **Llama 3.1 (8B)** by default. Open your terminal and run:
```bash
ollama run llama3.1:8b
```
*Note: Once it says "success", type `/bye` to exit the prompt. Ensure the Ollama application remains running in your system tray/background.*

## 💻 Running the Simulator

If you are using JupyterLab or a Jupyter Notebook:
1. Open the `.ipynb` file or paste the Python code into a new cell.
2. Run the cell.
3. The simulator will automatically launch in a new browser tab (usually at `http://127.0.0.1:7860`).

## 🎯 How to Use
The interface is designed for high-speed iteration. Configure the parameters on the left before entering the Arena on the right.

1. **Engine & Contract:** Paste the exact text of the clauses you want to dispute into the "Specific Clauses" box.
2. **Personas:** Define who you are and who the AI is playing. Use the pre-filled "Toxic Client" scenario for a quick start!
3. **Opponent's Constraints:** Define the AI's hidden agenda. Tell it why it has the upper hand (Leverage) and what it will do if you can't reach a deal (BATNA).
4. **The Arena:** Type your opening move in the chat interface. The AI will respond based on its programmed personality and strategic limits.

## 🛑 Stopping the Application
* **Close the App:** Interrupt the kernel in your Jupyter Notebook (click the "Stop" square icon).
* **Free up RAM:** To immediately unload the AI model from your computer's memory, run this in your terminal:
  ```bash
  ollama stop llama3.1:8b
  ```

## 🤖 Acknowledgments
This project was developed with code assistance and debugging support from **Gemini 3.1 Pro**.

## Contact
Created by [William H. Ongseputra](https://www.linkedin.com/in/wongseputra/).

## 📄 License
This project is licensed under the MIT License. Feel free to fork, modify, and improve!

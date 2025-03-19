# LLM-Driven-Cybersecurity-Compliance-Evaluator

## Overview

LLM-Driven Cybersecurity Compliance Evaluator is a Python-based tool that leverages a large language model (LLM) to assess a company's cybersecurity controls against predefined compliance requirements. The evaluator reads control data from CSV files, uses an AI model to determine if each control is "Met", "Partially Met", or "Not Met", and exports the results to an Excel file. An intuitive user interface has also been added to streamline the evaluation process for cybersecurity analysts and compliance teams.

## Features

- **Automated Compliance Assessment:**  
  Evaluates cybersecurity controls by interacting with an LLM to return standardized responses.
  
- **Data Processing:**  
  Reads compliance requirements and company controls from CSV files and exports the results to Excel.
  
- **User-Friendly Interface:**  
  Provides an interactive UI to load input files, trigger evaluations, and view/export results without writing code.
  
- **AI Integration:**  
  Utilizes the Ollama API (or similar LLM integration) for real-time analysis and decision-making.

## Tech Stack

- **Programming Language:** Python
- **Data Handling:** Pandas
- **User Interface:** (e.g., Streamlit, Tkinter, or your chosen UI framework)
- **AI Integration:** Ollama API (or an equivalent LLM API)
- **Output Format:** Excel (using Pandas' `to_excel` functionality)

## Installation

1. **Clone the Repository**

    ```bash
    git clone https://github.com/yourusername/LLM-Driven-Cybersecurity-Compliance-Evaluator.git
    cd LLM-Driven-Cybersecurity-Compliance-Evaluator
    ```

2. **Create a Virtual Environment and Activate It**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Unix or macOS
    # or
    venv\Scripts\activate  # On Windows
    ```

3. **Install Dependencies**

    ```bash
    pip install -r requirements.txt
    ```

4. **Configure API Keys**

   Ensure you have set any necessary API keys (e.g., for the Ollama API) in your environment variables or configuration files.

## Usage

### Using the User Interface

1. **Launch the UI:**

    If you're using Streamlit:
    ```bash
    streamlit run app.py
    ```
    Or, if using another framework (like Tkinter), run the main UI file:
    ```bash
    python main.py
    ```

2. **Follow the On-Screen Instructions:**

   - **Load** your CSV file containing cybersecurity compliance data.
   - **Evaluate** the controls by clicking the appropriate button.
   - **Review** the results directly in the UI or export them to an Excel file.

### Command-Line Usage

If you prefer running the evaluation without the UI:
```bash
python evaluator.py

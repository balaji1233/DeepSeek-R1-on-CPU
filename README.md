# DeepSeek-R1-on-CPU


Deep Seek R1 is an advanced open-source AI model designed for reasoning, coding, and problem-solving. This project demonstrates multiple methods to interact with Deep Seek R1 using the oLama framework. It highlights the process of downloading, running, and interfacing with the model through various methods—from the command line to user-friendly GUIs like Open Web UI, Chainlit, and Streamlit.



## Table of Contents

- [Overview](#overview)
- [Highlights](#highlights)
- [Key Insights](#key-insights)
- [Installation & Setup](#installation--setup)
  - [1. Using the oLama Framework](#1-using-the-olama-framework)
  - [2. Interaction Methods](#2-interaction-methods)
- [Usage Examples](#usage-examples)
- [Contributing](#contributing)
- [References](#references)

---

## Overview

This project demonstrates how to leverage the Deep Seek R1 model via the ollama framework to create impactful AI solutions. It includes:

- **Step-by-step model downloading:** Learn how to pull and run Deep Seek R1 from your terminal.
- **Multiple interfaces:** Utilize GUIs like Open Web UI, Chainlit, and Streamlit to interact with the model in a friendly, customizable environment.
- **Accessibility for limited hardware:** The oLama framework makes it possible to run large language models on devices without high-end computing power, democratizing access to cutting-edge AI.

---

## Highlights

- **🚀 Powerful AI Tools:** ollama enables users with modest hardware to tap into advanced large language models.
- **💻 Versatile Interaction:** Choose from terminal commands, Open Web UI, Chainlit, or Streamlit to interact with the model.
- **📥 Easy Model Downloading:** Follow clear, step-by-step instructions to download and set up Deep Seek R1.
- **🌐 User-Friendly GUIs:** Enhance your experience with intuitive interfaces that lower the barrier for non-technical users.
- **🛠️ Customizable Solutions:** Use Chainlit to personalize your interfaces for specific applications.
- **📊 Broad Applicability:** Adapt the model for diverse projects—from research tools to production-level applications.
- **📣 Community Engagement:** The project encourages you to share your creative applications and real-world experiences.

---

## Key Insights

- **🔍 Democratizing AI:** Tools like ollama make advanced models accessible even on lower-end hardware, enabling a wider range of users to experiment with AI.
- **⚙️ Command-Line Mastery:** A solid understanding of terminal commands unlocks the full potential of large language models.
- **🌟 Flexible Performance:** With options ranging from 1.5B to 671B parameters, you can balance resource constraints with performance needs.
- **📊 Seamless Visualization:** GUIs like Open Web UI and Streamlit provide a chat-like experience, making interactions with the model intuitive.
- **📉 Trade-Offs:** Smaller models may not produce production-ready outputs but are excellent for prototyping and learning.
- **🎨 Customization:** Chainlit empowers developers to tailor the UI to specific use cases, enhancing engagement and satisfaction.
- **🗣️ Ethical Considerations:** The project emphasizes avoiding controversial topics and maintaining responsible AI usage.

---

## Installation & Setup

### 1. Using the oLama Framework

The oLama framework simplifies running Deep Seek R1 locally. It allows you to download and execute the model with a few simple commands.

1. **Download and Install oLama:**  
   Visit [ollama.com/download](https://ollama.com/download) to install the version for your operating system.

2. **Verify Installation:**  
   ```bash
   ollama --version
   ```
   
## Pull the Deep Seek R1 Model

For a lightweight start, run the 1.5B parameter version:




```bash
ollama run deepseek-r1:1.5b
```
## 2. Interaction Methods

You can interact with Deep Seek R1 in several ways:

### Terminal
Directly type prompts in your command line.

### Open Web UI
Install via pip and run:
```bash
pip install open-webui
open-webui serve

```

## Usage Examples

### Command-Line Interaction

Type a prompt directly in your terminal:
```bash
ollama run deepseek-r1:1.5b "Explain the significance of retrieval-augmented generation."
```

## Using Open Web UI

After installing and serving Open Web UI, access [http://localhost:8080](http://localhost:8080) in your browser. Here you can chat with Deep Seek R1 through a friendly interface.

## Integrating with Chainlit or Streamlit

Leverage Python frameworks to create custom UIs. For example, a simple Streamlit app:

```python
import streamlit as st

st.title("Deep Seek R1 Chat")
user_input = st.text_input("Enter your question:")

if user_input:
    # Assume `query_deepseek` is a function that sends the prompt via oLama.
    response = query_deepseek(user_input)
    st.write(response)
```

## Contributing
Contributions are welcome! If you have ideas for improvements, new interaction methods, or additional features, please open an issue or submit a pull request.

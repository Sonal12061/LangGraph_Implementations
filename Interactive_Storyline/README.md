# Stranger Things Scene Generator 🎬🌌

This project creates an interactive scene-based storytelling experience in the style of *Stranger Things*, using LLMs like HuggingFace's Mistral and LangGraph for flow control. Users are guided through eerie, supernatural scenes with branching narrative choices, just like a playable text adventure.

## 🧠 Technologies Used

- **LangGraph**: For managing multi-step scene flows and stateful transitions.
- **HuggingFace Transformers (Mistral)**: For generating spooky scenes and multiple choice options.
- **Python**: Core language for logic, state classes, and prompt orchestration.
- **Jupyter Notebook**: Used for development and interactive testing.

## 📜 Features

- Generates atmospheric scenes inspired by *Stranger Things*.
- Presents 4 vivid narrative choices to the user after each scene.
- Supports back-and-forth interaction through a stateful graph.
- Integrates with HuggingFace's Mistral model manually (for customized response parsing).

## 🚀 How It Works

1. The system initializes a state graph with LangGraph.
2. Each state generates a scene and receives user input.
3. The user’s choice affects the path and next scene shown.
4. The narrative proceeds until a maximum depth or a “halt” signal.

## 🛠️ Setup Instructions

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/stranger-things-scene.git
   cd stranger-things-scene
   ```

2. Install dependencies:
   ```bash
   pip install langgraph huggingface_hub transformers ipywidgets
   ```

3. Run the notebook:
   Open `Stranger_Things_Scene.ipynb` in Jupyter and step through the cells.

## ✍️ Sample Prompt to Mistral

```python
prompt = """
You are a master storyteller in the style of Stranger Things...
"""
```

Expected output:
```json
{
  "scene": "You hear a distant crackle...",
  "choices": ["Follow the sound", "Stay put", "Call for help", "Investigate the streetlamp"]
}
```

## 🧩 Folder Structure

```
📁 stranger-things-scene/
├── Stranger_Things_Scene.ipynb
├── README.md
└── assets/
```

## 🧙‍♀️ Inspirations

- *Stranger Things* (Netflix series)
- Interactive Fiction / Choose Your Own Adventure
- LangChain & LangGraph for AI-driven story flows

## 🙌 Acknowledgements

- HuggingFace for open-access LLMs
- LangChain team for LangGraph
- The Duffer Brothers, for creating the Stranger Things universe!
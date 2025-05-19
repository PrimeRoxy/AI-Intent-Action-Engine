# 🧠 IntelliFlow - AI Intent Classification & Action Execution System

<div align="center">

![IntelliFlow Logo](https://img.shields.io/badge/IntelliFlow-AI%20Powered-blue?style=for-the-badge&logo=brain&logoColor=white)

**Repository:** `AI-Intent-Action-Engine`

*🚀 Transforming natural language queries into intelligent actions through AI-powered processing*

[![Python](https://img.shields.io/badge/Python-3.12+-blue?style=flat-square&logo=python)](https://python.org)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4-green?style=flat-square&logo=openai)](https://openai.com)
[![Streamlit](https://img.shields.io/badge/Streamlit-UI-red?style=flat-square&logo=streamlit)](https://streamlit.io)

</div>

---

## 🌟 Overview

**IntelliFlow** is a comprehensive Python-based system designed to facilitate intelligent message classification, action discovery, parameter generation, and API invocation. This cutting-edge solution creates a seamless interaction pipeline that understands user intent and executes relevant actions automatically.

🎯 **Perfect for:** Real estate transactions, customer service automation, intelligent chatbots, and any domain requiring intent-to-action transformation.

---

## 🏗️ System Architecture

```
User Query → Intent Classification → Action Discovery → Parameter Generation → User Input → Action Execution → Results
```

---

## 🔧 Core Components

### 1. 🔍 Intent Classifier (`intent_classifier.py`)
> **Intelligent Message Understanding**
- ✨ **Purpose:** Employs OpenAI's GPT-4 to classify messages into categories:
  - 📢 "INFO SHARED"
  - 🎯 "ACTION REQUEST" 
  - ❓ "ASK"
  - 🤔 "IMPLICIT ACTION"
- 💡 **Details:** Provides detailed analysis of message intent for real estate transactions
- 🎮 **Usage:** Execute script and provide messages for intelligent classification

### 2. 🎯 Action Discovery Engine (`action_discovery.py`)
> **Smart Action Mapping**
- ✨ **Purpose:** Analyzes queries and matches them with appropriate action IDs
- 💡 **Details:** Identifies the most suitable action or signals "No Action Found"
- 🎮 **Usage:** Input user queries to discover relevant action mappings

### 3. ⚙️ Parameter Generator (`parameter_generator.py`)
> **Dynamic Parameter Creation**
- ✨ **Purpose:** Generates input parameters required for specific actions
- 💡 **Details:** Extracts necessary information from configuration files
- 🎮 **Usage:** Provide action IDs to receive parameter specifications

### 4. 👤 Input Processor (`input_processor.py`)
> **User-Friendly Input Collection**
- ✨ **Purpose:** Guides users through parameter input with validation
- 💡 **Details:** Interactive prompts with data validation and missing info requests
- 🎮 **Usage:** Follow interactive prompts to provide necessary parameters

### 5. 🚀 Action Executor (`action_executor.py`)
> **Seamless API Integration**
- ✨ **Purpose:** Formats data and invokes APIs for action execution
- 💡 **Details:** Elegant result presentation completing the interaction cycle
- 🎮 **Usage:** Execute with user input to observe action results

---

## 🌐 Web Interface

### 🎨 IntelliFlow Streamlit Dashboard (`intelliflow_app.py`)
> **Modern & Intuitive UI**
- ✨ **Purpose:** Provides a beautiful web interface for system interaction
- 💡 **Details:** Process inputs, generate parameters, and display results seamlessly
- 🎮 **Usage:** Launch Streamlit app for web-based interaction

---

## 🚀 Quick Start

### 📋 Prerequisites

```bash
# Ensure Python 3.8+ is installed
python --version
```

### 🔨 Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/ai-intent-action-engine.git
   cd ai-intent-action-engine
   ```

2. **Install Dependencies**
   ```bash
   pip install openai streamlit requests python-dotenv
   ```

3. **Configure Environment**
   ```bash
   # Option 1: Environment Variable
   export OPENAI_API_KEY=your_api_key_here
   
   # Option 2: .env file
   echo "OPENAI_API_KEY=your_api_key_here" > .env
   ```

### 🎬 Launch Application

```bash
streamlit run intelliflow_app.py
```

🌐 **Access your dashboard at:** `http://localhost:8501`

---

## 🎯 Features

<table>
<tr>
<td>

**🤖 AI-Powered**
- Multi-stage AI pipeline
- GPT-4 powered classification
- Intelligent action mapping

</td>
<td>

**🔧 Flexible**
- Configurable action databases
- Multiple LLM support
- Domain adaptable

</td>
</tr>
<tr>
<td>

**🎨 User-Friendly**
- Modern web interface
- Interactive parameter collection
- Real-time feedback

</td>
<td>

**⚡ Robust**
- Error handling
- API rate limiting
- Performance monitoring

</td>
</tr>
</table>

---

## 🛠️ Customization Options

| Component | Customization | Description |
|-----------|--------------|-------------|
| 🗄️ **Action Database** | JSON Files | Add domain-specific actions |
| 🔍 **Classification** | Categories | Adjust intent categories |
| 🔗 **API Integration** | Endpoints | Configure different APIs |
| 🎨 **UI Theme** | Streamlit | Customize branding |

---

## ⚠️ Important Note

> **🔄 LLM Flexibility:** While IntelliFlow uses OpenAI's GPT models by default, you can integrate **any LLM**:
> - 🤖 Anthropic Claude
> - 🧠 Google Gemini  
> - 🤗 Hugging Face models
> - 🦙 Open-source alternatives (Llama, etc.)
>
> Simply modify the integration in `intent_classifier.py` according to your chosen model's requirements.

---

## 📋 Best Practices

- ✅ Ensure proper configuration file formatting
- ✅ Implement comprehensive error handling
- ✅ Regular action database updates
- ✅ Monitor system performance
- ✅ Test with domain-specific queries

---

## 🤝 Contributing

We welcome contributions! 

1. 🍴 Fork the repository
2. 🌟 Create a feature branch
3. 💻 Make your changes
4. ✅ Add comprehensive tests
5. 📝 Submit a pull request


<div align="center">

### 🚀 Ready to transform your queries into actions?

**[Get Started](#-quick-start)** 

---

*Made with ❤️ by the IntelliFlow *

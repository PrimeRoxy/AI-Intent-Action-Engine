🧠 IntelliFlow - AI Intent Classification & Action Execution System
<div align="center">
Show Image
Repository: ai-intent-action-engine
🚀 Transforming natural language queries into intelligent actions through AI-powered processing
Show Image
Show Image
Show Image
Show Image
</div>

🌟 Overview
IntelliFlow is a comprehensive Python-based system designed to facilitate intelligent message classification, action discovery, parameter generation, and API invocation. This cutting-edge solution creates a seamless interaction pipeline that understands user intent and executes relevant actions automatically.
🎯 Perfect for: Real estate transactions, customer service automation, intelligent chatbots, and any domain requiring intent-to-action transformation.

🏗️ System Architecture
mermaidgraph LR
    A[📝 User Query] --> B[🔍 Intent Classification]
    B --> C[🎯 Action Discovery]
    C --> D[⚙️ Parameter Generation]
    D --> E[👤 User Input]
    E --> F[🚀 Action Execution]
    F --> G[📊 Results]

🔧 Core Components
1. 🔍 Intent Classifier (intent_classifier.py)

Intelligent Message Understanding


✨ Purpose: Employs OpenAI's GPT-4 to classify messages into categories:

📢 "INFO SHARED"
🎯 "ACTION REQUEST"
❓ "ASK"
🤔 "IMPLICIT ACTION"


💡 Details: Provides detailed analysis of message intent for real estate transactions
🎮 Usage: Execute script and provide messages for intelligent classification

2. 🎯 Action Discovery Engine (action_discovery.py)

Smart Action Mapping


✨ Purpose: Analyzes queries and matches them with appropriate action IDs
💡 Details: Identifies the most suitable action or signals "No Action Found"
🎮 Usage: Input user queries to discover relevant action mappings

3. ⚙️ Parameter Generator (parameter_generator.py)

Dynamic Parameter Creation


✨ Purpose: Generates input parameters required for specific actions
💡 Details: Extracts necessary information from configuration files
🎮 Usage: Provide action IDs to receive parameter specifications

4. 👤 Input Processor (input_processor.py)

User-Friendly Input Collection


✨ Purpose: Guides users through parameter input with validation
💡 Details: Interactive prompts with data validation and missing info requests
🎮 Usage: Follow interactive prompts to provide necessary parameters

5. 🚀 Action Executor (action_executor.py)

Seamless API Integration


✨ Purpose: Formats data and invokes APIs for action execution
💡 Details: Elegant result presentation completing the interaction cycle
🎮 Usage: Execute with user input to observe action results


🌐 Web Interface
🎨 IntelliFlow Streamlit Dashboard (intelliflow_app.py)

Modern & Intuitive UI


✨ Purpose: Provides a beautiful web interface for system interaction
💡 Details: Process inputs, generate parameters, and display results seamlessly
🎮 Usage: Launch Streamlit app for web-based interaction


🚀 Quick Start
📋 Prerequisites
bash# Ensure Python 3.8+ is installed
python --version
🔨 Installation

Clone the Repository
bashgit clone https://github.com/yourusername/ai-intent-action-engine.git
cd ai-intent-action-engine

Install Dependencies
bashpip install openai streamlit requests python-dotenv

Configure Environment
bash# Option 1: Environment Variable
export OPENAI_API_KEY=your_api_key_here

# Option 2: .env file
echo "OPENAI_API_KEY=your_api_key_here" > .env


🎬 Launch Application
bashstreamlit run intelliflow_app.py
🌐 Access your dashboard at: http://localhost:8501

🎯 Features
<table>
<tr>
<td>
🤖 AI-Powered

Multi-stage AI pipeline
GPT-4 powered classification
Intelligent action mapping

</td>
<td>
🔧 Flexible

Configurable action databases
Multiple LLM support
Domain adaptable

</td>
</tr>
<tr>
<td>
🎨 User-Friendly

Modern web interface
Interactive parameter collection
Real-time feedback

</td>
<td>
⚡ Robust

Error handling
API rate limiting
Performance monitoring

</td>
</tr>
</table>

🛠️ Customization Options
ComponentCustomizationDescription🗄️ Action DatabaseJSON FilesAdd domain-specific actions🔍 ClassificationCategoriesAdjust intent categories🔗 API IntegrationEndpointsConfigure different APIs🎨 UI ThemeStreamlitCustomize branding

⚠️ Important Note

🔄 LLM Flexibility: While IntelliFlow uses OpenAI's GPT models by default, you can integrate any LLM:

🤖 Anthropic Claude
🧠 Google Gemini
🤗 Hugging Face models
🦙 Open-source alternatives (Llama, etc.)

Simply modify the integration in intent_classifier.py according to your chosen model's requirements.


📋 Best Practices

✅ Ensure proper configuration file formatting
✅ Implement comprehensive error handling
✅ Regular action database updates
✅ Monitor system performance
✅ Test with domain-specific queries


🤝 Contributing
We welcome contributions!

🍴 Fork the repository
🌟 Create a feature branch
💻 Make your changes
✅ Add comprehensive tests
📝 Submit a pull request


📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

<div align="center">
🚀 Ready to transform your queries into actions?
Get Started • View Demo • Documentation • Support

Made with ❤️ by the IntelliFlow team
</div>
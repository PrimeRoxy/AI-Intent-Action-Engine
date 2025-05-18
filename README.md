# IntelliFlow - AI Intent Classification & Action Execution System
**Repository:** ai-intent-action-engine

This repository contains a comprehensive Python-based system designed to facilitate intelligent message classification, action discovery, parameter generation, and API invocation. IntelliFlow creates a seamless interaction pipeline that understands user intent and executes relevant actions automatically.

## System Overview
IntelliFlow is an AI-powered interactive system that processes user queries through a multi-stage pipeline, from intent classification to action execution. The system is particularly optimized for real estate transactions involving customers and agents, but can be adapted for various domains.

## Core Components

### 1. Intent Classifier (intent_classifier.py)
**Purpose:**
Employs OpenAI's GPT-4 model to classify messages into predefined categories such as "INFO SHARED," "ACTION REQUEST," "ASK," and "IMPLICIT ACTION."
**Details:** Provides detailed analysis of message intent within the context of real estate transactions and customer-agent interactions.
**Usage:** Execute the script and provide messages for intelligent classification.

### 2. Action Discovery Engine (action_discovery.py)
**Purpose:**
Analyzes user queries and matches them with appropriate action IDs from a comprehensive JSON action database.
**Details:** Identifies the most suitable action based on user intent, returning the corresponding action ID or signaling "No Action Found."
**Usage:** Run the script and input user queries to discover relevant action mappings.

### 3. Parameter Generator (parameter_generator.py)
**Purpose:**
Generates input parameters required for executing specific actions based on the discovered action ID.
**Details:** Extracts necessary information from configuration files and presents the input parameters needed for action execution.
**Usage:** Execute the script with action IDs to receive corresponding input parameter specifications.

### 4. Input Processor (input_processor.py)
**Purpose:**
Guides users through providing input parameters for action execution, ensuring all required fields are captured.
**Details:** Prompts users for input based on identified parameters, validates provided data, and requests missing information when necessary.
**Usage:** Run the script, input queries, and follow interactive prompts to provide necessary parameters.

### 5. Action Executor (action_executor.py)
**Purpose:**
Formats user input data into JSON and invokes appropriate APIs for executing designated actions.
**Details:** Presents action outcomes in an elegant format, completing the full interaction cycle with users.
**Usage:** Execute the script with user input data to observe action execution results.

## Web Interface
### IntelliFlow Streamlit Dashboard (intelliflow_app.py)
**Purpose:**
Provides an intuitive web interface for seamless system interaction.
**Details:** Users can input queries through a modern web interface, with the system processing inputs, generating parameters, and presenting results using Streamlit.
**Usage:** Launch the Streamlit application and interact with IntelliFlow through the web dashboard.

## Setup Instructions

### Environment Configuration

**Install Python and Dependencies:**
Ensure Python 3.8+ is installed. Install required dependencies:
```bash
pip install openai streamlit requests python-dotenv
```

**Configure OpenAI API Key:**
Set up your OpenAI API key as an environment variable:
```bash
export OPENAI_API_KEY=your_api_key_here
```
Or create a `.env` file in the project root:
```
OPENAI_API_KEY=your_api_key_here
```

### Application Execution
**Launch IntelliFlow Dashboard:**
```bash
streamlit run intelliflow_app.py
```
**Interacting with IntelliFlow:**

*   Access the web interface at the provided local URL
*   Input your queries in natural language
*   Review intent classification results
*   Follow guided prompts for parameter input
*   View action execution results

## System Architecture
User Query → Intent Classification → Action Discovery → Parameter Generation → User Input → Action Execution → Results

## Features

*   **Multi-stage AI Pipeline:** Comprehensive query processing from intent to execution
*   **Intelligent Classification:** Advanced GPT-4 powered message categorization
*   **Dynamic Action Mapping:** Flexible action discovery from configurable databases
*   **Interactive Parameter Collection:** User-friendly input validation and prompting
*   **Web-based Interface:** Modern Streamlit dashboard for seamless interaction
*   **API Integration:** Robust action execution through REST API calls

## Customization

*   **Action Database:** Modify JSON action files to add domain-specific actions
*   **Classification Categories:** Adjust intent categories in the classifier configuration
*   **API Endpoints:** Configure action executor for different API integrations
*   **UI Themes:** Customize Streamlit interface for branding requirements

## Best Practices

*   Ensure all configuration files are properly formatted and accessible
*   Handle API rate limits and implement appropriate error handling
*   Regularly update action databases to maintain system relevance
*   Monitor system performance and optimize for specific use cases

## Technical Requirements

*   Python 3.8+
*   OpenAI API access
*   Streamlit framework
*   Valid API endpoints for action execution
*   JSON configuration files for actions and parameters

## Important Note
**LLM Flexibility:** This system currently uses OpenAI's GPT models for intent classification. However, you can integrate any other Large Language Model (LLM) such as Anthropic Claude, Google Gemini, Hugging Face models, or open-source alternatives like Llama. Simply modify the LLM integration in the intent classifier component according to your chosen model's API requirements and authentication methods.


## Contributing
Contributions to IntelliFlow are welcome! Please follow standard coding practices and ensure comprehensive testing before submitting pull requests.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

**IntelliFlow - Transforming natural language queries into intelligent actions through AI-powered processing.**


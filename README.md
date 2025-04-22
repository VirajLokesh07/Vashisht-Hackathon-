# GLOBE TRAIL 🌍

An intelligent travel planning application that leverages AI to create personalized travel itineraries. The system combines multiple AI agents to provide comprehensive travel information, recommendations, and detailed itineraries based on user preferences.

## Project Resources 📁

- [Google Drive](https://drive.google.com/drive/u/5/folders/1YNQMqTiZr8UxolAbB_YtSxr3-ywAWzbQ)

## Features ✨

- **Personalized Travel Plans**: Generate custom itineraries based on user interests
- **Multi-Agent System**: Utilizes specialized AI agents for different aspects of travel planning
- **Comprehensive Information**: Covers accommodations, costs, visa requirements, attractions, and more
- **Interactive Web Interface**: Easy-to-use Streamlit-based user interface
- **Downloadable Reports**: Export travel plans in text format

## Installation 🚀

1. Clone the repository
2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Ensure Ollama is installed and running locally (required for LLM functionality)

## Usage 💡

1. Start the application:
   ```bash
   streamlit run main.py
   ```
2. Enter your travel details:
   - Origin city
   - Destination city
   - Travel dates
   - Personal interests
3. Click "Generate Travel Plan" to create your itinerary
4. Download the generated plan

## Core Libraries 📚

### Streamlit
- **Purpose**: Web application framework
- **Usage**: Creates the interactive user interface
- **Features**: Form inputs, progress indicators, markdown rendering

### CrewAI
- **Purpose**: Multi-agent orchestration framework
- **Usage**: Manages specialized AI agents and their tasks
- **Components**:
  - Agents: Location expert, guide expert, planner expert
  - Tasks: Information gathering, guide creation, plan compilation

### LangChain
- **Purpose**: Large Language Model (LLM) framework
- **Usage**: Handles AI model interactions and tool integration
- **Features**:
  - LLM integration (Ollama)
  - Web search capabilities
  - Tool management

### Additional Dependencies
- **langchain_ollama**: Integration with Ollama LLM
- **langchain_community**: Community tools and utilities
- **DuckDuckGo Search**: Web search functionality

## Project Structure 📁

- `main.py`: Application entry point and Streamlit interface
- `TravelAgents.py`: AI agent definitions and configurations
- `TravelTasks.py`: Task definitions for different planning aspects
- `TravelTools.py`: Custom tools for web searching and information gathering
- `requirements.txt`: Project dependencies

## System Requirements 🖥️

- Python 3.8+
- Ollama running locally
- Internet connection for web searches
- Sufficient RAM for LLM operations

## Features in Detail 🎯

### Location Expert Agent
- Researches travel logistics
- Provides visa information
- Analyzes costs and accommodations
- Checks weather and local events

### Guide Expert Agent
- Recommends attractions
- Suggests local cuisine
- Plans activities based on interests
- Provides cultural insights

### Planner Expert Agent
- Combines all information
- Creates structured itineraries
- Optimizes daily schedules
- Provides practical tips

## Contributing 🤝

Contributions are welcome! Please feel free to submit pull requests.

## License 📄

This project is open source and available under the MIT License.

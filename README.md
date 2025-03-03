# Multi-Agent Article Research and Writing System

A system that uses multiple AI agents (Planner, Writer, and Editor) to collaboratively research and write articles on any given topic.

## Features

- Multi-agent collaboration for content creation
- Interactive topic input through command line
- Environment-based configuration for API keys
- Comprehensive content planning, writing, and editing workflow

## Prerequisites

- Python 3.8 or higher
- Mistral AI API key

## Installation

1. Clone the repository:
```bash
git clone <https://github.com/Pranavharshans/CrewAI-MultiAgent.git>
cd CrewAI-MultiAgent
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  
```

3. Install the required packages:
```bash
pip install -r requirements.txt
```

4. Create a `.env` file in the project root and add your Mistral AI API credentials:
```
OPENAI_API_KEY=your-mistral-api-key
OPENAI_API_BASE=https://api.mistral.ai/v1
OPENAI_MODEL_NAME=mistral-small
```

## Usage

Run the article generation script:
```bash
multi-agents.py
```

When prompted, enter the topic you want to write about. The system will:
1. Plan the article structure and research approach
2. Write the initial content
3. Edit and refine the final article

The final article will be displayed in markdown format.

## System Components

### Agents

1. **Content Planner**
   - Plans article structure
   - Identifies target audience
   - Determines key points and SEO keywords

2. **Content Writer**
   - Crafts the initial article
   - Follows planner's outline
   - Incorporates SEO keywords
   - Maintains engaging structure

3. **Editor**
   - Reviews and refines content
   - Ensures journalistic best practices
   - Maintains balanced viewpoints
   - Polishes final output


```

## Configuration

The system uses environment variables for configuration. Required variables:
- `OPENAI_API_KEY`: Your Mistral AI API key
- `OPENAI_API_BASE`: Mistral AI API endpoint
- `OPENAI_MODEL_NAME`: Model to use (default: mistral-small)

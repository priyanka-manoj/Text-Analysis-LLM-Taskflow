
# TaskFlow Support Intelligence System

## Overview
Taskflow is a project management tool. With growing customer base and increase in volume of customer support tickets, manual triaging becomes time consuming. By using the Groq API, this project aims to build a system to automate triaging with the help of LLM and also provide first response to the ticket dynamically at scale.

## Tech Stack
- Python
- Groq API (LLaMA 3.3 70B)
- Pandas, Plotly
- Jupyter Notebook

## Prompting Approach
- All the prompts were structured using BRIDGE framework
- Prompts that need classifications uses Zero-shot technique with temperature set to 0.
- The prompt to generate first response uses One-shot technique with temperature set to 0.7 in order to sound more human-like.

## Key Features
- Automated ticket classification
- Sentiment analysis
- Priority and ETA assignment  
- AI-generated first responses
- Escalation flagging
- Interactive visualizations using Plotly

## Key Findings
- 74% of customers expressed negative or frustrated sentiment, indicating a significant customer experience crisis on this day
- By triaging, it was found that the core functionality was buggy leading to an escalation rate of 22%
- Lack of KB made customers reach out to support for How-to & Guidance
- The volume of Feature Requests suggests that customers needs are unmet

## How to Run
1. Clone the repository
2. Install dependencies: `pip install groq pandas plotly jupyter`
3. Add your Groq API key
4. Open `taskflow-support.ipynb` in Jupyter
5. Run all cells sequentially
  
## Dataset
TaskFlow is a fictional SaaS company created for this project. 
The dataset of 50 support tickets was synthesised with the help 
of Claude (Anthropic) to represent realistic day-to-day issues 
faced in SaaS support teams.

## API Key Setup
1. Create a free account at console.groq.com
2. Generate an API key
3. Replace `"your_api_key_here"` in the notebook with your key
4. Never commit your actual API key to GitHub

   ## Review Branch Update
Minor README update for PR testing.

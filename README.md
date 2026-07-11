# tripmate_agenticai_langgraph

## ✈️ TripMate AI — A Multi-Agent Travel Planner with LangGraph

## An open-source AI travel planner that turns a natural-language trip request into a practical travel plan with flight suggestions, hotel ideas, and a day-by-day itinerary. The project uses a multi-agent workflow built with LangGraph, LangChain, and FastAPI.

## Tech Stack
- **LangGraph**: A framework for building multi-agent workflows.
- **LangChain**: A framework for developing applications powered by language models.
- **FastAPI**: A modern web framework for building APIs with Python.
- Python 3.10+
- FastAPI
- Jinja2 + HTML/CSS/JavaScript frontend
- LangGraph
- LangChain
- Groq LLMs
- PostgreSQL
- Tavily API
- AviationStack API

# <u>Project structure </u>
.
├── app.py                # FastAPI app entry point
├── backend.py            # LangGraph travel workflow
├── requirements.txt      # Python dependencies
├── static/               # Static frontend assets
├── templates/            # HTML templates
└── tools/                # Flight and web search integrations

# Prerequisites
# Before running the project locally, make sure you have:

- Python 3.10 or newer installed
- PostgreSQL running and accessible
- API keys for:
- Groq
- Tavily
- AviationStack

# Environment Variables
## Create a .env file in the project root with the following variables:
DATABASE_URL=postgresql://user:password@localhost:5432/travel_db
GROQ_API_KEY=your_groq_api_key
AVIATIONSTACK_API_KEY=your_aviationstack_api_key
TAVILY_API_KEY=your_tavily_api_key
DEFAULT_ORIGIN_IATA=DAC

# Installation
python -m venv .venv
source .venv/bin/activate   # On Windows: .venv\Scripts\activate
pip install -r requirements.txt

# Running the App
## Start the FastAPI server: python app.py

## Then open your browser at: http://127.0.0.1:8000/

# API Endpoints
- GET /health - Health check
- POST /api/travel - Submit a travel request


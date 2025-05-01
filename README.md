# mcp-server

pip install uv

uv init 

# Create environment
uv venv

# Activate the environment
.venv\Scripts\activate

uv add "mcp[cli]"

## mcp inspector
uv run mcp dev server/weather.py

## install weather in Claude app
uv run mcp install server/weather.py

## client side 
uv add mcp-use
uv add langchain-groq
uv pip install fastembed
uv run server/client.py
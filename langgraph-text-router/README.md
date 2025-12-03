# LangGraph Text Router

A small but production-style AI workflow using LangGraph and a local LLM (via Ollama).
Automatically classifies a user request over arbitrary text into one of three tasks:

- Summarization

- Bullet-point extraction

- Sentiment analysis

Includes optional LangSmith integration for tracing & observability of the multi-node workflow.


## Example Interaction

Text Task Router Demo 
```bash
What would you like me to do?
> summarize

Paste your text:
> This product is excellent and I use it every day.

== ROUTED TASK ==

summarize

== RESULT == 
[Task: summarize]
The user likes the product and finds it useful daily...
```
LangSmith Tracing
```
export LANGCHAIN_TRACING_V2=true
export LANGSMITH_API_KEY="your_key_here"
export LANGSMITH_PROJECT="langgraph-text-router"
```

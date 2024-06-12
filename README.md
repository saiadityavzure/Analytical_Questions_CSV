



How the agents think:
![alt text](image.png)


commands used:
1. curl http://localhost:11434/api/ps => List models that are currently loaded into memory. (GET /api/ps)
2. curl http://localhost:11434/api/generate -d '{  "model": "llama3" }'




Problems faced while serving ollama:
1.  ollama serve Error: listen tcp 127.0.0.1:11434: bind: Only one usage of each socket address (protocol/network address/port) is normally permitted.
For this error follow this following step:
In order to close the "local" ollama go to the bottom right of taskbar on windows click the up arrow, and quit ollama from the small tiny ollama app icon in the small arrow key menu. SO CONFUSING>
If you then go back and run ollama serve it should work now.


Aritcles used for reference:
1. https://medium.com/@thallyscostalat/talk-to-your-data-using-langchain-csv-agents-and-amazon-bedrock-07ee3d35e9f7
2. https://anukriti-ranjan.medium.com/langchain-csv-agent-a-chain-of-function-calls-part-1-f0290e6c4bf3
3. https://github.com/ollama/ollama/blob/main/docs/api.md => for locally running the LLM and serving the LLM as OpenAI like API


Other important references used:
1. https://github.com/langchain-ai/langchain/blob/master/MIGRATE.md?ref=blog.langchain.dev
2. https://api.python.langchain.com/en/latest/chat_models/langchain_openai.chat_models.base.ChatOpenAI.html
3. https://github.com/langchain-ai/langchain/blob/master/MIGRATE.md?ref=blog.langchain.dev

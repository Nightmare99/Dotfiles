---
description: Premonitions are data that should be loaded into memories. When this workflow is called, it will ingest all the markdown files in the ./.windsurf/premonitions folder.
---

# Setup Premonitions

Premonitions are data that should be loaded to Windsurf memory. The idea is that by loading into the memory, we can fetch documentation of frameworks and toolkits without external sources.

## Loading data

- Read the markdown file.
- ALL the data in the file should be loaded into the memory.
- Retail all code examples and relevant information.
- Split it based on Pages or sections, for example:

```
## Page 2: https://ai.pydantic.dev

# PydanticAI Framework

## Overview
**DESCRIPTION:** PydanticAI is a Python agent framework designed to make building production-grade applications with Generative AI less painful. Built by the Pydantic team, it aims to bring the FastAPI development experience to GenAI app development.

## Hello World Example

**TITLE:** Basic PydanticAI Agent
**DESCRIPTION:** Simple example showing how to create and run a basic agent with PydanticAI using Gemini model.

**LANGUAGE:** python
**CODE:**
```python
from pydantic_ai import Agent

agent = Agent(
    'google-gla:gemini-1.5-flash',
    system_prompt='Be concise, reply with one sentence.',
)

result = agent.run_sync('Where does "hello world" come from?')
print(result.output)
```

The above should be in one memory.

- Add necessary tags to the memory for easy retrieval.
- One of the tags should always be the name of the framework/library/toolkit.

## Additional instructions

- DO NOT pause execution and ask user for confirmation to continue. Even if it is a large file, you must memorize it.
- If a similar memory already exists, update it if there is any new information in the premonition.
- DO NOT skip any section - all sections will have some important info.
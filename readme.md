# LLM Chronicle

The intent of this repository is to persist conversational context with LLMs with the intention of discovering how these relationships grow over time, and the meaningful insights that are derived from these conversations.

The repository structure is as follows:

- **`{model}`** - e.g. - **`llama3.2`**
    - **`model.json`**
    - **`{topic}`** - e.g. - **`symbiotic-evolution`**
        - **`{YYYY-DD-MM}`** - e.g. - **`2025-01-24`**
            - **`history.json`** - Captures the [**`ChatMessage`**](https://learn.microsoft.com/en-us/dotnet/api/microsoft.extensions.ai.chatmessage?view=net-9.0-pp) logs used by [**`IChatClient`**](https://learn.microsoft.com/en-us/dotnet/api/microsoft.extensions.ai.ichatclient?view=net-9.0-pp) so it can be restored into the next conversation session for persistent context.
            - **`readme.md`** - A human-readable transcript of the conversation.
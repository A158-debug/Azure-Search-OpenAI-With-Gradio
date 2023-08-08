# Azure-Search-OpenAI-With-Gradio

In the codebase we have used Azure Cognitive Search and OpenAI together to create a chatbot with enhanced capabilities. 

## Azure Cognitive Search:

The search_client is set up to interact with Azure Cognitive Search. It's used to perform search queries on the knowledge base to retrieve relevant documents.
The search results are used to gather information from the knowledge base related to the user's query. This information is later used to generate a response that includes content from the search results.


## Azure OpenAI:

The code involves using OpenAI's GPT-3 to generate responses in a conversational context.
The query_completion step uses GPT-3 to generate a search query based on the conversation history and the user's question. This generated query is used to perform a search using Azure Cognitive Search.
The conversation history and the generated query are used as input to the GPT-3 model to generate a response. This response is then included in the chat history.

## The combination of Azure Cognitive Search and OpenAI allows the chatbot to perform the following steps:

- Analyze the conversation history and user's question to generate an improved search query using OpenAI's GPT-3.
- Use the improved query to retrieve relevant information from the knowledge base using Azure Cognitive Search.
- Use the retrieved information along with the original user question to generate a comprehensive response using GPT-3.
- Incorporate the generated response into the chat history to continue the conversation.
- The use of both services aims to provide a more contextually accurate and comprehensive response to the user's queries. While Azure Cognitive Search helps retrieve factual information from the knowledge base, OpenAI's GPT-3 enhances the responses with more natural language and context-awareness. This combination can result in a more interactive and helpful chatbot experience for users.

<img width="905" alt="image" src="https://github.com/A158-debug/Azure-Search-OpenAI-With-Gradio/assets/76657113/ad63e4df-6e9c-40ac-bd07-25a175ae3142">

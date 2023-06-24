### Sprinklr AMA ChatBot Using Langchain

The aim of this intern project is to develop a goal-oriented knowledge-based chatbot designed to convince users, be it individuals or brands using the chatbot to buy Sprinklr products. The current Sprinklr chatbot is very limited and static.

### Challenges

1. **Goal infusion:** Integrating sales-oriented goals into the chatbot’s core functions without compromising user experience.
2. **Data identification and utilization**: Determining which data sources will be most effective for the chatbot’s knowledge base.
3. **Data extraction and indexing:** Efficiently extracting relevant data and indexing it for use by the chatbot.
4. **Handling hallucinations:** Ensuring accuracy in the chatbot’s responses by avoiding false or misleading information.
5. **Output coherency:** Maintaining consistency across similar queries, regardless of the chatbot's phrasing.
6. **Validation dataset:** Developing a dataset for validation purposes, given the lack of an existing database from prior queries.
7. **Auto-update and internet access:** Enabling the chatbot to access the internet and update its knowledge base autonomously.

### Understanding the Workflow

<img width="1478" alt="image" src="https://github.com/uttam112/sprinklr/assets/123285882/452fc37d-8f25-4914-991f-fe0ff810fdac">


### ✨ Options

| Embeddings | InstructorEmbeddings | SentenceTransformers | OpenAI |
| --- | --- | --- | --- |
| Vector Stores | FAISS | Chroma |  |

## Memory

- ConversationBufferMemory
- ConversationBufferWindowMemory
- ConversationTokenBufferMemory
- ConversationSummaryMemory

<aside>
📌 **Obstacles**

- One of the key features that we wanted to make sure to include that  is the ability to ask follow up questions. We believe this is very important for any chat based interface.
- If the question is not about Sprinklr, politely inform them that you are tuned to only answer questions about Sprinklr.
- Filtering out closely related vector embeddings, we can minimize redundancy in the vector store. Similar vectors often represent similar or overlapping concepts or entities. Removing redundant vectors helps optimize storage space and computational resources. There will also be diversity in the information retrieval process.
- We don’t have a validation dataset. We wan’t to have some numbers before giving it to the sales team for their validation.
</aside>

# Future Goals

- Preventing Hallucinations
- Deciding Evaluation Metrics
- Evaluation Based on Embeddings
- Evaluation Based on index stores
- Evaluation Based on final answer

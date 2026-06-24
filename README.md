## Getting Started

### Prerequisites

* Bun
* OpenAI API Key
* Pinecone API Key

### Install Dependencies

```bash
bun install
```

### Configure Environment Variables

Create a `.env` file and add:

```env
OPENAI_API_KEY=your_openai_api_key
PINECONE_API_KEY=your_pinecone_api_key
PINECONE_INDEX_NAME=your_index_name
```

### Index Documents

Run the document indexing pipeline to:

* Load PDF documents
* Split documents into chunks
* Generate vector embeddings
* Store embeddings in Pinecone

```bash
bun prepare.js
```

### Start Chatbot

Run the chatbot application:

```bash
bun chat.js
```

## Project Structure

```text
prepare.js   -> Document ingestion and indexing
rag.js       -> Retrieval-Augmented Generation logic
chat.js      -> Chat interface
cg-internal-docs.pdf -> Sample document
```


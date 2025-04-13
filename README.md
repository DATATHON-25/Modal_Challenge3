🧠💪 Fitness Bot – Your AI-Powered Health & Wellness Companion
Fitness Bot is an intelligent chatbot designed to assist users with real-time, personalized advice on fitness, health, and nutrition. Powered by a Retrieval-Augmented Generation (RAG) architecture and OpenAI’s pre-trained language model, it offers an engaging and informative chat experience built for real-world use.

🚀 Project Overview
Fitness Bot combines curated domain knowledge, semantic search, and LLM-generated responses to simulate a virtual health and fitness coach. From answering workout questions to clarifying diet plans, it acts as a 24/7 assistant that scales.

🧰 Tech Stack
Python
Lang Chain
Open AI API
Hugging Face Transformer
Flask
HTML, CSS, JS

🧠 Approach & Architecture
Knowledge Base Construction - Curated data from 3 diverse sources in the fitness, health, and nutrition domain.
Text Chunking - Text content is split into 500-token chunks for optimized semantic indexing.
Embedding Generation - Generated 384-dimensional embeddings using Hugging Face’s LLaMA Mini v6 model.
Vector Storage with Pinecone - Stored over 12,000+ embedding vectors in Pinecone, enabling high-speed semantic search.
RAG Pipeline with LangChain - Used cosine similarity to retrieve relevant chunks
Injected the retrieved context into a prompt to OpenAI’s GPT model - Returned context-aware, coherent responses via LangChain’s RAG chain
Chat UI - Built a clean, interactive interface which is easy to use.

📈 Features
🧠 Context-Aware Responses
Accurate, helpful answers generated by GPT based on retrieved context from your knowledge base.

🔍 Semantic Retrieval
Smart document selection using vector similarity instead of keyword matching.

🧩 Modular Design
Easily extendable with APIs, additional data sources, and user personalization logic.

🎨 UI/UX Design
Simple and responsive chat interface
Fitness-themed color palette
Timestamped message bubbles
Works across devices (desktop/tablet/mobile)

🌍 Real-World Relevance
🤖 Acts as a virtual health assistant
🏋️ Ideal for gyms, trainers, and wellness apps
📱 Easily integrated into existing health tech platforms
🔄 Ready for future features: goal tracking, user profiles, and habit suggestions

🔮 Future Enhancements
 Add authentication & chat history
 Personalized fitness & diet plans
 Integration with fitness wearables
 Voice support (Web Speech API)
 Robust and easily accessible frontend deployment

💻 How to Run Locally
Clone the Repository
git clone https://github.com/DATATHON-25/Modal_Challenge3.git

Install Dependencies using pip install -r requirements.txt

Set Up API Keys in .env File
PINECONE_API_KEY=your_pinecone_key
OPENAI_API_KEY=your_openai_key
Make Sure to save when you change

Run the following Commands:
python pinecone_index.py
After you run this make sure that yourvector database has embeddings stored in it

python app.py
Open on localhost

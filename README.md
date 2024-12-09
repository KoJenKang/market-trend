# Trends Marketplace Project
In this project, we leveraged the Retrieval-Augmented Generation (RAG) approach to build a chatbot for the Carlson School's website, using Gemini, a large language model developed by Google. This project showcases the benefits of RAG compared to traditional generative AI systems and explores its business applications.
 
# What is RAG?
RAG combines the power of retrieval-based methods with generative AI to provide more accurate, real-time responses by grounding outputs in external, validated data sources.

### RAG vs. Traditional Generative AI

| **Feature**            | **Traditional AI**                | **RAG**                                      |
|-------------------------|------------------------------------|---------------------------------------------|
| **Data Source**         | Static, pre-trained knowledge     | Dynamic, real-time retrieval                |
| **Accuracy**            | Prone to hallucinations           | Grounded and factually accurate             |
| **Update Frequency**    | Requires retraining for updates   | Instantly retrieves the latest information  |
| **Scalability**         | Limited without costly retraining | Easily scales with external data            |

## Benefits of RAG

| **Benefit**            | **Description**                                                                 |
|-------------------------|---------------------------------------------------------------------------------|
| **Improved Accuracy**   | Reduces hallucinations by grounding responses in real-time, validated data.    |
| **Access to Real-Time Data** | Retrieves the latest information instead of relying on static datasets.        |
| **Cost-Efficient**      | Avoids the need to retrain large models for new datasets.                      |
| **Scalability**         | Seamlessly integrates with extensive external knowledge bases.                 |

Business Applications
Customer Support Automation:
Deliver accurate, dynamic responses based on company manuals and FAQs.
Research and Analysis:
Retrieve insights from large repositories for data-driven decision-making.
Content Creation:
Build fact-based reports, articles, and summaries from validated sources.
Compliance and Legal Research:
Ensure adherence to regulations by referencing up-to-date legal documents.
Enterprise Knowledge Management:
Provide employees with quick, accurate answers from internal company documents.

# How we did this?

Set up a pipeline to fetch new data from the source website, convert it to vectors, and update the vector database regularly.


# Code & files
To run the code, upload the data files from a folder named "data" in the Colab environment and set up the necessary key.

This version currently includes only the undergraduate data. Graduate data will be added later this week.

At this stage, the Gemini embedding function successfully converts text into vectors and stores the vector data in ChromaDB. After testing several queries, the database returned reasonable chunks, and the LLM (Gemini) provided appropriate responses.

📌[Colab](https://colab.research.google.com/drive/1_TYG8saveyjD1yY4RKJRxZfFySosIW6Q#scrollTo=sP_iDUhPOd2k)

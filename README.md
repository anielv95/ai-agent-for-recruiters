# Description

This AI agent is intended to help recruiters to understand my profile and my working experience and to confirm if I'm a good candidate for the open positions they have.

# Technical Details

This AI Agent is going to have the capacity of answer questions about my profile and about my professional experience as an AI/ML engineer.

I'm going to build a RAG architecture and I'm going to connect a Large Language Model from OpenAI and finally I'm going to deploy the 
system using gradio for the first version and docker with AWS Elastic Beanstalk to deploy it in cloud for the second version. 
The third version is going to be a production ready version with extended cappabilities. It is thought to be used by million of users for which
we need Elastic Kubernetes Services, a relational database like Redshift and a noSQL database like MongoDB. We will have also S3 bucket and
AWS Load Balancer to distribute the requests and AWS CloudFront to reduce the load in the EKS containers.

## Next steps

1. Add the resume to index the data
2. Create the text search sytem using Elasticsearch
3. Create the evaluation pipeline to evaluate the quality of the retriever part of the RAG
4. Implement the vector database to encode the semantics of the multiple chunks
5. Evaluate the quality of the 3 retrievers:
    1. Text search
    2. Vector search
    3. Hybrid search
6. Create the prompt to build the answers of the questions
7. Implement MLflow or Opik to track the changes of the prompt
8. Create the workflow to evaluate the whole RAG system.
9. Deploy the app in gradio.

## Project structure

└── README.md # this file contains the description of the project and technical details

# Using Open-Source Ollama Model (llama3.1 ) with Langchain


## Purpose: The purpose of this notebook was to run and play with Meta's Llama 3.1 8b model using Ollama, langchain and langserve without incurring any costs :). Essentially to see what can be done for free! (I still have much more to play about with, but this is a start!)

## This tutorial is based on 2 notebooks:

 - (i) Ollama + Langchain official documentation (https://python.langchain.com/docs/integrations/chat/ollama/)

 - (ii) A medium tutorial by Abonia Sojasingarayar (https://medium.com/@abonia/ollama-and-langchain-run-llms-locally-900931914a46) which sets up Langserve 

 I have provided other links to useful articles and resources. 


### What is langchain?

- LangChain is a framework for developing applications powered by large language models (LLMs). It simplifies every stage of the LLM application lifecycle:

- Development: Build your applications using LangChain's open-source building blocks, components, and third-party integrations.


### What is Ollama?

- Ollama is an open-source project that serves as a powerful and user-friendly platform for running LLMs on your local machine. It acts as a bridge between the complexities of LLM technology and the desire for an accessible and customizable AI experience. 


#### Why use Ollama? 

- Cost-Effectiveness
- Data Privacy & Security 
- Customization & Flexibility 
- Offline Access & Reliability 
- Experimentation & Learning 

See link for more info on Ollama: 

- https://medium.com/@1kg/ollama-what-is-ollama-9f73f3eafa8b

- Ollama - https://ollama.com/



### What is Meta Llama3.1 8B model?

- This project uses Open-source Meta Llama3.1 8B parameters model in use with llangchain to (i) Test out some of the models capabilities to answer simple questions and (ii) To create a simple Langserve UI. 

See link for more info on how to run models with Ollama step-by-step 

- https://medium.com/@gabrielrodewald/running-models-with-ollama-step-by-step-60b6f6125807  




### What is Langserve?
 
#### LangServe: Simplifying Deployment

- LangServe is a Python framework that helps developers deploy LangChain. It uses FastAPI to provide an easy webserver setup with features such as streaming outputs, batch processing, automatic schema generation and support for multiplie concurrent requests. 

- It is an ideal solution for developers who want to streamline the deployment of language models and chains.


- LangServe is designed to streamline the process of deploying LangChain applications as RESTful APIs. It integrates with FastAPI and utilizes Pydantic for data validation, enabling developers to transform their LangChain runnables and chains into production-ready API servers efficiently. Key features of LangServe include:

- Automatic Schema Inference: Input and output schemas are inferred from your LangChain objects and enforced on every API call, ensuring robust data handling.

- Efficient Endpoints: Provides /invoke, /batch, and /stream endpoints to handle multiple concurrent requests effectively.

- Playground Interface: Offers a playground at /playground/ for experimenting with different configurations and settings.

- Built-in Tracing: Optional integration with LangSmith for tracing and monitoring purposes.
These features make LangServe a valuable tool for developers aiming to deploy their LangChain applications swiftly and reliably.



### What is Langsmith? (not used in here as of yet) 

#### LangSmith: Enhancing Development and Monitoring

- LangSmith focuses on the development, debugging, testing, evaluation, and monitoring of LLM applications. It provides a suite of tools to gain deeper insights into the behavior of language models, facilitating the improvement of application performance and reliability. Key functionalities of LangSmith include:

- Debugging: Allows developers to trace and understand the decision-making processes of AI models, aiding in identifying and resolving issues.

- Testing and Evaluation: Enables the creation of datasets and evaluators to assess model performance against various inputs and expected outputs.

- Monitoring: Offers real-time monitoring capabilities to track the performance and usage metrics of deployed models.

- By providing these tools, LangSmith assists developers in refining their LLM applications, ensuring they perform as intended in real-world scenarios



### What is the key difference between LangServe and LangSmith? 

- LangServe is primarily concerned with the deployment aspect, transforming LangChain applications into accessible APIs for end-users.

- LangSmith focuses on the development lifecycle, offering tools for debugging, testing, evaluating, and monitoring LLM applications to enhance their quality and performance.

- Together, LangServe and LangSmith provide a comprehensive framework for developing, deploying, and maintaining robust LLM applications within the LangChain ecosystem.

#### Additional concepts that are worth looking more into if you want to understand this notebook more:

- Restful API's
    - FastAPI
    - Uvicorn


- (iii) 
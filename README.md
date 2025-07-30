# Multi-Agent RAG Support System for Azure and AWS Users Using CrewAI

> This project simulates a technical support team powered by CrewAI agents and a Retrieval-Augmented Generation (RAG) workflow. The system answers user queries by consulting cloud documentation from Azure and AWS, delivering responses in a format that mimics a professionally written support email.

## Table of Contents
* [General Information](#general-information)
* [Architecture Overview](#architecture-overview)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)
* [Contact](#contact)



## General Information

- This project implements a multi-agent support workflow using CrewAI, an agent orchestration framework.
- The goal is to provide relevant, clear, and actionable steps in response to user queries related to either Azure or AWS cloud platforms.
- The system uses two key sources of documentation — one for Azure and one for AWS. The agents collectively decide which to use and how to respond.
- To enhance readability and user experience, the final response is presented in the format of a support email—without being sent externally.
- This agentic RAG setup is ideal for scalable, intelligent customer support, knowledge base retrieval, and internal IT helpdesk tools.



## Architecture Overview

The system consists of three specialized CrewAI agents:

1. Router Agent  
   Determines whether the user's query pertains to Azure or AWS and routes the task accordingly.

2. Support Agent 
   Searches the selected documentation source and drafts a response based on retrieved content.

3. Senior Support QA Agent  
   Validates the quality and completeness of the answer. Reviews the support agent’s draft answer, delegates it back for revisions if needed, and approves the final response to ensure accuracy and completeness.

Each agent operates in sequence, mimicking a real-life support escalation path.



## Conclusion

- The project demonstrates how CrewAI agents can collaborate to build an intelligent, role-driven support system.
- Agent specialization allows for a modular, interpretable process, where each step in the support pipeline is clearly defined and traceable.
- The RAG architecture ensures that answers are grounded in real documentation, reducing hallucination risks often associated with LLMs.
- Formatting the response like a support email enhances clarity and user experience, making the solution feel more personalized and enterprise-ready.



## Sample Output Screemshots

### Screenshot 1
<img width="880" height="788" alt="image" src="https://github.com/user-attachments/assets/bfcd2d9d-6a03-4978-91e1-ca444eb6c446" />

### Screenshot 2
<img width="892" height="711" alt="image" src="https://github.com/user-attachments/assets/fca02293-8afc-4eb5-8701-26f502b489b3" />



## Technologies Used

- crewai 0.28.8
- crewai_tools 0.1.6
- langchain_community 0.0.29
- openai gpt-3.5-turbo

## Contact
Anusha Chaudhuri [anusha761]

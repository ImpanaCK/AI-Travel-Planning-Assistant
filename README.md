# AI-Travel-Planning-System-using-LangGraph

## Project Overview

This project implements a multi-agent travel planning system using LangGraph and Large Language Models (LLMs). 

Instead of relying on a single AI agent, the system uses multiple specialized agents that collaborate to search flights, find hotels, build itineraries, and generate a final personalized travel plan based on user input.

## Tools & Technologies

- Python
- LangGraph
- LangChain
- Large Language Models (LLMs)
- APIs
- External Tools

## System Workflow

The system follows a multi-agent workflow where customer queries are routed to the appropriate specialized agent.

### 1. Query Understanding

The system receives and analyzes the customer's request to determine what type of assistance is required.

### 2. Agent Routing

The request is routed to the appropriate specialized agent based on the task.

### 3. Specialized Agents

Different agents handle different responsibilities, allowing the system to divide complex customer support tasks into smaller tasks.

### 4. Tools & APIs

Agents can interact with external tools and APIs when additional information or actions are required.

### 5. Memory & Context

The system maintains relevant conversation context so that responses can be generated based on previous interactions.

### 6. Response Generation

After the required tasks are completed, the system generates a final response for the customer.

## Key Features

- Multi-agent collaboration
- Intelligent agent routing
- Context-aware responses
- Conversation memory
- API and external tool integration
- Automated customer support workflow

## Project Architecture

```text
Customer Query
      |
      v
Query Understanding
      |
      v
Agent Router
      |
      +------------+------------+
      |            |            |
      v            v            v
   Agent 1      Agent 2      Agent 3
      |            |            |
      +------------+------------+
                   |
                   v
            Tools / APIs
                   |
                   v
             Final Response
```
## Conclusion

This project demonstrates how multiple AI agents can work together to build an automated and context-aware customer support system. The architecture allows different agents to specialize in specific tasks while LangGraph manages the overall workflow and agent coordination.

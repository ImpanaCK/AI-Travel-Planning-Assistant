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
The system follows a multi-agent workflow where a user's travel request is routed to the appropriate specialized agent.

### 1. Request Understanding
The system receives and analyzes the user's travel request to determine origin, destination, dates, and preferences.

### 2. Agent Routing
The request is routed to the appropriate specialized agent based on the task (flights, hotels, or itinerary).

### 3. Specialized Agents
Different agents handle different responsibilities — flight search, hotel search, and itinerary planning — allowing the system to divide complex trip planning into smaller tasks.

### 4. Tools & APIs
Agents interact with external tools and APIs (flight and hotel data providers) when additional information is required.

### 5. Memory & Context
The system maintains relevant conversation context so a full travel plan can be generated across multiple turns of the conversation.

### 6. Response Generation
After the required tasks are completed, the system generates a final, consolidated travel plan for the user.

## Key Features
- Multi-agent collaboration
- Intelligent agent routing
- Context-aware travel planning
- Conversation memory
- API and external tool integration
- Automated end-to-end trip planning workflow

## Project Architecture
```text
User Travel Request
      |
      v
Request Understanding
      |
      v
Agent Router
      |
      +----------------+----------------+
      |                |                |
      v                v                v
Flight Search    Hotel Search    Itinerary Planning
      |                |                |
      +----------------+----------------+
                        |
                        v
                 Tools / APIs
                        |
                        v
                Final Travel Plan
```
## Conclusion
This project demonstrates how multiple AI agents can work together to build an automated and context-aware travel planning system. The architecture allows different agents to specialize in specific tasks — flights, hotels, itinerary — while LangGraph manages the overall workflow and agent coordination.

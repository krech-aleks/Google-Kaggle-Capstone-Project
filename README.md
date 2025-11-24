# Google-Kaggle-Capstone-Project
Capstone Project Writeup
Track
Concierge Agents

Problem & Solution Pitch
Problem
People often waste time checking the weather and still feel unsure about what to wear - especially in a city like Tokyo, where conditions change quickly.

Solution
I will build a Tokyo Outfit Advisor Agent that automatically fetches the latest weather forecast and gives simple, clear clothing recommendations based on real-time conditions.

Agent Purpose
This agent provides real-time clothing advice for walks in Tokyo based on the latest weather conditions. It uses the Gemini 2.5 Flash-Lite model to interpret user queries, search for current weather information, and generate clear, practical recommendations.

Features Included (Required 3+, I have 4):
・ LLM-powered agent ✔️ The main reasoning and planning steps are performed by a Gemini-based agent.

・ Built-in Google Search Tool (Grounded Web Search) ✔️ The agent retrieves live weather information for Tokyo using the integrated search tool.

・ Session & Memory Support ✔️ Through InMemorySessionService, the agent remembers earlier messages within the same session, enabling natural follow-up interactions.

・ Observability Plugins (Invocation counter + logging) ✔️ A custom plugin tracks how many times the agent is invoked. Logging is enabled for visibility during execution.

How the Agent Works
The user asks how to dress for a walk in Tokyo. The agent performs a grounded web search to obtain the current weather forecast and then generates clear, concise clothing advice. If the user asks follow-up questions (e.g., what else to bring), the agent uses session memory to recall its previous recommendation and answer consistently.

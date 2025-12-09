***Agent From Scratch***

This notebook is me trying to build a simple LLM agent that can decide when to call a tool (a Python function) and use its result in the final answer.

What it does

Sends a question to an LLM (Kimi-K2-Thinking from Hugging Face)

Model decides if a tool is needed

Executes a function (like get_temperature())

Returns a combined final response

How it works (quick steps)

Install + login to Hugging Face

Create a tool (I used a temperature function )

Define the tool schema so the LLM knows how to call it

Build an Agent class that:

checks for tool calls

runs the function

sends results back to the model

**This is a VISUAL REPRESENTATION of the User - Agent interaction**

<img width="1124" height="315" alt="Screenshot 2025-12-09 at 2 15 51 PM" src="https://github.com/user-attachments/assets/d86133e9-9836-4cf0-b3df-6676fd41bd95" />

Example
agent("What is the temperature in Delhi?")


This is just the first version — planning to add more tools and implement smarter behavior later! 

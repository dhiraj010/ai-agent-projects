# Day 1 Summary: Agent Types and Rule-Based Agent
A review of AI agent types and my rule-based thermostat agent from Day 1, written to solidify my learning.

## Agent Types
AI agents are smart programs that make decisions. Here are the main types I learned:

- **Rule-Based Agents**: Use fixed rules (e.g., "if temperature < 20°C, turn on heater"). Simple but can't learn new things.
- **Learning-Based Agents**: Learn from data (e.g., predicting trends with PyTorch). Great for complex tasks.
- **Multi-Agent Systems**: Teams of agents that collaborate (e.g., AutoGen for coding or trading). Good for big projects.
- **Reflex Agents**: React to the current situation (e.g., a basic thermostat). Fast but no planning.
- **Goal-Based Agents**: Plan to achieve goals (e.g., save energy). Smarter but more complex.

**Why It Matters**: Knowing these types helps me pick the right agent for my projects. For example, my thermostat agent is rule-based, but I could make it learning-based later.

## My Rule-Based Thermostat Agent
I built a simple thermostat agent that controls temperature using rules.

**How It Works**:
- Takes the current temperature as input.
- Uses rules:
  - If temperature < 20°C, turn on the heater.
  - If temperature > 25°C, turn on the AC.
  - Otherwise, do nothing.
- Example: For 18°C, it says "Turn on heater."

**Code Example**:
```python
def thermostat(temperature):
    if temperature < 20:
        return "Turn on heater"
    elif temperature > 25:
        return "Turn on AC"
    else:
        return "Do nothing"

print(thermostat(18))  # Output: Turn on heater
print(thermostat(22))  # Output: Do nothing
print(thermostat(27))  # Output: Turn on AC 
```

## Other Day 1 Concepts
I learned several skills to support my AI agent projects:

- **Git**: Set up a GitHub repo (`ai-agent-projects-new`) to save my work. I learned to add, commit, and push files.
- **AI Libraries**: Installed PyTorch, TensorFlow, and scikit-learn. Ran a PyTorch example to predict a line (linear regression).
- **Agent Frameworks**: Researched LangChain (for data-connected agents), AutoGen (for multi-agent teams), and Hugging Face (for pre-trained models).
- **Advanced Python**: Learned list comprehensions (quick lists), decorators (add features to functions), and error handling (catch mistakes).

**Why It Matters**: These skills are building blocks for my AI projects. Git keeps my work safe, libraries and frameworks help build smart agents, and Python makes my code efficient.
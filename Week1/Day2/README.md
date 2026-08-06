# Week 1 - Day 2 : System Role & Temperature

## Objective

Learn how to control the behavior and creativity of a Large Language Model (LLM) using **System Roles** and the **Temperature** parameter.

---

## Topics Covered

- System Role
- User Prompt
- Temperature
- Prompt Engineering Basics
- Chat Completion API

---

## Technologies Used

- Python
- Groq API
- python-dotenv

---

## Project Structure

```
day2/
│── sys_temp.py
│── README.md
```

---

## Code Overview

The program performs the following steps:

1. Loads the Groq API key securely from the `.env` file.
2. Creates a Groq client.
3. Defines the LLM model (`llama-3.3-70b-versatile`).
4. Assigns a **System Role** to instruct the model to behave as an experienced clothing brand manager.
5. Sends a user prompt requesting clothing brand name suggestions.
6. Uses a **Temperature** value of `2` to encourage more creative and diverse responses.
7. Prints the generated response.

---

## Sample Prompt

```text
Suggest me a cloth brand name for my clothing business.
```

### System Role

```text
You are the brand manager of my clothing business and you are an expert in brand name generation.
```

---

## Concepts Learned

### System Role

The **System Role** defines the personality, expertise, and behavior of the LLM before it receives the user's prompt.

Example:

- Brand Manager
- Software Engineer
- Teacher
- Doctor
- Travel Guide

Changing the system role changes how the model responds.

---

### Temperature

The **Temperature** parameter controls the randomness and creativity of the generated response.

| Temperature | Behavior |
|-------------|----------|
| 0.0 | Highly deterministic and consistent |
| 0.2 - 0.5 | More focused and predictable |
| 0.7 - 1.0 | Balanced creativity |
| 1.5 - 2.0 | Highly creative and diverse responses |

In this project:

```python
temperature = 2
```

This encourages the model to generate more imaginative brand names.

---

## How to Run

Install the required packages:

```bash
pip install groq python-dotenv
```

Run the program:

```bash
python sys_temp.py
```

---

## Key Learnings

- Understand the difference between **System Role** and **User Prompt**.
- Learn how the **Temperature** parameter influences model creativity.
- Build structured conversations using the Chat Completion API.
- Improve response quality by providing clear system instructions.

---

## Next Step

In the next lesson, I'll continue exploring Prompt Engineering techniques to design more effective prompts and improve LLM responses.

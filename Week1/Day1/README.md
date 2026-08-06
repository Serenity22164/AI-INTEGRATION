# Week 1 - Day 1 : First LLM API Call

## Objective

Learn how to make the first API call to a Large Language Model (LLM) using the Groq API.

---

## Topics Covered

- Setting up the Groq Python SDK
- Loading API keys securely using a `.env` file
- Creating a Groq client
- Sending a prompt to an LLM
- Receiving and printing the model's response

---

## Technologies Used

- Python
- Groq API
- python-dotenv

---

## Project Structure

```
day1/
│── hello_llm.py
│── README.md
```

---

## Code Overview

The program performs the following steps:

1. Loads the Groq API key from the `.env` file.
2. Creates a Groq client.
3. Selects the `llama-3.3-70b-versatile` model.
4. Sends a user prompt to the model.
5. Receives and prints the generated response.

---

## Sample Prompt

```text
do you know Pratyush Narain?
```

---

## Concepts Learned

- Environment Variables
- Secure API Key Management
- LLM API Calling
- Chat Completion API
- Prompt Construction

---

## How to Run

Install the required packages:

```bash
pip install groq python-dotenv
```

Run the program:

```bash
python hello_llm.py
```

---

## Key Learning

This project demonstrates the complete workflow of interacting with a Large Language Model through an API, from securely loading credentials to sending prompts and processing responses.

---

## Next Step

Day 2 covers:

- System Role
- Temperature
- Controlling the behavior of an LLM

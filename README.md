# Task 8: Rule-Based Chatbot

## Overview
A simple rule-based chatbot built with Python using `if-elif-else` logic. This project demonstrates basic natural language processing (NLP) concepts through pattern matching.

## Features
- Responds to basic greetings and questions
- Handles user input with case insensitivity
- Simple exit command
- Clear, structured control flow

## Code Structure
```python
def chatbot():
    print("Bot: Hi! I'm a rule-based chatbot. Type 'bye' to exit.")
    
    while True:
        user_input = input("You: ").lower().strip()  # Handle input
        
        if user_input == "bye":
            print("Bot: Goodbye! 👋")
            break
        elif "hello" in user_input or "hi" in user_input:
            print("Bot: Hello there! 😊")
        elif "how are you" in user_input:
            print("Bot: I'm just a bot, but thanks for asking! 🤖")
        elif "your name" in user_input:
            print("Bot: I'm Task 8 Bot!")
        else:
            print("Bot: I didn't understand that. Try 'hello' or 'how are you'?")

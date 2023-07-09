# simple-chatbot-using-python-code-
A simple chatbot is a computer program designed to simulate conversation with human users. It uses predefined responses or simple rules to understand and generate appropriate replies based on user input.
import random


responses = {
    "hello": "Hello, how can I help you?",
    "how are you": "I'm good, thank you!",
    "what's your name?": "My name is ChatBot.",
    "bye": "Goodbye! Have a great day!",
    "how is the day":"great ! what about you",
    "how is the weather now":"it cool"
    
    
}

def generate_response(user_input):
    user_input = user_input.lower()
    
    
    if user_input in responses:
        return responses[user_input]
    else:
        return "I'm sorry, I don't understand."


while True:
    
    user_input = input("User: ")
    
    
    response = generate_response(user_input)
    
    
    print("ChatBot:", response)
    

    if user_input.lower() == "how is the weather now":
        break

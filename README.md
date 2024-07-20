def simple_chatbot(input_text):
    # Convert input to lowercase for case-insensitive matching
    input_text = input_text.lower()

    # Define some basic rules and responses
    if 'hello' in input_text:
        return "Hello! How can I help you today?"
    elif 'goodbye' in input_text:
        return "Goodbye! Have a great day."
    elif 'your name' in input_text:
        return "I am a chatbot created to assist you."
    elif 'how are you' in input_text:
        return "I'm just a bot, but thanks for asking!"
    else:
        return "Sorry, I don't understand that. Could you please rephrase?"

# Main loop to simulate a conversation
print("Welcome! Type 'exit' to end the conversation.")
while True:
    user_input = input("User: ")
    if user_input.lower() == 'exit':
        print("Chatbot: Goodbye!")
        break
    response = simple_chatbot(user_input)
    print("Chatbot:", response)

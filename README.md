# codsoft_01
# Define a function to handle user inputs and generate responses
def simple_chatbot(user_input):
    # Convert user input to lowercase for easier matching
    user_input = user_input.lower()

    # Define predefined rules and responses
    if "hello" in user_input:
        return "Hello! How can I assist you today?"
    elif "how are you" in user_input:
        return "I'm just a chatbot, but I'm here to help!"
    elif "what's your name" in user_input:
        return "I'm a simple chatbot."
    elif "bye" in user_input:
        return "Goodbye! Have a great day!"
    else:
        return "I'm sorry, I don't understand. Please ask another question."

# Main loop for the chatbot
while True:
    user_input = input("You: ")
    if user_input.lower() == "exit":
        print("Chatbot: Goodbye!")
        break
    response = simple_chatbot(user_input)
    print("Chatbot:", response)

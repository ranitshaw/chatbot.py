# chatbot.py
# a chatbot where just two commands works age and byy
def chatbot(user_input):
    # Use 'if' for the first condition, not 'elif'
    if "age" in user_input.lower():
        return "I am ageless! I am an AI."
    elif "bye" in user_input.lower():
        return "Goodbye! Have a great day!"
    else:
        return "I don't understand that yet, I am still learning!"

while True:
    user = input("You: ")
    if user.lower() == "quit":
        break
    response = chatbot(user)
    print("RanitBot:", response)

 TASK3-Basic-Chatbot
 def chatbot():
    print("Bot: Hey! I'm your Python buddy. Type 'bye' anytime to stop chatting.")

    while True:
        user = input("You: ").lower()

        if user in ["hi", "hello", "hey"]:
            print("Bot: Hey there! Need help with something?")
        elif user in ["how are you", "how are you doing"]:
            print("Bot: I'm just code, but I'm feeling great! How about you?")
        elif user in ["what's your name", "who are you"]:
            print("Bot: I’m just your simple chatbot friend.")
        elif user in ["what do you do", "what can you do"]:
            print("Bot: I chat with you and try to answer basic stuff.")
        elif user in ["who made you", "who built you"]:
            print("Bot: A Python programmer brought me to life!")
        elif user in ["time", "what time is it"]:
            from datetime import datetime
            time_now = datetime.now().strftime("%I:%M %p")
            print(f"Bot: It's {time_now} right now.")
        elif user in ["date", "what's the date"]:
            from datetime import date
            today = date.today().strftime("%A, %B %d, %Y")
            print(f"Bot: Today is {today}.")
        elif user in ["bye", "exit", "quit"]:
            print("Bot: See you later! Have a great day.")
            break
        else:
            print("Bot: Hmm, I didn't get that. Try something else!")

chatbot()

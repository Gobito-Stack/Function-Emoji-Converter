# Function-Emoji-Converter
def emoji_converter(message):
    emoji = {
        ":)" : "😊",
        ":(" : "🥲"
    }
    messages = ""
    words = message.split(" ")
    for word in words:
        messages += emoji.get(word, word) + " "
    return messages
    


message = input("> ")
result = emoji_converter(message)
print(result)
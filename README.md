# FakeNewsHeadlineGenerarator

#1 - import the random module
import random

#2 - create subjects list
subjects = [
    "chirag paswan",
    "sharukh khan",
    "Virat kohli",
    "tamna bhatiya",
    "nirmala sita raman",
    "sarda kapur",
    "aaliya bhutt",
    "Prime minister Modi",
    "car driver from Bihar"
]

actions = [
    "lunches",
    "cancels",
    "dances with",
    "eats",
    "declares war on",
    "orders",
    "celebrates"
]

places_or_thinks = [
    "at red fort",
    "in Mumbai Local Train",
    "a plate of samosa",
    "inside parliament",
    "at Ganga Ghat",
    "during IPL Match",
    "at India Gate"
]

#3 - start the headline generation loop
while True:
    subject = random.choice(subjects)
    action = random.choice(actions)
    place_or_think = random.choice(places_or_thinks)

    headline = f"BREAKING NEWS: {subject} {action} {place_or_think}"
    print("\n" + headline)

    user_input = input("\nDo you want another headline? (yes/no): ").strip().lower()
    if user_input == "no":
        break

#print Goodbye message
print("\nThanks for using the Fake News Headline Generator. Have a fun day!")

# 1. import the random module

import random

# 2. create the subject

subject= [
    "Virat Kohli",
    "Shahruk Khan",
    "Salman Khan",
    "Nirmala Sitharaman",
    "A Mumbai Cat",
    "A Group of Monkeys",
    "A Prime Minister Narendra Modi",
    "Auto Rikshaw Driver from Delhi"
]

action = [
    "Launches",
    "Cancels",
    "Dance With",
    "Eat",
    "Party With",
    "Declare War",
    "Orders",
    "Celebration",
]

place_or_thing = [
    "at Red Fort",
    "in Mumbai local Train",
    "a Plate of Samosa",
    "inside parliment",
    "During IPL match",
    "at Film city",
    "at india gate",
    "on trees",
]

# 3. start the headline genration loop

while True:
    sub = random.choice(subject)
    act = random.choice(action)
    pla_or_thi = random.choice(place_or_thing)

    headline = f" BREAKING NEWS : {sub} {act} {pla_or_thi}"
    print("\n" + headline)

    user_input = input("\n Do you waant another headline?(yes/no)").strip().lower()
    if user_input == "no":
        break

#print thank you massage
print("Thank You For Using A Fake Headline Generator.Have a Fun Day")

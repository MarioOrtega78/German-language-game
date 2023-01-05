# German-language-game
Small game that tests knowledge of the German language
print("Welcome to the German language game")

x = input("Do you want to participate? \n Please 'y' for Yes or 'n' for No. ")
score = 0

if x.lower() == "y":
    print("Okay, let's go.")
    question_1 = input("What does 'Entschuldigung' stand for? ")
    if question_1.lower() == "sorry" or "excuse me":
        score += 1
        print("That is correct")
    else:
        print("Incorrect")

    question_2 = input("What does 'Ewigkeit' stand for? ")
    if question_2.lower() == "eternity":
        score += 1
        print("That is correct")
    else:
        print("Incorrect")

    question_3 = input("What does 'Beschreibung' stand for? ")
    if question_3.lower() == "description":
        score += 1
        print("That is correct")
    else:
        print("Incorrect")

    print("Your score was " + str(score) + "/3.")
    print("You achieved " + str(((score/3)*100)) + "% success.")

elif x.lower() == "n":
    print("No problem, see you later.")

else:
    print("That's not a valid response.")

print("That's the end of the game.")

# Chrismas-Guessing-Game-Using-Python

print("Welcome Onboard")
user = input("Enter yes to proceed: ")

game_details = """
Instructions:
1. This game is titled 'Guessing Game'.
2. This game has three phases, and each phase earns you two points.
3. You have at least two attempts for each phase.
"""
print(game_details)

user_name = input("Enter a User name to proceed: ")

# First phase of the game
first_phase = "What is Christmas truly all about?"
print(first_phase)

answer = "It's all about Jesus Christ being the reason for the season!"
hint = "It's all about Jesus Christ being "
print(hint)

# Initialize attempt counter
attempt = 0
max_attempts = 2
correct_answer = False

while attempt < max_attempts and not correct_answer:
    user_input = input("Enter your answer: ")
    final_answer = hint + user_input
    print(final_answer)

    # Compare answers in a case-insensitive manner
    if final_answer.strip().lower() == answer.lower():
        print("You passed this phase and earned 2 points!")
        correct_answer = True
    else:
        print("Try one last time")

    attempt += 1  # Increment the attempt counter

# If attempts are exhausted, print failure message
if not correct_answer:
    print("You have failed the first phase.")

#phase 2
phase_two = " where was jesus placed after he was born "
answer = "Manger"
print(phase_two)
#Attempt
attempt = 0
max_attempt = 2
correct_answer = False

while attempt < max_attempt and not correct_answer:
    user_input = input("Enter your answer ")
    final_answer = user_input

    #printing the user_input stored in the final answer
    print(final_answer)

    # comparing answers
    if final_answer.lower() == answer.lower():
        print("congrats you have earn two more point ")
        correct_answer = True
    else:
        print ("try again one more time ")

        attempt += 1

        if not correct_answer:
            print("you have failed this phase")


#phase 3
phase_three = " what are the three gift jesus got after his birth "
answer = "gold, frankincense and myrrh"
#print the question
print(phase_three)
#Clue
hint = " gold"
print(hint)

#User's Attept
attempt = 0
max_attempt = 2
correct_answer = False

# Looping
while attempt < max_attempt and not correct_answer:
    user_input = input("enter your answer: ")
    # concatenating user_input and hint
    final_answer = hint + user_input
    #comparing
    if final_answer.strip().lower() == answer.lower():
        print("congrats you have earn 2 more point! ")
        correct_answer = True
    else:
        print("try one more time ")

        attempt += 1

        if not correct_answer:
            print("you have failed this phase! ")

            remark = "Thank you for solving all questions. "
            print(remark)


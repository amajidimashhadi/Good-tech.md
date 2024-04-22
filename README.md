# Good-tech.md
a quiz for techs 
class Question:
    def __init__(self, prompt, answer):
        self.prompt = prompt
        self.answer = answer

# Define a list of questions
questions = [
    Question("how much air should be in a tire of fire truch?\n(a) 100psi\n(b) 200psi\n(c) 130psi\n", "c"),
    Question("when do you need to replace brakes on medunits?\n(a) when at 3mm\n(b) when metal to metal\n(c) never\n", "a"),
    Question("when is PM due for frie equipment'?\n(a) 6months\n(b) 3 months\n(c) non of the above\n", "a")
]

# Define a function to run the quiz
def run_quiz(questions):
    score = 0
    for question in questions:
        answer = input(question.prompt)
        if answer == question.answer:
            score += 1
    print("You got " + str(score) + "/" + str(len(questions)) + " correct")

# Call the function to run the quiz
run_quiz(questions)


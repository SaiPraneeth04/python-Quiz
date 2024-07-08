# python-Quiz

## Aim:
To create a quiz using python applications.

## Apparatus:
1. python 3.7 installation,
2. Windows 10 or above.

## Algorithm:
Step 1: Set Up Your Environment.
Step 2: Plan Your Quiz.
Step 3: Create a List of Questions.
Step 4: Write the Code.
Step 5: Write the Code.
Step 6: Run the code. Get the output.
Step 7: End the program.

## Program:
```
import random
#Question to be asked
quiz_data = [
    {
        "question": "What does HTML stand for?",
        "options": ["A. Hyperlink Text Markup Language", "B. Hyper Transfer Markup Language", "C. Hypertext Markup Language", "D. High-Level Text Markup Language"],
        "answer": "C"
    },
    {
        "question": "Which programming language is often used for web development?",
        "options": ["A. Python", "B. Java", "C. Ruby", "D. JavaScript"],
        "answer": "D"
    },
    {
        "question": "What is the primary function of CSS in web development?",
        "options": ["A. Data storage", "B. Styling and layout", "C. Server-side scripting", "D. Database management"],
        "answer": "B"
    },
    {
        "question": "What does the acronym SQL stand for?",
        "options": ["A. Structured Query Language", "B. Simple Query Language", "C. Standard Query Language", "D. Sequential Query Language"],
        "answer": "A"
    },
    {
        "question": "What is the output of the following code: `print(3 * 'Hello ')`?",
        "options": ["A. Hello Hello Hello Hello", "B. 9", "C. Hello Hello Hello", "D. Syntax Error"],
        "answer": "C"
    },
    {
        "question": "Which programming language is often used for data analysis and scientific computing?",
        "options": ["A. JavaScript", "B. Java", "C. Python", "D. C++"],
        "answer": "C"
    }
    
]
def ask_question(question_data):
    print(question_data["question"])
    for option in question_data["options"]:
        print(option)
    user_answer = input("Enter your answer (A,B,C,D): ").upper()
    if user_answer == question_data["answer"]:
        return True
    else:
        return False
#main body
if __name__=="__main__":
    score=0
    random.shuffle(quiz_data)
    for i in range(1,6):
        print(f'Question {i} of 5')
        if ask_question(quiz_data[i]):
            print("Correct\n")
            score += 1
        else:
            print(f"Wrong! The correct answer is {quiz_data[i]['answer']}.\n")

    print(f"You scored {score}/5.")
```
## Output:
![Screenshot 2024-07-08 133758](https://github.com/SaiPraneeth04/python-Quiz/assets/119390353/a962fd92-09d0-4dae-a396-172c7b43621e)

## Result:
Thus the project to create a quiz using python is successfully created.

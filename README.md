print("==============================")
print("        PYTHON TUTORIAL")
print("==============================")

choice = ""

while choice != "0":
    print()
    print("===== MAIN MENU =====")
    print("1. Lesson 1 - Introduction to Python")
    print("2. Lesson 2 - Print, Variables, Data Types, Input")
    print("3. Lesson 3 - Operators and If Statements")
    print("4. Practice Questions")
    print("0. End the program")
    choice = input("Choose: ")

    # ---------------- LESSON 1 ----------------
    if choice == "1":
        print()
        print("--- Lesson 1: Introduction to Python ---")
        print("A programming language is a language computers understand.")
        print("Python is easy to read and easy to learn.")
        print("Why learn Python?")
        print("1. Simple and easy to learn")
        print("2. Readable, almost like English")
        print("3. Used in AI, web, games, and automation")
        print("4. Huge community")
        print("Editors you can use: PyCharm, VS Code, Jupyter Notebook")
        print("Hello, World!")

    # ---------------- LESSON 2 ----------------
    elif choice == "2":
        print()
        print("--- Lesson 2: Print and Comments ---")
        # This is a comment. Python ignores it.
        print("Hello, World!")     # text needs quotes
        print(100)                 # numbers do not need quotes
        print(25.5)

        print()
        print("--- Lesson 2: Variables ---")
        name = "John"
        age = 20
        print(name)
        print(age)
        print(name, age)           # a comma prints many things at once

        print()
        print("--- Lesson 2: Data Types ---")
        my_text = "Maria"          # str (text)
        my_whole = 20              # int (whole number)
        my_decimal = 89.5          # float (decimal number)
        my_truth = True            # bool (True or False)
        print(my_text, type(my_text))
        print(my_whole, type(my_whole))
        print(my_decimal, type(my_decimal))
        print(my_truth, type(my_truth))

        print()
        print("--- Lesson 2: User Input ---")
        name = input("Enter your name: ")
        age = int(input("Enter your age: "))          # int() = whole number
        grade = float(input("Enter your grade: "))    # float() = decimal
        print("Name:", name)
        print("Age:", age)
        print(f"Student: {name}, Age: {age}, Final Grade: {grade}")

    # ---------------- LESSON 3 ----------------
    elif choice == "3":
        print()
        print("--- Lesson 3: Arithmetic Operators ---")
        a = 10
        b = 5
        print("a =", a)
        print("b =", b)
        print("Addition:", a + b)
        print("Subtraction:", a - b)
        print("Multiplication:", a * b)
        print("Division:", a / b)
        print("Floor Division:", a // b)
        print("Modulus:", a % b)
        print("Exponentiation:", a ** b)

        print()
        print("--- Lesson 3: Comparing Values ---")
        a = 10
        b = 5
        print("a =", a)
        print("b =", b)
        print("a == b :", a == b)   # equal to
        print("a != b :", a != b)   # not equal to
        print("a > b  :", a > b)    # greater than
        print("a < b  :", a < b)    # less than
        print("a >= b :", a >= b)   # greater than or equal to
        print("a <= b :", a <= b)   # less than or equal to

        print()
        print("--- Lesson 3: if, if-else, if-elif-else ---")
        age = 20
        print("age =", age)
        if age >= 18:
            print("You are an adult.")

        score = 65
        print("score =", score)
        if score >= 75:
            print("Passed")
        else:
            print("Failed")

        score = 85
        print("score =", score)
        if score >= 90:
            print("Excellent")
        elif score >= 80:
            print("Very Good")
        elif score >= 75:
            print("Passed")
        else:
            print("Failed")

    # ---------------- PRACTICE QUESTIONS ----------------
    elif choice == "4":
        print()
        print("--- Practice Questions ---")
        print("Tip: write each code in your editor and run it to find the answer!")
        print("You get 2 tries for every question.")

        # Question 1
        print()
        print("Question 1: What does print(17 // 3) show?")
        tries = 0
        while tries < 2:
            answer = input("Your answer: ")
            if answer.strip() == "5":
                print("Thats Correct Wonderful")
                break
            tries = tries + 1
            if tries == 1:
                print("ohh thats incorrect try again!")
            else:
                print("ohh thats incorrect. The correct answer is 5.")

        # Question 2
        print()
        print("Question 2: What does print(10 % 3) show?")
        tries = 0
        while tries < 2:
            answer = input("Your answer: ")
            if answer.strip() == "1":
                print("Thats Correct Wonderful")
                break
            tries = tries + 1
            if tries == 1:
                print("ohh thats incorrect try again!")
            else:
                print("ohh thats incorrect. The correct answer is 1.")

        # Question 3
        print()
        print("Question 3: What does print(2 ** 3) show?")
        tries = 0
        while tries < 2:
            answer = input("Your answer: ")
            if answer.strip() == "8":
                print("Thats Correct Wonderful")
                break
            tries = tries + 1
            if tries == 1:
                print("ohh thats incorrect try again!")
            else:
                print("ohh thats incorrect. The correct answer is 8.")

        # Question 4
        print()
        print("Question 4: What does print(15 / 3) show?")
        tries = 0
        while tries < 2:
            answer = input("Your answer: ")
            if answer.strip() == "5.0":
                print("Thats Correct Wonderful")
                break
            tries = tries + 1
            if tries == 1:
                print("ohh thats incorrect try again!")
            else:
                print("ohh thats incorrect. The correct answer is 5.0.")

        # Question 5
        print()
        print("Question 5: score = 85. What does print(score >= 90) show?")
        tries = 0
        while tries < 2:
            answer = input("Your answer (True or False): ")
            if answer.strip().lower() == "false":
                print("Thats Correct Wonderful")
                break
            tries = tries + 1
            if tries == 1:
                print("ohh thats incorrect try again!")
            else:
                print("ohh thats incorrect. The correct answer is False.")

        # Question 6
        print()
        print("Question 6: score = 65. Does the code below print Passed or Failed?")
        print("    if score >= 75:")
        print("        print(\"Passed\")")
        print("    else:")
        print("        print(\"Failed\")")
        tries = 0
        while tries < 2:
            answer = input("Your answer (Passed or Failed): ")
            if answer.strip().lower() == "failed":
                print("Thats Correct Wonderful")
                break
            tries = tries + 1
            if tries == 1:
                print("ohh thats incorrect try again!")
            else:
                print("ohh thats incorrect. The correct answer is Failed.")

        # Question 7
        print()
        print("Question 7: What data type is 25.5? (int, float, str, or bool)")
        tries = 0
        while tries < 2:
            answer = input("Your answer: ")
            if answer.strip().lower() == "float":
                print("Thats Correct Wonderful")
                break
            tries = tries + 1
            if tries == 1:
                print("ohh thats incorrect try again!")
            else:
                print("ohh thats incorrect. The correct answer is float.")

        print()
        print("You finished the practice questions!")

    # ---------------- END ----------------
    elif choice == "0":
        print("Goodbye! Happy coding!")

    else:
        print("Please type 1, 2, 3, 4, or 0.")

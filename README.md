Q1 = """ 1. The common name for the crime of stealing passwords is _______
A. spooling.B. identity theft.C. spoofing.D. hacking"""
Q2 = """2. If you want to secure a message, use a(n) ________
A. cryptology source.B. encryption key.C. encryption key.D. cryptosystem."""
Q3 =  """3. Which of the following software monitors and records computer transactions?
A. cryptology source.B. encryption key.C. audit controlD. cryptosystem."""
Q4 = """4. The scrambling of code is known as _______
A. encryption.B. firewalling.C. scramblingD. password-proofing"""

Name = input("Enter you Name :")
print()
print("Welcome to Quiz World: ",Name)
print()
question = {Q1 : "C", Q2 : "D", Q3 : "C", Q4 : "A"}
Score = 0
print("Your Question are : ")
for i in question:
    print()
    print(i)
    flag1 = input("You Want to Skip the Questions: Yes/No: ")
    if flag1 == "Yes":
        continue
    Your_Answer = input("Enter Your Choice : A/B/C/D:")
    print()
    if Your_Answer == question[i]:
        print("Yeah !! Your Answer is Correct",Your_Answer," and You Got 1 Point")
        Score = Score+1
        print("Your Score is :",Score)
        print()
    else:
        print("Ohh !! Your Answer is Wrong",Your_Answer," and You Lost 1 Point")
        Score = Score -1
        print("Your Score is :",Score)
        print()
        flag1 = input("You Want to Quit the Quiz: Yes/No: ")
        if flag1 == "Yes":
            break
print("Your Total Score :",Score)

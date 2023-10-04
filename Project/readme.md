# Crypto Wallet

![](22ROOSE-master768.gif)  
<sub>Illustration for Glenn Harvey</sub>

# Criteria A: Planning

## Problem definition

Ms. Sato is a local trader who is interested in the emerging market of cryptocurrencies. She has started to buy and sell electronic currencies, however at the moment she is tracking all his transaction using a ledger in a spreadsheet which is starting to become burdensome and too disorganized. It is also difficult for Ms Sato to find past transactions or important statistics about the currency. Ms Sato is in need of a digital ledger that helps her track the amount of the cryptocurrency, the transactions, along with useful statistics. 

An example of the data stored is 

| Date | Description | Category | Amount  |
|------|-------------|----------|---------|
| Sep 23 2022 | bought a house | Expenses | 10 BTC |
| Sep 24 2022 | food for house celebration | Food | 0.000001 BTC |


## Proposed Solution

Design statement:
I will to design and make a **Electric Ledger/Crypto Wallet** for a client, Ms.Sato who is a local trader intersed in  the emerging market of cryptocurrencies. The project will be about **helping her get information such as history of the coin and rate, track the amount of the cryptocurrency,the transactions, and get useful statics** and is constructed using the software **Python 3.10.7**. It will take **3 weeks** to make and will be evaluated according to the criteria shown below.

The digital coin used will be **Zcash**. Zcash was invented by a group of scientists and brought to life by Electric Coin Co. and Zooko Wilcox, a computer security specialist and original cypherpunk. The orign of Zcash is Zerocoin which is **the solution for the Bitcoin's biggest problem, safty**.
The Zerocoin Electric Coin Company (now Electric Coin Co.) was formed in 2015 to create the protocol, and Zcash was launched in October 2016. The Zcash Foundation was formed in 2017 to further support Zcash, and in 2020, the Zcash Major Grants organization launched to help fund additional developers and community projects.("WHO CREATED ZCASH?",https://z.cash/learn/who-created-zcash/)

## Justify the tools/structure of your solution
The biggest strength of Zcash is **the safty** of the coin suported by the concept of "zero-knowledge proof.". As I mentioned, the purpose of the coin is to solve the security problem. Moreover, as zcash is a decentralized virtual currency with **no central manager**,even if in the event of hacking damage, it is to recover from other networks and minimaize the damage. Therefore Zcash provids her completely safty experiecne to learn cryptocurrency.

I will use the software **Python3** to program my digital ledger. Python 3 is a top choice due to its simplicity, versatility, and robust features. First and foremost, Python's easy-to-read syntax allows for the development of complex systems with fewer lines of code, making the codebase clean and manageable. Additionally, Python's object-oriented programming (OOP) capabilities allow developers to create organized and modular code structures, making it easier to manage different aspects of the system, such as user authentication, transaction processing, and account management. Python's flexibility also allows seamless integration with databases, enabling efficient storage and retrieval of customer information and transaction history.

## Success Criteria
1. The electronic ledger is a text-based software (Runs in the Terminal).
2. The electronic ledger display the basic description of the cyrptocurrency selected.
3. The electronic ledger allows to enter, withdraw and record transactions.
4. This software hds sign in system.
5. The software shows exchange in yen.
6. The software shows the history of the transaction.

## Test Plan

| Description                        | Type of test   | Inputs                                                                                                                                                                                                                                                      | Outputs                                                                                                                                     |
|------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------|
| Sign up & menu                     | Unit test      | 1. Run the project1.py 2. Input "ayane" as name and "0405" as Password                                                                                                                                                                                      | Print welcome and menu on the screen and the name and password are stored in the database.csv.                                              |
| Log in & menu                      | Unit test      | 1. Run the project1.py 2. Input "ayane" as name and "0405" as Password                                                                                                                                                                                      | Print welcome and menu on the screen and the name and password are stored in the database.csv                                               |
| Basic description of Zcash         | Unit test      | 1. User inputs in "1" into prompt following the menu                                                                                                                                                                                                        | Print the basic description of Zcash                                                                                                        |
| Enter deposit                      | Unit test      | 1. User inputs in "2" into prompt following the menu 2. User inputs the amount of the Zcash user wants to deposit                                                                                                                                           | Print saved The date of trnsaction is written on savedcoin.csv                                                                              |
| Enter withdraw                     | unit test      | 1. User inputs in "3" into prompt following the menu 2. User inputs the amount of the Zcash user wants to withdraw.                                                                                                                                         | Print withdrawn If the amount is more than user's balance, print error The date of transaction is written on savedcoin.csv                  |
| View the balance                   | unit test      | 1. User inputs in "3" into prompt following the menu.                                                                                                                                                                                                       | Print the baance of the wallet from savedcoin.csv                                                                                           |
| Exchange                           | unit test      | 1. User inputs in "4" into prompt following the menu 2. User inputs the rate of Zcash in doll from the shown site on the screen. 3. User choses which money user wants to exchange. 4. User inputs the rate of the money from the shown site on the screen. | Show the site of the rate of Zcash to doll. Show the site of the rate of the money user chose. print the balance with the money user chose  |
| View past track of the transaction | unit test      | 1. User inputs in "5" into prompt following the menu.                                                                                                                                                                                                       | print the past track of the transaction                                                                                                     |
| Number input validation            | usability test | 1. User inputs invalid characters into the prompt when asked to put in number.                                                                                                                                                                              | print Error the input prompts user to input again.                                                                                          |
| Wrong name/password counter        | usability test | 1. User inputs wrong name/password when logging in.                                                                                                                                                                                                         | print Error prompts user to retry logging in. When the attempts is more than 3, user can't retry.                                           |
| Same name countre                  | usablity test  | 1. User tries to sign up with same name.                                                                                                                                                                                                                    | print Error prompts user to enter another name.                                                                                             |

# Criteria B: Design

## System Diagram
![System diagram of this program](https://github.com/ayyyane/unit1-2024/assets/142702159/c45003e6-c05c-4ae6-80c3-1c8d7b3bcf44)
**Fig.1 System diagram of this program**

## Flow Diagrams

## Record of Tasks
| Task No | Planned Action                          | Planned Outcome                                                                          | Time estimate | Target completion date | Criterion |
|---------|-----------------------------------------|------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Create system diagram                   | To have a clear idea of the hardware and software requirements for the proposed solution | 10min         | Sep 13                 | B         |
| 2       | Create flow diagram for login function  | A flow diagram and the code tested                                                       | 30min         | Sep 15                 | B,C       |
| 3       | Discuss with Client on Success Criteria | To have an understanding of what the client is expecting from the program                | 10min         | Sep 15                 | A         |
| 4       | code the Login system, Sign in system   | To protect the information from others                                                   | 1hr           | Sep 18                 | C         |
| 5       | Code the Menu                           | To have an items and title shown on the screen                                           | 30min         | Sep 20                 | C         |
| 6       | Code Main Functions                     | A function base of the program                                                           | 5hr           | Oct 1                  | C         |
| 7       | Form Test Plan                          | To have a flexible test                                                                  | 1.5hrs        | Oct 2                  | B         |
| 8       | Draw Flow Diagrams                      | To explain the login of the code cleary                                                  | 2hrs          | Oct 4                  | B         |
| 9       |  Testing followed Test Plan             | To allow other coders to understand the system                                           | 20min         | Oct 4                  | B         |


# Criteria C: Development
## Techiques Used:

1. Functions
2. For/While loops
3. If/then/else statements
4. List Comprehinsion
5. Import csv,datetime

## Login System
```.py
def login():
    attempts = 3
    output = False
    name = input("Enter your name")
    password = input("enter your password")

    with open("database.csv","r") as f:
        database = f.readlines()

    for line in database:
        user_pass = line.strip().split(",")
        if name == user_pass[0] and password == user_pass[1]:
            output = True
            print(f"welcome,{name}")
            break

    while output == False and attempts > 0:
        name = input("Error please enter your username again")
        password = input("Error please enter your password again")
        attempts -= 1
        for line in database:
            user_pass = line.strip().split(",")
            if name == user_pass[0] and password == user_pass[1]:
                output = True
                print(f"welcome,{name}")
                break

        if attempts == 0:
            print("You are not authorized. Existing")
            exit(1)
```

At first, I defined a function caleed login,this function has two inputs. It begins by initializing the number of login attempts allowed (attempts = 3) and a flag output to track the authentication status. The user is prompted to input their name and password. The code then reads user data from a file named "database.csv". Each line in the file is split into a list, with the first element representing the username and the second element representing the password.

The code first attempts to match the entered username and password with the data in the "database.csv". If a match is found, the output flag is set to True, indicating a successful login. The program prints a welcome message and exits the loop using the break statement. If no match is found and the attempts are still available, the user is prompted to re-enter their credentials. The process repeats within a loop until the correct credentials are provided or the allowed attempts are exhausted.

If the user fails to log in after the specified attempts, the code prints an error message stating that the user is not authorized and exits the program (exit(1)). This code simulates a basic login system where users have limited attempts to provide correct credentials, enhancing security and preventing unauthorized access.





   

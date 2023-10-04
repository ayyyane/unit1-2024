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

## sign in system

```.py
def sign_in():
    name = input("Enter your name")
    with open("database.csv","r") as f:
        existing_username = [line.split(",")[0].strip() for line in f.readlines()]
        while name in existing_username:
            print("This username is already used, please enter another one.")
            name = input("Enter different user name.")

    password = input("Set your password")
    with open("database.csv","a") as myfile:
        myfile.writelines(f"\n{name},{password}")
        print("welcome")

```

I defined a function sign_in() that allows users to create an account with a username and password. The user is prompted to input their desired username. The code reads existing usernames from a CSV file named "database.csv" and checks if the entered username already exists. If it does, the user is informed, and they are prompted to enter a different username. Once a username is provided, the user sets their password. The username and password are then appended as a new line in the "database.csv" file. Finally, a welcome message is printed, indicating a successful account creation process. 

## Deposit

```.py
def deposit():
    balance = 0
    with open("savedcoin.csv","r") as f:
        data = f.readlines()
    for line in data:
        date, amount = line.strip().split(',')
        balance += int(amount)
    msg_deposit = "Enter how much would you like to deposit"
    amount = validate_int_user(msg = msg_deposit,menu = "")
    balance += amount
    date = datetime.date.today()
    with open("savedcoin.csv","a")as f:
        line = f"{date},{amount}\n"
        f.writelines(line)
        print("saved")

```
I defined a function deposit() that handles deposit operations for the system. The code initializes the balance variable to zero and reads the transaction history from a CSV file called "savedcoin.csv". It then iterates through the file lines, parsing the dates and amounts of previous transactions and updating the balance variable accordingly. The user is prompted to input the amount they want to deposit, validated by the validate_int_user() function. The deposited amount is added to the existing balance, and the current date along with the deposit amount is written back to the "savedcoin.csv" file, indicating a successful transaction. This code allows users to deposit funds into their account, updating their balance and transaction history.

## Withdraw

```.py
def withdraw():
    balance = 0
    with open("savedcoin.csv","r") as f:
        data = f.readlines()
    for line in data:
        date, amount = line.strip().split(',')
        balance += int(amount)
    msg_withdraw = "Enter how much you would like to withdraw"
    amount = validate_int_user(msg = msg_withdraw, menu = "")
    date = datetime.date.today()
    if amount > balance:
        amount = input(f"You don't have enough coin to withdraw. Please enter less than {balance} ")

    with open("savedcoin.csv","a") as f:
        line = f"{date},-{amount}\n"
        f.writelines(line)
        print("withdrown")
```
I definesd a function withdraw() that handles withdrawal operations for the system. The code begins by initializing the balance variable to zero and reading the transaction history from a CSV file named "savedcoin.csv". It then iterates through the file lines, parsing the dates and amounts of previous transactions, and updates the balance variable accordingly. The user is prompted to input the amount they want to withdraw, which is validated using the validate_int_user() function. If the entered withdrawal amount is greater than the available balance, the user is prompted to enter a smaller amount. Once a valid withdrawal amount is provided, the current date along with the negative withdrawal amount is written back to the "savedcoin.csv" file, indicating a successful withdrawal. This code allows users to withdraw funds from their account, updating their balance and transaction history while ensuring the withdrawal does not exceed the available balance.

## Show balance

```.py
def show_balance():
    balance = 0
    with open("savedcoin.csv", "r") as f:
        data = f.readlines()
    for line in data:
        date, amount = line.strip().split(',')
        balance += int(amount)

    print(f"Your balance is {balance}")
```

I defined a function called show_balance which reads data from a file named "savedcoin.csv" containing transaction records. It initializes a variable balance to 0. The code then opens the file in read mode, reads each line, splits the line into date and amount using a comma as a delimiter, and adds the integer value of the amount to the balance variable. This process calculates the total balance by summing up all the amounts from the file. Finally, it prints a message displaying the calculated balance, using an f-string to include the value of balance. When you call this function, it reads the transaction data from the file, calculates the total balance, and prints the result, providing you with an overview of your financial balance based on the recorded transactions.

## Exchange

```.py
def exchange():
    user_input = int(input("which money do you want to exchange 1 Yen 🇯🇵,2 Euro🇪🇺,3 Chinese Yuan Renminbi🇨🇳,4 British Pound🇬🇧"))
    balance = 0
    balance = 0
    with open("savedcoin.csv", "r") as f:
        data = f.readlines()
    for line in data:
        date, amount = line.strip().split(',')
        balance += int(amount)
    dollar = float(input("Please go to this site https://crypto.com/price/zcash.\n Enter the rate"))
    if user_input == 1:
        yen = float(input("Please go to this site https://www.xe.com/currencyconverter/convert/?Amount=1&From=USD&To=JPY.\n Enter the rate "))
        amount = (balance*dollar*yen)
        print(f"You have {amount}yen")
    if user_input == 2:
        Euro = float(input("Please go to this site https://www.xe.com/currencyconverter/convert/?Amount=1&From=USD&To=EUR \n Enter the rate "))
        amount = balance*dollar*Euro
        print(f"You have {amount}euro")
    if user_input == 3:
        Chinese_Yuan_Renminbi = float(input("Please go to this site https://www.xe.com/currencyconverter/convert/?Amount=1&From=USD&To=CNY\n Enter the rate "))
        amount = balance*dollar*Chinese_Yuan_Renminbi
        print(f"You have {amount}chinese yuan renminbi")
    if user_input == 4:
        British_Pound= float(input("Please go to this site https://www.xe.com/currencyconverter/convert/?Amount=1&From=USD&To=GBP \n Enter the rate "))
        amount = balance * dollar *British_Pound
        print(f"You have {amount}british pound")

```
I defined a function called exchange that simulates a currency exchange system. First, the user is prompted to choose a currency to exchange: Yen, Euro, Chinese Yuan Renminbi, or British Pound. The user's account balance is then calculated by reading transaction data from the "savedcoin.csv" file. For each line in the file, the code extracts the date and amount, summing up the amounts to calculate the total balance.

The user is then asked to input the exchange rate, which they can obtain from specific websites provided in the prompts. Depending on the user's choice, the code calculates the equivalent amount in the selected currency by multiplying the user's balance (in dollars) with the given exchange rate. The calculated amount is then displayed to the user. (For example, if the user chose Yen, the program multiplies the balance in dollars with the Yen exchange rate to calculate the equivalent amount in Yen and prints this value.)

## History of the transaction

```.py
def history():
    with open("savedcoin.csv", "r") as file:
        record = file.readlines()
        i = 0
        for line in record:
            if i > 0:
                line = line.split(",")
                print(line[0] + ": " + line[1])
            i += 1
```

The history function allows users to view their transaction history stored in the "savedcoin.csv" file. Initially, the function opens the CSV file in read mode and reads all the lines. Inside the loop, the code iterates through each line in the file, splitting the line into elements using a comma as a delimiter. The variable i is used to skip the header row (assuming the first row contains column headers) by starting at 1. For each line in the file, it prints the date (stored in line[0]) and the transaction amount (stored in line[1]). This function provides users with a clear overview of their transaction history, displaying the date and corresponding transaction amounts in a readable format. The commented code at the beginning of the function suggests a different approach to reading and printing the entire file but is currently disabled.

## video of the program
[video of the program](https://drive.google.com/file/d/1SkazMX8hxPOiHwV5z3Xe5uH0mcAyZxc5/view?usp=sharing)



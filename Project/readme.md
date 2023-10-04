# Crypto Wallet

![](22ROOSE-master768.gif)  
<sub>Illustration for Glenn Harvey</sub>

# Criteria A: Planning

## Problem definition

Ms. Sato is a local trader who is interested in the emerging market of cryptocurrencies. She has started to buy and sell electronic currencies, however at the moment she is tracking all his transaction using a ledger in a spreadsheet which is starting to become burdensome and too disorganized. It is also difficult for Ms Sato to find past transactions or important statistics about the currency. Ms Sato is in need of a digital ledger that helps her track the amount of the cryptocurrency, the transactions, along with useful statistics. 

Apart for this requirements, Ms Sato is open to explore a cryptocurrency selected by the developer.
| Name   | Coin            |   | Name | Coin |
|--------|-----------------|---|------|------|
| Keeler | ETH             |   |      |      |
| Rocky  | DOGE            |   |      |      |
| Yuiko  | BNB(Binance)    |   |      |      |
| Jan    | Tether (USDT)   |   |      |      |
| Antoni | XRP(Ripple)     |   |      |      |
| Victor | Cardano (ADA)   |   |      |      |
| Manaha | LTC (LIte Coin) |   |      |      |
| Marina | Solano (SOL)    |   |      |      |
| May    | (DAI)           |   |      |      |
| Ayane  | Zcash (ZEC)     |   |      |      |
| Yosuke  | USD COIN  (USDC)  |   |      |      |
| Naomi  |  TRX Tron       |   |      |      |
| Amine  |  KLIMA          |   |      |      |

| Dylan  | Monero XMR    |   |      |      |
| Yoshi  | Shiba Inu (SHIB)    |   |      |      |


An example of the data stored is 

| Date | Description | Category | Amount  |
|------|-------------|----------|---------|
| Sep 23 2022 | bought a house | Expenses | 10 BTC |
| Sep 24 2022 | food for house celebration | Food | 0.000001 BTC |


## Proposed Solution

Design statement:
I will to design and make a **Electric Ledger/Crypto Wallet** for a client, Ms.Sato who is a local trader intersed in  the emerging market of cryptocurrencies. The project will be about **helping her get information such as history of the coin and rate, track the amount of the cryptocurrency,the transactions, and get useful statics** and is constructed using the software **Python 3.9**. It will take **3 weeks** to make and will be evaluated according to the criteria shown below.

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

# Criteria B: Design

## System Diagram

## Flow Diagrams
[add image]
**Fig.1** Flow diagram for the registration syste. Note: there is some Python code in the operarions.

## Record of Tasks
| Task No | Planned Action                          | Planned Outcome                                                                          | Time estimate | Target completion date | Criterion |
|---------|-----------------------------------------|------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Create system diagram                   | To have a clear idea of the hardware and software requirements for the proposed solution | 10min         | Sep 24                 | B         |
| 2       | Create flow diagram for login function  | A flow diagram and the code tested                                                       |               |                        |           |
| 3       |                                         |                                                                                          |               |                        |           |
# Criteria C: Development

## Login System
My client requires a system to protect the private data. I thought about using a login system to accomplish this requirement using a if condition and the open command to work with a csv file. 
in the The flow diagram for programi shown in　**Figure 1**first line of the code I am defining a function called try_login with two inputs, name and password both are type string The output
is boolean because I only need a True if the user an password exist in the database file.

```.py
def simple_login(user:str, password:str)->bool:
    '''
    Simple authentication, needs fle user.csv
    :param user: string
    :param password: string
    :return: True/False if user is in database
    '''
    with open("user.csv") as file:
        database = file.readlines()
    output = False
    for line in database:
        line_cleaned = line.strip() #remove \n
        user_pass = line_cleaned.split(",")
        if user == user_pass[0] and password == user_pass[1]:
            output = True
            break

    return output

#logo

attempts = 3
name = input("enter your name")
password = input("enter your password")
result = try_login(name = name, password = password)
while result ==False and attempts>0:
    name = input("[Error] please enter your username")
    password = intput("[Error] please enter your password")
    result = try_login(name = name, password = password)
attempts -= 1
if result == False:
    print("you are not authorized. existing")
    exit(1)

```
### basic description
my client requires the basic description of the cyptocurrency selected. I quoted the sentences to explain what Zecash is from official website.


Zcash is a cryptocurrency built to empower economic freedom. It is similar to Bitcoin in its design — in fact, Zcash was created from the original Bitcoin code base — but it uses a privacy technology that encrypts transaction information and allows users to shield their assets. Zcash was conceived by scientists at MIT, Johns Hopkins, and other respected academic and scientific institutions. You can buy or trade Zcash on most major exchanges, like Gemini and Coinbase.




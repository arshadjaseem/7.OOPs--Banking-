# 7.OOPs--Banking-
class BankAccount:
def __init__(self, account_holder, password, balance=0):
    self.account_holder = account_holder
    self.password = password
    self.balance = balance

def login(self, input_password):
    if self.password == input_password:
        print(f"\nWelcome {self.account_holder}!")
        return True
    else:
        print("Incorrect password.")
        return False

def deposit(self, amount):
    self.balance += amount
    print(f"Deposited: ${amount}. New balance: ${self.balance}")

def withdraw(self, amount):
    if amount <= self.balance:
        self.balance -= amount
        print(f"Withdrew: ${amount}. New balance: ${self.balance}")
    else:
        print("Insufficient funds.")

def check_balance(self):
    print(f"Your balance is: ${self.balance}")
if name == "main": account = BankAccount("arshad", "1234", 100) password = input("Enter your password to log in: ") if account.login(password): while True: print("\nChoose an option: \n1. Deposit \n2. Withdraw \n3. Check Balance \n4. Exit") choice = input("Enter your choice (1/2/3/4): ")

        if choice == '1':
            amount =float(input("Enter amount to deposit: "))
            account.deposit(amount)
        elif choice == '2':
            amount =float(input("Enter amount to withdraw: "))
            account.withdraw(amount)
        elif choice == '3':
            account.check_balance()
        elif choice == '4':
            print("Exiting...")
            break
        else:
            print("Invalid option. Please try again.")

---
title: Bank-Details
date: 2025-01-08
author: Your Name
cell_count: 4
score: 0
---

```python
class BankAccount:
    def __init__(self, account_number, balance=0):
        self.account_number = account_number
        self.balance = balance

    def deposit(self, amount):
        self.balance += amount
        print(f"Deposited {amount}. New balance: {self.balance}")

    def withdraw(self, amount):
        if amount > self.balance:
            print("Insufficient balance!")
        else:
            self.balance -= amount
            print(f"Withdrew {amount}. New balance: {self.balance}")
```


```python
# Create an account
```


```python
account = BankAccount("1234567890", 1000)
account.deposit(500)
account.withdraw(300)
account.withdraw(1500)
```

    Deposited 500. New balance: 1500
    Withdrew 300. New balance: 1200
    Insufficient balance!



```python

```


---
**Score: 0**

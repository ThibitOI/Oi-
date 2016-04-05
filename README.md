Every student at school has a LunchAccount that they use to purchase lunch every day. Each Account has a 
dollar amount stored and IDnumber the student uses to purchase their food. Complete the LunchAccount class
as indicated below.


Constructors
    - A LunchAccount has two instance variables, an IDnumber and a dollar amount. There is also a boolean
        that represents if the student is a valued customer. If a student has over $50 in their account,
        they are a valued customer. Create a constructor that sets these three instance variables.
        
Methods
    - public boolean buyLunch(double amount)
        Removes amount from the student's account to pay for lunch. You should check the amount of money
        in the account to ensure the student has enough money to pay for the lunch. Students are allowed
        to charge more than they have in the account, but they can never owe more than $5.
        
        Students that are valued customers receive 10% off their food. If a student ever owes money
        (their account balance is negative), they lose their valued status.
        
        Return true if the transaction was successful, false otherwise.
        
    - public void refreshFunds(double amount)
        Adds amount to the student's account for future purchases. If a student goes over $50, they become
        valued customers.
       
    - public void closeAccount()
        Close the account by setting the IDnumber to -1 and removing all the money from the account.
        Accounts may not be closed if they owe money.
        
        Transactions should not be allowed on closed accounts.
        
    - public double lendMoney(double amount)
        Students are allowed to lend money to their peers, however, they are never allowed to lend more
        than they have. Return the amount of money lent to the peer. If the student has more money in
        their account than the amount requested, then the student may lend the entire amount. However,
        if they do not have enough than they may only lend as much money as they have in the account.
     
    - Remember to add your standard class functionality to the bottom of this class

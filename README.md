# Account
You are required to use the Account class to simulate an ATM machine. 

(The Account class) Design a class named Account that contains:
  • A private int data field named id for the account(default 0)
  • A private double data field named balance for the account(default 0)
  • A private double data field named annualInterestRate that stores the current interest rate
    (default 0). Assume all accounts have the same interest rate.
  • A private Date data field named dateCreated that stores the date when the account was
    created.
  • A no-arg constructor that creates a default account.
  • A constructor that creates an account with the specified id and initial balance.
  • The accessor and mutator methods for id, balance, and annualInterestRate.
  • The accessor method for dateCreated.
  • A method named withdraw that withdraws a specified amount from the account.
  • A method named deposit that deposits a specified amount to the account.

You are required to use the Account class to simulate an ATM machine. Create ten accounts in
an array with id 0, 1, 2 ...9, and initial balance $50. 

The system prompts the user to enter an id. If the id is entered incorrectly, ask the user to enter a correct id. Once an id is accepted, the main menu is displayed as shown in the sample run. You can enter a choice 
1 for viewing the current balance, 
2 for withdrawing money, 
3 for depositing money, and 
4 for exiting the main menu. 

If the user tries to withdraw more money than is available, the program reports a “Not enough funds.”
message. 

Once you exit, the system will prompt for an id again. So, once the system starts, it will
not stop. To exit the program the user must -1 when an id is requested.

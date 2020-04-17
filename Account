/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author tsmith
 */
public class Account {
    
    //Declared variables
    private int id;
    public static int idNum = 0;
    private double balance = 50;
    private double annualInterestRate = 0;
    private Date dateCreated;
    
    //Default constructor with no parameters and no declared variables
    public Account(){
        
    }
    
    //Constructor with initial id and balance parameters 
    public Account(int id, double balance, double annualInterestRate, Date dateCreated){
        this.id = idNum++;
        this.balance = 50;
        this.annualInterestRate = annualInterestRate;
        this.dateCreated = dateCreated;
    }

    //Accessor and mutators for id, balance and annualInterestRate
    /**
     * @return the id
     */
    public int getId() {
        return id;
    }

    /**
     * @param id the id to set
     */
    public void setId(int id) {
        this.id = id;
    }

    /**
     * @return the balance
     */
    public double getBalance() {
        return balance;
    }

    /**
     * @param balance the balance to set
     */
    public void setBalance(double balance) {
        this.balance = balance;
    }

    /**
     * @return the annualInterestRate
     */
    public double getAnnualInterestRate() {
        return annualInterestRate;
    }

    /**
     * @param annualInterestRate the annualInterestRate to set
     */
    public void setAnnualInterestRate(double annualInterestRate) {
        this.annualInterestRate = annualInterestRate;
    }

    //Accessor for dateCreated
    /**
     * @return the dateCreated
     */
    public Date getDateCreated() {
        return dateCreated;
    }
    
    /*Widthdraw method that withdraws a specified amount 
    if statement used to ensure balance doen't go into negative */
    public void widthdraw(double amount){
        if(amount < getBalance()){
            balance = getBalance() - amount;
        }
        
        else{
            System.out.printf("Not enough funds! \nBalance: $%.2f", getBalance());

            //Line break
            System.out.println(" ");
        }
    }
    
    //Deposite method that deposits a specified amount
    public void deposit(double amount){
        balance = getBalance() + amount;
    }

    public String toString(){
        return String.format("Date: %d \nID Number: %d \nAnnual Interest Rate: %.2f \nBalance: $%.2f \n", dateCreated, id, annualInterestRate, balance);
    }
    
    public boolean equals(Account i){
        return i.id == this.id;
    }
}



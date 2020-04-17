/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author tsmith
 */

import java.util.Scanner;

public class AccountTester {
    
    public static void main(String[] args) {
        
        Scanner input = new Scanner(System.in);
        
        //Declared variables
        int size = 10, id = 0, menuNum = 0;
        double balance = 50, annualInterestRate = 0, amount;
        Date dateCreated;
        
        /*Array containing accounts 
        set to size which is initialized to 10 */
        Account [] atm = new Account[size];
        
        /*Machine instance used to create the multiple accounts
        for loop used to create the specified number of accounts */
        for(int i = 0; i < size; i++){
            dateCreated = new Date (4, 10, 2020);
            Account machine = new Account(id, balance, annualInterestRate, dateCreated);
            atm[i] = machine;
        }
        
        //Prompt for user to enter an Id
        System.out.print("Enter Id: ");
        id = input.nextInt();

        //Line break
        System.out.println(" ");
        
        /*While loop used to terminate program when user enters -1 for value
        If statement used to ensure correct id is entered
        esle if correct the menu is displayed */
        while(id != -1){   
            if(id >= 0 && id <= 9){
                System.out.print("MAIN MENU \n1: View balance \n2: Widthdraw \n3: Deposit \n4: Exit main menu \nEnter menu number: ");
                menuNum = input.nextInt(); 
            }

            else{
                System.out.println("Enter correct Id!");

                System.out.print("Enter Id: ");
                id = input.nextInt();
            }

            //Line break
            System.out.println(" ");

            //Switch statement used for user choice
            switch(menuNum){
                case 1 : System.out.printf("Balance: $%.2f \n", atm[id].getBalance());
                break;

                case 2 : System.out.print("Enter amount to widthdraw: ");
                         amount = input.nextDouble();

                         atm[id].widthdraw(amount);
                break;

                case 3 : System.out.print("Enter amount to deposit: ");
                         amount = input.nextDouble();

                         atm[id].deposit(amount);    
                break;

                case 4 : System.out.print("Enter Id: ");
                         id = input.nextInt();
                break;

            }

            //Line break
            System.out.println(" ");   

        }
        
        for(int i = 0; i < size; i++)
        System.out.println(atm[i].toString());
            
    }
    
}

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

public class ProductTester{
    
    public static void main (String [] args){
        
        Scanner input = new Scanner(System.in);
        

        //Declared variables
        String product_name = " ";
        int size = 10, unit_amount, menu_number, item_number, units;
        double unit_price;
     

        //Product array set to size which is initialized to 10 
        Product [] products = new Product [size];
        

        /*For loop prompting/requestig initial values to create a product and store each value in the array
        loop set to size which is initialized to 10 */
        for(int i = 0; i < size; i++){
 
            /*Prompts user for product information to be stored in array
            product name, unit amount, price*/
            System.out.print("Enter product name: ");
            product_name = input.next();
            
            System.out.print("Enter number of product: ");
            unit_amount = input.nextInt();
            
            System.out.print("Enter product unit price: ");
            unit_price = input.nextDouble();
            
            //line break
            System.out.println(" ");
            
            //Product instance
            Product item = new Product(product_name, unit_amount, unit_price);
            products[i] = item;
        }
        
        //Options to be used 
        System.out.println("Choose from the following menu options: \n1 - To add units to stock \n2 - To deduct units from stock \n3 - To print all items in the Inventory System \n4 - To Quit \n");
        menu_number = input.nextInt();
        

        /*While loop used to continueously show menu
        loop ends when user enters number 4
        Switch statement used for menu items*/
        while (menu_number != 4){
            switch (menu_number){
                case 1 : System.out.print("Enter item number to be edited: ");
                         item_number = input.nextInt();
                         
                         System.out.print("Enter units to be added: ");   
                         units = input.nextInt();
                        
                         products[item_number].addUnits(units);
                break;

                case 2 : System.out.print("Enter item number to be edited: ");
                         item_number = input.nextInt();
                         
                         System.out.print("Enter units to be deducted: ");   
                         units = input.nextInt();
                         
                         products[item_number].deductUnits(units);      
                break;

                case 3 : for(int i = 0; i < size; i++){
                            System.out.println(products[i].toString());
                         }
                break;

                case 4 : System.out.println("Exit Menu");
                break;
            }
            

            //line break
            System.out.println(" ");
            
            System.out.println("Choose from the following menu options: \n1 - To add units to stock \n2 - To deduct units from stock \n3 - To print all items in the Inventory System \n4 - To Quit \n");
            menu_number = input.nextInt();  
        }  
        

        //line break
        System.out.println(" ");
        
        System.out.println("Menu Exited!");   
        
        //line break
        System.out.println(" ");
    }
}

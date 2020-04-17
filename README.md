# Inventory
Creating an Inventory 
Create a Product class called Product with instance variables as follows (ensure encapsulation is enforced):
  o item number (The first starts at 0 and increments every time a new product is created)
  o the name of the product
  o the number of units in stock
  o the price of each unit

 Create two constructors:
  o A default constructor without parameters that will initialize numeric variable(s) with zeros, and String variable(s) with nulls.
  o Overload the default constructor, and create a constructor with parameters that initialize the instance variables.

 Write getter/accessor and setter/mutator methods for each of the four instance variables. Ensure that the number of units in stock and price of unit is non-negative.

 Override the toString() method from the object class that will show a description of each object that includes the variable values.

 Create a method in the Product class that will calculate the value of each inventory item, using the quantity on hand and price. (For example, if I have 10 cd’s at a cost of $50 each, the value in the inventory for that item is ($500)

 Override the equals() method from the object class, two objects are equal if their item number is the same.

 Create two new methods in the Product class, one that will allow the user to add to the number of units in stock, and one that will allow the user to deduct from the number of units in stock. Both methods should have a parameter for the number of items to add/deduct. Ensure the units don’t become negative.

 Create a Java main class called ProductTester to do the following:
Initializing Inventory
Initialize an array of size 10 that stores 10 Products (the item number corresponds to the location of the product.
Using a loop, request from the user the initial values to create a product and store each product in the array.
After the initialization:
Create a menu that displays the following menu options
  1. Add units in stock
  2. Deduct units in stock
  3. Print all items in the Inventory System
  4. Quit

Note: For menu items 1(add) and 2(deduct), you must first request from the user which product you want to edit, once the item is found, you should proceed by asking the quantity to add or deduct, otherwise you are to display a message accordingly and return to the main menu. The main menu continuously displays until Quit is selected.

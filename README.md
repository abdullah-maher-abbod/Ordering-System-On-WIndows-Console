# Ordering-System-On-WIndows-Console
This is one of the pojects i enjoied doing. The main purpose of this project is to create a time and space efficient system by utilizing Data Structures and Algorithms in C++
At the bottom you will find the code explanation.
C++ is a cross-platformed language which can be used to create a sophisticated high-performance application. 


Input output
 
 
![image](https://user-images.githubusercontent.com/53852691/224862865-9e881d5a-1c4e-4d16-9e0b-670cb7905678.png)
Figure 19: main menu options
Here is how it will be displayed to the user after executing the system and the user will enter the number to choose one of these options.


 
![image](https://user-images.githubusercontent.com/53852691/224862916-2986f9cb-7973-4d98-b6d5-35160752bd40.png)
Figure 20: create a new order
This is the output and the input of creating a new order where it asks for the delivery information first and then it will display the menu and it will generates order ID automatically, and ask the user to enter the order number form the menu and the quantity of the order and askes the user where they want to add another item to the order, if the user press 2 it will show the restaurant menu again to insert another item. If user press 1 it will display the receipt for the order as it shown below, and redirect the user to the main menu.
 
 
![image](https://user-images.githubusercontent.com/53852691/224862932-91be3010-fb17-4ca2-b8a4-98d0afa5db6c.png)
Figure 21: display order receipt


![image](https://user-images.githubusercontent.com/53852691/224862948-b07e216e-9fc4-475a-a0ff-6b9161783afa.png)

Figure 22: delete order
This the output and input of delete order which is inside search for order. The user will be given the option to search using order ID, or receipt name.



 ![image](https://user-images.githubusercontent.com/53852691/224862963-d3c5e9d9-7e43-4d8c-8c8b-8509047e98d7.png)

Figure 23: delete using order ID
After entering the order ID, it will display the order and ask user to delete the order if answer was y it will delete the order from the list.
 
 
 ![image](https://user-images.githubusercontent.com/53852691/224862981-c1211b62-2093-4081-b887-74b0945b4aa0.png)

Figure 24: Delete using receipt name
This for deleting using receipt name.


![image](https://user-images.githubusercontent.com/53852691/224863002-90fe501e-9798-4bec-bfc9-ca7bbec26625.png)

Figure 25: modify the delivery information
Here is modify which can also be using order ID, or receipt name. which will modify only name, phone, and address, and display the new delivery information.


![image](https://user-images.githubusercontent.com/53852691/224863017-19b24166-0d82-4002-94f2-cb95ef550f2d.png)

Figure 26: display and fulfil orders
Here is where all the order will be displayed and the user will be asked to fulfil order if yes then it will ask for the order ID and it will fulfil the order, and redirect the user to the main menu.


 ![image](https://user-images.githubusercontent.com/53852691/224863025-7673742b-4fb2-4d0f-b7ef-5135ffb217fe.png)

Figure 27: Exit the system
And the last option which is exit the system would happens once the user press 4.









Source code   
 ![image](https://user-images.githubusercontent.com/53852691/224863702-f21fbd0c-f61a-4178-84f1-114fdcfbebf0.png)

Figure 1: Three main classes
As it’s shown above there were three classes used in for the system. The first one (OrderlnLi) is the one using linked list to list the order information such as order ID, item ID, order type, quantity, price, and the delivery information like name, phone number, and address inside the node. As it’s shown below there are several methods were used to insert into the linked list like (insterttoend). 
 
 
 ![image](https://user-images.githubusercontent.com/53852691/224863724-0bd5fc1b-e4ef-49d1-8d07-80c0e06be6e7.png)

Figure 2: OrderinLI class


![image](https://user-images.githubusercontent.com/53852691/224863749-ece51772-f5ea-4c66-8a69-ccfd628cc3ef.png)

Figure 3: Burger_menu class
This is a subclass where having the restaurant menu and display the massages for the user and call the functions form the OrderlnLI class which having the important functions.
 
 
 ![image](https://user-images.githubusercontent.com/53852691/224863771-8e52c993-1a30-4036-97d2-fd54678dd374.png)

Figure 4: main class (order_system)
This class only having main menu options and called the functions form burger_menu class.
  


 ![image](https://user-images.githubusercontent.com/53852691/224863793-379243fb-db46-4da6-9e6a-a3669b6608b1.png)

Figure 5: insert to the linked list
This function which were used to store order information as it’s shown there is object created to allow the programmer to call the variables from the h file. 
 
 
 ![image](https://user-images.githubusercontent.com/53852691/224863820-49f480b9-b279-49f2-9e01-d50319e5fe00.png)

Figure 6: user entering information
And in this class were the inserttoend were called and user allowed to enter the information like ID, name, phone, address, quantity, while other will be automatically given.


 
 ![image](https://user-images.githubusercontent.com/53852691/224863833-dfa93eb7-82e7-4b74-8b19-3a0e9516361b.png)

Figure 7: search using order ID
 
 
 
 ![image](https://user-images.githubusercontent.com/53852691/224863843-c1aa5b43-6fb2-4be6-841e-096434effb32.png)

Figure 8: search using receipt name
After inserting the order into the list, the user can search using two different ways one is using the order ID which is in Figure 5, and user could search using receipt name as in Figure 6. Both of them using the same concept in searching, which is creating a pointer and make it equal to head to make it point to where the head points, and use while to make sure that current is not pointing on the last node which is empty. After condition is fulfilled it goes to if condition to check whether the user input is existing in the linked list so once it found it the rest of the information in the node will be displayed. Else if is to move current to the next node if the name is not found. Else is if the list is empty. And it was used to display the receipt of the order and in delete the order, as well as in modify the order.
 
 
 ![image](https://user-images.githubusercontent.com/53852691/224863859-c8f9ad87-9b89-4654-a920-b998af03dacd.png)

Figure 9: printing the order using search
 
 
 ![image](https://user-images.githubusercontent.com/53852691/224863869-fa09f13e-9493-493e-a339-80631c2728a8.png)

Figure 10: using search in delete using order ID
 
 
 ![image](https://user-images.githubusercontent.com/53852691/224863882-a96396c4-2620-4632-aa51-7061a7a59fc5.png)

Figure 11: search in delete using name
 
 
 ![image](https://user-images.githubusercontent.com/53852691/224863891-08457135-d46c-4ea2-b76b-b36eafc60aab.png)

Figure 12: modify using search by name and search by order ID
 
 
 ![image](https://user-images.githubusercontent.com/53852691/224863906-f6b888b3-b0fb-4e41-9b29-e91d20b6779a.png)

Figure 13: display orders and fulfil orders
As it’s shown above this the display function where all the orders will be displayed in order. There was pointer created and checking if the order Id in not equal to NULL then it will check again it the pointer is not pointing on NULL then it will print or display all the order information. After that user will be asked whether they want to fulfils any of the orders above if answered yes then will ask which order ID after that the fulfil function will be called.
 
 
 ![image](https://user-images.githubusercontent.com/53852691/224863915-f808972a-93d0-40ef-b3f9-fdb4076e772a.png)

Figure 14: fulfil function
This the fulfil function where it will search for the order and change the state of the order into F instead of N.




 ![image](https://user-images.githubusercontent.com/53852691/224863926-94f40f22-df3f-456e-8f20-434eaa0cce0e.png)

Figure 15: modify function

This the modify function where used in burger_menu class to modify delivery information like the name, phone number, and address.
 
 
 ![image](https://user-images.githubusercontent.com/53852691/224863941-87cdbfe0-d2de-4f27-8fef-aa638d54fae7.png)

Figure 16: delete first and delete item at
This the delete functions. Deletefirst where used to delete the first item in the order, it was called in the second function which is deleteitemat where the user will enter the item they want to delete.


 ![image](https://user-images.githubusercontent.com/53852691/224863955-110d880a-6af3-4ee6-92d0-c32dd9f6c304.png)

Figure 17: main menu for create new order
Here is the main class which will have only the main menu options the few functions to call the function form burger_menu, the purpose of that to make code manageable and look better and make it easy to reach for the errors.
As it shown it will display main menu option which are create new order, search for order which have (delete and modify options), and display all orders, and lastly Exit the system.
 
 
 
 ![image](https://user-images.githubusercontent.com/53852691/224863965-b015bf08-1aba-43a9-b705-a1edb7155167.png)

Figure 18: main menu options



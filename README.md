# Messenger 

This project is messenger which is designed to establish communication via text messages between 2 or more users 

## Featrues 

- Choosing your own nickname by typing it in "Nickname Selecter" window 
- Create chats by clicking "Create chat" button in main widonw and typing user's nickname in "Create chats" window
- Create group chats by clikcing "Create group chat" button in main window and typing user's nickname as well as group chat's name in "Create group chat" window 
- Move between different chats and group chats by cliking to each one individually on main window 
- Send messages to each group chat and chat 

## Establishing connection 
To establistion connection with a server user has to fill out IP address of that particular server.
Program, firslty, will ask user for an IP address in by opening "IP address validation" window 


## Methods 
```
start(Stage primaryStage)
```
The start method is the entry point for the JavaFX application. It sets up the user interface (UI) for IP address input, validates the format and correctness of the IP address entered by the user, and provides error feedback in real-time. If the IP address is valid, it proceeds to initialize a client model with the provided IP and opens a new window for the user to enter a nickname. If the IP address is invalid, an error message is displayed.



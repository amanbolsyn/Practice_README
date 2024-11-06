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
The start method initializes the JavaFX UI for IP address input, validates its format, and provides real-time error feedback. If valid, it creates a client model with the IP and opens a window for nickname input. If invalid, it displays an error message.

```
handle(WindowEvent event)
```
This method ensures that when the window is closed, the client disconnects from any network resources and the application exits cleanly.

```
isValidIPAddress(String ip) 
```
This method checks whether a given IP address is valid by attempting to resolve it using the InetAddress.getByName() method. If the IP address can be resolved, it returns true; otherwise, it returns false.

```
isValidIpFormat(String ip)
```
This method validates the format of an IP address by first checking if it matches the standard IPv4 pattern (e.g., xxx.xxx.xxx.xxx), and then verifying that each segment of the address is within the valid range of 0-255.

```
openNicknameWindow()
```
This method creates and displays a new window where the user can input their nickname. It validates the input to ensure the nickname is not empty and attempts to register the user. Upon successful registration, it opens the chat interface window. If the input is invalid, it shows an error alert.

```
openChatWindow(String nickname)
```
This method creates and displays a new window for the chat interface. It initializes a ListView for displaying chat messages, sets the appropriate cell formatting for each message, and customizes the appearance of the list items.

```
openCreateChatWindow()
```
This method creates and displays a new window for creating a chat. It allows the user to input a nickname, validate the input, and then call the ClientViewModel.createChat(nickname) method to create the chat. If the input is valid, it closes the window; otherwise, it shows a warning.



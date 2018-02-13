PoshChat
========
PoshChat V.1.1

This release of PoshChat includes two files:
Start-PoshChatServer.ps1
Start-PoshChatClient.ps1

#### Usage

##### To start the server:
Simply run the Start-PoshChatServer.ps1 to initiate the server operation.
Currently, the server operates under port 15600. This can be changed but is not recommended at this time. 

##### To start the client:
Run the Start-PoshChatClient.ps1 script to bring up the Chat Client window. 

![Chat Client UI](https://raw.githubusercontent.com/1RedOne/PoshChat/master/img/chatClient.png)

Type in a username in the Username field and the Server IP/Hostname
in the Server field and click connect. The chat client uses a dynamic port for its local connection and connects to remote port 15600.

Once connected to the server, you can see all other connected clients in the right hand frame. As new clients join and leave, the frame will update accordingly.


#### Using the chat client:

You can type messages into the message box and click send to send messages to everyone connected to the chat server. Messages from other clients will be routed
to your client as they are sent out.

To disconnect from the chat server, you can use the Disconnect button or close the window.

You can now send a direct message to a user by appending the "@" and then their username before sending a message.

> @User Hello there!

You can adjust the font size of the chat client by using the Edit>Font context menu. This is mostly a placeholder for that setting until I have finished the Options menu.

You can also save `.txt` file transcripts of your chat conversations, by clicking File \ Save Transcripts

![Chat Client UI](https://raw.githubusercontent.com/1RedOne/PoshChat/master/img/SaveTranscripts.png)

##### Text Color:

* Red -- System message stating an error or server disconnect
* Green -- System message stating a user has connected/disconnected from server
* Blue -- Shows the direct message that you sent to another user
* Orange -- Shows the direct message that has been sent to you by another user

---------------------------------

I have many more updates planned for this application. Some of which include:
* Able to select port types for both client and server to use
* Encrypt/decrypt messages being sent
* Options menu to select font size,weight, etc...
* Better shutdown of the chat server (besides just closing out the window)

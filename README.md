# multi-client-chat-system
A multi-client chat system in C++ based on socket programming

# Run
Firstly run the server script to get the server started. Once the server gets running you will be successfully be able to see the chat room.

First compile the server code.

    gcc -Wall -g3 -fsanitize=address -pthread server.c -o server
    
Run the server script along with the port.

    ./server 4444
    
Then any client can run the client script to get into the chatroom. The user or client must enter its name to be able to join the chatroom.

    gcc -Wall -g3 -fsanitize=address -pthread client.c -o client
    
Run the client script along with the same port on which server is connected.

    ./client 4444

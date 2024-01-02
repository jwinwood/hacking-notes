# SSH

__Secure Shell Protocol__

The SSH protocol uses encryption to secure the connection between a client and
a server. All user authentication, commands, outputs and file transferes are 
encrypted to protect against attacks in the network.

```
                 1. Client starts connection with server
            ------------------------------------------------->

               2. Server sends server public key  SSH Server
            <-------------------------------------------------
SSH Client                                                      SSH Server
              3. Negotiate parameters and open secure channel
            <-------------------------------------------------

                     4. User logs into server host OS
            ------------------------------------------------->
```

The protocol works in the client-server model. This means that the connection
is established by the client connecting to the server. The client drives the 
connection setup process and uses public key cryptography to verify the identity
of the SSH server.

Once setup, the SSH protocol uses strong symmetric encryption and hashing 
alogrithms to ensure the integrity and privacy of the data exchanged between
the client and server.

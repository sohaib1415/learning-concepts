 
# SSH

__SSH__ is a network protocol that allows one computer to securely connect to another computer over an unsecured network like the internet.

## History
- 1960 old method of communication was telnet(un-secure)
- 1995 SSH was invented as secure way of communication due to encryption(actual data is converted in cipher text which is not understandable to human/machine)

## Process
1. `Make SSH server` you need to have ssh running or that system. If it is Linux or Windows you can install openssh server and with this you will have the the system ready to be accessed over ssh and if it is Android or iOS again you will find some apps that you can run so that it
2. `Make SSH Client` install ssh client on windows like putty etc or if mac / linux terminal is used as ssh clint
3. `Authentication`
	- password: ssh user@ip/host
	- key-pair ssh-keygen -t rsa 
		- it will generate key prompt where to save public and private key with name
		- it will prompt to enter passphrase or password for private key
		- it will save public and private key
		- copy public key to server
### Steps
- client sends connection requests
- server sends random message
- client encrypt this message with private key and sends to server
- server decrypt it public key and on match authentication succeeds

- SSH is commonly implemented using the client-server model one computer is called the SSH client and another machine acts as the SSH server 
- SSH can then be set up using a pair of keys a public key that is stored on the SSH server and a private key that is locally stored on the SSH client 
- the SSH client which is usually your computer will make
contact with the SSH server and provides the ID of the key pair it wants to use to prove its identity 
- the SSH server then creates a challenge which is encrypted by the public key and sent back to the client you as a client then take the challenge decrypt it with your private key and send the original challenge back to the SSH server once
the negotiation is complete the connection is established

## Usage

- Securely log into a remote machine 
- Securely transmit files
- Safely issue remote commands and much more

## Resources
[Youtube Link](https://www.youtube.com/watch?v=lRMAJwMQ0Vc)

# Server

## Installation

 - clone project
 - add installation directory to path
 
```shell
# example, in my .zshrc|.bashrc
export PATH=$PATH:/home/quentinc/dev/perso/scripts/server
```

## Usage

Simply call 

```shell
$ server -p <port> [-v]
```
in the directory where you want to launch the php server

It will : 
 - Check the port (-p) option :
   - if it is a valid argument (4 charachter integer), it will choose it as port number
   - if it is not, or if it is not given, it will launch on default port (8000)
 - Check the current directory :
   - if it is a Symfony project root, it will launch a Symfony server on choosen port
   - if it is not, it will ask if you want to launch a php server on choosen port

If the option -v is given, the server verbose option will be -vvv, else it is set by default to -v 
   
Ctr/C to exit.

## TODO

 - add "path" option to launch in another directory

# Server

## Installation

 - clone project
 - add installation directory to path
 
```shell
# example, in my .zshrc|.bashrc
export PATH=$PATH:~/dev/server_script
```

## Usage

Simply call 

```shell
$ server <port>
```
in the directory where you want to launch the php server

It will : 
 - Check the port argument :
   - if it is a valid argument (4 charachter integer), it will choose it as port number
   - if it is not, or if it is not given, it will launch on default port (8000)
 - Check the current directory :
   - if it is a Symfony project root, it will launch a Symfony server on choosen port
   - if it is not, it will ask if you want to launch a php server on choosen port
   
Ctr/C to exit.

## TODO

 - add "path" argument to launch in another directory

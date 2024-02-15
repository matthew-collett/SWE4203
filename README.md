# Client-Server Tic-Tac-Toe
The 2020-2021 SWE4203 lab project designed to explore the fundamentals of client-server architecture and software maintenance through a classic Tic Tac Toe game, enabling two players to compete against each other in real-time.

## Project Description
This project implements a classic Tic Tac Toe game in a client-server architecture, allowing users to play against each other. 
The game supports dynamic connection handling, session management, and provides a user-friendly interface for hosting and joining games.

## Installation
### Prerequisites
- Ensure Java is installed on your system. Follow the installation guide [here](https://www3.ntu.edu.sg/home/ehchua/programming/howto/JDK_Howto.html).



## Compilation
Run as shown below `javac`.

```
javac src/*.java
```

## Running
Just run the `Main.java` file!
```
cd src
java Main # optionally pass in the port e.g. java Main 5000
```

This will start a server at [`localhost:3000`](http://localhost:3000) if you used the default port. To play against yourself, you will need to open two instances of [`localhost:3000`](http://localhost:3000). In the first instance, click `"Host Game"` and then copy the access code that appeared. In the second window, paste the access code in the `Access Code` field and then click `"Find Game"`. After, you will be able to take turns placing your markers. 

> Remember, the host always goes first!

## Development
### Hot Reload for Unix Systems
If you are on a Unix based system, you can use the following command to start a hot reload server.
```
# -r because the child process is persistent and -s because we are passing in a shell command
ls src/**/*.java src/**/*.html src/**/*.js src/**/*.css | entr -rs 'make && make serve'
```

Note that you will likely have to install [entr](http://eradman.com/entrproject/) before you can run the following command. It can be easily downloaded and installed using the link above or installed using your system's package manager. The following subsections show the commands for a few operating systems.

### Ubuntu
```
sudo apt-get update -y
sudo apt-get install -y entr
```

### Mac OS
```
brew install entr
```

## Swagger
This project defines a `swagger.yml` file which can be converted into a website for visualization.

To view this information, open up `index.html` in the browser of your choice. Alternatively, go to the [Swagger Editor](https://editor.swagger.io/), copy the contents of `swagger.yml` and paste the contents in the online editor.

<!-- #### Generation
First, ensure `redoc-cli` is installed.
```
npm install -g redoc-cli
```

Next, run:
```
redoc-cli bundle -o index.html swagger.yml
``` -->


## Current UML Architecture Diagram


## Current JS Dependencies


## API Control Flow Diagram
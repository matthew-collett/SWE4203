# <p align="center">SWE4203 Project - Tic-Tac-Toe Game</p>
<p align="center"><img src="https://github.com/matthew-collett/SWE4203/assets/97645707/a1893d4a-3759-40c1-81ca-6ea63350a937" width=700/></p>

## Project Description
The 2023-2024 SWE4203 project designed to explore the fundamentals of software evolution and maintenance through a classic client-server Tic Tac Toe game, enabling two players to compete against each other in real-time.

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

## UML Architecture Diagram
<p align="center"><img src="https://github.com/matthew-collett/SWE4203/assets/97645707/4f6e3fae-74cd-4285-ac86-4498adbbd81d" width=300></p>

## JS Dependencies
<p align="center"><img src="https://github.com/matthew-collett/SWE4203/assets/97645707/becc058d-8545-4e84-972e-cc5f68534c7c" width=300></p>

## API Control Flow Diagram
<p align="center"><img src="https://github.com/matthew-collett/SWE4203/assets/97645707/362fdd39-dd9b-4610-bb21-5a6f9be23d00" width=700></p>

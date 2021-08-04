# Sample code from Practical Cloud Native Development with MicroProfile 4.0, Chapter 7 MicroProfile Ecosystem Docker and Kubernetes

## Introduction

The samples in this repository are intended to be a supplement to the book, _Practical Cloud Native Development with
MicroProfile 4.0_ by Emily Jiang, Andy McCright, John Alcorn, David Chan, and Alasdair Nottingham. Chapter 7: MicroProfile Ecosystem Docker and Kubernetes discusses how to deploy cloud-native applications using Jakarta EE and MicroProfile technologies.
This repo contains the sample code featured in this chapter. All samples run on the Open Liberty application server.

## Running the samples

In order to run these samples, you will need to use [Git](https://git-scm.com/) and [Maven](https://maven.apache.org/)
along with a Java Development Kit v8 or higher - I recommend downloading from [AdoptOpenJDK](https://adoptopenjdk.net/).

These samples are best run in an IDE like VS Code, Eclipse, Intelli-J, etc. That way, you can view the source code while
running the sample in a separate window/tab.

To build the code samples and start the server, use the command: `mvn clean package liberty:run`
This will clean any previously built code, build the source code in the project, download the latest version of Open
Liberty (unless previously downloaded), package the application into a server, and start the server. The first time you
run this command may take a little while, but once Open Liberty has been downloaded and the server packaged, subsequent
starts will be much faster.

This command will run the server in the foreground. Once you see the magic message, 
`CWWKF0011I: The ch7 server is ready to run a smarter planet.`, you are ready to test the application. By default, the
server will listen on port 9080, so if you are attempting the "Hello World" sample from the first section you could
invoke the service with the URL, "http://localhost:9080/ch7/rest/secret" - you can put this directly in a web browser or
invoke it from the command line with a tool like [curl](https://curl.se/).

To stop the server in the current terminal window, press `Ctrl-C`.

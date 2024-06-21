# Week-2 Setting up the Server

## Project - Add Real-time collaboration to Music Blocks

### Overview

This week includes the goals of adding a basic layout for collaboration space, setting up a server for local development and testing, installing and configuring the socket.io and Y.js libraries, and implementing the server-side logic.

### Building the basic layout

This step required some reverse engineering. I have observed the implementation of #global and #local tabs on the planet and then implemented the logic of CollaborationSpace. This layout will serve the purposes given below.

1. Hosting the collaboration activities
2. Track collaborative projects
3. Search for Projects available to collaborate ( in V2 or V3 )
4. Chat application among the collaborators ( in V2 )

The Collaboration Space contains a blank screen and an exit button for now. When the exit button is clicked, it takes the user back to the #global tab.

### Setting up the server

In the development process, I would need a local server to test the implementation of the messages sent through the Y.js mechanism over the WebSockets. I have created an express sever named dmps configuring the Y.js and Socket.io for this.
I have also implemented the server logic by listening for the connection event and logging the connection message with their socket ID.

Thanks for reading!

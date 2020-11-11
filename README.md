
:::DOCUMENTATION:::

 this doc shows how to mausock.js
 to get the client require the module using the 'new' constructor, also mass the username or kil
 like this
 
    const mausock = require("./mausock.js")
    const client = new mausock("bot")
    client.on("ready",f)
    
 ok now api doc
 
 
 CLASSES:
   <mauSocketClient> Client
       Properties
          <Array> users
             Connected users to the chat; NOTE: Use getusers() instead since this variable does not update (may be different in the next versions)
       Functions
          send [string message] [asynchronous but optional]
             Sends a message and returns a promise returning the message, use 'await' to retrieve the message
          getusers [no arguments] [asynchronous]
             Gets the users and returns a promise, use 'await' to get the users.
       Events
          kicked [no callback arguments]
             Fires when the user is kicked, the socket is closed to prevent spam
          message [<Message> message]
             Fires when someone says a message, is called with a message object
          ready [no callback arguments]
             Fires when the bot is ready to be used.
    <Message> message
       Properties
          <User> author
             The user that provided the message
          <string> content
             The message's content
    <Author> author
       Properties
          <Number> id
             The user's ID
          <String> username
             The user's nickname or username; if the username wasn't set this is defaulted to 'unknown'
          <Boolean> bot
             If the user is a bot or not
          <Boolean> mod
             If the user is a moderator or not
             
             
also please don't spam my site
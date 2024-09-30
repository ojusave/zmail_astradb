

---
# High Level Context
## context
**Last Updated at:** 9/30/2024, 8:04:25 PM

Summary:
This code file, named `sendMessage.js`, contains functions for sending messages via the Zoom API, updating Zoom data, and handling bot events. It interacts with the Zoom API, executes Python scripts, and manages the flow of data between Zoom and an Astra DB database.

Methods:

1. sendChatMessage(chatbotToken, message, toJid, userJid)
   Sends a chat message to a specified user through the Zoom API.

   Example:
   ```javascript
   const chatbotToken = 'your_token_here';
   const message = 'Hello, this is a test message';
   const toJid = 'recipient_jid';
   const userJid = 'sender_jid';
   await sendChatMessage(chatbotToken, message, toJid, userJid);
   ```

2. updateZoomData()
   Fetches all Zoom data, runs a Python script to load the data into Astra DB, and returns a success message.

   Example:
   ```javascript
   const result = await updateZoomData();
   console.log(result);
   ```

3. handleBotEvent(req, res)
   Handles incoming bot events, processes commands, and sends responses back to Zoom Team Chat.

   Example:
   ```javascript
   app.post('/bot-event', handleBotEvent);
   ```

Public method:

handleBotEvent(req, res)
This is the main public method exported from the module, used to handle bot events.

Example:
```javascript
const express = require('express');
const app = express();
const { handleBotEvent } = require('./sendMessage');

app.post('/bot-event', handleBotEvent);
```

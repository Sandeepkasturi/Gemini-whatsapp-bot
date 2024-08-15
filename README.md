# AI Whatsapp Bot using NodeJS, Whatsapp-WebJS And Gemini AI

This WhatsApp bot is powered by Gemini AI API, where you can chat with this AI bot and get the desired result from the Gemini AI model. This bot can be used in groups or personal chats and only needs to be authenticated using the mobile WhatsApp app.

Output Preview: Let us have a look at how the final output will look like.
[demo.png](https://media.geeksforgeeks.org/wp-content/uploads/20240214020652/4_11zon.png)

# Prerequisites
 -- Node JS
 -- Whatsapp-web.js
 -- Gemini API KEY
## Approach to create AI Whatsapp Bot
If your ever used Whatsapp Web in your browser you can easily understood that we are just going to create one without any frontend.
We will create a simple node server, which send receive messages from whatsapp web and reply with Gemini AI.
To authenticate, we will use our whatsapp for scanning the QR code.
To create AI response we will be using Gemini API, we send prompt to API and it will generate response that we need to send back to user.

# Steps To Create The Project

Step 1: Creating Node App with the following command.

npm init -y

Step 2: Installing Required Packages

npm i whatsapp-web.js @google/generative-ai qrcode-terminal
In Non Window System Additional Installation Required
npm i puppeteer

# Project Structure
[demo2.png](https://media.geeksforgeeks.org/wp-content/uploads/20240216161936/project-structure.png)

The updated dependencies in package.json file will look like:

"dependencies": {
    "@google/generative-ai": "^0.2.1",
    "qrcode-terminal": "^0.12.0",
    "whatsapp-web.js": "^1.23.0"
}

Step 3: Get the API key from the Gemini AI API

To start the application run the following command.

node bot.js
Authenticate the server
After running the server you will find a QR code in terminal, Scan it using whatsapp mobile app.
Finally your bot is running on mobile number you used to authenticate.
Just message to this whatsapp number, where message should start with “.bot”, See the final result.

### Output:

[demo3.png](https://media.geeksforgeeks.org/wp-content/uploads/20240214020920/4_11zon.png)

# Make a Discord Bot Using Node js:-
let's learn how to make a simple Discord bot with Node.js. This tutorial aims at beginners with zero knowledge on how to make a Discord bot.
## Prerequisites
* Code editor (i.e. VS Code)
* Basic knowledge in JavaScript
* Node and npm installed in your machine
* A Discord account and server set up

## Step 1: Create an App in Discord
- First, we need to create a discord bot as an app in Discord. Go to https://discord.com/developers and sign in or create a developer account.

- Once you're logged in, click on `New Application` at the top right of the window.


<a href="#"><img width="100%" height="auto" src="https://i.postimg.cc/nVjYgdr6/Screenshot-from-2022-04-03-13-10-25.jpg" height="175px"/></a>


- Then you can create your app using fill in the details example name of bot etc and you will be  taken to your app's dashboard. Navigate to `Bot` and click `Add Bot` to enable your app as a bot.


<a href="#"><img width="100%" height="auto" src="https://i.postimg.cc/Y9wGPxPw/Screenshot-from-2022-04-03-13-19-42.jpg" height="175px"/></a>

* Go to to the bot section and enable the Bot app option for the app.

<a href="#"><img width="100%" height="auto" src="https://i.postimg.cc/htkfJrc7/Screenshot-from-2022-04-03-13-20-17.jpg" height="175px"/></a>

* Click Yes and go to the Bot details page.Now, you'll have your bot and see this section appear.


<a href="#"><img width="100%" height="auto" src="https://i.postimg.cc/90gfcPL0/Screenshot-from-2022-04-03-13-21-46.jpg" height="175px"/></a>

Click on 'Copy' to copy your token and save it somewhere, we'll need it for later.This is very secret token please dont publish anywhere.


## Step 2: Install bot into your server
- Go to the OAuth2 section and Select bot under the scope section.
- Also, give permission to your bot for you need basis.

<a href="#"><img width="100%" height="auto" src="https://i.postimg.cc/Mp5fLRSc/Screenshot-from-2022-04-03-13-31-14.jpg" height="175px"/></a>


- Now showing the link of your bot Like This Link:-
- 
<a href="#"><img width="100%" height="auto" src="https://i.postimg.cc/GmgG2YSW-/Screenshot-from-2022-04-03-13-36-19.jpg" height="175px"/></a>
- Copy this URL and paste it on a new tab. You will be redirected to the page as shown below:


<a href="#"><img width="100%" height="auto" src="https://i.postimg.cc/Xq0BBgWv/Screenshot-from-2022-04-03-13-38-58.jpg" height="175px"/></a>
- Install this bot to your preferred Discord server. For example, mine is the `CryptoDeveNepal` server I just created.

- If everything works correctly, your bot should now appear in your Discord server.


<a href="#"><img width="100%" height="auto" src="https://i.postimg.cc/4y5y7kw8/Screenshot-from-2022-04-03-13-39-16.jpg" height="175px"/></a>


<a href="#"><img width="100%" height="auto" src="https://i.postimg.cc/4y5y7kw8/Screenshot-from-2022-04-03-13-39-16.jpg" height="175px"/></a>

<a href="#"><img width="100%" height="auto" src="https://i.postimg.cc/HsksZN6g/Screenshot-from-2022-04-03-13-42-19.jpg" height="175px"/></a>
- Now our CryptoBotNp is live into server



# Step 3: Create Project Folder
Now let's make this bot work! Create a new project with the following terminal commands:

    mkdir discordBot
    cd discordBot
    npm init


# Step 4: Install packages
Now we need to install the npm packages for this project. Run this command below:
- `npm install discord.js axios dotenv`

The packages we have installed are:

- discord.js: a Node.js module to allow easy interactions with the Discord API.
- axios: allows making HTTP Promises easily with Node.js.
- dotenv: allows loading variables from process.env in Node apps


# Step 5: index.js
This will create an index.js file, where our bot functions will be written at.

If you see the bot installed in your server, it is currently offline. The first thing we need to do to code our discord bot is to create a discord bot client and log our bot in.

Import the discord.js package and create a new client like so:



Remember the token we copied in Step 1? Create an .env file and store the token there.

In your .env file:
- CLIENT_TOKEN=`'your token here'`

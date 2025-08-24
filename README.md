# Discord Chatbot

A simple and minimal Discord chatbot built with Node.js and the `discord.js` library. This bot can respond to slash commands and text messages, and is easily extendable.

## 🌟 Features
-Responds to `ping` slash command with `Pong!`
- Replies to any user message with a preset response
- Built using modern Discord.js v14 API
- Supports `.env` for environment variable management

## 🧾 Requirements

- Node.js (v18 or higher recommended)
- A Discord bot token from the [Discord Developer Portal](https://discord.com/developers/applications)

## 📁 Project Structure

```
discord-chatbot/
├── index.js          # Main bot file (event handling and login)
├── command.js        # Slash command registration script
├── .env              # Your secret bot token (not committed)
├── package.json      # Dependencies and scripts
└── package-lock.json # Locked dependencies
```

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Priyanshupriyadarshi29/discord-chatbot.git
cd discord-chatbot
```

### 2. Install dependencies

```bash
npm install
```

### 3. Set up your `.env` file

Create a `.env` file in the root folder with:

```
DISCORD_TOKEN=your_bot_token_here
```

### 4. Register slash commands

Run the following to register the `ping` command:

```bash
node command.js
```

> Make sure to replace the application ID in `command.js` with your actual bot's client ID.

### 5. Start the bot

```bash
npm start
```

## 💬 Usage

- **Text Message:** The bot replies `"Hi From Bot"` to any message (excluding bots).
- **Slash Command:** Type `/ping` in a Discord server where your bot is added to get `Pong!` as a reply.

## ✍️ Customization

To add more slash commands:

1. Modify the `commands` array in `command.js`  
2. Add handling logic inside `index.js` under `interactionCreate`

To change reply messages, update the `message.reply` and `interaction.reply` logic accordingly.



### 🙌 Author 

[Priyanshu Priyadarshi](https://github.com/Priyanshupriyadarshi29)

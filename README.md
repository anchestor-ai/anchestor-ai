<img src="https://i.ibb.co/RQ28H2p/banner.png" alt="banner">
<h1 align="center"><img src="./dashboard/images/logo-non-bg.png" width="22px"> Goat Bot - Bot Chat Messenger</h1>

<p align="center">
	<a href="https://nodejs.org/dist/v16.20.0">
		<img src="https://img.shields.io/badge/Nodejs%20Support-16.x-brightgreen.svg?style=flat-square" alt="Nodejs Support v16.x">
	</a>
	<img alt="size" src="https://img.shields.io/github/repo-size/ntkhang03/Goat-Bot-V2.svg?style=flat-square&label=size">
	<img alt="code-version" src="https://img.shields.io/badge/dynamic/json?color=brightgreen&label=code%20version&prefix=v&query=%24.version&url=https://github.com/ntkhang03/Goat-Bot-V2/raw/main/package.json&style=flat-square">
	<img alt="visitors" src="https://visitor-badge.laobi.icu/badge?style=flat-square&page_id=ntkhang3.Goat-Bot-V2">
	<img alt="size" src="https://img.shields.io/badge/license-MIT-green?style=flat-square&color=brightgreen">
</p>

- [📝 Note](#-note)
- [🚧 Requirement](#-requirement)
- [📝 Tutorial](#-tutorial)
- [💡 How it works?](#-how-it-works)
- [🔔 How to get notification when have new update?](#-how-to-get-notification-when-have-new-update)
- [🆙 How to Update](#-how-to-update)
- [🛠️ How to create new commands](#️-how-to-create-new-commands)
- [💭 Support](#-support)
- [📚 Support Languages in source code](#-support-languages-in-source-code)
- [📌 Common Problems](#-common-problems)
- [❌ DO NOT USE THE ORIGINAL UNDERGRADUATE VERSION](#-do-not-use-the-original-undergraduate-version)
- [📸 Screenshots](#-screenshots)
- [✨ Copyright (C)](#-copyright-c)
- [📜 License](#-license)

<hr>

## 📝 Note
- This is a messenger chatbot using a personal account and an [unofficial API](https://github.com/ntkhang03/fb-chat-api/blob/master/DOCS.md) ([Origin here](https://github.com/Schmavery/facebook-chat-api)). This may lead to your Facebook account being locked due to spam or other reasons.
- It is recommended to use a clone account (one that you're willing to dispose of at any time).
- ***I am not responsible for any problems that may arise from using this bot.***

## 🚧 Requirement
- Node.js 16.x [Download](https://nodejs.org/dist/v16.20.0) | [Home](https://nodejs.org/en/download/) | [Other versions](https://nodejs.org/en/download/releases/)
- Basic knowledge of **programming**, JavaScript, Node.js, and unofficial Facebook APIs.

## 📝 Tutorial
Tutorials have been uploaded on YouTube:
- For mobile: [Watch Here](https://www.youtube.com/watch?v=grVeZ76HlgA)
- For VPS/Windows: [Watch Here](https://www.youtube.com/watch?v=uCbSYNQNEwY)

Summary instructions can be found [here](https://github.com/ntkhang03/Goat-Bot-V2/blob/main/STEP_INSTALL.md).

## 💡 How it works?
The bot utilizes the unofficial Facebook API to send and receive messages from users. It has several event handlers to process different types of interactions:

### Event Handlers

- **onStart**: 
  - Checks if a user has called a command.
  - Validates user permissions and whether the user is banned.
  - Executes the command and logs information to the console.

- **onChat**:
  - Activated when a user sends a message.
  - Validates user permissions and executes the command if allowed.

- **onFirstChat**:
  - Triggered by the first message from the chat since the bot started.
  - Similar functionality to `onChat`.

- **onReaction**:
  - Triggered when a user reacts to a message.
  - Validates user permissions and executes the command if allowed.

- **onReply**:
  - Activated when a user replies to a message.
  - Similar to `onReaction` in functionality.

- **onEvent**:
  - Triggered by new events such as user joins or leaves.
  - Executes commands defined in the `GoatBot.eventCommands`.

- **handlerEvent**:
  - Processes all event commands defined in `GoatBot.eventCommands`.

## 🔔 How to get notification when have new update?
You can follow the repository on GitHub to receive notifications for new releases and updates.

## 🆙 How to Update
To update the bot to the latest version:
1. Pull the latest changes from the repository:
   ```bash
   git pull origin main

<div align="center">
  <br />
  <p>
    <a href="https://discord.js.org"><img src="https://discord.js.org/static/logo.svg" width="546" alt="discord.js" /></a>
  </p>
  <h1>Discord.js Selfbot v13 (Modernized)</h1>
  <p>
    <a href="https://www.npmjs.com/package/discord.js-selfbot-v13"><img src="https://img.shields.io/npm/v/discord.js-selfbot-v13.svg?color=blue" alt="npm version" /></a>
    <a href="https://www.npmjs.com/package/discord.js-selfbot-v13"><img src="https://img.shields.io/npm/dt/discord.js-selfbot-v13.svg?color=green" alt="npm downloads" /></a>
    <img src="https://img.shields.io/badge/Discord%20API-v10-purple.svg" alt="Discord API v10" />
    <img src="https://img.shields.io/badge/Built--in-Voice-orange.svg" alt="Built-in Voice" />
  </p>
</div>

> [!CAUTION]
> **Using this on a user account is prohibited by the [Discord TOS](https://discord.com/terms) and can lead to an account block.**
> **When using these libraries, you accept the risk of exposing your Discord Token.**
> **I don't take any responsibility for blocked Discord accounts that used this module.**

## About

<strong>Welcome to `discord.js-self-bot`, fully modernized for Discord API v10.</strong>

`discord.js-self-bot` is a [Node.js](https://nodejs.org) module that allows user accounts to interact with the Discord API. This updated repository is completely modernized to support **Discord API v10**, Gateway v10, and built-in Voice integration natively.

### What's New in this Modernized Version?
- **Discord API v10 & Gateway v10 Support:** Fully upgraded WebSocket configuration and intents parsing.
- **Anti-Detection & Spoofing:** Hardcoded to mimic the latest Discord Desktop Client (Windows 11, Chrome 138, Electron 36) to avoid Cloudflare/API blocks.
- **Clean & Warning-Free:** All deprecated sub-dependencies and linting warnings have been removed for a flawless installation experience.

---

## Features

- [x] **Core:** Messages, Guilds, Channels, Roles, and Interactions (Slash Commands, Buttons, Menus, Modals).
- [x] **Account Features:** RemoteAuth, Relationships (Friends), User Settings, Notes, and Billing.
- [x] **Voice & Audio:** Built-in `@discordjs/voice` integration. Join channels, play audio, and record directly out of the box.
- [x] **Advanced Events:** Full support for modern Gateway events (e.g., Polls, Voice Channel Effects, Auto-Moderation).
- [x] **Captcha & TOTP Handler:** Fully integrated MFA support utilizing the latest `otplib` v13.

## Installation

> [!NOTE]
> **Node.js 20.18.0 or newer is required**

```sh-session
npm install @deksdeveloper/discord.js-self-bot
```

## How to Get Your Token

> [!WARNING]  
> Never share your token with anyone!

Run the following code in the **Discord Console (Ctrl + Shift + I -> Console)** to copy your token to the clipboard:

```js
window.webpackChunkdiscord_app.push([
	[Symbol()],
	{},
	req => {
		if (!req.c) return;
		for (let m of Object.values(req.c)) {
			try {
				if (!m.exports || m.exports === window) continue;
				if (m.exports?.getToken) return copy(m.exports.getToken());
				for (let ex in m.exports) {
					if (m.exports?.[ex]?.getToken && m.exports[ex][Symbol.toStringTag] !== 'IntlMessagesProxy') return copy(m.exports[ex].getToken());
				}
			} catch {}
		}
	},
]);

window.webpackChunkdiscord_app.pop();
console.log('%cWorked!', 'font-size: 50px; color: green;');
console.log(`%cYou now have your token in the clipboard!`, 'font-size: 16px;');
```

## Need help?
Feel free to open an Issue or start a Github Discussion if you have questions about the new API v10 adaptations or voice integrations.

## Credits
- Based on the original [discord.js-selfbot-v13](https://github.com/aiko-chan-ai/discord.js-selfbot-v13) fork.
- Powered by the incredible core of [Discord.js](https://github.com/discordjs/discord.js).

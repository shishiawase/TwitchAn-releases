# TwitchAn

TwitchAn is a small Windows desktop app for Twitch stream monitoring, Discord notifications, and Twitch chat bot commands.

![TwitchAn main window](docs/assets/twitchan-main.png)

## Features

- Monitor a Twitch channel status from a compact desktop window.
- Send Discord webhook notifications when the stream goes online.
- Check Twitch, channel, and Discord setup from the main screen.
- Keep a local event log for stream checks, Discord delivery, and bot activity.
- Use a separate Twitch account as a chat bot.
- Create chat bot commands with regular expression triggers.
- Use response variables such as `{user}`, `{channel}`, `{args before}`, `{args after}`, and `{rand X to Y}`.
- Send timer-based bot messages to chat.
- Receive future updates through the built-in Tauri updater.

## Download

Download the latest Windows setup file from the [latest release](https://github.com/shishiawase/TwitchAn-releases/releases/latest).

Use the `TwitchAn_<version>_x64-setup.exe` asset. The `latest.json` and `.sig` files are updater metadata used by the app.

## Updating

Versions with updater support can check and install future updates from this public release channel.

Older builds without updater support must be replaced manually once by installing a newer setup file from Releases.

## Required Setup

TwitchAn needs your own Twitch application credentials to call Twitch APIs.

For Discord notifications, add a Discord webhook URL in the app settings.

For the chat bot, log in with the separate Twitch account that should send chat messages. The bot uses Twitch device-code login and stores bot authentication separately from the main app settings.

## Privacy

TwitchAn stores app settings locally on your PC. Secrets such as Twitch tokens and Discord webhook data are not published in this repository.

Do not share screenshots that reveal private webhook URLs, client secrets, or tokens.

## License

MIT License. See [LICENSE](LICENSE).

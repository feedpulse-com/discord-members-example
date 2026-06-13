# discord-members-example

> Example install for the **Discord Live Members** widget — part of the [FeedPulse](https://feed-pulse.com) free widget suite.

## What it does

Renders a live member counter for any public Discord server. Shows:

- **Total members** of the server
- **Currently online** (green dot count)
- **Server name + icon**

Updates every 60 seconds via Discord's own public Widget API — no bot installation, no OAuth flow, no admin permissions required. Just enable "Server Widget" in your Discord server's settings (Server Settings → Widget → Enable) and use any invite code.

## Why not use Discord's built-in widget?

Discord's own [widget.json endpoint](https://discord.com/developers/docs/resources/guild#get-guild-widget) returns raw JSON. This widget renders it as a clean, themeable HTML pill that sits naturally on a landing page or sidebar — no iframe, no Discord branding takeover, full colour control.

## Install

1. **Enable the Server Widget in Discord:** Server Settings → Widget → toggle ON. Discord generates an invite code automatically.
2. **Copy the invite code** (the last part of any standard invite URL — `discord.gg/XYZ123` → code is `XYZ123`).
3. **Paste the snippet** anywhere you want the badge:

```html
<script async src="https://feed-pulse.com/api/embed/discord_members?invite=YOUR_INVITE_CODE"></script>
```

## Customization params

| Param | Default | Description |
|---|---|---|
| `invite` | *(required)* | Discord invite code (the part after `discord.gg/`) |
| `theme` | `obsidian` | `obsidian`, `mint`, `sand`, `light`, `dark` |
| `w` | `260` | Widget width in pixels |
| `show_online` | `1` | `1` to show "online now" pill, `0` to hide |
| `lang` | `auto` | Label language — see the [main org README](https://github.com/feedpulse-com/.github) for the full 12-language list |

## Use cases

- **Game studio landing pages** — show your community is active before visitors join
- **Open-source project sites** — embed alongside the GitHub Stars badge for full social proof
- **SaaS docs sites** — link to your community Discord with the live counter for context
- **Indie-game forums** — show off your Discord member count instead of just linking
- **Streaming / creator pages** — Twitch + YouTube creators with a Discord community

## Live example

The widget is running on [feed-pulse.com/widgets](https://feed-pulse.com/widgets) — see it embedded on a real page. Customizer and generator at [feed-pulse.com/free-discord-members-widget](https://feed-pulse.com/free-discord-members-widget).

## Generate your own

Customize the theme + width at [feed-pulse.com/free-discord-members-widget](https://feed-pulse.com/free-discord-members-widget).

## License

[MIT](LICENSE)

## More widgets

19 free embeddable widgets at [feed-pulse.com/widgets](https://feed-pulse.com/widgets) — including GitHub stars, npm downloads, live traffic, weather, crypto/stock tickers, and more.

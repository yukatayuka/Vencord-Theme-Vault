# NSO - Needy Girl

A Vencord theme inspired from 
[yunffee/NSO-inspired-discord-theme](https://github.com/yunffee/NSO-inspired-discord-theme).

This is an original CSS theme: it does not bundle game artwork or assets from
the reference project. It pairs pale lilac and rose desktop surfaces with
pink details, pixel-style text and profile frames, and dark plum text.

## Visual research

The official [Steam screenshot gallery](https://store.steampowered.com/app/1451940/NEEDY_STREAMER_OVERLOAD/#app_screenshots)
is the primary visual reference. Two useful examples are the
[stream UI with its night backdrop](https://shared.fastly.steamstatic.com/store_item_assets/steam/apps/1451940/ss_c307ea74f79577d6ad54dbb3affff34141a8642d.1920x1080.jpg?t=1762834234)
and a [character-focused stream screen](https://shared.akamai.steamstatic.com/store_item_assets/steam/apps/1451940/ss_c60613e817ed66dd645cc0c22b037ceb148f16d6.1920x1080.jpg).
They show a desktop-style window, small title bars and taskbar, pixel-art
character portraits, blocky interface type, comment panels, and a vivid
violet-and-cyan night backdrop.

The game look is not just “pixel font.” It combines pixel-art characters and
compact, pixel-like UI details with pastel pink/lavender panels and playful
desktop-window framing. A useful theme translation is:

- Keep Discord's main reading areas light and calm, with dark plum text.
- Use restrained violet and hot pink for selected states, links, and active
  controls; keep larger background areas close in value and temperature.
- Let title bars, compact labels, and small separators carry the retro desktop
  cues. Pixelify Sans extends to message text, names, and profile details, with
  dark high-contrast ink to preserve legibility.
- Keep the overall interface pastel and bright. Use clean, crisp borders to
  suggest pixel-era windows without adding a neon night theme.

These are visual observations and design guidance, not sampled game color
specifications. The linked screenshots remain on Steam; no game artwork is
copied into this theme. Pixelify Sans is used throughout Discord's text UI,
including message content and profile details; code blocks retain their own
monospace styling.

## Install with Vencord

1. Copy `needy-girl.theme.css` into Vencord's `themes` folder.
   On a typical Windows install, this is `%AppData%\Vencord\themes`.
2. In Discord, open **User Settings > Vencord > Themes**.
3. Enable **Needy Girl**. If it does not appear, use **Reload Themes**
   in the Themes settings.

You can also paste the contents of the CSS file into Vencord's Custom CSS box.

## Customize

The palette and intended use are defined at the top of the CSS file:

| Role | Token | Color | Use |
| --- | --- | --- | --- |
| Main text | `--nso-ink` | `#382b43` | Message content, names, and headings |
| Secondary text | `--nso-ink-secondary` | `#6a5a72` | Timestamps and supporting text |
| Main accent | `--nso-violet` | `#64479a` | Brand states and active UI |
| Pink accent | `--nso-pink` | `#b74381` | Mentions and small highlights |
| Main surface | `--nso-paper` | `#fffafd` | Chat and app background |
| Lilac surface | `--nso-lilac` | `#f3eef8` | Server rail and channel sidebar |
| Rose surface | `--nso-rose-surface` | `#fbf2f8` | Member list |

The theme maps Discord's semantic background, text, and interaction tokens and
also styles key UI regions, message typography, command suggestions, and
stepped profile popout frames. Keep text dark on light surfaces. Discord
updates internal class names periodically, so variable-based colors are the
primary coverage and component selectors are supplemental. The profile frame
uses a small inline SVG as a CSS border-image source to make the corners
visibly stepped rather than merely square.

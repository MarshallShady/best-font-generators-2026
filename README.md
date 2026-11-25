# FontChanger — free Unicode font generator (copy & paste)

[FontChanger](https://getfontchanger.com/) is a free, no-sign-up Unicode font generator that
runs entirely in the browser. You type text once and it renders 330 bold, cursive, gothic,
bubble, glitch and decorated styles you can copy and paste into Instagram, Discord, TikTok, X,
WhatsApp or YouTube. There is nothing to install and no account to create. The same site hosts
a [kaomoji](https://getfontchanger.com/kaomoji/) library — Japanese-style text faces for bios,
nicknames and chat.

## What it does

- **330 styles on one screen.** Bold, italic, cursive, gothic, double-struck, small caps,
  bubble, squared, fullwidth, reversed, glitch and Zalgo, plus combining-mark styles
  (strikethrough, underline, wavy) and decorated variants (hearts, stars, flowers, brackets).
- **Live rendering, no generate button.** Every style card updates as you type, and the input
  box stays pinned to the top while you scroll the style list on a phone.
- **A compatibility badge on every style.** Each one is marked All platforms, Most platforms or
  Some phones, so you can see the risk of empty boxes before you paste.
- **A character limit checker.** Presets for Instagram bio 150, Instagram name 30, Discord
  username 32, X bio 160, TikTok bio 80, YouTube channel name 100 and Facebook bio 101. Go over
  and it shows the overage plus a one-tap trim.
- **Copy once, paste anywhere.** One tap copies a style; a Share button puts the converted text
  into a link, and saved styles stay in the browser.
- **Search and filters.** Filter by Bold, Cursive, Gothic, Aesthetic, Glitch or Bubble, search
  styles by name, or randomise per letter or per word.
- **Local conversion.** The text is converted in the page, not on a server.

## Site map

Converter and platform guides:

- [FontChanger](https://getfontchanger.com/) — the 330-style converter, character limit checker and share links.
- [Instagram fonts](https://getfontchanger.com/instagram-fonts/) — styles for the bio, captions and the 150-character bio limit.
- [Discord fonts](https://getfontchanger.com/discord-fonts/) — display names, server names and the 32-character name limit.
- [Cursive font generator](https://getfontchanger.com/cursive-font-generator/) — script and calligraphy styles for signatures and bios.
- [Bold text generator](https://getfontchanger.com/bold-text-generator/) — bold, bold italic and bold sans, the most widely supported Unicode letters.
- [Glitch text generator](https://getfontchanger.com/glitch-text-generator/) — glitch, Zalgo and combining-mark effects and where they break.
- [Reverse font generator](https://getfontchanger.com/reverse-font-generator/) — upside-down and mirrored text.

Kaomoji library:

- [Kaomoji](https://getfontchanger.com/kaomoji/) — 200 text faces in 17 mood categories (Happy, Love, Cute, Shy, Angry, Animals, Food, Gaming…) with Cat, Bear and Food filters; tap one to copy.
- [Kaomoji copy paste](https://getfontchanger.com/kaomoji/copy-paste/) — 180 short, widely supported faces grouped by where they are used: Discord nicknames, Instagram bios, status and chat.
- [Cute kaomoji](https://getfontchanger.com/kaomoji/cute/) — 133 kawaii faces in 11 categories, including 30 cats, 15 bears, 10 food faces and 20 hearts.

Spanish site:

- [Letras bonitas](https://getfontchanger.com/es/) — the Spanish home page.
- [Letras para Instagram](https://getfontchanger.com/es/letras-para-instagram/) — Instagram fonts in Spanish.
- [Letras para Discord](https://getfontchanger.com/es/letras-para-discord/) — Discord fonts in Spanish.
- [Letras cursivas](https://getfontchanger.com/es/letras-cursivas/) — cursive fonts in Spanish.
- [Letras negritas](https://getfontchanger.com/es/letras-negritas/) — bold text in Spanish.
- [Letras glitch](https://getfontchanger.com/es/letras-glitch/) — glitch text in Spanish.

Site pages:

- [About](https://getfontchanger.com/about/) — who runs the site and how styles are built.
- [Privacy](https://getfontchanger.com/privacy/) — what is stored locally and what is not collected.

## Platform character limits

Styled text is longer in bytes but the same length in characters, so the limit you have to watch
is the same one you already know. The built-in limit selector uses these figures:

| Platform | Limit | Notes |
|---|---|---|
| Instagram bio | 150 characters | Cut at 150 |
| Instagram name | 30 characters | The name field accepts styled letters |
| Instagram @username | styled letters rejected | Usernames only allow letters, numbers, periods and underscores |
| Discord display name | 32 characters | Some symbols are filtered |
| X (Twitter) bio | 160 characters | A few clients drop rare glyphs |
| TikTok bio | 80 characters | Nickname is cut at 30 |
| TikTok nickname | 30 characters | |
| YouTube channel name | 100 characters | The @handle must stay plain text |
| Facebook bio | 101 characters | |
| WhatsApp status | 139 characters | |

## FAQ

**Are these real fonts?**
No. Every style is a different set of Unicode characters that already look bold, cursive or
gothic. Your apps keep using their own fonts; the characters themselves have a different shape,
which is why nothing has to be installed and the person receiving the text needs nothing either.

**Why does my text turn into boxes or question marks?**
A box (tofu) means the app found no glyph for that character on that device. Mathematical bold
and italic letters are supported almost everywhere; small caps, double-struck, circled and
squared letters are newer. Pick a style marked All platforms, or a simpler variant of the same
look.

**Why does a style look broken on an older Android phone?**
Older Android builds ship fonts that are missing some of the newer letter blocks, and
combining-mark styles (strikethrough, underline, wavy) need one extra mark per letter — one
missing mark can make a whole word look broken. Those styles are labelled Some phones for that
reason.

**How are characters counted?**
The counter follows what the platform counts: each styled letter is still one character, so a
bold "hello" is five characters, not ten. Combining-mark styles add an invisible mark per
letter, and a few platforms count those separately — the limit selector shows the overage and
offers a one-tap trim, so you never have to count by hand.

**Can I use styled text in a username or handle?**
Usually not. Instagram, TikTok, X, YouTube and Discord reserve the unique username or handle for a
restricted character set. Styled text belongs in display names, bios, captions, comments and
messages.

**Does styled text survive in Discord?**
Yes for messages, display names and server or channel names. Discord trims display names at 32
characters and filters a few control and zero-width characters, so bold, gothic or bubble
variants are the safest choices there.

**Is it really free?**
Yes. Every style, copy, share and the character limit checker are free, with no account, no
download, no watermark and nothing to install.

## Technical notes

- **Built with Unicode, not font files.** There is no .ttf or .otf output. The tool maps your
  text to Unicode characters that already exist in the fonts the platform uses.
- **Conversions run in your browser.** There is no conversion API and no upload: the text you
  type stays on the page. Saved styles and recent picks live in the browser's local storage only,
  and clearing site data removes them.
- **Share links contain your text.** The Share button puts the converted text into the URL
  fragment and query string, so a shared link holds exactly what was typed — share it
  deliberately.
- **Works without JavaScript.** The catalog is server-rendered HTML, so every style is still
  visible with JavaScript disabled; the converter then behaves as a static preview.
- **Three rendering engines.** Most styles replace letters with a per-style character table; two
  further engines attach combining marks (underline, strikethrough, glitch) or transform the
  string itself (upside-down, mirrored). Decorated variants such as Cursive Hearts or Thin Gothic
  come from mixing them.

## Changelog

- **2026-11-25** — rewrote this README as a description of the tool: replaced the ranked list
  with a site map, added the three kaomoji pages, ported the platform character limit table and
  documented how conversion works.
- **2026-11** — earlier revisions of this README.

Released under the MIT License — see [LICENSE](LICENSE).

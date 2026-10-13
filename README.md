# Pause First

**Plain-English cybersecurity lessons for older adults.**

Pause First is a single-page website that teaches seniors how to spot scams and stay safe on the phone, in email, and online. It is built around one habit: *scammers need you to rush, so pause first.*

**Live site:** https://cruhling289.github.io/elderlyfraudprotection/

## What's inside

- **Real or scam? practice game.** Five sample messages (texts, a phone call, a computer pop-up). Each answer comes with a plain explanation of the warning signs.
- **Five short lessons.** Phone calls, emails and texts, passwords and sign-in codes, shopping and banking, and updates and devices.
- **Three rules to remember.** Slow down, check another way, and never pay with gift cards, wire transfers or crypto.
- **If something already happened.** Calm next steps and free U.S. help lines.

## Designed for older readers

- Large, high-contrast text set in [Atkinson Hyperlegible](https://brailleinstitute.org/freefont), a typeface made for legibility
- Built-in text size buttons (normal, large, extra large) that remember the reader's choice
- Big tap targets and a simple one-column layout that works on phones, tablets and desktops
- Light and dark mode that follow the device setting
- Visible keyboard focus, screen-reader labels, and reduced-motion support
- No sign-up, no ads, no tracking

## Run it locally

There is nothing to install or build. The whole site is one HTML file.

1. Download or clone this repository.
2. Open `index.html` in any web browser.

It also works offline. The only thing that won't load without internet is the Google Fonts typeface; the page falls back to Verdana or Tahoma.

## Publish with GitHub Pages

1. Make sure the page is named `index.html` and sits at the top level of the repository.
2. On GitHub, go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and the `/ (root)` folder, then click **Save**.
5. After a minute or two, your site is live at `https://cruhling289.github.io/elderlyfraudprotection/`.

## Customize it

Everything is in `index.html`.

| To change | Where to look |
|---|---|
| Practice messages | The `Q` array in the `<script>` at the bottom of the file |
| Lessons | The `<details>` blocks in the `#lessons` section |
| Three rules | The `.rule` blocks in the `#rules` section |
| Help line numbers | The `.help` block in the `#help` section |
| Colors | The CSS variables at the top of the `<style>` block (light and dark sets) |
| Default text size | `font-size` on the `html` rule (18px by default) |

Each practice message in `Q` looks like this:

```js
{
  k: "Text message",            // type of message
  f: "From: 29278",             // who it appears to be from
  m: "The message text...",     // what the message says
  s: true,                      // true = scam, false = real
  w: "Why it is or isn't a scam" // explanation shown after answering
}
```

### Tips for good practice messages

- Mix scams and genuine messages so readers don't learn "always answer scam."
- Base examples on scams people are really seeing: package delivery fees, "grandchild in trouble" calls, fake tech support, bank impersonation, and Medicare or Social Security calls.
- Keep explanations short and kind. Point to the clues without making anyone feel foolish.

## Presenting to a group

- Show the practice game on a projector and let the room vote before revealing each answer.
- Set the text size to large or extra large before you start.
- Share the site with a QR code or a large-print handout instead of a long web address.
- Finish by asking everyone to agree on a family code word.

## Important notes

- **Check the phone numbers before sharing widely.** The help lines (National Elder Fraud Hotline, AARP Fraud Watch Helpline, FTC) are for the United States and may change over time. Please confirm them before each presentation.
- **This is a learning guide,** not professional security, legal or financial advice.
- Sample phone numbers and web addresses in the practice messages are made up for teaching.

## Contributing

Suggestions are welcome, especially from older adults, caregivers and educators. Open an issue or pull request with new practice messages, clearer wording, or accessibility improvements.

## License

Add a license of your choice (for example, [MIT](https://choosealicense.com/licenses/mit/)) as a `LICENSE` file in the repository, and update this section to match.

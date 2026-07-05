# Customization guide

You only need a text editor and a browser. Open `index.html`, make a small change, save it, then refresh the browser to see the result. Keeping a backup before large edits is always handy.

## Change the name

Find the main `<h1>` heading inside the `<body>`. Replace its current words with a generic or consented greeting, for example:

```html
<h1>Hey, Someone Special!</h1>
```

Change only the words between the opening `<h1>` and closing `</h1>` tags.

## Change the main message and question

The introduction is the paragraph marked `id="message"`:

```html
<p id="message">Write your friendly message here.</p>
```

The main question is the `<h2>` immediately below it:

```html
<h2>Would you like to hang out?</h2>
```

Keep personal details generic unless everyone involved has agreed to their publication.

## Edit the No button messages

Scroll to the `<script>` section and find `function moveNoButton()`. Each condition sets a new message with a line like:

```js
smallText.textContent = "The No button is feeling shy!";
```

Replace the text inside the quotation marks. Do not remove the quotation marks or the semicolon. The final `else` message appears on the fifth and every later attempt.

To change the text shown before the first attempt, edit the paragraph with `id="smallText"` in the HTML.

## Edit the final success screen

Near the bottom of the `<script>`, find:

```js
yesBtn.addEventListener("click", () => {
```

The backtick-wrapped HTML below it becomes the success screen. Edit the emoji, `<h1>`, `<p>`, and `<h2>` text there. Keep the opening and closing backticks in place.

## Change colors

Colors live in the `<style>` section near the top of `index.html`:

- `body` contains the page's `background: linear-gradient(...)`.
- `.card` controls the white card and its shadow.
- `h1` controls the main heading color.
- `#yesBtn` controls the Yes button.
- `#noBtn` controls the No button.

Hex colors look like `#ff4f9a`. A color picker can give you replacement hex values. The success screen has inline color styles inside the `yesBtn` click handler, so update those too if you want it to match.

## Change button labels

Find these two elements in the HTML:

```html
<button id="yesBtn">Yes</button>
<button id="noBtn">No</button>
```

Change the visible words or emojis, but keep both `id` values unchanged because JavaScript uses them.

## Replace emojis

Emojis are plain text in the heart, buttons, messages, and success-screen template. Replace them as you would any other character. Save the file as UTF-8 so emojis display correctly.

If you prefer an image, place it in `assets/images/` and replace the heart element with:

```html
<img src="assets/images/your-image.png" alt="Decorative heart" width="64">
```

Use an accurate `alt` description, and only share images you have permission to use.

## Add or remove music

Music is not included by default.

1. Put a licensed audio file at `assets/audio/music.mp3`.
2. Add this near the top of the `<body>`:

   ```html
   <audio id="music" loop>
     <source src="assets/audio/music.mp3" type="audio/mpeg">
   </audio>
   ```

3. Add a play button inside the card:

   ```html
   <button type="button" onclick="document.getElementById('music').play()">
     Play music
   </button>
   ```

Browsers often block autoplay until someone interacts with the page. A visible play button is reliable and gives visitors control over sound.

To remove music later, delete the `<audio>` element, the play button, and the audio file. If your customized version already contains different audio code, also remove any JavaScript that calls `.play()`.

## Check your changes

Refresh `index.html` in a browser and verify:

- The text and emoji display correctly.
- Both buttons work.
- The No button stays reachable on a phone-sized screen.
- The success screen contains no unintended personal information.
- Audio, if added, has controls and uses an asset you may legally share.

# Crush Website 

A playful, beginner-friendly HTML/CSS/JavaScript template for asking someone special a fun question. The **Yes** button leads to a happy ending, while the **No** button makes a cheeky escape on hover or touch.

Everything lives in one `index.html` file, so it is easy to customize, share, and host—no framework or build step needed.


## Features

- One-file HTML, CSS, and JavaScript setup
- Runaway **No** button for mouse and touch screens
- Custom messages after each escape attempt
- Animated heart and cheerful success screen
- Responsive card layout for phones and desktop browsers
- No dependencies, accounts, or build tools
- Friendly starting point for first-time creators


## Get the template

### Download as a ZIP

1. Open the (https://github.com/Meshtech254/my-crush_)
2. Select **Code**.
3. Select **Download ZIP**.
4. Extract the ZIP somewhere easy to find.

### Clone with Git

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
cd YOUR-REPOSITORY
```

Replace the URL and folder name with your real repository details.

## Run locally

Open `index.html` in any modern browser—double-clicking the file is usually enough. There is no installation or local server required.

If you prefer a local server, an editor extension such as Live Server also works, but it is optional.

## Customize it

Open `index.html` in a text editor such as VS Code, Notepad, or TextEdit.

- **Name:** edit the `<h1>` text near the top of the `<body>`, using something generic like “Hey, Someone Special!”
- **Message and question:** edit the paragraph with `id="message"` and the `<h2>` below it.
- **Colors:** edit the color values in the `<style>` section. The main pink is `#ff4f9a`, and the page background uses a `linear-gradient`.
- **Buttons:** edit the text inside `#yesBtn` and `#noBtn`; change their appearance in the matching CSS rules.
- **No-button messages:** edit the `smallText.textContent` lines inside `moveNoButton()`.
- **Success screen:** edit the HTML inside the `yesBtn` click handler near the end of the file.

The detailed beginner walkthrough is in [docs/customization.md](docs/customization.md).

### Add music or audio

The template does not include an audio file by default, but it supports normal browser audio. Put an audio file in `assets/audio/`, add an `<audio>` element to `index.html`, and start playback from a button click. Browsers commonly block autoplay until a visitor interacts with the page, so click-to-play is the most reliable approach. See [the music instructions](docs/customization.md#add-or-remove-music).

Only use audio you created or have permission to share.

## Deploy

- **GitHub Pages:** push the project to GitHub, then enable Pages from the repository's **Settings → Pages** screen.
- **Netlify Drop:** drag the project folder (with `index.html` at its root) into Netlify Drop.
- **Vercel:** import the GitHub repository as a new project and deploy it as a static site.

Full step-by-step instructions are in [docs/deployment.md](docs/deployment.md).

## Folder structure

```text
.
├── assets/
│   ├── audio/          # Optional music or sound files
│   ├── images/         # Optional images
│   └── screenshots/    # README screenshots
├── docs/
│   ├── customization.md
│   └── deployment.md
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── index.html          # The complete website
├── LICENSE
├── README.md
└── SECURITY.md
```

Empty asset folders include `.gitkeep` files so Git can retain the structure.

## Browser and mobile compatibility

The template uses standard HTML, CSS, and JavaScript and should work in current versions of Chrome, Edge, Firefox, and Safari. The layout is responsive, and the runaway button listens for both mouse hover and touch. Very old browsers are not officially supported.

Test your customized version on both a phone and a computer before sharing it—the escaping button needs room to roam.

## Privacy and respect

Keep it sweet, respectful, and pressure-free. Do not publish real names, phone numbers, addresses, photos, private messages, or other personal details without clear consent. Anyone can view the contents of a public repository and public website. Please respect the other person's answer and boundaries, even when the **No** button is feeling mischievous.

Read [SECURITY.md](SECURITY.md) before publishing your version.

## Contributing

Improvements and new theme ideas are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request.

## Credits

Created by **Meshtech254**.

- GitHub: (https://github.com/Meshtech254/my-crush_)


If you remix the template, a small credit is appreciated but not required by the license.

## License

Released under the [MIT License](LICENSE). You may use, modify, and share the template, including in personal and commercial projects, subject to the license terms.

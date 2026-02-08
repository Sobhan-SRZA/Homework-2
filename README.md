# 📚 Homework-2 Documentation

Welcome to the comprehensive documentation for **Homework-2**, a static portfolio website showcasing personal projects, primarily Discord bots developed using Node.js and JavaScript/TypeScript. This document explains the entire source code structure, features, and details in a GitHub-friendly format. It covers the website's setup, HTML/CSS implementation, and high-level overviews of the featured bot projects (based on descriptions in the code). Since this is a static site, there are no databases, commands (beyond deployment), or dynamic functions—everything is client-side HTML/CSS.

This project is deployed via GitHub Pages for easy hosting. Feel free to fork, contribute, or use it as a template! 🚀

## 🌟 Overview

Homework-2 is a simple, responsive portfolio website built with pure HTML and CSS. It highlights three Discord bot projects: Padio (radio player), TickerBoy (ticket manager), and PC Bot (multi-purpose bot). The site includes sections for projects, about us, and contact, with basic interactivity like a language selector and search bar (non-functional in this static version).

Key highlights:
- **Tech Stack**: HTML5, CSS3 (with custom fonts and animations).
- **Theme**: Green-toned design inspired by tech/nature themes.
- **Deployment**: Automated via GitHub Actions to GitHub Pages.
- **License**: MIT License (open-source and permissive).
- **No Backend**: Purely static—no JavaScript, databases, or server-side logic.

This site serves as a personal showcase. If you're looking to extend it, consider adding JavaScript for dynamic features like real language switching or search functionality.

## 🗂 Project Structure

The repository follows a clean, minimal structure for a static site. Here's the file tree:

```
Homework-2/
├── .gitignore                # Ignores compressed files like .zip, .rar, .tar.gz
├── .github/
│   └── workflows/
│       └── static.yml        # GitHub Actions workflow for deploying to GitHub Pages
├── fonts/
│   └── Vazir-Medium-FD-WOL.woff  # Custom Persian font (not included in provided source, assumed to exist)
├── images/                   # Folder for images (e.g., icons, project thumbnails)
│   ├── padio.png
│   ├── search-icon.webp
│   ├── ticker-boy.webp
│   ├── pc-bot.png
│   └── ... (other images referenced in HTML/CSS)
├── index.html                # Main HTML file: The entire website content
├── LICENSE                   # MIT License file
├── README.md                 # Basic README with social links and Discord widgets
├── style.css                 # All styling: Layout, animations, responsive design
```

- **Root Files**: Core files like HTML, CSS, and config.
- **Directories**:
  - `.github/workflows`: Handles CI/CD for deployment.
  - `fonts`: Custom font files for Persian text support.
  - `images`: Static assets for icons and project visuals.

Total files: ~10 (including workflow and assets). The site is lightweight and loads quickly.

## ⚙️ Features and Bot Descriptions

The website features a header with navigation, content sections, and a footer. Here's a breakdown:

### Website Features
- **Header Navigation** 📍: Includes logo, language selector (Persian/English/French—UI only, no content translation), and links to sections (#projects, #about-us, #contact).
- **Search Bar** 🔍: Animated search input that expands on hover/focus (pure CSS).
- **Projects Section** 🛠: Cards displaying bot projects with images, descriptions, and tech stacks.
- **About Us Section** ℹ️: Placeholder Lorem Ipsum text (customizable).
- **Contact Section** 📧: Simple email suggestion.
- **Footer** ©: Copyright notice.
- **Animations** ✨: Loading fade-in/scale for all divs; hover effects on cards/images.
- **Responsive Design** 📱: Adjusts for screens <600px (header becomes column layout).
- **Custom Scrollbar** 🖱: Green-themed for aesthetic consistency.
- **Font**: Uses 'Vazir' for Persian support, fallback to Arial/etc.

No JavaScript means no dynamic features—everything is styled via CSS.

### Featured Bot Projects (Based on Website Descriptions)
The site showcases three Discord bots. Since the actual bot source code isn't included, descriptions are derived from the HTML content. These are high-level overviews—assume they're Node.js-based bots for Discord.

1. **Padio - Discord Radio Player Bot** 🎵
   - **Description**: A high-performance bot that plays radio/music in Discord, creating enjoyable moments for hours.
   - **Features**:
     - Music playback with quality audio.
     - Likely supports commands for play, pause, queue, etc.
   - **Tech Stack**: Node.JS, JavaScript.
   - **Commands (Hypothetical based on typical bots)**:
     - `/play <url/song>`: Start playing music.
     - `/pause`: Pause current track.
     - `/skip`: Skip to next track.
     - `/queue`: View current playlist.
   - **Usage**: Invite to server, use slash commands for music management.

2. **TickerBoy - Ticket Management Bot** 🎟
   - **Description**: Handles ticket management in Discord servers, taking care of everything so you don't have to worry.
   - **Features**:
     - Ticket creation, assignment, and closure.
     - Moderation tools for support tickets.
   - **Tech Stack**: Node.JS, JavaScript.
   - **Commands (Hypothetical)**:
     - `/ticket create <reason>`: Open a new ticket.
     - `/ticket close`: Close current ticket.
     - `/ticket assign <user>`: Assign ticket to a moderator.
     - `/tickets list`: View open tickets.
   - **Usage**: Ideal for support servers; automates user queries.

3. **PC Bot - All-Purpose Discord Bot** 🤖
   - **Description**: Multi-functional bot that manages tickets and more (similar to TickerBoy but broader).
   - **Features**:
     - Ticket management + general utilities (e.g., moderation, fun commands).
     - Versatile for various server needs.
   - **Tech Stack**: Node.JS, JavaScript, TypeScript.
   - **Commands (Hypothetical)**:
     - `/help`: Show command list.
     - `/mod ban <user>`: Ban a user.
     - `/fun meme`: Generate a random meme.
     - `/ticket ...` (as above).
   - **Usage**: All-in-one for community servers.

**Note**: These bots are not part of this repository's code—they're referenced projects. For real bot implementation, you'd need Discord.js library, event handlers (e.g., `client.on('message')`), and a bot token.

## 📝 HTML Structure

The `index.html` is the core file. It's structured as a single-page app with sections:

- **<head>**: Meta tags, title, favicon, CSS link.
- **<body>**: Wrapped in `.container` div.
  - **.header**: Logo, language select, nav links, search bar.
  - **.content**: Sections for #projects (cards), #about-us (paragraphs), #contact.
  - **.footer**: Copyright.

Key Elements:
- Semantic sections (<section id="...">) for accessibility.
- Project cards: Each with <img>, <h4>, <p>, and tech spans.
- No forms or scripts—pure markup.

## 🎨 CSS Details

`style.css` handles all styling with modern CSS features:

- **Fonts**: @font-face for 'Vazir' (Persian support).
- **Reset**: * selector for box-sizing/margin reset.
- **Scrollbar**: Custom green theme.
- **Layout**: Flexbox for header/projects; grid implied via container.
- **Animations**: @keyframes 'loading' (scale/opacity fade-in) applied to all divs.
- **Hover Effects**: Transitions for colors, shadows, scales.
- **Media Query**: @media (max-width: 600px) for mobile header.
- **Classes**: .pointer (cursor), .projects--card (cards with tech tags).

No variables or preprocessors—plain CSS.

## 🔧 Commonly Used Functions/Patterns

Since this is static HTML/CSS:
- **No JavaScript Functions**: Pure markup. For dynamic bots (referenced), common patterns include:
  - Discord.js: `client.login(token)`, `client.on('ready')`, `client.on('interactionCreate')` for slash commands.
- **CSS Patterns**:
  - Transitions: `transition: all .5s ease-in-out;` (used extensively for hovers).
  - Flexbox: For layouts like .header and .projects--cards.
  - Pseudo-elements: For search bar animations.

Template for Bot Commands (Hypothetical for referenced bots):
- Slash Command Template: Using Discord.js Interactions API.
  ```js
  const { SlashCommandBuilder } = require('@discordjs/builders');

  module.exports = {
    data: new SlashCommandBuilder()
      .setName('play')
      .setDescription('Play a song'),
    async execute(interaction) {
      // Logic here
      await interaction.reply('Playing!');
    },
  };
  ```

## 🗄 Databases (Storage)

This static website has **no databases**—no storage, no backend. Everything is hardcoded in HTML.

For the referenced Discord bots (hypothetical based on typical setups):
- **Database Types**: Often MongoDB or SQLite for persistence.
- **Stored Data Examples**:
  - **Tickets Collection** (MongoDB Schema Example):
    ```json
    {
      "_id": ObjectId,  // Type: ObjectId
      "userId": "1234567890",  // Type: String (Discord user ID)
      "ticketId": 1,  // Type: Number
      "status": "open",  // Type: String (enum: 'open', 'closed')
      "createdAt": Date,  // Type: Date
      "messages": [  // Type: Array of Objects
        { "content": "Help needed", "author": "user123" }
      ]
    }
    ```
  - **Music Queue** (In-Memory or Redis Example):
    ```json
    {
      "guildId": "987654321",  // Type: String (Discord server ID)
      "queue": [  // Type: Array of Strings
        "https://youtube.com/song1",
        "https://youtube.com/song2"
      ],
      "currentTrack": "song1",  // Type: String
    }
    ```
- **No Storage in This Repo**: If adding bots, integrate Mongoose for MongoDB.

## 🚀 Setup and Commands

To run locally:
1. Clone the repo: `git clone <repo-url>`
2. Open `index.html` in a browser.

Deployment Commands (via GitHub):
- Push to main: Triggers `.github/workflows/static.yml` for GitHub Pages deploy.
- Manual: Use GitHub Actions tab to trigger workflow.

No npm/yarn commands—static site!

## 🤝 Contributing

Fork the repo, make changes, and PR! Issues welcome for improvements like JS integration or real bot code. 🌱

## 📜 License

MIT License—see [LICENSE](./LICENSE) for details.

---

Built with ❤️ by Sobhan-SRZA. Last updated: February 08, 2026. If this doc helps, star the repo! ⭐
# Kevin Nnorom — Portfolio

Personal portfolio of **Kevin Nnorom**, web developer and founder of **KEVTECH**. A fast, responsive, single-page site showing my services, projects and skills, with a contact form that sends messages straight to my inbox.

**Live site:** https://YOUR-SITE-URL

## Features

- Fully responsive layout that works on low-end phones and wide monitors
- Dark theme with smooth scroll animations (respects reduced-motion settings)
- Mobile menu and highlighted navigation for the current section
- Project cards with screenshots linking to live demos
- Contact form delivered by email through Web3Forms
- Floating WhatsApp button and social links
- Link-sharing preview tags (Open Graph)
- One HTML file with no build step and no dependencies

## Projects shown

| Project | Description | Link |
|---|---|---|
| **PhishGuard** | Phishing URL detector with a four-stage analysis pipeline and an explainable 0–100 risk score | [Live demo](https://phishguard-88dk.onrender.com/) |
| **Auto Grove Dealership** | Car buy-and-rent platform for a Lagos dealership with live inventory and WhatsApp enquiries | [Live demo](https://autogrovedealership.nnoromkevinjunior.workers.dev/) |

## Tech stack

HTML, CSS and vanilla JavaScript. Fonts: Space Grotesk, Inter and JetBrains Mono from Google Fonts.

## Project structure

```
.
├── index.html    # the whole site (HTML, CSS, JS, embedded screenshots)
├── preview.png   # 1200x630 image for link previews
└── README.md
```

## Run locally

Open `index.html` in a browser, or start a local server for more realistic testing:

```bash
py -m http.server 8000
```

Then visit http://localhost:8000. (On Mac/Linux, use `python3 -m http.server 8000`.)

## Contact form setup

The form uses [Web3Forms](https://web3forms.com). The access key is in the script at the bottom of `index.html`:

```js
var WEB3FORMS_KEY = 'your-access-key';
```

The key is safe to be public because it can only send email to the address it was created for. To use your own, get a free key at web3forms.com and replace it.

## Editing content

- **Projects:** edit the cards inside the `#projects` section
- **Stats:** edit the numbers in the hero section
- **Social links:** update the links in the hero and contact sections
- **Link preview:** upload `preview.png`, then add this inside `<head>` with your real address:
  ```html
  <meta property="og:image" content="https://YOUR-SITE-URL/preview.png">
  ```

## Deployment

Hosted as a static site on Cloudflare. Upload `index.html` and `preview.png` (Workers static assets or Pages), or connect this repository for automatic deploys on every push.

## Contact

- Email: nnoromkevinjunior@gmail.com
- WhatsApp: https://wa.me/2349052995396
- GitHub: https://github.com/Kevin2008101
- Instagram: https://www.instagram.com/kevte_ch
- TikTok: https://www.tiktok.com/@kevin12869
- LinkedIn: https://www.linkedin.com/i

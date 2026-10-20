# C Thejaswini | Personal Portfolio Website

A responsive personal portfolio for a B.Tech Computer Science & Engineering student, built for an HTML & CSS internship project.

**This project uses HTML and CSS only.** There is no JavaScript, no framework, no build step and no backend.

## Overview

A single-page site with a deep navy-charcoal theme, off-white text and one teal accent colour, plus an off-white Projects section for contrast. All details come from the resume of C Thejaswini.

## Technologies used

- HTML5 (semantic elements)
- CSS3 (custom properties, Grid, Flexbox, media queries, `aspect-ratio`, `object-fit`)

## Features

- Sticky header with CSS-only navigation and a "Let's Connect" button
- Hero with the profile photo (rounded rectangle on desktop, circle on phones), name, tagline, "Explore My Projects" and "View GitHub" buttons, and a quick-stats card that sits below the photo
- About section with facts, interests, coursework, and education / learning timelines
- Skills grouped into editable chip cards
- One "My Projects" section: three equal cards with the same layout
- A highlighted "More Code on My GitHub" banner right after the project cards
- Contact section with email, GitHub and LinkedIn links
- Footer with name and tagline, quick links, GitHub / LinkedIn / email links, copyright and back-to-top
- Skip link, visible keyboard focus, descriptive links, alt text, `prefers-reduced-motion` support
- Works from 320 px phones to large desktops, with no horizontal scrolling

## Folder structure

```
portfolio-project/
├── index.html
├── style.css
├── images/
│   └── profile.jpeg
├── screenshots/
│   └── README.txt
└── README.md
```

## Open the site locally

Double-click `index.html`. It opens in any modern browser. Nothing needs to be installed.

## Edit your skills

In `index.html`, find the comment **`EDIT YOUR SKILLS HERE`** (inside the Skills section).

- **Add a skill:** copy a line like `<li class="chip">Python</li>`, paste it inside the group you want, change the text.
- **Remove a skill:** delete its `<li>` line.
- **Rename a group:** edit the text in its `<h3>`.
- **Add a group:** copy a whole `<article class="skill-card"> ... </article>` block.

Save, then refresh the browser. The small tags in the hero (React.js, JavaScript, Python, Responsive design) are separate; edit them under the `HERO TAGS` comment.

## Replace personal details

Everything is plain text in `index.html`. Search for these to update them:

- Name: `C Thejaswini`
- College and degree: `VEMU Institute of Technology`, `B.Tech`
- Years, CGPA and percentages: About section and timelines
- Email: `thejaswini1707@gmail.com` (appears in the `mailto:` link and its text)
- GitHub: `github.com/thejaswini1707`
- LinkedIn: `linkedin.com/in/theja-swini-c-826176377`
- Profile photo: replace `images/profile.jpeg` with your own file of the same name (portrait, 3:4 ratio works best). It is used in the hero only; the crop is controlled by `object-position` on `.hero-photo img` in `style.css`.
- Copyright year: search for `&copy; 2026` in the footer and update it each year (there is no JavaScript to do this automatically)
- Colours: change the values under `:root` at the top of `style.css` (`--accent` is the teal; `--bg` is the navy)

## Add projects and links

- Copy an entire `<article class="project"> ... </article>` block and edit the text. All projects use the same card, so they stay equal.
- Each card has a commented-out `PROJECT LINKS` block. Remove the `<!--` and `-->` and replace `PASTE-REPO-URL` / `PASTE-LIVE-URL` with your real URL. Delete any link that does not exist.
- The "More Code on My GitHub" banner sits right after the project cards (`class="github-cta"`).
- Only add links to repositories or live sites that really exist.
- Each card preview is a simple CSS label. To use a real screenshot, save it as `images/learnmate.png`, `images/packcheck.png` or `images/vemu-portal.png`; it covers the label automatically. Until the files exist, a small CSS rule (`.project-img::after`) hides the browser's broken-image icon; you can delete that rule once all three images are added.

## Browser testing checklist

- [ ] Chrome, Edge, Firefox and Safari (latest versions)
- [ ] Phone width (about 320-375 px), tablet (about 768 px), laptop (about 1280 px), large screen (1920 px)
- [ ] No horizontal scrollbar at any width
- [ ] Every navigation link jumps to the right section
- [ ] Tab through the page: every link shows a visible focus outline
- [ ] Turn on "reduce motion" in your OS: animations stop, content still shows
- [ ] `mailto:`, GitHub and LinkedIn links open correctly

## Screenshot checklist

- [ ] Desktop, tablet and mobile captures saved in `screenshots/`
- [ ] Captures are real browser screenshots of your finished site

## Optional: host on GitHub Pages

1. Create a repository on GitHub and upload all files, keeping `index.html` at the top level.
2. Go to **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
4. After a minute or two, the site appears at `https://<your-username>.github.io/<repo-name>/`.

## Before you submit

Check that all details in `index.html` are correct and current, add real project links if you have them, add your own photo, and add real screenshots.

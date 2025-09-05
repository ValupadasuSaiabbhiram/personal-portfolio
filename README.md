# Sai Abbhiram — Portfolio Website

> Personal portfolio website showcasing projects, skills, and contact information.

---

## Table of Contents

* [About](#about)
* [Demo](#demo)
* [Built With](#built-with)
* [Features](#features)
* [Project Structure](#project-structure)
* [Getting Started](#getting-started)

  * [Prerequisites](#prerequisites)
  * [Install](#install)
  * [Run Locally](#run-locally)
  * [Build for Production](#build-for-production)
* [Resume / CV](#resume--cv)
* [Deployment](#deployment)
* [Contributing](#contributing)
* [License](#license)
* [Contact](#contact)

---

## About

This repository contains the source code for **Sai Abbhiram**'s personal portfolio website. It presents projects, skills, certificates, and contact information — designed to be lightweight, responsive, and easy to deploy.

## Demo

[click here to check out demo](https://saiabbhiram-portfolio.vercel.app/)

![Website UI Preview](/public/screenshot/screenshot.png)

## Built With

* Vite (React)
* React
* Tailwind CSS
* Node.js

> See `package.json` for exact dependency versions.

## Features

* Home / About section
* Projects gallery with links to repositories and demos
* Contact form (mailto or integrated form endpoint)
* Downloadable resume (stored in `public/resume/`)
* Responsive layout and accessible components

## Project Structure

```
public/
  └─ resume/                 # Place resume PDF(s) here (served at /resume/...)
src/
  ├─ components/             # React components (AboutSection, ContactSection, etc.)
  ├─ assets/                 # Images, icons, and other static assets
  └─ pages/                  # Page-level components

package.json
vite.config.js
README.md
```

## Getting Started

Follow these instructions to get a local copy running.

### Prerequisites

* Node.js (v16 or later recommended)
* npm or Yarn

### Install

```bash
# clone repository
git clone <repo-url>
cd personal-portfolio

# install dependencies
npm install
# or
# yarn
```

### Run Locally

```bash
# start dev server
npm run dev
```

Open `http://localhost:5173` (or the port Vite reports) in your browser.

### Build for Production

```bash
npm run build
npm run preview  # to locally preview the production build
```

## Resume / CV

Your resume(s) should be placed in `public/resume/`. Files inside `public/` are served from the root of the site, so a file placed at `public/resume/resume.pdf` will be available at:

```
/resume/resume.pdf
```

To link it from React, use an absolute path from the root, for example:

```jsx
<a href="/resume/resume.pdf" download>Download CV</a>
```

If you'd rather open in a new tab instead of forcing download, remove the `download` attribute and add `target="_blank" rel="noopener noreferrer"`.

## Deployment

Common deployment options:

* **Vercel** — excellent for Vite/React projects; connect your GitHub repo and deploy
* **Netlify** — drag & drop or connect repo; set build command `npm run build` and publish directory `dist`
* **GitHub Pages** — use `gh-pages` or GitHub Actions to deploy the `dist` folder

## Contributing

Contributions are welcome. Suggested workflow:

1. Fork the repo
2. Create a feature branch: `git checkout -b feat/my-change`
3. Commit your changes: `git commit -m "feat: short description"`
4. Push to your branch and open a PR

Keep commit messages clear and follow the conventional style used in the project (e.g. `feat:`, `fix:`, `chore:`).

## License

Include a license file if you want to share this project publicly (for example, MIT). If you don't want to include a license yet, mention that the repo is `All rights reserved`.

## Contact

Sai Abbhiram Valupadasu

* Location: Hyderabad, India
* Email: valupadasusaiabbhiram@gmail.com
* LinkedIn: https://www.linkedin.com/in/sai-abbhiram-valupadasu/
* GitHub: https://github.com/ValupadasuSaiabbhiram

---

*Last updated: 2025-09-05*

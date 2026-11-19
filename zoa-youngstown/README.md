# ZOA Youngstown Chapter Website

Simple, clean single-page site ready to go live quickly.

## Files
- `index.html` — the entire website (edit this file to change any text)
- `logo.svg` — place the official ZOA logo here (see below)

## 1. Add the official ZOA logo
1. Download the official logo from:
   https://commons.wikimedia.org/wiki/File:Zionist_Organization_of_America_logo.svg
2. Save it as `logo.svg` in the same folder as `index.html`.
3. (Alternative) You can use a PNG version if preferred — just rename the `src` in the HTML.

## 2. Connect the subscription form so data is stored in a table (recommended)

### Option A – Google Form + Google Sheet (easiest & free)
1. Go to https://forms.google.com and create a new form.
2. Add these required questions (Short answer):
   - Full Name
   - Phone
   - Street Address
   - City
   - State
   - ZIP Code
3. Click **Responses** → **Link to Sheets**. This creates your data table.
4. Click **Send** → **Embed** (or get the form link).
5. In `index.html`, replace the entire `<form id="subscribe-form">...</form>` block with the Google Form embed code.
6. In Google Forms settings, set the confirmation message to:
   > Thank you for subscribing. We will send you a handwritten letter with further instructions.

You will then see every submission in the linked Google Sheet and can download it as Excel/CSV anytime.

### Option B – Formspree (also free tier)
1. Sign up at https://formspree.io
2. Create a new form and copy the endpoint (looks like `https://formspree.io/f/xxxxxxxx`)
3. Change the form tag in `index.html` to:
   ```html
   <form action="https://formspree.io/f/YOUR_ID" method="POST">
   ```
4. Formspree will email you the submissions and you can export them.

## 3. Put the site live (takes a few minutes)

### Easiest free options:
- **Netlify Drop**: Go to https://app.netlify.com/drop → drag the whole folder. Instant live URL.
- **GitHub Pages**: Create a repo, upload the files, turn on Pages.
- **Cloudflare Pages**: Similar one-click deploy.

You can later point a custom domain (e.g. youngstownzoa.org or zoayoungstown.org) to it.

## 4. Editing later
Open `index.html` in any text editor (Notepad, VS Code, etc.).  
All important text is clearly written — change the About paragraph, goals list, contact details, or form labels as needed. No special tools required.

## Contact placeholders
In the Contact section you will see example email/phone. Just replace those lines with the real chapter details when ready.

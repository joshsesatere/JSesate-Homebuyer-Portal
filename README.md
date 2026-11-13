# Joshua Sesate Homebuyer Portal

A responsive, multi-page static website starter for a Southern California real estate buyer portal.

## Included pages
- `index.html` — homepage
- `buyer-process.html` — buying process overview
- `resources.html` — buyer education center
- `buyer-registration.html` — buyer inquiry / qualification form
- `about.html` — advisor profile
- `contact.html` — contact information
- `404.html` — not-found page

## Run locally
Open `index.html` in a browser. For a local web server, run:
```bash
python -m http.server 8000
```
Then visit `http://localhost:8000`.

## Deploy to Cloudflare Pages for free
1. Create a GitHub repository (for example, `joshua-sesate-homebuyer-portal`).
2. Upload the contents of this folder to the repository root. Do not upload the outer ZIP itself.
3. In Cloudflare Dashboard, open **Workers & Pages** → **Create** → **Pages** → **Connect to Git**.
4. Select the repository and production branch (`main`).
5. For this plain HTML/CSS/JS site, leave the build command blank and set the build output directory to `/` (or `.` if the UI requires a relative directory).
6. Deploy. Future pushes to the connected branch will trigger new deployments.

## Lead form setup — important
The included buyer registration form is a safe starter/demo. It opens the visitor's email application with the submitted fields prefilled; it does **not** store leads in a database or send them automatically.

Before public launch, replace this behavior with a real form endpoint or embed a Google Form/Jotform/approved CRM form. Configure the destination account yourself, test submissions, and publish a privacy notice that accurately describes what is collected, where it goes, retention, and how users can request access/deletion. Do not collect Social Security numbers, bank account numbers, passwords, or sensitive loan documents through this basic website.

## Customization
- Colors, typography, layout, and responsive styles: `assets/styles.css`
- Navigation and shared page footer are repeated in each HTML page.
- Mobile menu and starter form behavior: `assets/site.js`
- Update business details only after verifying current brokerage-approved advertising wording.

## Before publishing
- Have the responsible broker review the website and all advertising/disclosures.
- Confirm the required California DRE and brokerage identification/disclosures and any required fair housing / equal housing language.
- Review privacy, accessibility, security, and communications-consent requirements.
- Do not imply MLS/IDX access or real-time listing availability. No IDX feed is included.
- Verify all links, phone/email, forms, and mobile layouts.

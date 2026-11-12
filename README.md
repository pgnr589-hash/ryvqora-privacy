# RYVQORA AI — Privacy website

This repository contains static public pages for the RYVQORA AI privacy policy and data-deletion instructions.

## Files
- `index.html` — landing page
- `privacy-policy/index.html` — privacy policy
- `data-deletion/index.html` — user-facing deletion instructions
- `style.css` — shared styling

## Publish with GitHub Pages
1. Create a **public** repository named `ryvqora-privacy` under the GitHub account that owns the username `ryvqora-privacy` (if that is your actual username).
2. Upload all files and folders from this ZIP to the repository's top level. Do not upload the enclosing `ryvqora-privacy-site` folder itself.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch **main** and folder **/(root)**, then save.
6. Wait for the Pages deployment to finish.
7. Open and test:
   - `https://ryvqora-privacy.github.io/ryvqora-privacy/`
   - `https://ryvqora-privacy.github.io/ryvqora-privacy/privacy-policy/`
   - `https://ryvqora-privacy.github.io/ryvqora-privacy/data-deletion/`

If `ryvqora-privacy` is not your GitHub username, replace that part of the URLs with your actual username.

## Meta setup
- In Meta for Developers, open **App settings → Basic**.
- Set **Privacy Policy URL** to the exact published HTTPS privacy-policy URL.
- Save changes and open the URL in a private/incognito browser window to confirm it is publicly accessible.
- Use the data-deletion instructions URL only for a setting that asks for a user-facing deletion/instructions URL.
- If Meta asks for a **Data Deletion Callback URL**, this static site is not enough. Implement a secure backend callback endpoint that follows Meta's current documentation.

## Before publishing — accuracy checklist
The policy is a starter draft based on the information supplied that integration tokens are stored locally. Review it against the actual app build and update it if needed:
- Confirm where tokens, drafts, logs, media, and settings are stored.
- Confirm which social permissions and AI providers are used.
- Explain any server, analytics, crash-reporting, or cloud services if the app uses them.
- Confirm how users can actually disconnect accounts and clear local data.
- Make sure the contact email is one you are comfortable publishing publicly.
- Do not claim encryption, deletion timelines, or “no sharing” unless verified.

GitHub Pages hosts static pages; it does not run a backend or process Meta callback POST requests.

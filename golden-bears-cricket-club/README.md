# Golden Bears Cricket Club website

A customised, bilingual (English/Swedish), mobile-friendly club website based on the structure and open-source Jekyll Club Website template:
https://github.com/sdhutchins/jekyll-club-website

This starter is prepared for free GitHub Pages hosting. It includes:
- Home page and club introduction
- Youth team/programme overview (U9/U11/U13/U15 are editable placeholders; confirm actual groups)
- Fixtures and results page with clearly marked empty states
- News and announcements page
- Player/parent registration page (Google Forms link placeholder)
- Sponsors and support page
- English/Swedish language switcher
- Responsive mobile navigation

## 1. Create the GitHub repository

1. Sign in to GitHub using an account controlled by the club.
2. Create a **public** repository named `YOUR-USERNAME.github.io` (replace YOUR-USERNAME with the club's GitHub username).
3. Upload the contents of this project ZIP to the repository root. Do not upload the enclosing ZIP folder.
4. Commit to the `main` branch.

The resulting address will be `https://YOUR-USERNAME.github.io/`.

## 2. Enable GitHub Pages

1. Open repository **Settings → Pages**.
2. Under **Build and deployment**, select **Deploy from a branch**.
3. Select branch `main` and folder `/ (root)`.
4. Save. GitHub Pages will build and publish the site. The first deployment may take a few minutes.
5. Visit `https://YOUR-USERNAME.github.io/`.

GitHub Pages documentation: https://docs.github.com/en/pages

## 3. Club-specific setup before launch

Search and replace these placeholders:
- `ADD-CLUB-EMAIL` with the club's public contact email.
- `https://docs.google.com/forms/` in `join.md` with the actual Google Form URL.
- Update `_config.yml` if the GitHub Pages URL or repository arrangement changes.
- Confirm the actual youth age groups, training details and season information.
- Add approved club logo, photos and sponsor logos (obtain permission first).
- Replace the GB monogram with the club's approved logo if available.

## 4. Updating content

- Edit `teams.md` for teams and youth programmes.
- Edit `fixtures.md` for upcoming fixtures and verified results.
- Add dated Markdown posts under `_posts/` using the `post` layout; they will appear automatically on the News page.
- Edit `sponsors.md` for partner details.
- Edit `join.md` for the registration link and contact information.

For a simple volunteer workflow, use GitHub's web editor: open a file, click the pencil icon, make the change and commit it.

## 5. Registration and privacy

The registration button is only a placeholder until the club creates and links its own form. For under-18 players, a parent/legal guardian should submit the form. Collect only information the club genuinely needs, restrict access to responses, publish a privacy notice, set a retention period, and confirm appropriate GDPR/legal basis and guardian consent arrangements. Do not publish player contact details, birth dates, medical details or other personal data on the public website.

Google Forms: https://forms.google.com/

## 6. Local preview (optional)

Install Ruby and Bundler, then run:
```bash
bundle install
bundle exec jekyll serve
```
Open http://localhost:4000.

## 7. Licensing and attribution

The original Jekyll Club Website template is published under the MIT License. Review the original repository's LICENSE and retain its copyright and licence notice when reusing its code. This customised starter contains original club-specific copy and styling; it is not an official release from the original template author.

Original template: https://github.com/sdhutchins/jekyll-club-website

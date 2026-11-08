# Portfolio maintenance guide

This repository is the live GitHub Pages portfolio for **MrNullbyte01**.

Website files:
- `index.html` — portfolio page content and project cards
- `styles.css` — responsive styling
- `script.js` — footer year
- `assets/` — current profile photo, certificate files, and portfolio screenshots
- `README.md` — GitHub repository overview
- `projects/README.md` — index of dedicated project repositories

## Update the website

1. Edit the relevant file in this repository.
2. Keep local asset paths and filenames in sync with the files in `assets/`.
3. Preview the page at desktop and mobile widths.
4. Check every navigation link, project link, image, and contact link.
5. Commit the change to `main` after review.
6. Check the GitHub Pages deployment status in the repository's Actions / Pages settings.

Do not upload a replacement starter ZIP over the live repository; update only the files that actually need changing.

## Current profile photo

The website currently loads:

`assets/profile-photo.jpeg`

To replace it, upload the new image using this exact filename or update the image path in `index.html`. Check the crop on mobile and desktop before committing.

## Current education document

The website currently displays:

- `assets/Texnoera-Diploma.jpg`

The PDF copy is also stored as `assets/Texnoera-Diploma.pdf`. If replacing the certificate image, keep the filename or update both the link and image source in `index.html`.

## Project repositories

Project-specific files are kept in their own repositories rather than duplicated in the portfolio website:

- [NULL Motherboard](https://github.com/MrNullbyte01/NULL-Motherboard)
- [Cisco Networking Labs](https://github.com/MrNullbyte01/Cisco-Networking-Labs)
- [Raspberry Pi Cyberdeck](https://github.com/MrNullbyte01/Raspberry-Pi-Cyberdeck)
- [BlackBerry Passport Revival](https://github.com/MrNullbyte01/BlackBerry-Passport-Revival)
- [CTF Writeups](https://github.com/MrNullbyte01/CTF-Writeups)

Update the portfolio project card and the repository README when a project's status changes. Never describe a design as fabricated, a device as tested, or a course as certified unless there is evidence.

## Training and certification accuracy

- List a course as completed only when it has actually been completed.
- List a certification as earned only after the credential has been issued.
- CCNA preparation is not the same as holding a CCNA certification.
- Keep self-assessed language levels labelled as self-assessed.

## Final review checklist

- [ ] All local image paths point to files that exist.
- [ ] Navigation anchors work.
- [ ] External links point to the intended repositories and profiles.
- [ ] The profile image and certificate image load.
- [ ] Project descriptions match the current repository contents.
- [ ] No secrets, API keys, passwords, private keys, or personal device identifiers are present.
- [ ] Desktop and mobile layouts remain readable.

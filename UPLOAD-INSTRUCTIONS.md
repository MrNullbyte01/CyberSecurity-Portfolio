# Portfolio refresh — upload instructions

This package is a replacement starter version for your existing GitHub Pages repository.

## Files
- `index.html` — portfolio website
- `styles.css` — responsive dark cybersecurity styling
- `script.js` — current year in footer
- `README.md` — GitHub repository/profile portfolio text
- `assets/` — photo and diploma placeholders
- `projects/` — folders for Packet Tracer labs, Raspberry Pi cyberdeck, BlackBerry Passport, and CTF write-ups

## How to publish
1. Download and extract the ZIP.
2. Open your repository: https://github.com/MrNullbyte01/CyberSecurity-Portfolio
3. Upload/replace the files in the repository root, preserving the `assets/` and `projects/` folders.
4. Commit the changes to the branch configured for GitHub Pages (usually `main`).
5. Wait for GitHub Pages to rebuild, then check https://mrnullbyte01.github.io/CyberSecurity-Portfolio/.

## Replace your photo
- Replace `assets/profile-photo-placeholder.svg` with your real photo file, preferably named `profile-photo.jpg`.
- In `index.html`, change the profile image path to `assets/profile-photo.jpg`.
- Only publish a photo you are comfortable making public.

## Add your diploma photo
- Add a photo named `assets/texnoera-diploma.jpg`.
- In `index.html`, change the diploma image path from `assets/texnoera-diploma-placeholder.svg` to `assets/texnoera-diploma.jpg`.
- Hide any ID number, certificate serial number, QR code, or other details you do not want publicly indexed before uploading.

## Add Packet Tracer labs
- Put `.pkt` files and screenshots inside `projects/packet-tracer-labs/`.
- Update the table in `README.md` with each lab's actual name and status.

## Important accuracy notes
- The Ethical Hacking course status is worded cautiously. Update it to "Completed" only if you finished it and received the credential.
- Do not add CCNA as an earned certification unless you have passed the exam.
- Project cards are labelled in progress / documentation pending where full details were not supplied.
- The LinkedIn URL is normalised to remove tracking parameters.

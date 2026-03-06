# Handwerker & Blitz – one-page website

## 1) Deploy to GitHub Pages
1. Create a new GitHub repository.
2. Upload all files from this project to the repository root.
3. Commit and push.
4. In GitHub: **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select the branch (usually `main`) and folder `/ (root)`.
7. Save. After a short moment, GitHub Pages will publish the site.

## 2) Add portfolio images and edit `portfolio.json`
1. Put your before/after images into `/images/portfolio/`.
2. Open `portfolio.json`.
3. Add a new object using the same structure as the existing examples:
   - `title`
   - `category` (use one of: `Küche`, `Möbel`, `Boden`, `Türen & Leisten`, `Montage`, `Garten`, `Reparaturen`)
   - `city`
   - `beforeImage`
   - `afterImage`
   - `description.de`, `description.ru`, `description.en`
4. Make sure the file paths match your image names exactly.
5. Commit and upload the updated files.

## 3) Replace the Google reviews link later
Right now the reviews button uses a placeholder link:
- `https://example.com/google-business-profile`

To replace it:
1. Open `index.html`.
2. Search for `example.com/google-business-profile`.
3. Replace it with your real Google Business Profile reviews link.
4. Save and upload the file again.

## Notes
- Theme choice is saved in `localStorage`.
- Language choice is saved in `localStorage`.
- The portfolio is loaded from `portfolio.json` on the client side.
- No analytics, no tracking scripts, no external JS libraries.

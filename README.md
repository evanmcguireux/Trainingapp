# BarryP Tri Build - Flat Netlify Version

This version has no folders or subfolders. Upload the files directly into the root of a GitHub repository.

## Files

- `index.html` - the complete app, including HTML, CSS and JavaScript
- `netlify.toml` - tells Netlify to publish the repository root
- `README.md` - this guide

## Deploy on Netlify from GitHub

1. Create a new GitHub repository.
2. Upload these files directly into the repository root.
3. In Netlify, choose **Add new site** then **Import an existing project**.
4. Select the repository.
5. Use these Netlify build settings if asked:
   - Build command: leave blank
   - Publish directory: `.`
6. Deploy.

## Notes

This is a static single-page app. It uses browser `localStorage` to save your pain, stiffness and flare logs on the device you use.

This app is training-planning software, not medical advice. If Achilles pain is sharp, worsening, swollen, causing altered gait, or present at rest, stop running and seek professional medical assessment.

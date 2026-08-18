# BarryP Tri Build - Flat Netlify Fixed Version

This version has no folders or subfolders. Upload these files directly into the root of a GitHub repository.

## Files

- `index.html` - the complete app, including HTML, CSS and JavaScript
- `package.json` - includes a harmless `npm run build` script so Netlify does not fail if the UI has `npm run build` saved
- `netlify.toml` - publishes the repository root
- `README.md` - this guide

## Why this fixes the Netlify error

Your Netlify log showed Netlify was still running `npm run build` from the Netlify UI. The previous flat version had no `package.json`, so Netlify failed before deployment. This version includes a minimal `package.json` with a build script that succeeds without generating a build folder.

## Netlify settings

If Netlify asks manually, use:

- Build command: `npm run build`
- Publish directory: `.`

If you prefer, you can also remove the build command in the Netlify UI later, but this package works even if `npm run build` remains set.

## Notes

This is a static single-page app. It uses browser `localStorage` to save your pain, stiffness and flare logs on the device you use.

This app is training-planning software, not medical advice. If Achilles pain is sharp, worsening, swollen, causing altered gait, or present at rest, stop running and seek professional medical assessment.

# Splash Engine V5

GitHub Pages-ready repo structure for the Splash prompt generator.

## Deploy
1. Upload all files in this folder to your GitHub repo root.
2. Keep `index.html` in the repo root.
3. In GitHub, go to **Settings → Pages**.
4. Set source to **Deploy from branch**.
5. Choose your main branch and `/root`.
6. Save.

## Structure
- `index.html` → live app entry file
- `version.json` → current release metadata
- `versions/v1.0.0/index.html` → version snapshot backup
- `.nojekyll` → avoids GitHub Pages processing issues

## Update flow
- Replace root `index.html` with the new build
- Duplicate the same file into a new folder under `versions/`
- Update `version.json`

## Notes
This build keeps imports, resources, generator logic, and fixed randomizer/original mode behavior in one standalone HTML file.

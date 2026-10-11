# F1 Live Centre — Free Public Website

A static, F1-app-inspired fan dashboard designed for GitHub Pages. It reads timing data from a community-run F1 live API, so this site does not require your computer to remain on and does not require OpenF1 credentials.

## What it shows

- Live timing tower: positions, gaps, team names/colours, tyre compound and stint where supplied
- Session status, lap count, fastest lap, weather, race-control messages and pit activity where supplied
- Automatic refresh every 15 seconds
- Mobile-friendly layout

## Important limitations

- Data comes from the community API at `https://f1-live-api.onrender.com`, not from an official Formula 1 service. The API is operated by a third party and may change, go offline, or be unavailable during a session.
- Its hosted instance is on Render; free services can sleep after inactivity and may take about a minute to wake. The first load may therefore be slow.
- This API is not a guaranteed service. Verify it during a practice or qualifying session before relying on it for a race.
- Data availability may vary outside active sessions, and some values can be missing.
- The site is public because you chose “anyone with the link.” GitHub Pages requires a public repository on GitHub Free. Do not add passwords, tokens, or private information to this repository.
- This is an unofficial fan project and is not affiliated with Formula 1.

## Publish with GitHub Pages (free)

1. Download and extract this ZIP.
2. Open https://github.com/new and create a repository named `f1-live-centre`. Set it to **Public**. Do not add a README or `.gitignore` during creation.
3. On the new repository page, choose **Add file → Upload files**.
4. Upload `index.html`, `README.md`, and `.nojekyll` from this folder. Upload the files themselves, not the ZIP file and not the parent folder.
5. Click **Commit changes**.
6. Open the repository's **Settings → Pages**.
7. Under **Build and deployment**, choose **Deploy from a branch**. Select branch `main` and folder `/ (root)`, then click **Save**.
8. Wait for GitHub Pages to publish. The URL will usually look like `https://YOUR-GITHUB-USERNAME.github.io/f1-live-centre/`.
9. Open the URL and test the dashboard. Share that URL with your friends.

## API source

Community API repository and documentation: https://github.com/harsh779/f1-live-api
API instance: https://f1-live-api.onrender.com

The dashboard queries `/status`, `/timing`, `/weather`, `/race-control`, and `/pits` at 15-second intervals to reduce load on the public API.

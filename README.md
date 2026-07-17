# Gridiron Command

Gridiron Command is a single-player American football game designed for iPhone, iPad, and desktop browsers. Choose a team, call offensive and defensive plays, manage downs and field position, and play a complete four-quarter game against the computer.

## Play locally

Open `index.html` in a modern browser. Some browsers restrict offline/PWA features when opening files directly, but the game itself still runs.

## Publish with GitHub Pages

1. Create a new public GitHub repository, such as `gridiron-command`.
2. Upload every file and folder from this project to the repository root.
3. Open the repository's **Settings**.
4. Select **Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select the `main` branch and `/ (root)`, then save.
7. GitHub will display the public site address after deployment.

The usual address format is:

`https://YOUR-USERNAME.github.io/gridiron-command/`

## Install on iPhone

1. Open the GitHub Pages address in Safari.
2. Tap Safari's Share button.
3. Tap **Add to Home Screen**.
4. Launch Gridiron Command from its new icon.

The included web app manifest and service worker let the game behave like an installed web app and cache its files for offline use after the first successful visit.

## Project files

- `index.html` — complete game, graphics, interface, and game logic
- `manifest.webmanifest` — installable web-app configuration
- `service-worker.js` — offline caching
- `icons/` — iPhone and PWA icons
- `.nojekyll` — prevents unnecessary Jekyll processing on GitHub Pages

## Updating the game

After editing files, change `CACHE_NAME` in `service-worker.js` from `gridiron-command-v1` to a new value such as `gridiron-command-v2`. This forces installed copies to download the updated files.

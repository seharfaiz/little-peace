# A Little Place Called Mine ♡
A private Next.js site. Everything you write stays in your own browser (localStorage). No servers, keys or accounts.

## Run on Windows (PowerShell)
1. Install Node.js LTS from https://nodejs.org (restart PowerShell afterwards). Check: `node -v`
2. Extract and start:
```
Expand-Archive "$HOME\Downloads\a-little-place-called-mine.zip" -DestinationPath "$HOME\Documents"
cd "$HOME\Documents\little-place"
npm install
npm run dev
```
3. Open http://localhost:3000

## Check and build
```
npm run lint
npm run build
npm start
```
## Deploy free (Vercel)
Push the folder to a GitHub repo, sign in at vercel.com with GitHub, choose "Add New Project", import the repo, click Deploy. Netlify and Cloudflare Pages also work.

## Troubleshooting
- "npm is not recognized": reinstall Node.js and reopen PowerShell.
- Scripts blocked: run `Set-ExecutionPolicy -Scope CurrentUser RemoteSigned`.
- Port busy: `npm run dev -- -p 3001`.
- Writing disappeared: browser data was cleared; it lives only on that browser and device.

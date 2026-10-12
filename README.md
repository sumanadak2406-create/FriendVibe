# FriendVibe — free friend quiz website

A mobile-friendly Bengali quiz creator built with plain HTML, CSS and JavaScript. No build tools or paid APIs required.

## Run locally
Open `index.html` in a browser, or run a local server:
```bash
python -m http.server 8000
```
Then open `http://localhost:8000`.

## Publish free with GitHub Pages
1. Create a GitHub account and a new public repository.
2. Upload `index.html`, `style.css`, `app.js`, and `README.md` to the repository root.
3. Open repository **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
5. After publishing, your website will be available at the GitHub Pages URL shown there, with HTTPS.

Alternative: create a new project in Cloudflare Pages or Netlify and deploy these static files.

## Important limitations
- This is a working front-end MVP. Quiz data is encoded into the share URL, so quiz creation and answering work without a server.
- **Responses are not stored or aggregated across devices.** To collect all friends' answers and show the creator a shared results dashboard, connect a backend such as Supabase and add database tables, Row Level Security, and server-side validation.
- Because quiz contents are stored in the URL, keep the quiz to non-sensitive information. Do not include passwords, private details, or other people's personal data.
- Results are for entertainment only, not a real assessment of trust or friendship.
- The quiz URL grows as you add questions. Keep the number of questions and answer lengths reasonable.

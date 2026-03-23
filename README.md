# Why Am I Broke? 💸
> A brutally honest AI-powered money diagnosis tool

Most finance apps tell you **what** you spent. This tool tells you **what's actually wrong** — and gives you one specific action to fix it this week.

---

## What it does

You enter 8 simple numbers about your income and spending. The tool:

1. Breaks down your spending into a visual chart
2. Identifies your **#1 money leak**
3. Gives you a blunt, personalised AI diagnosis
4. Suggests **one concrete action** you can take this week

No sign up. No data stored. No fluff.

---

## Live Demo

🔗 [whyambroke.vercel.app](https://whyambroke.vercel.app)

---

## Tech Stack

| Layer | Tool |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| AI | Claude API (Anthropic) |
| Hosting | Vercel (free tier) |
| Backend | None needed |

---

## Run it locally

**Step 1 — Clone the repo**
```bash
git clone https://github.com/yourusername/why-am-i-broke.git
cd why-am-i-broke
```

**Step 2 — Add your API key**

Open `why-am-i-broke.html` in any text editor and find this line:
```js
const API_KEY = "YOUR_API_KEY_HERE";
```
Replace `YOUR_API_KEY_HERE` with your Anthropic API key from [console.anthropic.com](https://console.anthropic.com).

**Step 3 — Open in browser**

Just double-click the HTML file. No server, no install, no terminal commands needed.

---

## Deploy to Vercel

1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com) and sign in with GitHub
3. Click **New Project** → select this repo
4. Click **Deploy**

Your tool is live in 60 seconds. ✅

---

## Project Structure

```
why-am-i-broke/
│
├── why-am-i-broke.html   ← The entire app (one file)
└── README.md             ← You are here
```

---

## How the AI works

When the user clicks "Diagnose My Money", the app:

1. Collects all the input values from the form
2. Builds a structured prompt with the financial data
3. Sends it to the Claude API (`claude-sonnet-4-20250514`)
4. Parses the response into a **Diagnosis** and an **Action**
5. Displays it instantly — no page reload

The AI is prompted to be specific, blunt, and use the actual numbers — not give generic advice.

---

## Important — API Key Safety

⚠️ **Never commit your API key to GitHub.**

Before pushing to GitHub, make sure your key is replaced back with the placeholder:
```js
const API_KEY = "YOUR_API_KEY_HERE";
```

For production, use an environment variable or a serverless function to protect your key.

---

## Roadmap

- [ ] Add currency selector (USD, EUR, GBP)
- [ ] Monthly comparison (track progress over time)
- [ ] Shareable result card (image)
- [ ] Dark / light mode toggle
- [ ] WhatsApp share button

---

## Contributing

Got an idea to make the diagnosis sharper? Found a bug? PRs are welcome.

1. Fork the repo
2. Create a branch (`git checkout -b feature/your-idea`)
3. Commit your changes
4. Open a pull request

---

## License

MIT — free to use, modify, and build on.

---

Built with curiosity and a suspicion that subscriptions are the problem.

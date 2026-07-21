# 🚀 Deploy your profile README (New Eridu edition)

Your GitHub **profile** README is a special repo named **exactly** your username.

## 1. Create the magic repo
- Repo name **must equal your GitHub username** (e.g. if you're `janeproxy`, the repo is `janeproxy/janeproxy`).
- Make it **Public** and tick **"Add a README file"**.
- GitHub will show a little hint: *"You found a secret! …this special repository…"* — that's the one.

## 2. Drop in these files
Copy into the repo, keeping the folders:

```
README.md
.github/workflows/snake.yml
assets/            (optional — for your Jane Doe image)
```

## 3. Find & replace 5 things in README.md
| Placeholder        | Replace with                                  |
|--------------------|-----------------------------------------------|
| `YOUR_USERNAME`    | your GitHub username (every widget uses it)   |
| `YOUR%20NAME`      | your name in the top banner (keep `%20` = space) |
| `<YOUR NAME>` etc. | the dossier + `whoami` fields                 |
| social `href`s     | your real LinkedIn / X / Discord / email      |
| `assets/jane-doe.png` | (optional) your own image, then uncomment it |

> 💡 In VS Code: `Ctrl+Shift+H` → replace `YOUR_USERNAME` across the file in one shot.

## 4. Wake up the snake 🐍
The snake needs one manual kick to exist:
1. Push the files (make sure your default branch is `main`).
2. Go to the repo's **Actions** tab → enable workflows if prompted.
3. Open **"Generate Contribution Snake"** → **Run workflow**.
4. It creates an `output` branch with the SVG. The README already points at it.
   - Re-runs automatically every 12h and on each push.

If the snake image 404s, the workflow just hasn't run yet — run it once from the Actions tab.

## 5. (Optional) Add Jane Doe art
- Save an image to `assets/jane-doe.png`.
- In `README.md`, find the `boot New_Eridu.exe` section, delete the comment block, and uncomment the `<img src="assets/jane-doe.png" ...>` line.
- Use art you have the rights to (your own screenshot/render, or officially shareable art).

## Widgets used (all free, render live on GitHub)
- **capsule-render** — waving banner + footer + ZZZ slice
- **readme-typing-svg** — animated headline
- **github-readme-stats** — stats card + top languages
- **streak-stats (demolab)** — contribution streak
- **github-readme-activity-graph** — contribution feed line chart
- **github-profile-trophy** — trophy case
- **Platane/snk** — the contribution snake
- **komarev ghpvc** — visitor counter
- **shields.io** — all the badges

Everything is themed to one neon palette:
`#F72585` magenta · `#7B2FF7` purple · `#00E5FF` cyan · `#FF2E63` Jane-red · `#10002B` void-bg

# GitHub Profile Setup Guide

> Complete setup for Ahmad's GitHub profile README repository.

---

## Folder Structure

```
YOUR_USERNAME/                    # Repo name MUST match your GitHub username
├── README.md                     # Profile page (this file)
├── SETUP.md                      # This guide
└── .github/
    └── workflows/
        └── snake.yml             # Contribution snake generator
```

After the snake workflow runs, GitHub creates an **`output`** branch automatically with generated SVGs.

---

## Quick Start

### 1. Create the profile repository

1. Go to [github.com/new](https://github.com/new)
2. **Repository name:** your exact GitHub username (e.g. `ahmad`)
3. **Visibility:** Public
4. Check **Add a README file** (optional — you'll replace it)
5. Create repository

### 2. Push these files

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_USERNAME.git
cd YOUR_USERNAME

# Copy README.md, SETUP.md, and .github/workflows/snake.yml into the repo

git add .
git commit -m "feat: add premium GitHub profile README"
git push origin main
```

### 3. Replace all placeholders

Search and replace in `README.md`:

| Placeholder | Replace with |
|---|---|
| `YOUR_USERNAME` | Your GitHub username |
| `YOUR_LINKEDIN` | LinkedIn handle or slug |
| `YOUR_TWITTER` | Twitter/X handle |
| `YOUR_EMAIL@example.com` | Your email |
| `YOUR_PORTFOLIO.com` | Portfolio URL |
| `YOUR_DISCORD_ID` | Discord user ID |
| `YOUR_CITY, YOUR_COUNTRY` | Location |
| `YOUR_WAKATIME_USERNAME` | WakaTime username (optional) |
| `YOUR_SPOTIFY_ID` | Spotify user ID (optional) |

### 4. Enable the contribution snake

1. Go to **Actions** tab in your profile repo
2. Enable workflows if prompted
3. Run **Generate Snake Animation** manually (`workflow_dispatch`)
4. Wait ~1 minute — an `output` branch will appear with SVG files
5. Snake animation will auto-update daily via cron

### 5. Pin featured projects

Create repos matching the placeholder names **or** update pin card URLs in README to your real projects:

- `k8s-platform-toolkit`
- `terraform-aws-modules`
- `ai-infra-agent`
- `devops-automation-suite`

---

## Widget Sources & Setup

| Widget | Source | Setup |
|---|---|---|
| Typing SVG | [readme-typing-svg](https://github.com/DenverCoder1/readme-typing-svg) | Edit lines in URL — no auth |
| Header/Footer wave | [capsule-render](https://github.com/kyechan99/capsule-render) | Edit text/color params |
| GitHub Stats | [github-readme-stats](https://github.com/anuraghazra/github-readme-stats) | Replace `YOUR_USERNAME` |
| Streak Stats | [github-readme-streak-stats](https://github.com/DenverCoder1/github-readme-streak-stats) | Replace username |
| Activity Graph | [github-readme-activity-graph](https://github.com/Ashutosh00710/github-readme-activity-graph) | Replace username |
| Top Languages | github-readme-stats | Same as stats |
| Profile Views | [github-profile-views-counter](https://github.com/antonkomarev/github-profile-views-counter) | Replace username |
| Skill Icons | [skill-icons](https://github.com/tandpfun/skill-icons) | Edit icon list in URL |
| Repo Pins | github-readme-stats | Point to real repos |
| Dev Quote | [quotes-github-readme](https://github.com/PiyushSuthar/github-readme-quotes) | No setup |
| Trophies | [github-profile-trophy](https://github.com/ryo-ma/github-profile-trophy) | Replace username |
| Contribution Snake | [snk](https://github.com/Platane/snk) | GitHub Actions workflow |
| Shields.io Badges | [shields.io](https://shields.io/) | Customize badge URLs |

### Optional: WakaTime

1. Get API key from [wakatime.com/settings/api-key](https://wakatime.com/settings/api-key)
2. Uncomment WakaTime block in README
3. For private stats, self-host [github-readme-stats](https://github.com/anuraghazra/github-readme-stats#deploy-on-your-own) with `WAKATIME_API_KEY`

### Optional: Spotify Now Playing

1. Deploy [spotify-github-profile](https://github.com/kittinan/spotify-github-profile)
2. Uncomment Spotify block in README
3. Add your Spotify user ID

---

## Recommended Customization Sites

| Resource | URL | Use for |
|---|---|---|
| Shields.io | https://shields.io | Custom badges |
| Simple Icons | https://simpleicons.org | Brand colors & SVG icons |
| Skill Icons | https://skillicons.dev | Dev stack icon grid |
| Capsule Render | https://capsule-render.vercel.app/demo/ | Animated headers |
| Typing SVG Demo | https://readme-typing-svg.demolab.com/demo/ | Hero typing effect |
| Readme Stats Demo | https://github-readme-stats.vercel.app/demo | Theme preview |
| Awesome Profile README | https://github.com/abhisheknaiidu/awesome-github-profile-readme | Inspiration |
| GitHub Profile Generator | https://rahuldkjain.github.io/gh-profile-header-img/ | Custom header images |
| Giphy / LottieFiles | https://giphy.com · https://lottiefiles.com | Subtle animations |

---

## Theme Tips

- **Dark-theme friendly:** `tokyonight` theme is used across all stat cards
- **Consistency:** Keep one accent color (sky blue `#38bdf8` used throughout)
- **Mobile:** Tables are used sparingly; stat cards stack naturally on mobile
- **Performance:** Avoid too many external requests — this README is balanced

---

## Bonus Ideas (Elite Tier)

1. **GitHub Actions badge wall** — Show CI/CD status badges from your top repos
2. **Blog RSS feed** — Embed latest posts via [github-readme-blog](https://github.com/gautamkrishnar/blog-post-workflow)
3. **LeetCode / HackerRank stats** — If you do competitive coding
4. **Custom 3D contribution chart** — [3D chart action](https://github.com/DenverCoder1/github-3d-contribution-graph)
5. **Terminal-style intro** — [github-readme-terminal](https://github.com/shreehari-revankar/github-readme-terminal)
6. **AWS/GCP cert badges** — Add Credly or official certification shields
7. **Pinned Gists** — Showcase useful scripts/snippets
8. **Sponsor button** — Enable GitHub Sponsors if applicable
9. **Visitor geo map** — [clustrmaps](https://clustrmaps.com) (use sparingly)
10. **Dynamic resume PDF link** — Auto-updated via Actions from a `resume/` folder
11. **Recent blog/dev.to posts** — Workflow to inject latest articles
12. **Custom ASCII art header** — Minimal, terminal-aesthetic alternative to GIF banner

---

## Troubleshooting

| Issue | Fix |
|---|---|
| Stats show "user not found" | Replace `YOUR_USERNAME` everywhere |
| Snake not showing | Run workflow manually; check `output` branch exists |
| Broken pin cards | Repo must be public and name must match exactly |
| Images not loading | GitHub caches README — wait 5–10 min or change URL slightly |
| Workflow permission denied | Enable Actions + set `contents: write` permission |

---

<p align="center"><sub>Happy building, Ahmad.</sub></p>

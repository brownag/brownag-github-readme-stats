# GitHub Readme Stats Generator

This repository uses GitHub Actions and [stats-organization/github-readme-stats-action](https://github.com/stats-organization/github-readme-stats-action) to statically generate GitHub Readme Stat Cards on a weekly interval (Sunday at midnight). 

This serves as a 1:1 replacement for the dynamic Vercel-hosted version to avoid rate-limiting and downtime.

## Generated Cards

- **Main Stats Card:** `generated/github-readme-stats.svg`
- **Top Languages Card:** `generated/github-readme-stats-top-langs.svg`

---

## 1:1 README.md Replacement Markup

To update your profile README (at `brownag/brownag`), replace the dynamic URLs with the raw links to the statically generated files:

### 1. Main Stats Card

**Original:**
```html
<img src="https://brownag-github-readme-stats.vercel.app/api?username=brownag&show_icons=true&theme=dark"/>
```

**Replacement:**
```html
<img src="https://raw.githubusercontent.com/brownag/brownag-github-readme-stats/main/generated/github-readme-stats.svg"/>
```

### 2. Top Languages Card

**Original:**
```markdown
![Top Langs](https://brownag-github-readme-stats.vercel.app/api/top-langs/?username=brownag&hide=html,less,css,scss,TeX,cypher&layout=compact&theme=dark)
```

**Replacement:**
```markdown
![Top Langs](https://raw.githubusercontent.com/brownag/brownag-github-readme-stats/main/generated/github-readme-stats-top-langs.svg)
```

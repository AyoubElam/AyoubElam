<h1 align="center">Hey 👋 What's Up?</h1>

<h3 align="center">Full Stack Developer | Building Digital Experiences</h3>

###

<div align="center">
  <img src="https://skillicons.dev/icons?i=react" height="40" alt="react logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=nextjs" height="40" alt="nextjs logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=vue" height="40" alt="vue logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=angular" height="40" alt="angular logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=ts" height="40" alt="typescript logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=js" height="40" alt="javascript logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=nodejs" height="40" alt="nodejs logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=express" height="40" alt="express logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=nestjs" height="40" alt="nestjs logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=python" height="40" alt="python logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=django" height="40" alt="django logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=flask" height="40" alt="flask logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=mongodb" height="40" alt="mongodb logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=postgres" height="40" alt="postgresql logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=mysql" height="40" alt="mysql logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=redis" height="40" alt="redis logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=graphql" height="40" alt="graphql logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=docker" height="40" alt="docker logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=kubernetes" height="40" alt="kubernetes logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=aws" height="40" alt="aws logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=firebase" height="40" alt="firebase logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=tailwind" height="40" alt="tailwind logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=html" height="40" alt="html5 logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=css" height="40" alt="css3 logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=git" height="40" alt="git logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=github" height="40" alt="github logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=vscode" height="40" alt="vscode logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=figma" height="40" alt="figma logo" />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=linux" height="40" alt="linux logo" />
</div>

###

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=AyoubElam&hide_title=false&hide_rank=false&show_icons=true&include_all_commits=true&count_private=true&disable_animations=false&theme=dracula&locale=en&hide_border=false&order=1" height="150" alt="stats graph" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=AyoubElam&locale=en&hide_title=false&layout=compact&card_width=320&langs_count=5&theme=dracula&hide_border=false&order=2" height="150" alt="languages graph" />
</div>

###

<div align="center">
  <img src="https://streak-stats.demolab.com?user=AyoubElam&locale=en&mode=daily&theme=dracula&hide_border=false&border_radius=5&order=3" height="150" alt="streak graph" />
  <img src="https://github-profile-trophy.vercel.app?username=AyoubElam&theme=dracula&column=-1&row=1&margin-w=8&margin-h=8&no-bg=false&no-frame=false&order=4" height="150" alt="trophy graph" />
</div>

###

<br clear="both">

<img src="https://raw.githubusercontent.com/AyoubElam/AyoubElam/output/snake.svg" alt="Snake animation" />

###

<div align="center">
  <a href="https://www.linkedin.com/in/ayoub-elamrani-059120317/" target="_blank">
    <img src="https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&label=&color=0077B5&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="linkedin logo" />
  </a>
  <a href="https://discord.com/users/cheezy._.11" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Discord&logo=discord&label=&color=7289DA&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="discord logo" />
  </a>
</div>

###

<div align="center">
  <img src="https://visitor-badge.laobi.icu/badge?page_id=AyoubElam.AyoubElam&" alt="visitor count" />
</div>

---

### 🐍 Generate Snake Animation

To enable the snake animation, create `.github/workflows/snake.yml` in your repository:

```yaml
name: Generate Snake

on:
  schedule:
    - cron: "0 */12 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      
      - uses: Platane/snk@v3
        with:
          github_user_name: AyoubElam
          outputs: |
            dist/snake.svg
            dist/snake-dark.svg?palette=github-dark

      - uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

After creating this file, go to **Actions** tab in your repository and run the workflow manually!

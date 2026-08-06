<div align="center">

# 🚀 REMA FARVEEN SHAHUL HAMMED

<img src="https://readme-typing-svg.herokuapp.com?font=Orbitron&size=32&duration=2500&pause=1000&color=00F7FF&center=true&vCenter=true&width=900&lines=Welcome+To+My+GitHub+Portfolio;Aspiring+Software+Engineer;Artificial+Intelligence+Enthusiast;Full+Stack+Developer;Java+Python+React+Developer" />

<br>

<img src="https://capsule-render.vercel.app/api?type=waving&height=180&color=0:0f2027,50:203a43,100:2c5364&text=Welcome&fontColor=ffffff&fontSize=55"/>

</div>

---

# 👩‍💻 About Me

🎓 B.Sc Information Technology Student

💻 Aspiring Software Engineer

🤖 AI Enthusiast

🌐 Full Stack Developer

🚀 Passionate about building innovative software solutions.

---

# 🌌 Live Contribution Snake

<p align="center">

<img src="https://raw.githubusercontent.com/Remafarveen/Remafarveen/output/github-contribution-grid-snake-dark.svg">

</p>

---

# 🚀 Rocket Mission

Coming Soon...

(Animated Rocket Shooting Projects)

---

# 🛠 Tech Stack

<p align="center">

<img src="https://skillicons.dev/icons?i=java,python,c,cpp,php,html,css,js,react,nodejs,mongodb,mysql,git,github,vscode,linux"/>

</p>

---

# 📊 GitHub Stats

<p align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=Remafarveen&show_icons=true&theme=tokyonight&hide_border=true"/>

<img height="170" src="https://github-readme-streak-stats.herokuapp.com/?user=Remafarveen&theme=tokyonight&hide_border=true"/>

</p>

<p align="center">

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Remafarveen&theme=react-dark"/>

</p>

---


<div align="center">
name: Generate Snake

on:
  schedule:
    - cron: "0 */12 * * *"
  workflow_dispatch:
  push:
    branches:
      - main

permissions:
  contents: write

jobs:
  generate:
    runs-on: ubuntu-latest

    steps:
      - name: Generate GitHub Contribution Snake
        uses: Platane/snk/svg-only@v3
        with:
          github_user_name: Remafarveen
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark

        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

      - name: Push Snake Animation
        uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist

        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}






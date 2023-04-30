Thank you for visit my Github. 👋

About me @TALES LIMA
-I am a javascript, javascript framework, php and php framework expert

-My main skill: REACT, SASS, MYSQL, CSS, BOOTSTRAP, SEO, PHP, C, C++, JAVASCRIPT, JQUERY, HTML5, UI, LINUX, BASIC JAVA, etc...

-My database skill: MongoDB, Mysql,
<div>
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=Tales1982&show_icons=true&theme=tokyonight"/>
 <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Tales1982&layout=compact&theme=tokyonight"/>
</div>
<h2>Languages and Tools:</h2>

<!--
**tales1982/tales1982** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: Tales Lima
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  

# 👩🏻‍💻 George Rodrigues

**`Desenvolvedor Backend`**

Me chamo George Rodrigues, tenho 22 anos e sou natural Recife/PE. Atualmente, estou cursando Desenvolvimento de Sistemas no ETE, sou desenvolvedor fullstack porem voltado para backend

<p align="left">
    <a href="https://www.youtube.com/@larissakich?sub_confirmation=1">
        <img 
            alt="youtube subscribers" 
            title="Inscreva-se no meu canal" 
            src="https://custom-icon-badges.demolab.com/youtube/channel/subscribers/UCo-gJ8RnTn5akHqHvO55DVA?color=%23E05D44&label=Inscreva-se&logo=video&logoColor=white&style=for-the-badge&labelColor=CE4630"
        />
    </a>
    <a href="https://www.youtube.com/@larissakich">
        <img 
            alt="youtube views" 
            title="Vizualizações no YouTube" 
            src="https://custom-icon-badges.demolab.com/youtube/channel/views/UCo-gJ8RnTn5akHqHvO55DVA?color=%23E1AD0E&logo=eye&logoColor=white&style=for-the-badge&labelColor=C79600"
        />
    </a> 
    <a href="https://github.com/Larissakich?tab=repositories&sort=stargazers">
        <img 
            alt="Total de estrelas" 
            title="Total de estrelas GitHub" 
            src="https://custom-icon-badges.demolab.com/github/stars/Larissakich?color=55960c&style=for-the-badge&labelColor=488207&logo=star&label=estrelas"
        />
    </a>
    <a href="https://github.com/Larissakich?tab=followers">
        <img 
            alt="Seguidores" 
            title="Me siga no GitHub" 
            src="https://custom-icon-badges.demolab.com/github/followers/Larissakich?color=236ad3&labelColor=1155ba&style=for-the-badge&logo=github&label=Seguidores&logoColor=white"
        />
    </a>
</p>

---

### 🤖 Linguagens e Tecnologias

<img 
    align="left" 
    alt="HTML"
    title="HTML" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg" 
/>
<img 
    align="left" 
    alt="CSS" 
    title="CSS"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg" 
/>
<img 
    align="left" 
    alt="JavaScript" 
    title="JavaScript"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg" 
/>
<img 
    align="left" 
    alt="TypeScript"
    title="TypeScript" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg" 
/>
<img 
    align="left" 
    alt="React"
    title="React" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/react/react-original.svg" 
/>
<img 
    align="left" 
    alt="Next.js" 
    title="Next.js"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nextjs/nextjs-original.svg" 
/>
<img 
    align="left" 
    alt="Bootstrap"
    title="Bootstrap" 
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/bootstrap/bootstrap-original.svg" 
/>
<img 
    align="left" 
    alt="Tailwind" 
    title="Tailwind"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/tailwindcss/tailwindcss-original.svg" 
/>
<img 
    align="left" 
    alt="SASS" 
    title="SASS"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/sass/sass-original.svg" 
/>
<img 
    align="left" 
    alt="PHP" 
    title="PHP"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/php/php-original.svg" 
/>
<img 
    align="left" 
    alt="Laravel" 
    title="Laravel"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/laravel/laravel-original.svg" 
/>
<img 
    align="left" 
    alt="JQuery" 
    title="JQuery"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/jquery/jquery-original.svg" 
/>
<img 
    align="left" 
    alt="Git" 
    title="Git"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/git/git-original.svg" 
/>
<img 
    align="left" 
    alt="Python" 
    title="Python"
    width="30px" 
    style="padding-right: 10px;" 
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" 
/>

##

<div align-cneter>

<img src="https://raw.githubusercontent.com/George-Dev04/George-Dev04/output/snake.svg" alt="Animação de cobra" />

Sbake.yml:
name: Gerar animação de cobra

on:

schedule: # executar a cada 12 horas

- cron: "* */12 * * *"

workflow_dispatch:

push:

branches:

- master

jobs:

generate:

permissions:

contents: write

runs-on: ubuntu-latest

timeout-minutes: 5

steps:

- name: generate snake.svg

uses: Platane/snk/svg-only@v3

with:

github_user_name: ${{ github.repository_owner }}
outputs: dist/snake.svg?palette=github-dark

- name: enviar snake.svg para o branch de saída

uses: crazy-max/ghaction-github-pages@v3.1.0

with:
target_branch: output
build_dir: dist
env:
GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

</div> 

##








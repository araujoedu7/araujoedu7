

- 🌱 I’m currently learning languages ​​such as: JavaScript, TypeScript, HTML5 and CSS3


<div style="display: inline_block"><br>
  <img align="center" alt="ea-Js" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
  <img align="center" alt="ea-Ts" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-plain.svg">
  
  <img align="center" alt="ea-HTML" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
  <img align="center" alt="ea-CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
 
  <img align="right" alt="Tem uma foto aqui =)" height="150" style="border-radius:50px;" src="">
</div>


<br>
<br>

<div> 
  
  <a href="https://instagram.com/e.araujo07" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
 <a href="https://discord.gg/Du7.zip" target="_blank"><img src="https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white" target="_blank"></a> 
  <a href = "mailto:ea144027@gmail.com"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
 

name: Generate Datas 
  
 on: 
   schedule: # execute every 12 hours 
     - cron: "* */12 * * *" 
   workflow_dispatch: 
  
 jobs: 
   build: 
     name: Jobs to update datas 
     runs-on: ubuntu-latest 
     steps: 
       # Snake Animation 
       - uses: Platane/snk@master 
         id: snake-gif 
         with: 
           github_user_name: rafaballerini 
           svg_out_path: dist/github-contribution-grid-snake.svg 
  
       - uses: crazy-max/ghaction-github-pages@v2.1.3 
         with: 
           target_branch: output 
           build_dir: dist 
         env: 
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }} 
   


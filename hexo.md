## How to build your website on github use hexo
1. Install the Hexo
````
npm install -g hexo-cli
````

2. Create a repository in github and named as 
````
username.github.io
````
3. Creat your local project, such as myblog. Then run follow command to download hexo project:
````
$ hexo init <folder>
$ cd <folder>
$ npm install
````
4. Put your local project to github repositories
````
git init
git add.
git commit -m 'upload'
git remote add origin git@github.com:Daisy/AKgit.git
git push -u origin main
````
5. install hexo-deployer-git to deploy
````
$ npm install hexo-deployer-git --save
````
and add to the config:
````
deploy:
  type: git
  repo: https://github.com/<username>/<project>
  # example, https://github.com/hexojs/hexojs.github.io
  branch: main
````
6. Run clean and deploy
````
hexo clean && hexo deploy
````

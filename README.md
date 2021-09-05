# MrBaiYinL.github.io
--部署

Hexo 提供了快速方便的一键部署功能，让您只需一条命令就能将网站部署到服务器上。
``` bash
$ hexo deploy
```

安装 hexo-deployer-git。
``` bash
$ npm install hexo-deployer-git --save
```

修改配置
``` bash
deploy:
  type: git
  repo: <repository url> #git@github.com:johnsmith/johnsmith.github.io.git
  branch: [branch] #分支
  message: [message] #自定义提交信息
  ```

生成站点文件并推送至远程库，执行 
``` bash
$ hexo clean && hexo deploy
```
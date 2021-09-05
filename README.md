# MrBaiYinL.github.io


source：该文件夹是存放我们自己文章的地方，文章存放在该目录下的_posts文件夹中。

themes：用于存放博客的主题信息。

_config.yml：是hexo博客的配置文件，很多配置信息都在这里面。

public文件夹，该文件夹就是用于存放静态页面的地方，该文件夹下的静态页面都是根据配置文件动态生成的，所以只要修改配置文件_config.yml中的配置信息，就可以使生成的静态页面发生改变

hexo clean和hexo g
hexo clean：表示清除原来的缓存，它会直接把原来编译生成的静态文件夹public直接删除；hexo g：又会再次根据配置文件生成静态页面。

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
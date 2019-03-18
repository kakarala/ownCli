# ownCli
## 最简单的脚手架搭建教程
1. npm init -y // 初始化一个新的项目，创建一个package.json和默认配置
2. 在package.json中添加
  ```
  "bin": {
    "own-cli": "bin/own-cli"
  }
  ```
  **其中own-cli是以后将要使用的命令， 其中bin/own-cli就是命令调用的文件**
3. 在bin/own-cli的第一行写上
  ```
  #!/usr/bin/env node
  ```
  **这是告诉系统，下面这个脚本，使用nodejs来执行**
4. 下面添加一个console.log('hello world');
5. 跳转到该项目的主目录
  ```
  $ npm install -g
  // 如果有错误，请使用下面的
  $ sudo npm install -g
  ```
6. 最后需要
  ```
  $ npm link
  // 如果有错误，请使用下面的
  $ sudo npm link
  ```
## 大功告成，最后就可以输入own-cli,就能出现hello world.

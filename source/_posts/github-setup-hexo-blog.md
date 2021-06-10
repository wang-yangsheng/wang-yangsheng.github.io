---
title: setup github hexo blog  
date: 2021-06-11 00:12:01
tags:
---

# github 上部署hexo模板blog  

如果系统没有安装nodejs,npm，先安装nodejs,npm  
reference:<https://www.cnblogs.com/WangYangkai/p/14426337.html>  
<br>

* clone github 仓库的源码  
$ git clone https://github.com/wang-yangsheng/wang-yangsheng.github.io.git  
<br>

* 初始化hexo工程  
$ cd wang-yangsheng.github.io/  
$ npm install  
$ npm install hexo-deployer-git  
<br>

* 生成blog网页  
$ hexo g  
$ hexo s  
<br>

或者  
$ hexo clean && hexo g && hexo s  
<br>

* 进行网页开发：增加blog.md文本，改动源码； 
本地调试网页...  
<br>
<br>

* 提交改动,到hexo分支 
$ git status  
$ git add [file]  
$ git commit [file] -m "git log"  
$ git push -u origin hexo  
<br>  

* 提交网页文件，到master分支
$ hexo d  
<br>

```
wys@ubuntu:~/tmp/wang-yangsheng.github.io$ hexo --help
INFO  Validating config
Usage: hexo <command>

Commands:
  clean     Remove generated files and cache.
  config    Get or set configurations.
  deploy    Deploy your website.
  generate  Generate static files.
  help      Get help on a command.
  init      Create a new Hexo folder.
  list      List the information of the site
  migrate   Migrate your site from other system to Hexo.
  new       Create a new post.
  publish   Moves a draft post from _drafts to _posts folder.
  render    Render files with renderer plugins.
  server    Start the server.
  version   Display version information.

Global Options:
  --config  Specify config file instead of using _config.yml
  --cwd     Specify the CWD
  --debug   Display all verbose messages in the terminal
  --draft   Display draft posts
  --safe    Disable all plugins and scripts
  --silent  Hide output on console

For more help, you can use 'hexo help [command]' for the detailed information
or you can check the docs: http://hexo.io/docs/
wys@ubuntu:~/tmp/wang-yangsheng.github.io$ 
```
<br>  

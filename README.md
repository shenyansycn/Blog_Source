# Blog_Source


补充一下使用Blog文件夹同步的几个注意事项：
1. 如果主题是通过git管理的，需要将主题文件夹下的.git文件夹删除，才能同步Blog文件夹（.git文件夹是隐藏的，需要显示隐藏文件才能删除，Linux下需要rm -rf命令才能删除，Mac没用过，不清楚）。
2. 按照Blog目录下自带的.gitignore文件，node_modules文件夹是不会同步的，所以同步之后需要自己再次进行npm install，但是注意，不要进行hexo init了，否则_config.yml全都白弄了。

然后给你看一下同步之后的目录：
https://github.com/Xuanwo/xuanwo.github.io/tree/blog

推荐一下里面的git shell.lnk文件，自带启动参数，无需配置git和nodejs环境，直接可以在同一个窗口运行git和hexo。

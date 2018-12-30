#微信公众号批量抓取
##运行环境

1. 需要安装Python 3.5 如果运行2.7的会出现一点小bug 目前暂时没有精力改成2.7版本

2. 关于安装库，我用的都是标准的，如果连requests 或者ftplib都木有的话我也不好说什么是吧。pymysql这个库链接MySQL还是不错的

##文件介绍
1. preparerequest.py这个文件是以前版本，当时key没有和公众号关联一个key可以获取多个公众号文章列表，
2. wechetcrawl.py这个是最新的，运行它你可以立刻看到他在做什么：主要就是将fiddler4获取到mp.weixin.qq.com的request的
response获取到的txt解析然后获取其中内容并放置到mysql中.
3. 其他的txt文件是fiddler获取下来的，new_response是我的程序生成的

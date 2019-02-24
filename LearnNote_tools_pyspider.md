1. 如何进入mac os的/Library/Frameworks/Python...文件？
进入系统地Library而不是文件的Library：左上角“前往”，或者 command+shift+G

2. pyspider 不支持python3.7
pyspider的github已经有人有了solution，但尚未合并成功。所以我打算本地fix bug，然后运行。
依然不行，虽然我把本地所有"async"关键字都改成了”async_mode“,依然还有其它文件跑不过。例如pyspider依赖于PhantomJS，而安装PhantomJS在MAC又一堆事。
所以随便浏览了下自己动手用python写爬虫，发现可能几十行代码就能搞定（事实上最后只用12行代码就成）。而且现成的工具只special于特定网站的图片or文本or视频，且那些网站也在不断做反被抓取的更新（也就是说，现成工具发布的时候能用不代表现在还能用）。想想实现过程也就是”请求+保存“，所以打算自己写。

卸载pyspider：
pip list
pip uninstall pyspider



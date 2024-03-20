<!-- win-bat.md -->
#### Title: windows cmd batch file
#### Date: July 11th, 2018

## Windows 批处理


+ ! 感叹号 

    一般windows bat文件里面用 **%** 来表示变量

    < ```shell
    < set var = 123
    < echo %var%
    < ```  

    然后今天遇到了一个用感叹号来表示变量的情况

    < ```shell
    < set var = (abcdefg)
    < set var = !var!
    < echo var and !var!
    < ```

    看文档，这个一般是用来做延迟绑定用的，因为windows的cmd解释器不会一条一条的去解释执行，所以需要使用!来代替%，实现延迟绑定。

    具体文档可以参考[这里](http://www.bathome.net/thread-1205-1-1.html)，这个比较全面。


    待续。。。

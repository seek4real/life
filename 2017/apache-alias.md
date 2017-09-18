Title: Apache Alias configuration on MacOS X  
Author: $whoami :me  
Date: Sept one day, 2017  
Copyright: me  

### Apache alias configuration MacOS X ###

---

MacOS X 已经自带了apache，直接配置就可以使用了。

默认的配置文件在:
```bash
/private/etc/apache2/httpd.conf
```

因为Alias的mod是默认就开启了load的，所以直接在配置添加
> ``` 
> Alias /webpath /local/file/path
> <Directory /local/file/path>
>	Order allow,deny
>	Allow from all
> </Directory>
> #如果访问出现403权限的问题，（如果确保你设置的本地目录有访问权限）就加上下面的
> #ps: apache默认用户组是_www需要确保设置的目录可以又执行权限
> <Directory /local/file/path>
> 	Require all granted
> </Directory>
> ```

详情参考这里:
[apache wiki](https://wiki.apache.org/httpd/ClientDeniedByServerConfiguration)

---
除了设置Alias还可以通过设置 **用户配置** 已经设置 **虚拟目录** 的方法

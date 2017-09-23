<!-- shell-cmd.md -->
### shell command

+ 显示目录或者文件占用空间情况
  < ```shell 
  < du -hs
  < ```

+ 系统服务管理
  < ```shell
  < # on *nix
  < chkconfig servicename
  < # or
  < service servicename [stop | start | restart]
  < # on OS X
  < launchctl servicename
  < ```

+ 查询dns除了nslookup以外，还可以使用dig
  < ```shell
  < dig +/- options [domain] @DNSSERVER type
  < dig +short code.hoolai.com @8.8.8.8 A
  < ```

+ netstat查看网络统计看，还可以使用iproute2

+ 除了whoami, 竟然还有 who am i, WTF
  <    who am i

continue soon...


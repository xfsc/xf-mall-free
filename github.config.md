


- 通过这个网站查询到dns的节点IP地址 [fastly.net.ipaddress.com](https://fastly.net.ipaddress.com/)
- 修改hosts文件 `C:\Windows\System32\drivers\etc\hosts`
```bash
# Copyright (c) 1993-2009 Microsoft Corp.
#
# This is a sample HOSTS file used by Microsoft TCP/IP for Windows.
#
# This file contains the mappings of IP addresses to host names. Each
# entry should be kept on an individual line. The IP address should
# be placed in the first column followed by the corresponding host name.
# The IP address and the host name should be separated by at least one
# space.
#
# Additionally, comments (such as these) may be inserted on individual
# lines or following the machine name denoted by a '#' symbol.
#
# For example:
#
#      102.54.94.97     rhino.acme.com          # source server
#       38.25.63.10     x.acme.com              # x client host

# localhost name resolution is handled within DNS itself.
#	127.0.0.1       localhost
#	::1             localhost


140.82.113.3 github.com
```

- 以管理员方式打开 `cmd` 执行 `ipconfig /flushdns` 手动刷新系统DNS缓存
```bash
Microsoft Windows [版本 10.0.14393]
(c) 2016 Microsoft Corporation。保留所有权利。

C:\Windows\system32>ipconfig /flushdns

Windows IP 配置

已成功刷新 DNS 解析缓存。

C:\Windows\system32>
```


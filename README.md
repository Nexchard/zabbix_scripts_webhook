下载zabbix通过﻿webhook﻿发送给企业微信webhook的脚本，并拷贝到指定的目录中﻿
```
[root@zabbix-server01 ~]# wget http://file.oldxu.net/zabbix/zabbix_wechat_webhook
[root@zabbix-server01 ~]# chmod +x zabbix_wechat_webhook
[root@zabbix-server01 ~]# mv zabbix_wechat_webhook /usr/lib/zabbix/alertscripts/
```

执行脚本，参数1:企业微信token、参数2: 用户名称，参数3:消息主题，参数4:消息内容
```
[root@zabbix-server01 ~]# /usr/lib/zabbix/alertscripts/zabbix_wechat_webhook d5439b70-b7b8-47f8-8351-d3312c069e66 "张三" "服务器故障" "抓紧修复"
2099/04/08 23:36:31 Message sent to WeChat
```

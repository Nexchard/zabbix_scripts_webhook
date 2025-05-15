## 企业微信webhook
下载zabbix通过﻿webhook﻿发送给企业微信webhook的脚本，并拷贝到指定的目录中﻿
```
[root@zabbix-server01 ~]# wget http://file.oldxu.net/zabbix/zabbix_wechat_webhook
[root@zabbix-server01 ~]# chmod +x zabbix_wechat_webhook
[root@zabbix-server01 ~]# mv zabbix_wechat_webhook /usr/lib/zabbix/alertscripts/
```

执行脚本，参数1:企业微信token、参数2: 用户名称，参数3:消息主题，参数4:消息内容
```
[root@zabbix-server01 ~]# /usr/lib/zabbix/alertscripts/zabbix_wechat_webhook d5439b70-b7b8-47f8-8351-d33126 "张三" "服务器故障" "抓紧修复"
2099/04/08 23:36:31 Message sent to WeChat
```
## 
下载zabbix通过﻿webhook﻿发送给钉钉机器人的脚本，并拷贝到指定的目录中

```
[root@zabbix-server ~]# wget http://file.oldxu.net/zabbix/zabbix_dingding_webhook
[root@zabbix-server ~]# chmod +x zabbix_dingding_webhook
[root@zabbix-server ~]# mv zabbix_dingding_webhook /usr/lib/zabbix/alertscripts/
```


执行脚本

- 参数1：钉钉的webhook、

- 参数2：用户名（指定手机号可以明确@对应的用户）

- 参数3：消息主题

- 参数4：消息内容

  ```
  [root@zabbix-server ~]# /usr/lib/zabbix/alertscripts/zabbix_dingding_webhook 4dd9e8f234c87533aa44079da5f7b9dd93393944939c6f "199xxxxx59" "服务器故障TEST" "抓紧修复"
  ```

执行结果

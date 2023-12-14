# 利用iptables设置端口转发

1. 便捷地设置iptables流量转发规则
2. 当域名解析的地址发生变化时，自动更新流量转发规则，不需要手动变更（适用于ddns域名）

## 用法

下载运行
```shell

bash natcfg.sh
```

输出如下：

```
#############################################################
# Usage: setup iptables nat rules for domian/ip             #
# Website:                      #
# Author:                         #
# Github:         #
#############################################################

你要做什么呢（请输入数字）？Ctrl+C 退出本脚本
1) 增加转发规则          3) 列出所有转发规则
2) 删除转发规则          4) 查看当前iptables配置
#?
```

此时按照需要，输入1-4中的任意数字，然后按照提示即可

## 卸载
下载运行
```shell
bash uninstall.sh
```

## 查看日志

```shell
journalctl -exu dnat
```


配置文件在

```shell
/etc/dnat/conf
```


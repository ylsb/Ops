# Operator

如果现在给你 500 台服务器，你会如何管理？
提示

- 服务器均为Linux，操作系统有Redhat、CentOS、Ubuntu

- 服务器上运行着各类应用，如Nginx、MySQL、Redis、ElasticSearch、Python、Java等

- 简述主要思路，并尝试编写一些脚本，体现出主要内容即可

- 独立完成，提供代码的 GitHub 仓库链接即可

思路：主要从一下几方面入手：
1，统一管理 （ansible，各种云助手统一管理云服务器）
2，监控平台（zabbix，prometheus+grafana） 监控服务器与各种服务的性能
3，如果服务器分布在不同的公有云或私有云，可以尝试用vpn打通各网络拓扑的网关，将所以服务器纳入到统一的内网
4，建立内部包管理仓库，如自建yum仓库，apt仓库，集群机器统一升级时，可以先更新一部分机器，待系统稳定无异常时，将更新包推到自建仓库，再统一更新
5，日志集中分析工具 （elk）
6，持续集成和发布工具
7，安全漏洞扫描工具

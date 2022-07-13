## Confeagle: Automated Analysis of Configuration Vulnerabilities inWeb Applications

#### Web应用程序中配置漏洞的自动分析

## 摘要：

通用web应用程序漏洞扫描器虽然能有效发现多种类型的漏洞，但在识别配置漏洞方面能力有限。

在本文中，我们提出一种有效结合分层配置扫描和web应用程序的初步源代码分析的方法，以检测潜在的配置漏洞，根据标准度量量化严重程序，并促进修复其中发现的漏洞。

## Introdction：

配置错误可能发生在web体系结构的不同层、而==环境==和==应用程序==级别的配置错误是常见的。

该工具能自动扫描应用程序目录层次结构和应用程序源代码来检测、修复配置漏洞（在实际部署软件之前）

使用CCSS（commom configuration scoring system）对配置漏洞进行评分





## Contribution：

1.提出new idea：自动递归的扫描应用程序目录和源代码来检测、量化、修复配置漏洞

2.使用CCSS给配置漏洞打分

3.实现并评估工具：14款PHP软件，另外和三款漏洞扫描工具做了对比



#### 什么是应用程序级别的配置错误呢？

==规则来自于最佳实践值、用户手册、专家意见，需要人工提取==



1.配置解析



2.配置漏洞评分

0～10分 主要由两部分构成：exploitability 和impact



3.修复

自动修复配置漏洞（做不到完全自动化，需要少量的人工），修复后再次使用第二步漏洞分析来检验是否真的修复



## 评估

##### A.默认安装的配置漏洞分析

存在三类漏洞：1）信息泄露

2）拒绝服务

3）会话劫持



##### B.和通用的漏洞扫描工具对比

通用的漏洞扫描器在检测和环境相关的配置漏洞有一些作用，但无法发现应用程序级别的配置漏洞



## 相关工作

1）Early Detection of Security Misconfiguration Vulnerabilities in Web Applications,” in ARES. IEEE, 2011,

没有分析应用程序级别的配置漏洞

2）Detection of configuration vulnerabilities in distributed (web) environments,” CoRR, vol. abs/1206.6757, 2012.

此方法侧重于检测系统级别的配置漏洞，漏洞与其可能导致的潜在攻击之间的联系不明显

3）A study and implementation of vulnerability assessment and misconfiguration detection,” in APSCC, 2008, pp. 1252–1257.

使用CVSS打分、CCE检测配置漏洞

其他的一些相关工作都==没有考虑application level的配置漏洞==


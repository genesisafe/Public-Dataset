# Public-Dataset
Cyber security public dataset
## KDD99
> KDD CUP 99 dataset 就是KDD竞赛在1999年举行时采用的数据集。1998年美国国防部高级规划署（DARPA）在MIT林肯实验室进行了一项入侵检测评估项目收集而来的数据。
- 内容类型: 网络流量，主机行为
- 是否特征化: 是
- 适用范围: 主机入侵检测，异常流量监控

http://kdd.ics.uci.edu/databases/kddcup99/kddcup99.html

## HTTP DATASET CSIC 2010
> HTTP DATASET CSIC 2010 包含已经标注过的针对web服务的请求。数据量约5w条。下载地址已经为我们分类好了训练用的正常数据，测试用的正常数据，测试用的异常数据。
- 内容类型: 网络流量
- 是否特征化：否
- 使用范围: WAF类产品，异常流量监控

http://www.isi.csic.es/dataset/

## honeypot.json
> honeypot 是由多种类型的蜜罐采集回来的数据。主要是WEB请求。约99万条数据。由于没有分类和规整，需要自己数据清洗，也可以用作校验模型的数据。
- 内容类型: 网络流量
- 是否特征化：否
- 使用范围: WAF类产品，异常流量监控

http://www.secrepo.com/honeypot/honeypot.json.zip

## Masquerading User Data
> Masquerading User Data 是Matthias Schonlau 教授通过正常数据构造出来用于训练和检测 Masquerading User攻击的数据集。
> (内部攻击者分为两种，一种是内鬼[Traitor]，一种是窃取了身份凭证的正常用户的伪装者[Masquerading User]）
> 由于是构造出来的数据，缺乏实际攻击的真实性，在一定程度上，训练出来的模型会存在一定的过拟。
- 内容类型: 主机行为
- 是否特征化：否
- 使用范围: 入侵检测类 用户异常行为识别

http://www.schonlau.net/intrusion.html

## ADFA IDS Datasets
> ADFA IDS Datasets 是澳大利亚国防大学发布的一套关于HIDS的数据集。分为linux（ADFA-LD）和window（ADFA-WD）。
- 内容类型: 主机行为
- 是否特征化：是
- 使用范围: 入侵检测

https://www.unsw.adfa.edu.au/australian-centre-for-cyber-security/cybersecurity/ADFA-IDS-Datasets/


## 域名相关
> 正常域名和可疑域名检测。 主要用于DGA的检测。这里直接用Alexa Top 100W 作为正常域名。用其他的开放的DGA数据作为黑样本。
- 内容类型: 文本样本
- 是否特征化：否
- 使用范围: 入侵检测 异常流量 WAF

http://s3.amazonaws.com/alexa-static/top-1m.csv.zip
http://data.netlab.360.com/dga/
http://www.secrepo.com/misc/zeus_dga_domains.txt.zip


## Webshell
> 这里github有一个比较多样本的收集。涵盖了很多的语言。
- 内容类型: 文本样本
- 是否特征化：否
- 使用范围: 入侵检测 异常流量 WAF

https://github.com/tennc/webshell

## 登录日志
> auth.log 主要是都是登录失败的日志 适合用作判断是爆破登录还是正常的输错密码
- 内容类型: 主机行为
- 是否特征化：否
- 使用范围: 入侵检测 异常流量 WAF

http://www.secrepo.com/auth.log/auth.log.gz

## 恶意URL
> malicious-URLs 在Github上面一个 使用机器学习去检测恶意URL的项目 ，里面有一个训练集，有做标记是正常的URL还是恶意的URL
- 内容类型: 文本样本
- 是否特征化：否
- 使用范围: 入侵检测 异常流量 WAF

https://github.com/faizann24/Using-machine-learning-to-detect-malicious-URLs

## 综合数据
> 在github上有一个叫 Security-Data-Analysis 的项目，里面有4个实验室 每个实验室的数据都不一样，包含http，连接记录，域名，host等等。
- 内容类型: 网络流量
- 是否特征化：否
- 使用范围: 异常流量

https://github.com/sooshie/Security-Data-Analysis

## he Malware Capture Facility Project
> MCFP 是捷克理工大学 用于捕抓恶意软件的而抓去的网络流量。里面的数据非常多，有他们自己分析出来的恶意流量，也有所有的流量，包括网络文件，日志，DNS请求等
- 内容类型: 网络流量
- 是否特征化：否
- 使用范围: 异常流量 WAF

https://mcfp.weebly.com/mcfp-dataset.html

## 恶意软件数据库
> MalwareDB 包含了恶意软件列表 hash,检测结果，所属域名等数据
- 内容类型: 文本样本
- 使用范围: 特征库 入侵检测

http://malwaredb.malekal.com/

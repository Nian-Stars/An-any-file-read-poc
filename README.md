# MilesightVPN任意文件读取漏洞POC脚本
## 使用方法如下:
# 单一URL检测
## 1、通过命令行界面去检测单个的URL地址，使用-U参数传递URL参数
## 2、观察返回的结果,如果显示is vulnerable!说明这个URL中存在这个漏洞，否则表示漏洞不存在
# 批量URL检测
## 1、可以将利用FOFA搜索到的资产或者说想要测试的URL放入到任意的TXT文件中
## 2、通过命令行界面去调用存储着URL的TXT文件，使用-U参数对文件中的URL进行批量的扫描
## 3、观察返回的结果,如果显示is vulnerable!说明这个URL中存在这个漏洞，否则表示漏洞不存在
< br >
# 脚本进行单一URL检测的使用方法演示：
## 此处演示使用的是FoFa中找到的一个"资产"
## 1、使用python3 Any-File-Read.py -u http://xxxxx.com进行执行
## 2、观察返回的结果
# 执行结果如下
![示例](https://github.com/Nian-Stars/An-any-file-read-poc/blob/main/res-one.jpg)
# 脚本进行批量URL检测的使用方法演示：
## 此处演示使用的是FoFa中找到的一个"资产"
## 1、使用python3 Any-File-Read.py -f url.txt进行执行
## 2、观察返回的结果
# 执行结果如下
![示例](https://github.com/Nian-Stars/An-any-file-read-poc/blob/main/res-some.jpg)
< br >
# 扫描到存在的漏洞URL之后，我们选择一个URL进行访问检测
## 访问结果如下：
![示例](https://github.com/Nian-Stars/An-any-file-read-poc/blob/main/burp.jpg)
< br >
# 免责声明：
# 文章所涉及内容，仅供安全研究与教学之用，由于传播、利用本文所提供的信息而造成的任何直接或者间接的后果及损失，均由使用者本人负责，作者不为此承担任何责任。

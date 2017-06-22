# NKU-SMS-RSS
RSS support for School of Mathematical Sciences, Nankai University

## 说明
每十分钟抓取一次[南开数院](http://sms.nankai.edu.cn)的文章标题、日期及链接，生成xml文件便于订阅rss，同时推送邮件。

## 订阅
 - 学院新闻：[http://www.oncemath.com/sms-rss/xyxw.xml](http://www.oncemath.com/sms-rss/xyxw.xml)
 - 本科生教育：[http://www.oncemath.com/sms-rss/bksjy.xml](http://www.oncemath.com/sms-rss/bksjy.xml)
 - 研究生教育：[http://www.oncemath.com/sms-rss/yjsjy.xml](http://www.oncemath.com/sms-rss/yjsjy.xml)
 - 科研动态：[http://www.oncemath.com/sms-rss/kydt.xml](http://www.oncemath.com/sms-rss/kydt.xml)
 - 学生工作：[http://www.oncemath.com/sms-rss/xsgz.xml](http://www.oncemath.com/sms-rss/xsgz.xml)
 - 公共数学：[http://www.oncemath.com/sms-rss/ggsx.xml](http://www.oncemath.com/sms-rss/ggsx.xml)
 
## 使用
 - 需要Python3环境，并按需安装模块
 - 更改`config/config.py`中的相关配置信息，同时在`config/receivers`中添加收件人信息(奇数行填写收件人的姓名等相关信息，偶数行填写对应的邮箱地址)
 - 通过命令`python3 main.py`即可运行，可配合crontab进行定时作业
 
## 注意
 - 使用crontab时，务必确保代码内的路径都是恰当的**绝对路径**，否则可能会报错
 - 在服务器上运行时，注意不要泄露`config/config.py`中的密码等相关信息
 
## 其他
感谢[@yqnku](http://www.quicy.cn)

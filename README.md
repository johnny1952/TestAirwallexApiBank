# TestAirwallexApiBank

## 介绍
API Test framework:
JMeter 4.0 + Jenkins 2.127

## 维护脚本
- 用例CRUD
使用JMeter4打开testBank1.jmx，并进行用例增删改查。

- 修改测试环境
修改env.csv文件，把内容改为目的环境ip或域名即可。

## 运行测试
- 在Jenkins上执行；

- 或通过命令行远程执行构建：
Run the tests:
curl "http://203.195.231.169:8080/job/test-jmeter-Airwallex-API-bank-1/buildWithParameters?token=TESTAIRWALLEX&env=preview.airwallex.com" --user test:test

如果需要更换环境，则修改env的参数值即可。

## 查看结果
View test result:
http://203.195.231.169:8080/job/test-jmeter-Airwallex-API-bank-1/HTML_20Report/

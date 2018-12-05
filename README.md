# Work-Notes
## Kali Linux ssh
開啟
```
$ sudo service ssh start
```
查詢是否開啟
```
$ netstat -ap | grep ssh
```

## Putty ssh root 登入
vim /etc/ssh/sshd_config
```
PermitRootLogin yes
```

## Kali Linux sources.list 來源
vim /etc/apt/sources.list
```
#中科大
deb http://mirrors.ustc.edu.cn/kali kali-rolling main non-free contrib
deb-src http://mirrors.ustc.edu.cn/kali kali-rolling main non-free contrib

#阿里雲
deb http://mirrors.aliyun.com/kali kali-rolling main non-free contrib
deb-src http://mirrors.aliyun.com/kali kali-rolling main non-free contrib

#清大
deb http://mirrors.tuna.tsinghua.edu.cn/kali kali-rolling main contrib non-free
deb-src https://mirrors.tuna.tsinghua.edu.cn/kali kali-rolling main contrib non-free

#浙大
deb http://mirrors.zju.edu.cn/kali kali-rolling main contrib non-free
deb-src http://mirrors.zju.edu.cn/kali kali-rolling main contrib non-free

#東軟大
deb http://mirrors.neusoft.edu.cn/kali kali-rolling/main non-free contrib
deb-src http://mirrors.neusoft.edu.cn/kali kali-rolling/main non-free contrib

#官方源
deb http://http.kali.org/kali kali-rolling main non-free contrib
deb-src http://http.kali.org/kali kali-rolling main non-free contrib
```

## Discover index 解釋

|Index|Description|
|:----:|:----|
|atp* ||
|autorun-* ||
|dhcp* ||
|dns-* ||
|elastalert ||
|elastalert_error ||
|elastalert_status ||
|freenas-* ||
|metricbeat* ||
|nmap* ||
|officesan-* ||
|other* ||
|pa3020* ||
|proxy-* ||
|service ||
|softwareasset-* ||
|sslvpnnew* ||
|sslvpnold* ||
|usg-* ||
|winlogbeat*||
|xecprobe-* ||
|zyxelsocedr-* ||

## 常見詞彙
EDR
```
Endpoint Detection and Response(端點偵測及回應解決方案)
EDR 是自動化鑑識的流程，是去分析軌跡而不只是去掃惡意程式。
例如，某端點一掃，沒有發現病毒但事實上已被入侵，因為駭客不一定要安裝病毒或後門，
只要新增一個帳號，就可以從外連線進來，放置可疑的檔案。
即使駭客攻擊主程式變成已知的惡意程式後，就可被掃毒軟體刪掉，但駭客可以隨時再回來，再安裝新的後門。
```

ELK
```
ELK 是由 Elasticsearch、Logstash 及 Kibana 三個系統所組成的 Log 蒐集、分析、查詢系統。
```

ATP
```

```

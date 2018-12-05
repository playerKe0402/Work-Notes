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

|index|Description|Event ID|Description|
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


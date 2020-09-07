安装SpeedTest:
```
yum install wget -y

wget https://bintray.com/ookla/rhel/rpm -O bintray-ookla-rhel.repo

mv bintray-ookla-rhel.repo /etc/yum.repos.d/

yum install speedtest -y

speedtest
```
删除冲突项:
```
rpm -qa | grep speedtest | xargs -I {} sudo yum -y remove {}
```

# clickhouse-setup
clickhouse数据库和集群设置

### 集群依赖
zookeeper集群，设置参考[zookeeper-setup](./https://github.com/miaoyc666/zookeeper-setup)

### 准备工作
##### 1.目录创建
```bash
mkdir -p /etc/clickhouse-server   # yum安装时会创建该目录，/etc/clickhouse-server为默认目录
mkdir -p /run/clickhouse-server
mkdir -p /data/clickhouse
mkdir -p /var/log/clickhouse
```

##### 2.编辑配置文件
```bash
cp config.xml metrika.xml users.xml /etc/clickhouse-server  # 如已编辑好，直接拷贝到默认配置目录
```

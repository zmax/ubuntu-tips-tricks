## 計算空間的使用量

```bash
du -sh ./*
du -shL ./*
```

## 備份

```
# 從 A server 備份到本機
rsync -avz --delete --ignore-errors user@a-server:/pathA/ /pathB/

# 從本機備份到 A server
rsync -avz --delete --ignore-errors /pathB user@a-server:/pathA
```

## 查用什麼程式占用了什麼 port

```
sudo lsof -i -n -P | grep TCP
```

## Service auto-start

```
# To start a daemon at startup
# defaults => default run levels 2,3,4 and 5
update-rc.d service_name defaults

# To remove
update-rc.d serivce_name remove

```
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

## 讓 service 自動啟動

```
# To start a daemon at startup
# defaults => default run levels 2,3,4 and 5
update-rc.d service_name defaults

# To remove
update-rc.d serivce_name remove

```


## 教學連結

- [How to Install the Ajenti Control Panel and Ajenti V on Ubuntu 14.04](https://www.digitalocean.com/community/tutorials/how-to-install-the-ajenti-control-panel-and-ajenti-v-on-ubuntu-14-04)
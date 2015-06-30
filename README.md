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
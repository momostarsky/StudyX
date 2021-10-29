### 调整 ubuntu swap 大小
[来源](https://www.jianshu.com/p/e656bead51ee)

- 执行

```sudo swapon -s```

命令，查看是否已经存在swap file

- 如果第一步存在swapfile则需要先禁用

```sudo swapoff /swapfile```

- 修改swap 空间的大小为8G

```sudo dd if=/dev/zero of=/swapfile bs=1M count=8192```

- 设置文件为“swap file”类型

```sudo mkswap /swapfile```

- 启用swapfile


```sudo swapon /swapfile```



作者：_核桃_
链接：https://www.jianshu.com/p/e656bead51ee
来源：简书
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。

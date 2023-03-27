# rc_operation_manual

## ---2023/3/28 Update---

1.

雷达IP ：192.168.1.11

需要在上位机设置静态IP

设置方法链接：

[ubuntu修改配置IP地址和DNS的方法总结（4种）_ubuntu修改ip_豆豆技术派的博客-CSDN博客](https://blog.csdn.net/davidhzq/article/details/102991577)

具体应使用eno1网卡，不要用其他网卡。

具体参照如下设置：

```
auto eno1
iface eno1 inet static
address 192.168.1.20
netmask 255.255.255.0
gateway 0.0.0.0
```

2.

设置主从机IP

参考博客操作：[一遍成功的ROS主从机详细配置_zhanghm1995的博客-CSDN博客](https://blog.csdn.net/zhanghm1995/article/details/106781954)

3.调解offset

先全部给0，到达指定位置后，再取负数

具体用 rostopic echo命令查看数据

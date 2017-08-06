# Test Plan

<!-- TOC -->

- [Test Plan](#test-plan)
    - [待测算法](#待测算法)
    - [性能指标](#性能指标)
    - [测试场景](#测试场景)
    - [实验拓扑](#实验拓扑)
    - [测试工具](#测试工具)
    - [测试内容](#测试内容)

<!-- /TOC -->

## 待测算法

1.  测试组：
    +   bbr
    +   bic
    +   cubic
    +   highspeed
    +   htcp
    +   hybla
    +   illinois
    +   scalable
    +   vegas
    +   yeah
2.  对照组：
    +   reno
    +   ctcp

## 性能指标

+   Retransmission Ratio
+   RTT
+   Thoroughput
+   Fairness
+   Efficiency
+   Goodput
+   Download Time

## 测试场景

+   100M 局域网
+   1G -10G 数据中心内部高速网络
+   1M - 10M 国内互联网
+   亚马逊跨国网络

## 实验拓扑

+   2 × 2 哑铃型拓扑
+   单臂双方向
+   单臂单方向

## 测试工具

+   FTP
+   Iperf 3
+   Traffic Generator
+   PING
+   Mininet
+   iftop
+   getsockopt
+   tcp_probe
+   ss

## 测试内容

+   真实网络测试
    +   
+   Mininet 仿真测试
    +   在不同延迟下的吞吐率测试
    +   在不同丢包率下的吞吐率测试
    +   在不同带宽下的吞吐率测试
    +   以上组合

<h1>Test Plan</h1>

<!-- TOC -->

- [待测算法](#待测算法)
- [性能指标](#性能指标)
- [测试场景](#测试场景)
- [实验拓扑](#实验拓扑)
- [测试工具](#测试工具)
- [测试内容](#测试内容)
- [Reference](#reference)

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

+   Retransmission Ratio（重传率）：iperf 3 提供了应该发出的总流量，用 iftop 可以获取此 TCP 链接实际发出的总流量，相减即可获得被重传的流量
+   RTT
+   Thoroughput（吞吐量）：以 iperf 3 提供的带宽
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

+   2 × 2 双向双通道
+   1 × 1 单向单通道
+   1 × 1 单向双通道

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

## Reference

+   Grieco L A, Mascolo S. Performance evaluation and comparison of Westwood+, New Reno, and Vegas TCP congestion control[M]. ACM, 2004.
+   Lai Y C, Yao C L. TCP congestion control algorithms and a performance comparison[C]// Computer Communications and Networks, 2001. Proceedings. Tenth International Conference on. IEEE, 2001:523-526.
+   Lukaseder T, Bradatsch L, Erb B, et al. A Comparison of TCP Congestion Control Algorithms in 10G Networks[C]// Local Computer Networks. IEEE, 2016:706-714.
+   Yeganeh S H, Yeganeh S H, Yeganeh S H, et al. BBR: congestion-based congestion control[J]. Communications of the Acm, 2017, 60(2):58-66.

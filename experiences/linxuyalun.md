# Interview

## Alibaba 流量产品事业部

### 一面

#### 简历相关

1. 为什么使用微服务？casecloud 的微服务架构是怎么样的？
2. Istio 是怎么应用在项目中的，数据面的流量是怎么走的，怎么利用 Istio 的各种 Kind 做的流量控制？了解 Istio 控制面吗？都有哪些组件构成，各有啥作用？xDS 是什么，都包括哪些，各做哪些事？
3. casecloud 中鉴权服务是怎么做的？流量是如何控制的？
4. Kubernetes 中 CRD 的作用以及如何开发？

#### 基础知识相关

1. TCP 四次挥手，具体流程，time_wait 和 close_wait 哪个是主动哪个是被动？
2. IP 分片是什么？TCP 和 UDP 谁更容易分片，为什么？TCP 如何保证准确性？
3. 写一个 TCP 服务大致的流程是什么？
4. I/O 多路复用是什么？epoll 和 select 有啥差别？
5. 简述堆排序；
6. Golang 中使用过的网络编程用的什么库，咋用的？
7. Golang GC 是怎么弄的？

#### 算法

1. 确定链表中存在环；
2. 二叉树翻转；
3. 确定存在环的链表的环的起点。

#### 复盘

1. 一些比较擅长的点回答的不够充分；
2. 整体的节奏被面试官带走了，没有引导面试官的提问方向，在网络这一块周旋的时间过长，可以把重点多往 Kubernetes 方向带；
3. 过于紧张。

### 二面

#### 简历相关

1. casecloud 是什么，业务上解决了什么事？你具体负责了哪些工作，都干了什么？
2. 鉴权服务怎么做的？为什么要这么做？
3. casecloud 的架构是什么？假设有一个人申请债权，整体流量鉴权都是怎么走的？
4. 你们集群服务的动态扩缩容是怎么做的？具体的实现细节？
5. 整个项目里的难点都有哪些？你是怎么做的？
6. 都看过云原生哪些项目源码？

#### 基础知识

1. 有一个队列，能入队出队，还能同时拿到队列最小值。这个数据结构咋实现？
2. 哈希表实现？
3. 讲一讲 http 拥赛控制原理？
4. 进程间通信都有哪些方法？
5. socket 编程了解情况？
6. Golang 语言特性都有哪些？Golang goroutine 底层实现是怎样的？
7. 如何写一个高并发服务器？
8. service mesh 是啥？它的作用是什么？解决了什么事？
9. serverless 优缺点？聊了一些毕设相关话题，怎么解决冷启动优化的？怎么解决进程间通信的？怎么调度的？
10. 技术上面的爱好？未来规划？

#### 复盘

1. 吸取了第一次的经验，在遇到不是很清楚的地方讲一些类似技术的细节；
2. 有在引导话题。

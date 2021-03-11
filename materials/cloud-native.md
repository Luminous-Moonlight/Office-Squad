# Cloud-Native

## Kubernetes

### Basic

* 基本架构：都有啥组件，都是干啥的，部署在哪种类型节点上；
* 声明式 API ：作用和意义，GVK 的意思；
* 集群资源管理：Label，污点和容忍；QoS；
* 各种 Kind 的基础知识：
  * Pod：Init Pod，Pause 容器，Pod Hook，Pod Lifecycle
  * Deployment：为啥要分为 Deployment，ReplicaSet 和 Pod 三级；
  * StatefulSet：作用意义，更新模式；
  * 其他常见的 Kind 等；

* 参考：[Kubernetes Handbook](https://jimmysong.io/kubernetes-handbook/)。

### Pro

* [What happens when I type `kubectl run`?](https://github.com/jamiehannaford/what-happens-when-k8s/tree/master/zh-cn) 
* Informer Model：[图解原理](https://www.kubernetes.org.cn/6905.html)和[深入剖析](https://cloudnative.to/blog/client-go-informer-source-code/)；
* Scheduler：[阅读调度设计精要](https://draveness.me/system-design-scheduler/)，直接搜“Kubernetes 是生产级别的容器调度和管理系统”快速跳转到 Kubernetes 部分；
* Network：TODO；
* CNI，CSI，CRI：TODO；
* Etcd：[Etcd 分布式存储原理](https://draveness.me/etcd-introduction/)；
* 常见[面试题](https://github.com/cloudnativeto/sig-kubernetes/issues/37)。

## Istio

### Basic

* 基础架构：区分控制面（Pilot，Citadel，Galley）和数据面（Envoy），以及它们的作用；
* Sidecar：sidecar 作用和意义；透明流量劫持；
* 流量控制：常见 Kind 和作用；
* 参考：[Istio Handbook](https://www.servicemesher.com/istio-handbook/concepts/istio.html)。


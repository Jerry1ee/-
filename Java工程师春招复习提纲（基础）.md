### Java基础部分

#### JVM虚拟机

##### Java运行时数据区域和内存模型

- 内存布局以及特点
- OOM异常、Stackoverflow异常的场景
- 垃圾收集算法、分代理论、常见GC场景、可达性分析、常见垃圾收集器
- Java内存模型

##### **类文件结构**

了解即可

##### **类加载机制**

- 类加载时机和类的生命周期
- 类加载过程（加载、验证、准备、解析、初始化）
- 类加载器、双亲委派模型、Java模块化

##### Java内存模型与线程

- Java主内存和工作内存、内存交互操作
- volatile型变量相关以及原子性、可见性和有序性
- 线程的实现与调度、状态转换

##### 线程安全与锁优化

- Java线程安全及实现方法
- CAS操作以及问题
- 锁优化（自旋锁、自适应自旋、锁消除、锁粗化、轻量级锁、偏向锁）

附上一份读书笔记 https://blog.csdn.net/weixin_43925277/article/details/104313943

#### Java基础

##### 基础知识

- 面向对象概念、Java语言的特性、封装多态继承和抽象
- 基本数据结构、拆箱装箱
- HashCode方法以及equals和“==”
- Java异常处理机制
- Java反射机制
- Java注解和JDK8之后的新特性

##### 基础集合类源码

- Integer、String

- List接口及实现类
- HashMap、HashSet以及TreeMap
- ConcurrentHashMap以及HashTable
- java.util.concurrent包下，重入锁，闭锁和原子类，ThreadLocal，线程池

##### 语言应用

- 锁在Java编程的应用
- IO操作在Java的应用以及网络编程

### MySQL数据库

##### SQL**语句执行过程**

- 客户端、server层及存储引擎
- 连接器-查询缓存-分析-优化-执行步骤
- 各种引擎的区别

##### log文件

- redolog 和binlog以及undolog
- 两阶段提交
- binlog的写入机制和策略

##### 事务隔离

- 隔离性和隔离级别
- 事务隔离的实现 MVCC
- 事务启动方式
- 幻读以及如何解决

##### 索引

- 常见索引存储模型
- InnoDB为什么用B+树
- 聚簇和非聚簇索引、回表操作、索引维护
- 索引覆盖和最左前缀原则、索引下推
- 索引的选择与优化问题
- change buffer
- 自增主键和普通主键

##### 锁

- 全局锁、表锁和行锁
- 视图的作用
- 两阶段锁和死锁
- 间隙锁和索引联系起来的规则

**其他**

- 刷脏页时刻
- 重建表的注意事项
- 表的备份与恢复，保证主备一致性及并行复制
- 全字段排序以及rowid排序
- 磁盘临时表、优先队列算法和归并排序算法
- 长连接和连接池
- 慢查询怎么追踪问题所在
- 读写分离方案的设计
- 临时表的使用场景和特性

##### 语言使用

- join的使用注意事项，执行的原理及优化
- “%”、group by 、order by 等使用注意事项
- having 和 where and  的使用
- limit 怎么用的

### 计算机网络

##### 整体架构

- 各种分层模型以及区别
- 网络协议的目的

##### 物理层和链路层

- 链路层都有哪些设备？
- MAC的含义，多路访问协议
- IP和MAC如何关联
- 交换机和Hub，交换机的拓扑结构
- 网关的作用

**网络层**

- ICMP（**Internet Control Message Protocol**）协议格式和目的，查询报文和差错报文
- ping是怎么工作的
- IP怎么来的，DHCP的工作原理，子网掩码和网段含义
- 路由策略与动态路由协议（OSPF和BGP），了解即可

##### 传输层

- UDP和TCP含义、特点及区别
- UDP包格式及使用场景
- TCP包格式、三次握手和四次挥手各步骤状态图
- TCP顺序和丢包的解决方案、超时重传、流量控制、拥塞控制及滑动窗口机制

##### 应用层

- Socket套接字及连接过程，细节问题
- Http协议格式，内容
- Http1.0,1.1,2.0区别，与websocket的区别
- Https怎么实现，具体内容，与Http的区别
- 流媒体协议、P2P、DNS协议以及CDN（了解即可）

##### 其他

- 云原生网络通信 Flannel和Calico
- RPC协议，SOAP协议
- 描述从输入网址到获得网页结果的整个过程

### 操作系统

##### 进程线程

- 进程和线程的区别
- 实现方式

##### 死锁

- 原因、条件及处理方法

##### 内存管理

- 常驻、虚拟、共享内存，如何映射
- 分页分段管理、缺页
- 内核态和用户态切换

##### 其他

- IO模型（BIO/NIO/AIO）
- 零拷贝
- Linux的基础知识

### 数据结构与算法

- 了解常用数据结构（链表、队列、栈、树、图等），原理特点和实现
- 刷题
  - 剑指offer
  - leetcode 热题Top100

### 拓展的

以下部分不再属于基础方面，每个部门都可以延伸出很多知识

#### NoSQL数据库

- Redis和MongoDB各自特点，区别，使用场景
- 数据结构及底层原理
- 使用实践

#### 框架

Spring Boot、Netty、TomCat、RocketMQ、RabbitMQ、Dubbo等

##### 以springBoot为例

- 介绍，优势、好处、IOC及AOP的原理
- 自动配置和起步依赖的原理
- 源码（拓展）

#### 设计模式

明白原理，一些简单实现

#### 分布式

- 分布式锁和事务
- zookeeper、Spring Cloud组件以及对比

#### 云原生

- k8s、docker的原理及实现
- docker和虚拟机的异同

#### 开源中间件

#### gitflow项目开发流程

#### 






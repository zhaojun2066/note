# java 基础
#### 面向对象、面向过程
#### 平台无关性
#### 编译过程
#### java 反编译工具 ，并举例说明怎么使用
#### 字节码
#### jvm
#### java 语法糖 以及 原理 
#### 语法糖 语法糖：switch 支持 String 与枚举、泛型、自动装箱与拆箱、方法变长参数、枚举、内部类、条件编译、 断言、数值字面量、for-each、try-with-resource、Lambda表达式
#### java 语言规范
#### java 是值传递还是引用传递，还是二者都有
#### 什么是多态、方法重写与重载
#### 怎么实现继承、怎么实现组合
#### 基本数据类型有哪些，以及它们的取值范围
#### 什么是浮点型，什么是单精度，什么是双精度，浮点型为什么不能用来存储金额，应该怎么存储金额
#### 什么是包装类型，什么是自动拆包箱，自动的时候要注意什么
#### Integer 是有缓存机制，具体原理是怎么实现的，其他类型Long之类的有缓存机制吗
#### String 类型相关，intern()方法是干什么用的,StringBuffer ,StringBuilder原理区别
#### String + ，jdk 做了什么优化
#### 字符串一般怎么拼接
#### 字符串池、常量池（运行时常量池、Class常量池）、intern，要深入理解
#### transient
#### synchronized 原理
#### volatile 原理
#### switch 原理

#### java反射是什么，都用再什么场景，实际你用过吗？
#### 什么叫代理模型？ 动态代理、静态代理，两种方式怎么实现？
#### AOP 怎么实现？原理

#### 序列化和反序列怎么实现，单例怎么防止序列化或者反序列化一个新的对象
#### 序列化实现 Serializable 和 Externalizable 二者有什么区别
#### 序列化反序列化 java相关的类 ObjectOutput  ObjectInput ObjectOutputStream ObjectInputStream
#### 怎么让某个字段不进行序列化，静态字段会序列化吗

#### 什么注解，怎么实现注解，一般你会用再什么场景
#### 泛型、类型擦除、限定通配符和非限定通配符、上下界限定符extends 和 super
#### 正表达式相关

####JMS JMX 都是什么

==========================  


#### java 集合相关的类图继承关系
#### Set List 有啥区别在java中。
#### HashMap、HashTable、ConcurrentHashMap区别
#### ArrayList和LinkedList和Vector的区别
#### HashMap 数据结构、put、get 原理、扩容原理
#### Set 怎么实现数据不重复，HashSet原理。
#### java8 中 stream 用法。
#### Collection和Collections区别
#### Arrays.asList获得的List使用时需要注意什么
#### fail-fast 和 fail-safe 
#### CopyOnWriteArrayList
#### ConcurrentHashMap原理 

==============  

#### 枚举是什么，枚举有哪些用法和场景
#### 枚举怎么实现单例，以及枚举的序列化和反序列的控制
#### 为什么枚举实现单例 是线程安全的

=======================
#### 什么是 字符流、字节流、输入流、输出流
#### 什么是同步、异步、阻塞、非阻塞
#### 什么是BIO、AIO、NIO，他们的区别是什么

#### 异常分哪些类型
#### try-with-resources 怎么使用
#### 什么是Error 什么是Exception
#### 具体你遇到的运行时异常，至少5个
#### finally return 执行的顺序，举例说明


======
#### 什么是并行
#### 什么是并发
#### 并行和并发的区别
#### java 如何实现线程 
#### 自己实现线程池，线程池怎么用
#### 说说java自带的线程池ThreadPoolExecutor 参数的意思，你平时都怎么用这个类
#### 如何实现线程安全，有哪些方法。

#### 锁： CAS、乐观锁与悲观锁、数据库相关锁机制、分布式锁、偏向锁、轻量级锁、重量级锁、monitor、锁优化、锁消除、锁粗化、自旋锁、可重入锁、阻塞锁、死锁
#### 死锁，举例说明，然后说说如何避免

#### synchronized和lock的区别、不使用synchronized如何实现一个线程安全的单例
#### 聊聊java的内存模型（不是jvm内存结构，别记混了）
#### synchronized和原子性、可见性和有序性之间的关系
#### volatile和原子性、可见性和有序性之间的关系，说说实际怎么用volatile
#### happens-before、内存屏障、编译器指令重排和CPU指令重排

#### sleep wait notify notifyAll 说明
#### ThreadLocal 原理 和使用场景
#### java并发包你用过哪些 举例说明
    Thread、Runnable、Callable、ReentrantLock、ReentrantReadWriteLock、Atomic*、Semaphore、CountDownLatch、、ConcurrentHashMap、Executors


============================== 



#### jvm 内存结构 （java8之后有什么变化）
#### class 文件格式
#### jvm 运行时数据区：堆、栈、方法区、直接内存、运行时常量池、
#### 什么是堆 什么是栈
#### java 对象一定会分配到堆上吗？
#### new java 对象怎么内存的过程？
#### 垃圾回收算法 重点看，新老生代怎么回收。
#### cms 垃圾回收重点看

#### 类加载机制
#### 编译和反编译
#### 什么JIT
#### 反编译工具
    javap 、jad 、CRF

#### jvm 启动参数 
    -Xmx、-Xmn、-Xms、Xss、-XX:SurvivorRatio、
    -XX:PermSize、-XX:MaxPermSize、-XX:MaxTenuringThreshold
#### java 对象模型
    oop-klass、对象头
#### 虚拟机性能监控与故障处理工具 都要会用
    jps, jstack, jmap、jstat, jconsole, jinfo, jhat, javap, btrace、TProfiler Arthas       
    
================

#### 怎么实现递归
#### CPU缓存，L1，L2，L3和伪共享
#### 设计模型 23中 ，实际用过多少
#### 单例有哪些实现方式，说说区别，怎么防止反序列单例
#### 不用synchronized和lock，实现线程安全的单例模式
#### 自己实现AOP
#### 自己实现IOC

    

    
     
    




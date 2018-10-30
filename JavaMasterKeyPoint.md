### 介绍  
  
* [请你介绍下所做的项目](https://mp.weixin.qq.com/s/brSm7ZrV53U6qZPIsUxQdQ?)  
    周期、技术、功能、整体架构、承担角色、优缺点、困难及成长。  
  
### Java基础  
  
#### 基础  
  
* [面向对象特征](https://blog.csdn.net/lyg_come_on/article/details/52781884)  
    封装、继承和多态。  
* [final, finally, finalize的区别](https://blog.csdn.net/cyl101816/article/details/67640843)  
    final是关键字。被final修饰的类，就意味着不能再派生出新的子类，不能作为父类而被子类继承。  
    finally是关键字。在异常处理时提供finally块来执行任何清除操作。  
    finalize()是方法。Object类的finalize()在垃圾收集器将对象从内存中清除出去之前做必要的清理工作。  
* [int 和 Integer 有什么区别](https://blog.csdn.net/login_sonata/article/details/71001851)  
    int是基本数据类型。  
    Integer是int的包装类型，是对象。  
    基本数据类型：boolean，char，byte，short，int，long，float，double。  
    包装类型：Boolean，Character，Byte，Short，Integer，Long，Float，Double。  
* [重载和重写的区别](https://blog.csdn.net/u010697681/article/details/79414112#_73)  
    重写（Override）是指子类对父类方法的一种重写，只能比父类抛出更少的异常，访问权限不能比父类的小。被重写的方法不能是 private的，否则只是在子类中重新定义了一个方法；  
    重载（Overload）表示同一个类中可以有多个名称相同的方法，但这些方法的参数列表各不相同。函数的返回值不同不可以构成重载。  
* [抽象类和接口有什么区别](https://blog.csdn.net/dengminghli/article/details/71056874)  
    1.抽象类可以有具体方法，可以没有抽象方法，而接口中只能存在抽象方法（默认 public abstract），Java8 中接口中会有 default 方法。  
    2.抽象类中可以有普通的成员变量；接口中的变量必须是 static final 类型的，必须被初始化 , 接口中只有常量，没有变量。  
    3.一个类只能继承一个抽象类（单继承），但可以实现多个接口（多继承）。  
    4.抽象类中允许含有静态代码块和静态方法，而接口类不能。  
* [说说反射的用途及实现](https://blog.csdn.net/SongYuxinIT/article/details/81872066)  
    反射允许程序在运行时对其内部成员进行操作，最重要的用途就是开发各种通用框架。  
    反射主要功能有：获取Class对象、构造器、成员变量和方法；创建对象；调用方法。  
* [说说自定义注解的场景及实现](https://blog.csdn.net/qq_37581282/article/details/82655326)  
    登录、权限拦截、日志处理，以及各种 Java 框架，如 Spring ，Hibernate，JUnit。  
* [HTTP 请求的 GET 与 POST 方式的区别](https://www.cnblogs.com/ouyanxia/p/8205307.html)  
    GET：  
    请求的数据会附加在URL之后，以?分割URL和传输数据，多个参数用&连接；  
    在HTTP规范中，没有对长度和大小限制，但是浏览器和服务器对URL的长度有限制；  
    明文传输会造成数据泄露及CSRF攻击；  
    产生一个TCP数据包。  
    POST：  
    请求的数据放置在HTTP请求包的包体中；  
    理论无限制，但是服务器会对POST提交数据大小进行限制；  
    参数在消息主体中，参数不会被保存在缓存、浏览器历史或日志中；  
    产生两个TCP数据包。  
* [session 与 cookie 区别](https://blog.csdn.net/liyifan687/article/details/80077928)  
    Cookies是服务器在本地机器上存储的小段文本并随每一个请求发送至同一服务器，是在客户端保持状态的方案。  
    Session是存在服务器的一种用来存放用户数据的类HashTable结构。浏览器发送请求时，服务器自动生成了HashTable和Session ID来唯一标识这个HashTable，并将其发送到浏览器。浏览器再次请求会将Session ID一并发送到服务器，服务器提取出Session ID，找到对应的HashTable。  
    区别：  
    Session 能够存储任意的 Java 对象，Cookie 只能存储 String 类型的对象;  
    一个在客户端一个在服务端。Cookie伪造；  
    域的支持范围不一样，跨域资源共享。  
* [JDBC 流程](https://www.cnblogs.com/lightandtruth/p/9473862.html)  
    注册驱动  
    建立连接(Connection)  
    创建运行SQL的语句(Statement)  
    运行语句  
    处理运行结果(ResultSet)  
    释放资源  
* [MVC 设计思想](https://blog.csdn.net/daijin888888/article/details/51169156)  
    将一个软件按照模型、视图、控制器进行划分。其中，模型用来封装业务逻辑，视图用来实现表示逻辑，控制器用来协调模型与视图。  
    优点：  
    实现模型的复用，不用关心处理结果如何展现；  
    代码的维护性更好；  
    方便测试；  
* [equals 与 == 的区别](https://blog.csdn.net/g_66_hero/article/details/71081315)  
    ==比较的是内存地址；  
    equals用来比较的是两个对象的内容是否相等，重写Object类的equals方法，默认是==；  
    String中当且仅当该参数不为 null，并且是与此对象表示相同字符序列的 String 对象时，结果才为 true。  
* [NIO和IO的区别](https://www.jb51.net/article/50621.htm)  
    IO 面向流 阻塞  
    NIO 面向缓冲 非阻塞IO 选择器  
* [JAVA 锁有哪些种类，以及区别](https://www.cnblogs.com/lxmyhappy/p/7380073.html)  
    公平锁/非公平锁  
    可重入锁  
    独享锁/共享锁  
    互斥锁/读写锁  
    乐观锁/悲观锁  
    分段锁  
    偏向锁/轻量级锁/重量级锁  
    自旋锁  
* [Java 对象的生命周期](https://blog.csdn.net/moneyshi/article/details/53033578)  
    创建阶段、应用阶段、不可见阶段、不可达阶段、收集阶段、终结阶段、对象空间重新分配阶段  
* [JVM](https://blog.csdn.net/hsk256/article/details/49104955)  
* JVM内存划分  
    方法区，虚拟机栈，本地方法栈，堆，程序计数器  
  
* GC算法  
    引用计数法，无法解决循环引用问题  
    可达性算法，可以作为GC Roots的对象：  
    虚拟机栈中引用的对象  
    方法区类静态属性引用的对象  
    方法区常量池引用的对象  
    本地方法栈JNI引用的对象  
  
* 垃圾收集的方法  
    标记-清除：效率不高，会产生大量内存碎片。  
    复制算法：内存划分为8:1:1三部分，Eden区，Survior区。老年代中。  
    标记-整理：解决标记-清除产生大量内存碎片的问题。  
    分代收集：在新生代对象生存期短，有大量对象死去，采用复制算法。老年代里对象存活率高，没有额外的空间，使用标记-整理 或者 标记-清除。  
  
* 内存模型  
    线程之间的共享变量存储在主内存（main memory）中，每个线程都有一个私有的本地内存（local memory），本地内存中存储了该线程以读/写共享变量的副本。  
    线程A与线程B之间如要通信的话，必须要经历下面2个步骤：  
    1、首先，线程A把本地内存A中更新过的共享变量刷新到主内存中去。  
    2、然后，线程B到主内存中去读取线程A之前已更新过的共享变量。  
  
* 类加载过程  
    加载，验证，准备，解析，初始化  
  
* 双亲委派  
    当一个类收到了类加载请求时，不会自己先去加载这个类，而是将其委派给父类，由父类去加载，如果此时父类不能加载，反馈给子类，由子类去完成类的加载。  
    确保了在各种加载环境的加载顺序，保证了唯一性和运行的安全性。  
  
* 类加载器有哪些？  
    实现通过类的权限定名获取该类的二进制字节流的代码块叫做类加载器。  
    主要有一下四种类加载器:  
    启动类加载器(Bootstrap)用来加载java核心类库，无法被java程序直接引用。  
    扩展类加载器(Extension):它用来加载 Java 的扩展库。Java 虚拟机的实现会提供一个扩展库目录。该类加载器在此目录里面查找并加载 Java 类。  
    应用程序类加载器(System)：它根据 Java 应用的类路径CLASSPATH来加载 Java 类。一般来说，Java 应用的类都是由它来完成加载的。可以通过 ClassLoader.getSystemClassLoader()来获取它。  
    用户自定义类加载器，通过继承 java.lang.ClassLoader类的方式实现。  
  
* 内存分配与回收策率以及Minor GC和Major GC  
    对象优先在堆的Eden区分配。  
    大对象直接进入老年代。  
    长期存活的对象将直接进入老年代。  
    当Eden区没有足够的空间进行分配时，虚拟机会执行一次Minor GC.Minor Gc通常发生在新生代的Eden区，在这个区的对象生存期短，往往发生Gc的频率较高，回收速度比较快;Full Gc/Major GC 发生在老年代，一般情况下，触发老年代GC的时候不会触发Minor GC,但是通过配置，可以在Full GC之前进行一次Minor GC这样可以加快老年代的回收速度。  
  
#### 集合  
  
* [List 和 Set 区别](https://www.cnblogs.com/IvesHe/p/6108933.html)  
    List，Set都是继承自Collection接口；  
    List有顺序，可重复，检索效率高，插入删除效率低；  
    Set无顺序，不可重复，检索效率低，删除和插入效率高。  
    
* [List 和 Map 区别](https://www.cnblogs.com/IvesHe/p/6108933.html)  
    List是对象集合，允许对象重复。  
    Map是键值对的集合，不允许key重复。  
* [Arraylist 与 LinkedList 区别](https://blog.csdn.net/qq_32679815/article/details/78907437)  
    Arraylist基于数组，检索效率高，插入删除效率低；  
    LinkedList基于链表，检索效率低，删除和插入效率高。  
* [ArrayList 与 Vector 区别](https://www.cnblogs.com/efforts-will-be-lucky/p/7053666.html)  
    Vector是多线程安全的，ArrayList不是，Vector效率比ArrayList低；  
    初始10，空间不足的时候，扩容方式不同，Vector可以设置增长因子，而ArrayList不可以。  
* [HashMap 和 Hashtable 的区别](https://www.cnblogs.com/efforts-will-be-lucky/p/7053666.html)  
    HashMap 把 HashTable 的contains方法替换为containsValue()和containsKey()方法;  
    Hashtable 是同步的，HashMap 是非同步的，HashMap 效率高;  
    HashMap 允许空键值，而 Hashtable 不允许。  
* [HashSet 和 HashMap 区别](https://www.cnblogs.com/codercui/p/6841730.html)  
    Set是线性结构，Set中的值不能重复，HashSet是Set的hash实现，HashSet中值不能重复是用HashMap的key来实现的。  
    Map是键值对映射，可以空键空值。HashMap是Map接口的hash实现，key的唯一性是通过key值hash值的唯一来确定，value值是则是链表结构。  
* [HashMap 和 ConcurrentHashMap 的区别](https://www.cnblogs.com/heyonggang/p/9112731.html)  
    ConcurrentHashMap对整个桶数组进行了分割分段(Segment)，然后在每一个分段上都用lock锁进行保护，相对于HashTable的syn关键字锁的粒度更精细了一些，并发性能更好，而HashMap没有锁机制，不是线程安全的；  
    HashMap的键值对允许有null，但是ConcurrentHashMap都不允许。  
* [HashMap 的工作原理及代码实现](http://www.importnew.com/28263.html)  
    初始容量16，负载因子0.75，扩容后数组大小为当前的 2 倍。  
    原理：  
    根据 key 的 hashcode 计算 hash 值。  
    找到相应的数组下标：hash & (length – 1)。  
    遍历该数组位置处的链表，Entry的hash与key hash相等，并且key equals。  
    Java 8在链表长度大于8后替换为红黑树。  
* [ConcurrentHashMap 的工作原理及代码实现](http://www.importnew.com/28263.html)  
    segment。  
    并发操作使用 CAS。  
    循环获取锁。  
* [HashMap 的优化](http://www.importnew.com/21429.html)  
    考虑加载因子地设定初始大小 (int) ((float) expectedSize / 0.75F + 1.0F)  
    减小加载因子  
    String类型的key，不能用==判断或者可能有哈希冲突时，尽量减少长度  
    使用定制版的EnumMap  
    使用IntObjectHashMap  
  
#### 线程  
  
* [创建线程的方式及实现](https://www.cnblogs.com/wxw7blog/p/7727510.html)  
    Thread，Runnable，Callable，使用Executor  
    Runnable和Callable的区别：  
    Callable方法是call()，Runnable方法是run()；  
    Callable执行后可返回值，Runnable不能返回值；  
    call方法可以抛出异常，run方法不可以  
    Callable可以获取一个Future对象，表示异步计算的结果。可以了解任务执行情况，可取消任务，还可获取执行结果。  
* [sleep() 、join()、yield()有什么区别](https://blog.csdn.net/u011296485/article/details/77914205)  
    sleep()不释放锁，必须捕获异常  
    wait()是Object类中的，wait，notify和notifyAll只能在同步方法或同步代码块中调用  
    yield()方法只会给相同优先级或更高优先级的线程运行的机会。  
    join()使所属的线程对象x正常执行run()方法中的任务，而使当前线程z进行无限期的阻塞，直到线程x执行完成之后(销毁后)再继续执行线程z后面的代码。在内部使用wait()方法进行等待。  
    注意：在执行notify()或notifyAll()方法后，当前线程不会马上释放该对象锁，需要等到notify()或notifyAll()方法所在的同步方法或同步代码块执行完成，当前线程才会释放锁。  
* [说说 CountDownLatch 原理](https://www.jianshu.com/p/7c7a5df5bda6?ref=myread)  
    一个任务A，它要等待其他4个任务执行完毕之后才能执行  
    Sync继承AQS，await()，countDown()  
* [说说 CyclicBarrier 原理](https://www.jianshu.com/p/060761df128b)  
    让一组线程等待至某个状态之后再全部同时执行  
    ReentrantLock，Condition，Generation  
    await()，dowait()，reset()  
* [说说 Semaphore 原理](https://www.jianshu.com/p/060761df128b)  
    Semaphore可以控同时访问的线程个数，通过 acquire() 获取一个许可，如果没有就等待，而 release() 释放一个许可。  
    Sync继承AQS，acquire()，release()  
* [说说 CountDownLatch 与 CyclicBarrier 区别](https://blog.csdn.net/u010697681/article/details/79414112#_CountDownLatch__CyclicBarrier__614)  
    CountDownLatch  
    减计数方式  
    计算为0时释放所有等待的线程  
    计数为0时，无法重置  
    调用countDown()方法计数减一，调用await()方法只进行阻塞，对计数没任何影响  
    不可重复利用  
  
    CyclicBarrier  
    加计数方式  
    计数达到指定值时释放所有等待线程  
    计数达到指定值时，计数置为0重新开始  
    调用await()方法计数加1，若加1后的值不等于构造方法的值，则线程阻塞  
    可重复利用  
* [CountDownLatch、CyclicBarrier、Semaphore 用法](http://www.cnblogs.com/dolphin0520/p/3920397.html)  
    见上  
* [说说 Exchanger 原理](http://lixuanbin.iteye.com/blog/2166772)  
    ThreadLocal  
    exchange  
* [ThreadLocal 原理分析](https://www.cnblogs.com/dolphin0520/p/3920407.html)  
    在每个线程Thread内部有一个ThreadLocal.ThreadLocalMap类型的成员变量threadLocals，键值为当前ThreadLocal变量，value为变量副本（即T类型的变量）。  
    初始时，在Thread里面，threadLocals为空，当通过ThreadLocal变量调用get()方法或者set()方法，就会对Thread类中的threadLocals进行初始化，并且以当前ThreadLocal变量为键值，以ThreadLocal要保存的副本变量为value，存到threadLocals。  
    然后在当前线程里面，如果要使用副本变量，就可以通过get方法在threadLocals里面查找。  
* [讲讲线程池的实现原理](http://www.cnblogs.com/dolphin0520/p/3932921.html)  
    ThreadPoolExecutor  
    成员：核心线程数，最大线程数，空闲时间及单位，阻塞队列（ArrayBlockingQueue，LinkedBlockingQueue，SynchronousQueue），线程工厂，拒绝处理  
    主要方法：execute()，submit()，shutdown()，shutdownNow()  
    1、线程池状态：RUNNING，SHUTDOWN，STOP，TERMINATED  
    2、任务的执行  
    3、线程池中的线程初始化  
    4、任务缓存队列及排队策略  
    下面都假设任务队列没有大小限制：  
    如果线程数量<=核心线程数量，那么直接启动一个核心线程来执行任务，不会放入队列中。  
    如果线程数量>核心线程数，但<=最大线程数，并且任务队列是LinkedBlockingDeque的时候，超过核心线程数量的任务会放在任务队列中排队。  
    如果线程数量>核心线程数，但<=最大线程数，并且任务队列是SynchronousQueue的时候，线程池会创建新线程执行任务，这些任务也不会被放在任务队列中。这些线程属于非核心线程，在任务完成后，闲置时间达到了超时时间就会被清除。  
    如果线程数量>核心线程数，并且>最大线程数，当任务队列是LinkedBlockingDeque，会将超过核心线程的任务放在任务队列中排队。也就是当任务队列是LinkedBlockingDeque并且没有大小限制时，线程池的最大线程数设置是无效的，他的线程数最多不会超过核心线程数。  
    如果线程数量>核心线程数，并且>最大线程数，当任务队列是SynchronousQueue的时候，会因为线程池拒绝添加任务而抛出异常。  
    任务队列大小有限时  
    当LinkedBlockingDeque塞满时，新增的任务会直接创建新线程来执行，当创建的线程数量超过最大线程数量时会抛异常。  
    SynchronousQueue没有数量限制。因为他根本不保持这些任务，而是直接交给线程池去执行。当任务数量超过最大线程数时会直接抛异常。  
    5、任务拒绝策略  
    ThreadPoolExecutor.AbortPolicy:丢弃任务并抛出RejectedExecutionException异常。  
    ThreadPoolExecutor.DiscardPolicy：也是丢弃任务，但是不抛出异常。  
    ThreadPoolExecutor.DiscardOldestPolicy：丢弃队列最前面的任务，然后重新尝试执行任务（重复此过程）  
    ThreadPoolExecutor.CallerRunsPolicy：由调用线程处理该任务  
    6、线程池的关闭  
    7、线程池容量的动态调整  
* [线程池的几种方式与使用场景](https://blog.csdn.net/cyantide/article/details/50880211)  
    newFixedThreadPool(int nThreads)  
    创建一个固定长度的线程池，每当提交一个任务就创建一个线程，直到达到线程池的最大数量，这时线程规模将不再变化，当线程发生未预期的错误而结束时，线程池会补充一个新的线程  
    newCachedThreadPool()  
    创建一个可缓存的线程池，如果线程池的规模超过了处理需求，将自动回收空闲线程，而当需求增加时，则可以自动添加新线程，线程池的规模不存在任何限制  
    newSingleThreadExecutor()  
    这是一个单线程的Executor，它创建单个工作线程来执行任务，如果这个线程异常结束，会创建一个新的来替代它；它的特点是能确保依照任务在队列中的顺序来串行执行  
    newScheduledThreadPool(int corePoolSize)  
    创建了一个固定长度的线程池，而且以延迟或定时的方式来执行任务，类似于Timer。  
* [线程的生命周期](https://blog.csdn.net/houbin0912/article/details/77969563)  
    新建(New)、就绪(Runnable)、运行(Running)、阻塞(Blocked)和死亡(Dead)  
  
#### 锁机制  
  
* [说说线程安全问题](https://www.cnblogs.com/xumanbu/p/4203504.html)  
    程序运行在多线程环境下吗？  
    多线程是否会共享一个资源并且对这个共享资源有读和写操作？  
    1、将对象设置成无状态的  
    2、使用局部对象  
    3、可以考虑使用ThreadLocal  
    4、使用线程同步  
* [volatile 实现原理](https://blog.csdn.net/calledwww/article/details/79350426)  
    保证内存可见性（但不保证操作的原子性）。  
    防止指令重排。  
    通过内存屏障和禁止指令重排序来保证内存可见性的：  
    在每个volatile写操作的前面插入一个StoreStore屏障。  
    在每个volatile写操作的后面插入一个StoreLoad屏障。  
    在每个volatile读操作的后面插入一个LoadLoad屏障。  
    在每个volatile读操作的后面插入一个LoadStore屏障。  
* [synchronized 实现原理](https://www.cnblogs.com/paddix/p/5367116.html)  
    进入时，执行 monitorenter，将计数器 +1，释放锁 monitorexit 时，计数器-1；  
    当一个线程判断到计数器为 0 时，则当前锁空闲，可以占用；反之，当前线程进入等待状态。  
  
    Synchronized 是在加锁，加对象锁。对象锁是一种重量锁（monitor），synchronized 的锁机制会根据线程竞争情况在运行时会有偏向锁（单一线程）、轻量锁（多个线程访问 synchronized 区域）、对象锁（重量锁，多个线程存在竞争的情况）、自旋锁等。  
  
    该关键字是一个几种锁的封装。  
* [synchronized 底层优化](http://www.cnblogs.com/paddix/p/5405678.html)  
    重量级锁，轻量级锁，偏向锁，适应性自旋，锁粗化，锁消除  
* [synchronized 与 lock 的区别](https://www.cnblogs.com/iyyy/p/7993788.html)  
    1、synchronized是关键字，Lock是java类；  
    2、synchronized无法判断是否获取锁的状态，Lock可以判断是否获取到锁；  
    3、synchronized会自动释放锁(a 线程执行完同步代码会释放锁 ；b 线程执行过程中发生异常会释放锁)，Lock需在finally中手工释放锁（unlock()方法释放锁），否则容易造成线程死锁；  
    4、用synchronized关键字的两个线程1和线程2，如果当前线程1获得锁，线程2线程等待。如果线程1阻塞，线程2则会一直等待下去，而Lock锁就不一定会等待下去，如果尝试获取不到锁，线程可以不用一直等待就结束了；  
    5、synchronized的锁可重入、不可中断、非公平，而Lock锁可重入、可判断、可公平（两者皆可）  
    6、Lock锁适合大量同步的代码的同步问题，synchronized锁适合代码少量的同步问题。  
* [AQS 源码分析](https://blog.csdn.net/aesop_wubo/article/details/7555956)  
    AQS采用的是CLH队列  
    CANCELLED：因为超时或者中断，结点会被设置为取消状态，被取消状态的结点不应该去竞争锁，只能保持取消状态不变，不能转换为其他状态。处于这种状态的结点会被踢出队列，被GC回收；  
    SIGNAL：表示这个结点的继任结点被阻塞了，到时需要通知它；  
    CONDITION：表示这个结点在条件队列中，因为等待某个条件而被阻塞；  
    PROPAGATE：使用在共享模式头结点有可能牌处于这种状态，表示锁的下一次获取可以无条件传播；  
    0：None of the above，新结点会处于这种状态。  
  
    public final void acquire(int arg);  
    public final void acquireInterruptibly(int arg);  
    public final void acquireShared(int arg);  
    public final void acquireSharedInterruptibly(int arg);  
    protected boolean tryAcquire(int arg);  
    protected int tryAcquireShared(int arg);  
    public final boolean tryAcquireNanos(int arg, long nanosTimeout) throws InterruptedException;  
    public final boolean tryAcquireSharedNanos(int arg, long nanosTimeout) throws InterruptedException;  
  
    public final boolean release(int arg);  
    protected boolean tryRelease(int arg);  
    protected boolean tryReleaseShared(int arg);  
* [ReentrantLock 实现原理](https://www.cnblogs.com/xrq730/p/4979021.html)  
    ReentrantLock根据传入构造方法的布尔型参数实例化出Sync的实现类FairSync和NonfairSync，分别表示公平的Sync和非公平的Sync。  
    NonfairSync.lock()->AQS.acquire(1)->NonfairSync.tryAcquire(1)->Sync.nonfairTryAcquire(1)->AQS.addWaiter(1)->AQS.enq(node)0>AQS.acquireQueued(node, 1)->Node.predecessor()->AQS.shouldParkAfterFailedAcquire(pNode,node)->AQS.parkAndCheckInterrupt()  
    NofairSync.unlock()->AQS.release()->NofairSync.tryRelease()->AQS.unparkSuccessor(node)->AQS.acquireQueued()->Node.predecessor()->AQS.shouldParkAfterFailedAcquire(pNode,node)->AQS.parkAndCheckInterrupt()  
* [CAS 乐观锁](https://blog.csdn.net/caisongcheng_good/article/details/79916873)  
    CAS是项乐观锁技术，当多个线程尝试使用CAS同时更新同一个变量时，只有其中一个线程能更新变量的值，而其它线程都失败，失败的线程并不会被挂起，而是被告知这次竞争中失败，并可以再次尝试。CAS是一种非阻塞式的同步方式。  
    CAS 操作包含三个操作数 —— 内存位置（V）、预期原值（A）和新值(B)。如果内存位置的值与预期原值相匹配，那么处理器会自动将该位置值更新为新值。否则，处理器不做任何操作。无论哪种情况，它都会在 CAS 指令之前返回该位置的值。  
* [ABA 问题](https://www.cnblogs.com/549294286/p/3766717.html)  
    因为CAS需要在操作值的时候检查下值有没有发生变化，如果没有发生变化则更新，但是如果一个值原来是A，变成了B，又变成了A，那么使用CAS进行检查时会发现它的值没有发生变化，但是实际上却变化了。ABA问题的解决思路就是使用版本号。在变量前面追加上版本号，每次变量更新的时候把版本号加一，那么A－B－A 就会变成1A-2B－3A。  
* [乐观锁的业务场景及实现方式](https://blog.csdn.net/lxy344x/article/details/76560243)  
    乐观锁，使用版本标识来确定读到的数据与提交时的数据是否一致。提交后修改版本标识，不一致时可以采取丢弃和再次尝试的策略。  
    CAS操作包含三个操作数，内存位置（V）,预期原值（A）和新值（B）。如果内存位置的值与预期原值相匹配，那么处理器会西东将该位置值更新为新值。否则，处理器不做任何操作。  
  
* [Java 8 新特性](http://www.importnew.com/11908.html)  
    Lambda 表达式  
    接口默认与静态方法  
    方法引用  
    重复注解和扩展注解  
    Optional  
    Stream  
    新Date/Time API，不可变的、线程安全的  
    Base64  
    并行数组  
    HashMap 的底层实现：链表大于8会转换为红黑树  
    JVM 由元空间代替了永久代，元空间并不在虚拟机中，而是使用本地内存  
  
### 核心篇  
  
#### 数据存储  
  
* [MySQL 索引使用的注意事项](http://blog.720ui.com/2017/mysql_core_04_index_item/)  
    1、不要在列上使用函数和进行运算  
    2、尽量避免使用 != 或 not in或 <> 等否定操作符  
    3、尽量避免使用 or 来连接条件  
    4、多个单列索引并不是最佳选择  
    5、复合索引的最左前缀原则  
    6、覆盖索引的好处  
    7、范围查询对多列查询的影响  
    8、索引不会包含有NULL值的列  
    9、隐式转换的影响  
    10、like 语句的索引失效问题  
* [说说反模式设计](http://blog.720ui.com/2017/mysql_core_07_anti-pattern/)  
* [说说分库与分表设计](http://blog.720ui.com/2017/mysql_core_08_multi_db_table/)  
    垂直拆分，把表的字段进行拆分，即一张字段比较多的表拆分为多张表，这样使得行数据变小。  
    水平拆分，有许多策略，例如，取模分表，时间维度分表，以及自定义 Hash 分表，例如用户 ID 维度分表等  
    存在分布式事务的问题。  
    存在跨节点Join的问题。  
    存在跨节点合并排序、分页的问题。  
    存在多数据源管理的问题。  
  
    分表：提高并发性能  
    分库：减轻 MySQL 服务器的压力，仍然存在同一个物理机上的资源竞争和瓶颈，包括 CPU、内存、磁盘 IO、网络带宽等。  
* [分库与分表带来的分布式困境与应对之策](http://blog.720ui.com/2017/mysql_core_09_multi_db_table2/)  
    1、数据迁移与扩容问题  
    2、表关联问题  
    3、分页与排序问题  
    4、分布式事务问题  
    5、分布式全局唯一ID  
* [分库与分表1](https://www.cnblogs.com/sunny3096/p/8595058.html)  
* [分库与分表2](https://www.cnblogs.com/sheseido/p/8880091.html)  
* [水平分库如何做到平滑扩展](https://baijiahao.baidu.com/s?id=1584744472767329273&wfr=spider&for=pc)  
* [分库分表后如何部署上线](https://www.cnblogs.com/rjzheng/p/9597810.html)  
    停机部署法  
    双写部署法-消息队列  
    双写部署法-binlog  
    
    验数据一致性  
    验数量  
    验关键性的几个字段  
    拼字符串md5进行加密  
* [说说 SQL 优化之道](http://www.cnblogs.com/yunfeifei/p/3850440.html)  
    EXPLAIN  
    只要一行数据时使用 LIMIT 1  
    建索引  
    在Join表的时候使用相当类型的例，并将其索引  
    避免 SELECT *  
    尽可能的使用 NOT NULL  
* [数据库优化的几个阶段](https://www.cnblogs.com/rjzheng/p/9619855.html)  
    优化sql和索引  
    搭建缓存  
    读写分离  
    利用分区表  
    垂直拆分  
    水平拆分  
* [MySQL 遇到的死锁问题](https://www.cnblogs.com/zejin2008/p/5262751.html)  
    当多个用户并发地存取数据 时，在数据库中就会产生多个事务同时存取同一数据的情况。若对并发操作不加控制就可能会读取和存储不正确的数据，破坏数据库的一致性。加锁是实现数据库并 发控制的一个非常重要的技术。在实际应用中经常会遇到的与锁相关的异常情况，当两个事务需要一组有冲突的锁，而不能将事务继续下去的话，就会出现死锁，严 重影响应用的正常执行。  
* [存储引擎的 InnoDB 与 MyISAM](http://blog.720ui.com/2017/mysql_core_02_innodb_myisam/)  
    1、InnoDB支持事务，MyISAM不支持。  
    2、MyISAM适合查询以及插入为主的应用，InnoDB适合频繁修改以及涉及到安全性较高的应用  
    3、InnoDB支持外键，MyISAM不支持  
    4、从MySQL5.5.5以后，InnoDB是默认引擎  
    5、InnoDB不支持FULLTEXT类型的索引  
    6、InnoDB中不保存表的行数，需要扫描一遍整个表来计算有多少行，但是MyISAM只要简单的读出保存好的行数即可。  
    7、对于自增长的字段，InnoDB中必须包含只有该字段的索引，但是在MyISAM表中可以和其他字段一起建立联合索引  
    8、清空整个表时，InnoDB是一行一行的删除，效率非常慢。MyISAM则会重建表  
    9、InnoDB支持行锁  
* [数据库索引的原理](https://blog.csdn.net/suifeng3051/article/details/52669644)  
* [为什么要用 B-tree](https://blog.csdn.net/bigtree_3721/article/details/73151472)  
    鉴于B-tree具有良好的定位特性，其常被用于对检索时间要求苛刻的场合，例如：  
    1、B-tree索引是数据库中存取和查找文件(称为记录或键值)的一种方法。  
    2、硬盘中的结点也是B-tree结构的。与内存相比，硬盘必须花成倍的时间来存取一个数据元素，这是因为硬盘的机械部件读写数据的速度远远赶不上纯电子媒体的内存。与一个结点两个分支的二元树相比，B-tree利用多个分支（称为子树）的结点，减少获取记录时所经历的结点数，从而达到节省存取时间的目的。  
* [聚集索引与非聚集索引的区别](https://blog.csdn.net/zc474235918/article/details/50580639)  
* [数据库事务](https://www.cnblogs.com/fjdingsd/p/5273008.html)  
    ACID，脏读，不可重复读，虚读。  
    读未提交，读已提交，可重复读，串行化。  
    默认隔离级别是可重复读。  
* [limit 20000 加载很慢怎么解决](http://ourmysql.com/archives/1451)  
* [选择合适的分布式主键方案](http://www.cnblogs.com/haoxinyue/p/5208136.html)  
    1、数据库自增长序列或字段  
    2、UUID  
    3、UUID的变种  
    4、Redis生成ID  
    5、Twitter的snowflake算法  
    6、利用zookeeper生成唯一ID  
    7、MongoDB的ObjectId  
* [选择合适的数据存储方案](http://blog.720ui.com/2017/db_better_db_use/)  
    1、关系型数据库 MySQL  
    2、内存数据库 Redis  
    3、文档数据库 MongoDB  
    4、列族数据库 HBase  
    5、全文搜索引擎 ElasticSearch  
* [ObjectId 规则](https://www.cnblogs.com/weilunhui/p/6861938.html)  
    时间戳：  
    　　时间戳，前四个字节是从标准纪元开始的时间戳，单位是秒。可提供秒级别的唯一性。  
    　　由于时间戳在前，这意味着ObjectId大致按照插入的顺序排列。  
    　　这四个字节也隐含了文档的创建时间。  
    机器：  
    　　主机的唯一标识符。通常是机器主机的散列值（hash）。这样可以确保不同的机器生成不同的ObjectId　　  
    PID：  
    　　为了确保在同一台机器上并发的多个进程产生的ObjectID是唯一的，接下来者两个字节产生来自于进程的标识符  
    计数器：  
    　　最后三个字节是一个自动增加的计数器，确保相同的进程同一秒产生的ObjectId也是不一样的一秒钟最多允许每个进程拥有2563个不同的ObjectId  
* [聊聊 MongoDB 使用场景](https://yq.aliyun.com/articles/64352)  
    应用不需要事务及复杂 join 支持	必须 Yes  
    新应用，需求会变，数据模型无法确定，想快速迭代开发	？  
    应用需要2000-3000以上的读写QPS（更高也可以）	？  
    应用需要TB甚至 PB 级别数据存储	?  
    应用发展迅速，需要能快速水平扩展	?  
    应用要求存储的数据不丢失	?  
    应用需要99.999%高可用	?  
    应用需要大量的地理位置查询、文本查询	？  
* [倒排索引](https://www.cnblogs.com/zlslch/p/6440114.html)  
* [聊聊 ElasticSearch 使用场景](https://blog.csdn.net/king866/article/details/53557250)  
    1、全文搜索（搜索引擎） 在一组文档中查找某一单词所在文档及位置  
    2、模糊匹配 通过用户的输入去匹配词库中符合条件的词条  
    3、商品搜索 通过商品的关键字去数据源中查找符合条件的商品  
* [行列转换](https://www.cnblogs.com/johden2/p/5692765.html)  
* [left join on 后 and 和 where 的区别](https://www.cnblogs.com/johden2/p/5692765.html)  
  
#### 缓存使用  
  
* [Redis 有哪些类型](https://blog.csdn.net/hcmony/article/details/80694560)  
    string，hash，list，set，zset  
    
* [Redis 内部结构](https://www.cnblogs.com/wykCN/p/4533231.html)  
    字符串、双端链表、字典、跳跃表  
* [Redis 内存淘汰机制](https://blog.csdn.net/hcmony/article/details/80694560)  
    定期删除+惰性删除策略  
    定期删除 redis默认每个100ms随机抽取检查，是否有过期的ke，有过期key则删除。  
    惰性删除策略 获取某个key的时候，redis会检查一下，这个key如果设置了过期时间那么是否过期了？如果过期了此时就会删除。  
    内存淘汰策略的  
    1、noeviction：当内存不足以容纳新写入数据时，新写入操作会报错。应该没人用吧。  
    2、allkeys-lru：当内存不足以容纳新写入数据时，在键空间中，移除最近最少使用的key。推荐使用，目前项目在用这种。  
    3、allkeys-random：当内存不足以容纳新写入数据时，在键空间中，随机移除某个key。应该也没人用吧，你不删最少使用Key,去随机删。  
    4、volatile-lru：当内存不足以容纳新写入数据时，在设置了过期时间的键空间中，移除最近最少使用的key。这种情况一般是把redis既当缓存，又做持久化存储的时候才用。不推荐  
    5、volatile-random：当内存不足以容纳新写入数据时，在设置了过期时间的键空间中，随机移除某个key。依然不推荐  
    6、volatile-ttl：当内存不足以容纳新写入数据时，在设置了过期时间的键空间中，有更早过期时间的key优先移除。不推荐  
* [聊聊 Redis 使用场景](https://blog.csdn.net/hcmony/article/details/80694560)  
    1、String 一般做一些复杂的计数功能的缓存。  
    2、hash 这里value存放的是结构化的对象，比较方便的就是操作其中的某个字段。  
    3、list 使用List的数据结构，可以做简单的消息队列的功能。另外还有一个就是，可以利用lrange命令，做基于redis的分页功能，性能极佳，用户体验好。  
    4、set 因为set堆放的是一堆不重复值的集合。所以可以做全局去重的功能。为什么不用JVM自带的Set进行去重？因为我们的系统一般都是集群部署，使用JVM自带的Set，比较麻烦，难道为了一个做一个全局去重，再起一个公共服务，太麻烦了。  另外，就是利用交集、并集、差集等操作，可以计算共同喜好，全部的喜好，自己独有的喜好等功能。  
    5、sorted set sorted set多了一个权重参数score,集合中的元素能够按score进行排列。可以做排行榜应用，取TOP N操作。另外，参照另一篇《分布式之延时任务方案解析》，该文指出了sorted set可以用来做延时任务。最后一个应用就是可以做范围查找。  
* [Redis 持久化机制](http://blog.720ui.com/2016/redis_action_03_rdb_aof/)  
    快照，AOF  
* [Redis 集群方案与实现](http://blog.720ui.com/2016/redis_action_04_cluster/)  
    先更新数据库，再更新缓存  
    先删除缓存，再更新数据库  
    先更新数据库，再删除缓存  
* [Redis 为什么是单线程的](https://blog.csdn.net/hcmony/article/details/80694560)  
    操作的对象是内存中的数据结构。如果在多线程中操作，那就需要为这些对象加锁。最终来说，多线程性能有提高，但是每个线程的效率严重下降了。而且程序的逻辑严重复杂化。  
    1、纯内存操作  
    2、单线程操作，避免了频繁的上下文切换  
    3、采用了非阻塞I/O多路复用机制  
* [缓存崩溃](https://blog.csdn.net/hcmony/article/details/80694560)  
    1、给缓存的失效时间，加上一个随机值，避免集体失效。  
    2、使用互斥锁，但是该方案吞吐量明显下降了。  
    3、双缓存。我们有两个缓存，缓存A和缓存B。缓存A的失效时间为20分钟，缓存B不设失效时间。自己做缓存预热操作。  
* [缓存降级](https://blog.csdn.net/hcmony/article/details/80694560)  
    1、利用互斥锁，缓存失效的时候，先去获得锁，得到锁了，再去请求数据库。没得到锁，则休眠一段时间重试  
    2、采用异步更新策略，无论key是否取到值，都直接返回。value值中维护一个缓存失效时间，缓存如果过期，异步起一个线程去读数据库，更新缓存。需要做缓存预热(项目启动前，先加载缓存)操作。  
    3、提供一个能迅速判断请求是否有效的拦截机制，比如，利用布隆过滤器，内部维护一系列合法有效的key。迅速判断出，请求所携带的Key是否合法有效。如果不合法，则直接返回。  
* [使用缓存的合理性问题](http://blog.720ui.com/2016/redis_action_01_use_core/)  
    1、热点数据，缓存才有价值  
    2、频繁修改的数据，看情况考虑使用缓存  
    3、数据不一致性  
    4、缓存更新机制  
    5、缓存可用性  
    6、缓存服务降级  
    7、缓存预热  
    8、缓存穿透  
  
#### 消息队列  
  
* [消息队列的使用场景](https://blog.csdn.net/seven__________7/article/details/70225830)  
    异步处理，应用解耦，流量削锋和消息通讯  
  
* [消息的重发补偿解决思路](https://blog.csdn.net/wangtaomtk/article/details/51531278)  
* [消息的幂等性解决思路（已解答，待补充）](https://www.jianshu.com/p/8b77d4583bab?utm_campaign)  
* [消息的堆积解决思路](https://docs.oracle.com/cd/E19148-01/820-0843/6nci9sed1/index.html)  
* [自己如何实现消息队列](https://www.cnblogs.com/yswenli/p/9029587.html)  
* [如何保证消息的有序性](https://yq.aliyun.com/articles/73672)  
  
### 框架篇  
  
#### Spring  
  
* [BeanFactory 和 ApplicationContext 有什么区别](https://blog.csdn.net/qq_36074233/article/details/76153039)  

* [Spring IOC 如何实现](https://www.jianshu.com/p/5c781f264467?from=groupmessage)  
* [Spring IOC 容器初始化过程](https://www.cnblogs.com/chenjunjie12321/p/6124649.html)  
    Resource定位（Bean的定义文件定位）  
    将Resource定位好的资源载入到BeanDefinition  
    将BeanDefiniton注册到容器中  
* [Spring Bean 的生命周期](https://blog.csdn.net/a327369238/article/details/52193822)  
    postProcessBeanFactory(ConfigurableListableBeanFactory c)  
    实现BeanFactoryPostProcessor接口  
    
    postProcessBeforeInstantiation(Class<？>c,String beanName)  
    实现InstantiationAwareBeanPostProcessor接口  
    
    postProcessAfterInstantiation(Object bean,String beanName)  
    同上  
    
    postProcessPropertyValue  
    同上  
    
    setBeanName(String beanName)  
    实现BeanNameAware接口  
    
    setBeanFactory(BeanFactory factory)  
    实现BeanFactoryAware接口  
    
    postProcessBeforeInitialization(Object bean,String beanName)  
    实现InstantiationAwareBeanPostProcessor接口  
    
    afterPropertiesSet()  
    实现InitializingBean接口  
    
    xml_init()  
    init-method=”xml_init”  
    
    postProcessAfterInitialization(Object bean,Strign beanName)  
    实现BeanPostProcessor接口  
    
    destroy()  
    实现DisposableBean接口  
    
    xml_destroy()  
    destroy-method=”xml_destroy”  
* [说说 Spring AOP](https://www.cnblogs.com/hongwz/p/5764917.html)  
* [Spring AOP 实现原理](https://blog.csdn.net/moreevan/article/details/11977115/)  
* [动态代理（cglib 与 JDK）](https://blog.csdn.net/u013126379/article/details/52121096)  
    如果目标实现了接口，默认情况下会采用JDK的动态代理实现AOP  
    JDK动态代理只能对实现了接口的类生成代理  
    CGLIB是针对类实现代理，主要是对指定的类生成一个子类，覆盖其中的方法  
* [Spring 事务实现方式](https://blog.csdn.net/liaohaojian/article/details/70139151)  
* [Spring 事务底层原理](https://blog.csdn.net/u010853261/article/details/78118619)  
* [如何自定义注解实现功能](https://www.jb51.net/article/131472.htm)  
* [Spring MVC 运行流程](https://blog.csdn.net/james_shu/article/details/54616120)  
* [Spring MVC 启动流程](https://www.cnblogs.com/RunForLove/p/5688731.html)  
* [Spring MVC 和 Struts 的区别](https://blog.csdn.net/generalyy0/article/details/7003974)  
    类级别 方法级别  
* [Spring 的单例实现原理](https://blog.csdn.net/cs408/article/details/48982085)  
    普通单例不能被继承，单例注册表，HashMap对象  
* [Spring 框架中用到了哪些设计模式](https://www.cnblogs.com/jifeng/p/7398852.html)  
* [Spring 其他产品（Srping Boot、Spring Cloud、Spring Secuirity、Spring Data、Spring AMQP 等）](https://www.jianshu.com/p/b3e4aaa83a7d)  
  
#### Netty  
  
* [为什么选择 Netty](https://blog.csdn.net/a953713428/article/details/65629552)  
* [说说业务中，Netty 的使用场景](http://www.52im.net/thread-163-1-1.html)  
* [原生的 NIO 在 JDK 1.7 版本存在 epoll bug](https://www.cnblogs.com/JAYIT/p/8241634.html)  
* [什么是TCP 粘包/拆包，解决办法](https://blog.insanecoder.top/tcp-packet-splice-and-split-issue/)  
* [Netty 线程模型](https://blog.csdn.net/wangjinnan16/article/details/78377642)  
* [说说 Netty 的零拷贝](https://my.oschina.net/plucury/blog/192577)  
* [Netty 内部执行流程](https://www.cnblogs.com/f1194361820/p/5656440.html)  
* [Netty 重连实现](http://www.importnew.com/25046.html)  
  
### 微服务篇  
  
#### 微服务  
  
* [前后端分离是如何做的](http://blog.720ui.com/2016/arch_web_server/)  

* [如何解决跨域](http://blog.720ui.com/2016/web_cross_domain/)  
    CORS跨域资源共享，Nginx  
* [微服务哪些框架](https://www.sohu.com/a/201844693_100038984)  
* [你怎么理解 RPC 框架](http://blog.jobbole.com/92290/)  
    服务消费方（client）调用以本地调用方式调用服务；  
    client stub接收到调用后负责将方法、参数等组装成能够进行网络传输的消息体；  
    client stub找到服务地址，并将消息发送到服务端；  
    server stub收到消息后进行解码；  
    server stub根据解码结果调用本地的服务；  
    本地服务执行并将结果返回给server stub；  
    server stub将返回结果打包成消息并发送至消费方；  
    client stub接收到消息，并进行解码；  
    服务消费方得到最终结果。  
* [说说 RPC 的实现原理](https://blog.csdn.net/top_code/article/details/54615853)  
* [说说 Dubbo 的实现原理](https://blog.csdn.net/chao_19/article/details/51764150)  
    Consumer服务消费者，Provider服务提供者。Container服务容器。  
    服务提供者暴露服务的主过程：   
    首先ServiceConfig类拿到对外提供服务的实际类ref，然后将ProxyFactory类的getInvoker方法使用ref生成一个AbstractProxyInvoker实例，到这一步就完成具体服务到invoker的转化。接下来就是Invoker转换到Exporter的过程。  
    服务消费的主过程：   
    首先ReferenceConfig类的init方法调用Protocol的refer方法生成Invoker实例。接下来把Invoker转为客户端需要的接口  
* [你怎么理解 RESTful](https://www.cnblogs.com/binlin1987/p/6971808.html)  
* [说说如何设计一个良好的 API](https://www.jdon.com/48452)  
* [如何理解 RESTful API 的幂等性](https://blog.csdn.net/garfielder007/article/details/55684420)  
* [如何保证接口的幂等性](https://blog.csdn.net/jks456/article/details/71453053)  
    全局唯一ID，去重表，插入或更新，多版本控制，状态机控制  
* [说说 CAP 定理、 BASE 理论](https://www.jdon.com/37625)  
    一致性、可用性、分区容忍性；基本可用、软状态、最终一致；  
* [怎么考虑数据一致性问题](http://www.infoq.com/cn/articles/solution-of-distributed-system-transaction-consistency)  
* [说说最终一致性的实现方案](http://iamzhongyong.iteye.com/blog/2240891)  
    可靠消息最终一致性（事务型消息队列、消息队列+定时补偿机制）  
    TCC编程模式  
    最大努力通知  
* [你怎么看待微服务](https://blog.csdn.net/kde/article/details/51817622)  
* [微服务与 SOA 的区别](https://www.cnblogs.com/ynuo/p/5913955.html)  
* [如何拆分服务](https://blog.csdn.net/u012422829/article/details/68951579?utm_source=itdadao&utm_medium=referral)  
* [微服务如何进行数据库管理](http://www.infoq.com/cn/news/2017/07/managing-data-in-microservices)  
* [如何应对微服务的链式调用异常](https://segmentfault.com/a/1190000011578125)  
    错误或延迟，重试，路由，服务发现，可观察性  
* [对于快速追踪与定位问题](http://www.infoq.com/cn/articles/how-to-realize-distributed-tracking/)  
    植入点或埋点  
    公司	选项	是否开源	优缺点  
    淘宝	EagleEye	否	主要基于内部HSF实现，HSF没有开源，故鹰眼也没有开源  
    Twitter	Zipkin	是	基于Http实现，支持语言较多，比较适合我们公司业务  
    点评	CAT	是	自定义改造难度大，代码比较复杂，侵入代码，需要埋点  
    京东	Hydra	是	主要基于Dubbo实现，不适合公司Http请求为主的场景  
* [微服务的安全](https://segmentfault.com/a/1190000005891501)  
  
#### 分布式  
  
* [谈谈业务中使用分布式的场景](https://blog.csdn.net/jek123456/article/details/54666545)  
  
* [Session 分布式方案](https://blog.csdn.net/u010164936/article/details/56666285)  
    客户端Cookie加密  
    粘性Session  
    服务器Session复制  
    Session共享(缓存)
    Session持久化到数据库
* [分布式锁的场景](https://www.cnblogs.com/yuyutianxia/p/7149363.html)  
    交易系统的金额修改，同一时间只能又一个人操作，比如秒杀场景，同一时间只能一个用户抢到，比如火车站抢票等  
* [分布是锁的实现方案](https://www.cnblogs.com/yuyutianxia/p/7149363.html)  
    基于数据库  
    基于缓存  
    基于Zookeeper  
    从理解的难易程度角度（从低到高）: 数据库 > 缓存 > Zookeeper  
    从实现的复杂性角度（从低到高）: Zookeeper >= 缓存 > 数据库  
    从性能角度（从高到低）: 缓存 > Zookeeper >= 数据库  
    从可靠性角度（从高到低）: Zookeeper > 缓存 > 数据库  
* [分布式事务](https://blog.csdn.net/mine_song/article/details/64118963)  
* [集群与负载均衡的算法与实现](https://www.cnblogs.com/data2value/p/6107450.html)  
    负载均衡算法(随机算法，轮询及加权轮询，最小连接及加权最小连接，哈希算法，IP地址散列，URL散列)  
    负载均衡算法的手段(DNS->数据链路层->IP层->Http层)  
    DNS域名解析、数据链路层负载均衡(LVS)、IP负载均衡(SNAT)、HTTP重定向负载均衡(少见)、反向代理负载均衡(nginx)  
* [CDN](https://help.aliyun.com/document_detail/27101.html?spm=a2c4g.11186623.6.542.17262a14QEcvN2)  
* [Hadoop](https://blog.csdn.net/qq_26437925/article/details/78467216)  
  
#### 安全问题  
  
* [安全要素与 STRIDE 威胁](http://blog.720ui.com/2017/security_stride/)  
    身份假冒（Spoofing）  
    篡改（Tampering）  
    抵赖（Repudiation）  
    信息泄露（Information Disclosure）  
    拒绝服务（Denial of Service）  
    特权提升（Elevation of Privilege）  
  
* [防范常见的 Web 攻击](https://blog.csdn.net/wen_special/article/details/80461394)  
    XSS攻击  
    CSRF攻击  
    SQL注入  
    DDOS攻击  
* [服务端通信安全攻防](http://blog.720ui.com/2016/security_data_transmission/)  
    Base64加密传输  
    DES对称加密  
    AES对称加密  
    升级到HTTPS  
    URL签名  
    双向RSA加密  
* [HTTPS 原理剖析](https://www.cnblogs.com/digdeep/p/4832885.html)  
    1、客户端把支持的协议版本、密钥算法、压缩方法发送给服务端  
    2、服务端确认协议版本、加密算法，以证书的形式返回给客户端 证书中还包含了 公钥 颁证机构 网址 失效日期等  
    3、客户端验证证书，生成一个随机数用证书中的公钥加密，用随机数加密握手消息+握手消息HASH值(签名)发送给服务端  
    4、服务端用私钥来解密取出随机数，用随机数解密握手消息与HASH值，并与传过来的HASH值做对比确认是否一致。然后用随机数加密一段握手消息(握手消息+握手消息的HASH值 )给客户端    
    5、客户端用随机数解密并计算握手消息的HASH，如果与服务端发来的HASH一致，此时握手过程结束，之后所有的通信数据将由之前浏览器生成的随机密码并利用对称加密算法进行加密  
* [HTTPS 降级攻击](http://blog.720ui.com/2016/security_https_tls/)  
    禁用 SSL 3.0 加密协议，防止TLS 1.2 或者 TLS 1.1 或者 TLS 1.0降级到 SSL 3.0 加密协议。  
* [HTTP2.0 与 HTTP1.1 区别](https://blog.csdn.net/sjhuangx/article/details/52299726)  
    二进制格式  
    多路复用  
    报头压缩  
    响应主动推送到客户端缓存  
* [授权与认证](http://blog.720ui.com/2017/msa_oauth2/)  
* [基于角色的访问控制](http://blog.720ui.com/2017/msa_rbac/)  
* [基于数据的访问控制](http://blog.720ui.com/2017/msa_rbac_data/)  
  
#### 性能优化  
  
* [性能指标有哪些](https://www.cnblogs.com/Tpf386/p/7879446.html)  

* [网站流量与性能分析指标](https://blog.csdn.net/st18401238353/article/details/79061032)  
* [如何发现性能瓶颈](http://www.cnblogs.com/zhangyublogs/p/4965870.html)  
* [性能调优的常见手段](https://blog.csdn.net/fanyun_01/article/details/79942408)  
* [说说你在项目中如何进行性能调优](http://blog.51cto.com/caotian/2074652)  
    1、扩容 ，扩容的理解，就是扩充服务器并行处理的能力，简单来说就是加服务器，增加处理请求的能力，例如增加nginx 、tomcat等应用服务器的个数，或者物理服务器的个数，还有加大服务器带宽等等，这里考虑的是硬件方面  
    2、调优 ，调优，包括系统调优和代码调优 。 系统调优就是说加快处理速度，比如我们所提到的CDN、ehcache、redis等缓存技术，消息队列等等，加快服务间的响应速度，增加系统吞吐量，避免并发，至于代码调优，这些就需要多积累了，比如重构、工厂等， 数据库调优    
* 一条sql执行过长的时间，你如何优化，从哪些方面？  
    1、查看sql是否涉及多表的联表或者子查询，如果有，看是否能进行业务拆分，相关字段冗余或者合并成临时表（业务和算法的优化）  
    2、涉及链表的查询，是否能进行分表查询，单表查询之后的结果进行字段整合  
    3、如果以上两种都不能操作，非要链表查询，那么考虑对相对应的查询条件做索引。加快查询速度  
    4、针对数量大的表进行历史表分离（如交易流水表）  
    5、数据库主从分离，读写分离，降低读写针对同一表同时的压力，至于主从同步，mysql有自带的binlog实现 主从同步  
    6、explain分析sql语句，查看执行计划，分析索引是否用上，分析扫描行数等等  
    7、查看mysql执行日志，看看是否有其他方面的问题  
  
### 工程篇  
  
#### 需求分析  
  
* [你如何对需求原型进行理解和拆分]
* [说说你对功能性需求的理解]
* [说说你对非功能性需求的理解]
* [你针对产品提出哪些交互和改进意见]
* [你如何理解用户痛点]
  
#### 设计能力  
  
* [说说你在项目中使用过的 UML 图]
* [你如何考虑组件化]
* [你如何考虑服务化]
* [你如何进行领域建模]
* [你如何划分领域边界]
* [说说你项目中的领域建模]
* [说说概要设计]
  
#### 设计模式  
  
* [你项目中有使用哪些设计模式]
* [说说常用开源框架中设计模式使用分析]
* [说说你对设计原则的理解]
* [23种设计模式的设计理念]
* [设计模式之间的异同，例如策略模式与状态模式的区别]
* [设计模式之间的结合，例如策略模式+简单工厂模式的实践]
* [设计模式的性能，例如单例模式哪种性能更好。]
* [单例模式有几种写法](https://blog.csdn.net/nsw911439370/article/details/50456231)  
    懒汉、饿汉、枚举、静态内部类、双重校验锁
  
#### 业务工程  
  
* [你系统中的前后端分离是如何做的]
* [说说你的开发流程]
* [你和团队是如何沟通的]
* [你如何进行代码评审]
* [说说你对技术与业务的理解]
* [说说你在项目中经常遇到的 Exception]
* [说说你在项目中遇到感觉最难Bug，怎么解决的]
* [说说你在项目中遇到印象最深困难，怎么解决的]
* [你觉得你们项目还有哪些不足的地方]
* [你是否遇到过 CPU 100% ，如何排查与解决]
* [你是否遇到过 内存 OOM ，如何排查与解决]
* [说说你对敏捷开发的实践]
* [说说你对开发运维的实践]
* [介绍下工作中的一个对自己最有价值的项目，以及在这个过程中的角色]
  
#### 软实力  
  
* [说说你的亮点]
* [说说你最近在看什么书]
* [说说你觉得最有意义的技术书籍]
* [说说个人发展方向方面的思考]
* [说说你认为的服务端开发工程师应该具备哪些能力]
* [说说你认为的架构师是什么样的，架构师主要做什么]
* [说说你所理解的技术专家]
  
### HR 篇  
  
* [你为什么离开之前的公司]
* [你为什么要进我们公司]
* [说说职业规划]
* [你如何看待加班问题]
* [谈一谈你的一次失败经历]
* [你觉得你最大的优点是什么]
* [你觉得你最大的缺点是什么]
* [你在工作之余做什么事情]
* [你为什么认为你适合这个职位]
* [你觉得自己那方面能力最急需提高]
* [你来我们公司最希望得到什么]
* [你希望从这份工作中获得什么]
* [你对现在应聘的职位有什么了解]
* [您还有什么想问的]
* [你怎么看待自己的职涯]
* [谈谈你的家庭情况]
* [你有什么业余爱好]
* [你计划在公司工作多久]

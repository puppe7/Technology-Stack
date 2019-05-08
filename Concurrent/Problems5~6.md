

#### 6.volatile关键字的作用
1） 保证数据的可见性， 数据更新时会刷新到主内存
2) volatile则会对禁止语义重排序  
3) 与CAS结合保证原子性-原子类-AtomicInteger  
扩展：CAS原理  
硬件支持一条指令完成操作(4,5是现代处理器才有的指令）  
（1)测试并设置（Tetst-and-Set）  
（2)获取并增加（Fetch-and-Increment）  
（3)交换（Swap）  
（4)比较并交换（**Compare-and-Swap**）  
（5)加载链接/条件存储（Load-Linked/Store-Conditional）  
ABA 问题

#### 7.final关键字  

总结了一些使用final关键字的好处：  
final关键字提高了性能。JVM和Java应用都会缓存final变量。  
final变量可以安全的在多线程环境下进行共享，而不需要额外的同步开销。  
使用final关键字，JVM会对方法、变量及类进行优化。 

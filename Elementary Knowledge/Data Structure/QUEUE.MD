### 《java队列——queue详细分析》

非阻塞队列：ConcurrentLinkedQueue(无界线程安全)，采用CAS机制（compareAndSwapObject原子操作）。  
阻塞队列：ArrayBlockingQueue(有界)、LinkedBlockingQueue（无界）、DelayQueue、PriorityBlockingQueue，采用锁机制；使用 ReentrantLock 锁。
《LinkedList、ConcurrentLinkedQueue、LinkedBlockingQueue对比分析》


#### 1.多线程有什么用？
1）充分利用多核CPU优势  
2）防止阻塞--单核CPU并不会提升效率，反而会因上下文不断切换，导致效率低。但多线程，可以在某个线程挂起时，其他线程依旧能运行  
3）便于建模--多任务项目，可以分成多个子任务，分别创建线程执行任务  

#### 2.创建线程的方式
1） 继承Thread  

2） 实现Runable--相对来说更灵活

3） 通过Callable和Future创建线程  

#### 3.start()方法和run()方法的区别
start()启动线程-run方法会在不同线程交替执行
run()线程方法,如果使用该方法，则同一般单线程一样

#### 4.Runnable接口和Callable接口的区别
Runnable接口中的run()方法的返回值是void，它做的事情只是纯粹地去执行run()方法中的代码而已；Callable接口中的call()方法是有返回值的，是一个泛型，和Future、FutureTask配合可以用来获取异步执行的结果。



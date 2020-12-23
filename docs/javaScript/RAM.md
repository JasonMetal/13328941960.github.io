# 内存问题
  ## 垃圾收集
   JavaScript 具有自动垃圾收集机制。
   这种垃圾收集机制的原理：找到那些不在继续使用的变量，然后释放其占用的内存。
   垃圾收集器会按照固定的时间间隔来执行这一操作。

   ### 标记清除
   JavaScript 中最经常用的垃圾收集方式是**标记清除**。当变量进入环境时，就将这个变量标记为“进入环境”。
   当变量离开环境时，则将其标记为“离开环境”。

   ### 引用计数
   另一个不太常见的垃圾收集策略叫作**引用计数**。引用计数的含义时跟踪记录每个值被引用的次数，
   当这个值的引用次数变成0时，则回收其内存。
1.采用I/O复用的网络模型,但这要分装到Net命名空间去,这样让网络层的逻辑脱离逻辑应用层，
在这之前要解决的问题是 一下的2点，这要写一个类来分装网络包

2.i/o复用型模型实现Reactor模型的网络络库

// TODO
1. 实现一个异步日志系统,用一个线程专门处理写入,加入时间、文件名及路径、
以及输入日志的行数.

2. 应用层,如何封包拆包

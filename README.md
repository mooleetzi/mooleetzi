### basic information

nickname: mooleetzi  
school: Sichuan University  
major: master of computer technology  
email: 13208308200@163.com

### award

1. [2021 Pingcap tinykv 分布式存储训练营 第 4 名](https://asktug.com/t/topic/393068)

### recent focus

static analysis

### learnt course

1. [MIT 6.830](#mit-6830)
2. [MIT 6.S081](#mit-6s081)
3. [MIT 6.824](#mit-6824)
4. [PingCAP Tinykv](#tinykv)

#### MIT 6.830

1. 使用 JAVA 完成一款支持 sql 解析和优化的数据库管理系统

2. 实现基于 HeapFile 的数据存储功能,并具备 BufferPool(基于 LRU 算法),支持 Page 缓存与淘汰功能。
3. 实现基于环路检测（cycleDetect）的锁管理

4. 支持 Sql 解析和查询优化,基于 Histogram 实现了 Join 优化器。

5. 实现事务功能,基于 Page 粒度下的 2PL 协议和 cycleDetect 实现事务 ACID。通过 Redo-log 和 Checkpoint 机制,支持事务的回滚与恢复。

6. 完成了 B+树索引模块,支持查询,插入删除,以及页合并,页分裂的特性。

#### MIT 6.S081

1. 在 qemu 上模拟 riscv，对 xv6 内核进行功能扩展（C+少量 ricv 汇编）
2. 给 xv6 添加功能方法 sleep，通过 pipe 实现 IPC...
3. 实现系统调用 trace
4. 了解 xv6 页表机制，实现可检测哪些页面被访问过
5. 了解陷入过程、riscv 寄存器以及 xv6 方法调用栈，在此基础上实现 backtrace；增加系统调用实现计算程序消费的 CPU 时间
6. 实现 copy-on-wirte fork
7. 实现用户级线程切换
8. to be continued...

#### MIT 6.824

1. 使用 go 实现 Raft 协议的教学方案
2. 了解 MapReduce 模型
3. 实现基于 Raft 协议的副本容错
4. 在第 3 点的基础上完成 KV 存储
5. 在第 4 点的基础上实现分片（Multi-Raft）`由于参加TinyKV，这部分没有实现`

#### TinyKV

1. 使用 go 实现支持分布式事务的键值存储系统

2. PingCAP / Talent-plan TinyKV 训练营第 4 名

3. 基础实现: 根据 Raft 论文,实现了 Raft 模块,具备 Leader 选举,日志复制,Snapshot 等基础功能
4. 对 Proposal 消费提出自己的模型
5. 基于 Region 分区的 Multi-Raft 支持，实现 Region Split 和 Region Merge
6. 搭建 Scheduler 模块,通过 Region 心跳收集,对 Region 进行负载均衡调度,平衡每个 Store 上的 Regoin。
7. 实现了 MVCC 多版本并发控制,并基于 Percolator 模型,支持高性能分布式事务。
8. `824 和 TinyKV 给我最大的收获是结合日志 Debug。给了我对着以10w行为单位的log进行debug的能力；TinyKV实现过程中也培养了我和队友交流的效果，享受思维的碰撞`

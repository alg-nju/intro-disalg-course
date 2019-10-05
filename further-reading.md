# 《分布式算法入门》课程相关论文

## 计算模型与基础理论


```latex bib
@article{Lamport78,
author = {Leslie Lamport},
title = {Time, clocks, and the ordering of events in a distributed system},
journal = {Commun. ACM},
volume = {21},
number = {7},
year = {1978},
issn = {0001-0782},
pages = {558--565},
doi = {http://doi.acm.org/10.1145/359545.359563 },
publisher = {ACM},
address = {New York, NY, USA},
}
```



```latex bib 
@inproceedings{Mattern89,
author = {Friedemann Mattern},
title = {Virtual time and global states of distributed systems},
booktitle = {Proc. International Workshop on Parallel and Distributed Algorithms},
address = {Holland},
year = {1989},
pages = {215--226},
}
```

```latex bib
@article{Herlihy91,
author = {Herlihy, Maurice},
title = {Wait-free Synchronization},
journal = {ACM Trans. Program. Lang. Syst.},
issue_date = {Jan. 1991},
volume = {13},
number = {1},
month = jan,
year = {1991},
issn = {0164-0925},
pages = {124--149},
numpages = {26},
url = {http://doi.acm.org/10.1145/114005.102808},
publisher = {ACM},
} 
```

```latex bib
@inproceedings{Herlihy11,
author = {Herlihy, Maurice and Shavit, Nir},
title = {On the Nature of Progress},
booktitle = {Proceedings of the 15th International Conference on Principles of Distributed Systems},
series = {OPODIS'11},
year = {2011},
isbn = {978-3-642-25872-5},
location = {Toulouse, France},
pages = {313--328},
numpages = {16},
url = {http://dx.doi.org/10.1007/978-3-642-25873-2_22 },
}
```


```latex bib
Lamport 提出 atomic/regular/safe registers 的概念 (Part I: Basic formalism)

@article{Lamport86,
author={Lamport, Leslie},
title={On interprocess communication. Part I: Basic formalism},
journal={Distributed Computing},
volume={1},
number={2},
pages={77-85},
year={1986},
url={http://dx.doi.org/10.1007/BF01786227},
publisher={Springer-Verlag},
}
```

```latex bib
Lamport 提出 atomic/regular/safe registers 的概念 (Part II: Algorithms)

@article{Lamport86,
author={Lamport, Leslie},
title={On interprocess communication. Part II: Algorithms},
journal={Distributed Computing},
volume={1},
number={2},
pages={86-101},
year={1986},
url={http://dx.doi.org/10.1007/BF01786228},
publisher={Springer-Verlag},
}
```

```latex b
定义linearizability (将 Lamport 的 atomic registers 定义扩展到更复杂的数据结构)

@article{Herlihy90,
author = {Herlihy, Maurice P. and Wing, Jeannette M.},
title = {Linearizability: a correctness condition for concurrent objects},
journal = {ACM Transactions on Programming Languages and Systems},
volume = {12},
issue = {3},
month = {July},
year = {1990},
pages = {463--492},
url = {http://doi.acm.org/10.1145/78969.78972},
publisher = {ACM},
}
```

```latex 
在 message-passing 系统上模拟 atomic registers

@article{Attiya95,
author = {Attiya, Hagit and Bar-Noy, Amotz and Dolev, Danny},
title = {Sharing Memory Robustly in Message-passing Systems},
journal = {J. ACM},
issue_date = {Jan. 1995},
volume = {42},
number = {1},
month = jan,
year = {1995},
issn = {0004-5411},
pages = {124--142},
numpages = {19},
url = {http://doi.acm.org/10.1145/200836.200869},
publisher = {ACM},
} 
```

```latex 
多写的register的regularity的定义

@article{Shao11,
author = {Shao, Cheng and Welch, Jennifer L. and Pierce, Evelyn and Lee, Hyunyoung},
title = {Multiwriter Consistency Conditions for Shared Memory Registers},
journal = {SIAM J. Comput.},
issue_date = {February 2011},
volume = {40},
number = {1},
month = jan,
year = {2011},
issn = {0097-5397},
pages = {28--62},
numpages = {35},
url = {http://dx.doi.org/10.1137/07071158X},
doi = {10.1137/07071158X},
acmid = {2078669},
publisher = {Society for Industrial and Applied Mathematics},
address = {Philadelphia, PA, USA},
keywords = {multiwriter registers, mutual exclusion, quorum systems, regularity, shared memory consistency},
} 
```

```latex 
存储访问的公理化建模

@article{Misra86,
author = {Misra, J.},
title = {Axioms for Memory Access in Asynchronous Hardware Systems},
journal = {ACM Trans. Program. Lang. Syst.},
issue_date = {Jan. 1986},
volume = {8},
number = {1},
month = jan,
year = {1986},
issn = {0164-0925},
pages = {142--153},
numpages = {12},
url = {http://doi.acm.org/10.1145/5001.5007},
doi = {10.1145/5001.5007},
acmid = {5007},
publisher = {ACM},
address = {New York, NY, USA},
}
```

```latex bib
consensus number

@article{Herlihy91,
author = {Herlihy, Maurice},
title = {Wait-free Synchronization},
journal = {ACM Trans. Program. Lang. Syst.},
issue_date = {Jan. 1991},
volume = {13},
number = {1},
month = jan,
year = {1991},
issn = {0164-0925},
pages = {124--149},
numpages = {26},
url = {http://doi.acm.org/10.1145/114005.102808},
publisher = {ACM},
} 
```

```latex bib
@inproceedings{Golab11,
author = {Golab, Wojciech and Li, Xiaozhou and Shah, Mehul A.},
title = {Analyzing consistency properties for fun and profit},
booktitle = {Proceedings of the 30th annual ACM SIGACT-SIGOPS symposium on Principles of distributed computing},
series = {PODC '11},
year = {2011},
pages = {197--206},
url = {http://doi.acm.org/10.1145/1993806.1993834 },
publisher = {ACM},
}
```


## 重要问题与经典算法


```
Lamport's Bakery 算法

@article{Lamport74,
author = {Lamport, Leslie},
title = {A New Solution of Dijkstra's Concurrent Programming Problem},
journal = {Commun. ACM},
issue_date = {Aug. 1974},
volume = {17},
number = {8},
month = aug,
year = {1974},
issn = {0001-0782},
pages = {453--455},
numpages = {3},
url = {http://doi.acm.org/10.1145/361082.361093},
publisher = {ACM},
} 
```

```latex 
Lamport的Paxos算法

@misc{Lamport01,
   author = {Leslie Lamport},
   title = {Paxos Made Simple},
   year = {2001},
   month = {nov},
   howpublished = {\url{https://research.microsoft.com/en-us/um/people/lamport/pubs/paxos-simple.pdf}}
}
```



### 不可能性结果

```latex bib
@article{Fischer85,
author = {Fischer, Michael J. and Lynch, Nancy A. and Paterson, Michael S.},
title = {Impossibility of Distributed Consensus with One Faulty Process},
journal = {J. ACM},
issue_date = {April 1985},
volume = {32},
number = {2},
month = apr,
year = {1985},
issn = {0004-5411},
pages = {374--382},
numpages = {9},
url = {http://doi.acm.org/10.1145/3149.214121 },
doi = {10.1145/3149.214121},
acmid = {214121},
publisher = {ACM},
address = {New York, NY, USA},
} 
```

```
@book{Attiya14,
 author = {Attiya, Hagit and Ellen, Faith},
 title = {Impossibility Results for Distributed Computing},
 year = {2014},
 isbn = {9781627051712},
 publisher = {Morgan \& Claypool},
 }
```


```
@Article{Fich2003,
 author="Fich, Faith and Ruppert, Eric",
 title="Hundreds of impossibility results for distributed computing",
 journal="Distributed Computing",
 year="2003",
 month="Sep",
 day="01",
 volume="16",
 number="2",
 pages="121--163",
 issn="1432-0452",
 doi="10.1007/s00446-003-0091-y",
 url="https://doi.org/10.1007/s00446-003-0091-y"
}
```


## 形式化规约与验证

### 模型检验

``` latex bib
@inproceedings{Guo11,
 author = {Guo, Huayang and Wu, Ming and Zhou, Lidong and Hu, Gang and Yang, Junfeng and Zhang, Lintao},
 title = {Practical Software Model Checking via Dynamic Interface Reduction},
 booktitle = {Proceedings of the Twenty-Third ACM Symposium on Operating Systems Principles},
 series = {SOSP '11},
 year = {2011},
 isbn = {978-1-4503-0977-6},
 location = {Cascais, Portugal},
 pages = {265--278},
 numpages = {14},
 url = {http://doi.acm.org/10.1145/2043556.2043582},
 doi = {10.1145/2043556.2043582},
 acmid = {2043582},
 publisher = {ACM},
 address = {New York, NY, USA},
 keywords = {dynamic interface reduction, software model checking, state space reduction},
} 
```

### 定理证明

```latex bib
@inproceedings{Hawblitzel15,
 author = {Hawblitzel, Chris and Howell, Jon and Kapritsos, Manos and Lorch, Jacob R. and Parno, Bryan and Roberts, Michael L. and Setty, Srinath and Zill, Brian},
 title = {IronFleet: Proving Practical Distributed Systems Correct},
 booktitle = {Proceedings of the 25th Symposium on Operating Systems Principles},
 series = {SOSP '15},
 year = {2015},
 isbn = {978-1-4503-3834-9},
 location = {Monterey, California},
 pages = {1--17},
 numpages = {17},
 url = {http://doi.acm.org/10.1145/2815400.2815428},
 doi = {10.1145/2815400.2815428},
 acmid = {2815428},
 publisher = {ACM},
 address = {New York, NY, USA},
} 
```


## 系统设计与实现

### 分布式系统基础

``` latex bib
CAP 定理 (由Eric Brewer在2000年提出; 此处所选是12年后Gilbert和Lynch对CAP定理所作的阐释)

@article{Gilbert12,
author = {Seth Gilbert and Nancy A. Lynch},
title = {Perspectives on the CAP Theorem},
journal ={Computer},
volume = {45},
number = {2},
year = {2012},
pages = {30-36},
doi = {http://doi.ieeecomputersociety.org/10.1109/MC.2011.389},
publisher = {IEEE Computer Society},
}
```

```latex bib
PACELC 权衡 (可看作CAP定理的扩展)

@article{Abadi12, 
author={Abadi, Daniel J.}, 
title={Consistency Tradeoffs in Modern Distributed Database System Design: CAP is Only Part of the Story}, 
journal={Computer}, 
year={2012}, 
month={Feb},
volume={45}, 
number={2}, 
pages={37-42}, 
doi={10.1109/MC.2012.33}, 
publisher = {IEEE Computer Society},
}
```



### 分布式存储系统

``` latex bib
分布共享内存系统

@article{Li89,
author = {Li, Kai and Hudak, Paul},
title = {Memory Coherence in Shared Virtual Memory Systems},
journal = {ACM Trans. Comput. Syst.},
issue_date = {Nov. 1989},
volume = {7},
number = {4},
month = nov,
year = {1989},
issn = {0734-2071},
pages = {321--359},
numpages = {39},
url = {http://doi.acm.org/10.1145/75104.75105},
doi = {10.1145/75104.75105},
acmid = {75105},
publisher = {ACM},
address
```



```latex 
Google的Paxos实现

@inproceedings{Chandra07,
author = {Chandra, Tushar D. and Griesemer, Robert and Redstone, Joshua},
title = {Paxos Made Live: An Engineering Perspective},
booktitle = {Proceedings of the Twenty-sixth Annual ACM Symposium on Principles of Distributed Computing},
series = {PODC '07},
year = {2007},
pages = {398--407},
url = {http://doi.acm.org/10.1145/1281100.1281103},
publisher = {ACM},
} 
```

```latex 
Google的Bigtable

@article{Chang08,
author = {Chang, Fay and Dean, Jeffrey and Ghemawat, Sanjay and Hsieh, Wilson C. and Wallach, Deborah A. and Burrows, Mike and Chandra, Tushar and Fikes, Andrew and Gruber, Robert E.},
title = {Bigtable: A Distributed Storage System for Structured Data},
journal = {ACM Trans. Comput. Syst.},
issue_date = {June 2008},
volume = {26},
number = {2},
month = jun,
year = {2008},
pages = {4:1--4:26},
articleno = {4},
url = {http://doi.acm.org/10.1145/1365815.1365816},
publisher = {ACM},
} 
```

```
Google的Megastore

@inproceedings{Baker11,
title = {Megastore: providing scalable, highly available storage for interactive services},
author  = {Jason Baker and Chris Bond and James C. Corbett and JJ Furman and Andrey Khorlin and James Larson and Jean-Michel Leon and Yawei Li and Alexander Lloyd and Vadim Yushprakh},
booktitle = {Proc. CIDR'11, Conference on Innovative Data System Research},
year  = {2011},
pages = {223--234}
URL = {http://www.cidrdb.org/cidr2011/Papers/CIDR11_Paper32.pdf},
}
```

```latex bib
Google的Spanner

@inproceedings{Corbett:2012,
author = {Corbett, James C. and Dean, Jeffrey and Epstein, Michael and Fikes, Andrew and Frost, Christopher and Furman, J. J. and Ghemawat, Sanjay and Gubarev, Andrey and Heiser, Christopher and Hochschild, Peter and Hsieh, Wilson and Kanthak, Sebastian and Kogan, Eugene and Li, Hongyi and Lloyd, Alexander and Melnik, Sergey and Mwaura, David and Nagle, David and Quinlan, Sean and Rao, Rajesh and Rolig, Lindsay and Saito, Yasushi and Szymaniak, Michal and Taylor, Christopher and Wang, Ruth and Woodford, Dale},
title = {Spanner: {Google's} globally-distributed database},
booktitle = {Proc. OSDI'12, USENIX Symposium on Operating Systems Design and Implementation},
year = {2012},
pages = {251--264},
url = {http://dl.acm.org/citation.cfm?id=2387880.2387905},
publisher = {USENIX},
} 
```

```latex b
Amazon的Dynamo

@inproceedings{DeCandia07,
author = {DeCandia, Giuseppe and Hastorun, Deniz and Jampani, Madan and Kakulapati, Gunavardhan and Lakshman, 
   Avinash and Pilchin, Alex and Sivasubramanian, Swaminathan and Vosshall, Peter and Vogels, Werner},
title = {Dynamo: Amazon's Highly Available Key-value Store},
booktitle = {Proceedings of Twenty-first ACM SIGOPS Symposium on Operating Systems Principles},
series = {SOSP '07},
year = {2007},
pages = {205--220},
url = {http://doi.acm.org/10.1145/1294261.1294281},
doi = {10.1145/1294261.1294281},
publisher = {ACM},
} 
```



```latex 
Facebook's Cassandra (Open source counterpart of Amazon's Dynamo)

@article{Lakshman10,
author = {Lakshman, Avinash and Malik, Prashant},
title = {Cassandra: A Decentralized Structured Storage System},
journal = {SIGOPS Oper. Syst. Rev.},
issue_date = {April 2010},
volume = {44},
number = {2},
month = apr,
year = {2010},
pages = {35--40},
url = {http://doi.acm.org/10.1145/1773912.1773922},
doi = {10.1145/1773912.1773922},
publisher = {ACM},
} 
```



```
Facebook's Tao for social graph

@inproceedings {Bronson13,
author = {Nathan Bronson and Zach Amsden and George Cabrera and Prasad Chakka and Peter Dimov and Hui Ding 
   and Jack Ferris and Anthony Giardullo and Sachin Kulkarni and Harry Li and Mark Marchukov and Dmitri Petrov 
   and Lovro Puzar and Yee Jiun Song and Venkat Venkataramani},
title = {TAO: Facebook{\textquoteright}s Distributed Data Store for the Social Graph},
booktitle = {Presented as part of the 2013 USENIX Annual Technical Conference (USENIX ATC 13)},
year = {2013},
pages = {49--60},
url = {https://www.usenix.org/conference/atc13/technical-sessions/presentation/bronson},
publisher = {USENIX},
}
```

```latex 
Yahoo's PNUTS

@article{Cooper08,
author = {Cooper, Brian F. and Ramakrishnan, Raghu and Srivastava, Utkarsh and Silberstein, Adam and Bohannon, 
   Philip and Jacobsen, Hans-Arno and Puz, Nick and Weaver, Daniel and Yerneni, Ramana},
title = {PNUTS: Yahoo!'s Hosted Data Serving Platform},
journal = {Proc. VLDB Endow.},
issue_date = {August 2008},
volume = {1},
number = {2},
month = aug,
year = {2008},
pages = {1277--1288},
url = {http://dx.doi.org/10.14778/1454159.1454167},
doi = {10.14778/1454159.1454167},
publisher = {VLDB Endowment},
}
```



### 分布式协同服务

```latex bi
Yahoo的Zookeeper

@inproceedings{Hunt10,
author = {Hunt, Patrick and Konar, Mahadev and Junqueira, Flavio P. and Reed, Benjamin},
title = {{ZooKeeper}: wait-free coordination for Internet-scale systems},
booktitle = {Proc. ATC'10, USENIX Annual Technical Conference},
year = {2010},
location = {Boston, MA},
pages = {145--158},
url = {http://portal.acm.org/citation.cfm?id=1855840.1855851},
publisher = {USENIX},
}
```

```latex bib
Zab protocol in Zookeeper: adapted from Paxos

@inproceedings{Junqueira11,
author = {Junqueira, Flavio P. and Reed, Benjamin C. and Serafini, Marco},
title = {Zab: high-performance broadcast for primary-backup systems},
booktitle = {Proc. DSN'11, IEEE/IFIP Conference on Dependable Systems and Networks},
year = {2011},
pages = {245--256},
url = {http://dx.doi.org/10.1109/DSN.2011.5958223},
publisher = {IEEE},
}
```

```latex bib
Google's Chubby, the lock service

@inproceedings{Burrows:2006,
author = {Burrows, Mike},
title = {The {Chubby} lock service for loosely-coupled distributed systems},
booktitle = {Proc. OSDI'06, USENIX Symposium on Operating Systems Design and Implementation},
year = {2006},
pages = {335--350},
url = {http://dl.acm.org/citation.cfm?id=1298455.1298487},
publisher = {USENIX},
}
```

```latex b
基于tupple space的协同

@article{Gelernter85,
author = {Gelernter, David},
title = {Generative Communication in Linda},
journal = {ACM Trans. Program. Lang. Syst.},
issue_date = {Jan. 1985},
volume = {7},
number = {1},
month = jan,
year = {1985},
issn = {0164-0925},
pages = {80--112},
numpages = {33},
url = {http://doi.acm.org/10.1145/2363.2433},
doi = {10.1145/2363.2433},
acmid = {2433},
publisher = {ACM},
address = {New York, NY, USA},
}
```
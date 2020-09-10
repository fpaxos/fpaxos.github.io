Flexible Paxos is the simple observation that it is not necessary to require all quorums in Paxos to intersect. It is sufficient to require that the quorum used by the leader election phase (phase-1) will overlap with the quorums used by previous replication phases (phase-2). Majority quourms are one such way to meet this requirement, but many more exist. Thus, Paxos is just a single point on a broad spectrum of possibilities for safely reaching distributed consensus.
To learn more about Flexible Paxos and how it is used to build more resilient distributed systems, take a look at the lists of articles, papers, talks, and open source projects below.

#### Papers

* [Flexible Paxos: Quorum intersection revisited](https://arxiv.org/pdf/1608.06696v1.pdf) - The original paper describing Flexible Paxos
* [Fast Flexible Paxos: Relaxing Quorum Intersection for Fast Paxos](https://arxiv.org/abs/2008.02671) - extending Flexible Paxos to Fast Paxos
* [Paxos Made EPR: Decidable Reasoning about Distributed Protocols](https://dl.acm.org/doi/abs/10.1145/3140568)
* [DPaxos: Managing Data Closer to Users for Low-Latency and Mobile Applications](https://dl.acm.org/doi/abs/10.1145/3183713.3196928)
* [Multileader WAN Paxos: Ruling the Archipelago with Fast Consensus](https://cse.buffalo.edu/tech-reports/2017-01.pdf)
* [A Generalised Solution to Distributed Consensus](https://arxiv.org/abs/1902.06776)
* [Dissecting the Performance of Strongly-Consistent Replication Protocols](https://dl.acm.org/doi/abs/10.1145/3299869.3319893)
* [Near-Optimal Latency Versus Cost Tradeoffs in Geo-Distributed Storage](https://www.usenix.org/conference/nsdi20/presentation/uluyol)
* [On the Parallels between Paxos and Raft, and how to Port Optimizations](https://dl.acm.org/doi/abs/10.1145/3293611.3331595)
* [WPaxos: Wide Area Network Flexible Consensus](https://ieeexplore.ieee.org/abstract/document/8765834)
* [Bipartisan Paxos: A Modular State Machine Replication Protocol](https://arxiv.org/abs/2003.00331)
* [Flexible Paxos: An Industry Perspective](https://www.diva-portal.org/smash/record.jsf?pid=diva2%3A1119350&dswid=7912)
* [Unifying Consensus and Atomic Commitment for Effective Cloud Data Management](https://dl.acm.org/doi/abs/10.14778/3303753.3303765)
* [Linearizable Quorum Reads in Paxos](https://www.usenix.org/conference/hotstorage19/presentation/charapko)
* [Matchmaker Paxos: A Reconfigurable Consensus Protocol](https://arxiv.org/abs/2007.09468)
* [FleetDB: Follow-the-workload Data Migration for Globe-Spanning Databases](https://cse.buffalo.edu/tech-reports/2018-02.pdf)
* [On the Significance of Consecutive Ballots in Paxos](https://arxiv.org/abs/2006.01885)
* [Low-Latency Geo-Replicated State Machines with Guaranteed Writes](https://dl.acm.org/doi/pdf/10.1145/3380787.3393686)
* [State-Machine Replication for Planet-Scale Systems](https://dl.acm.org/doi/abs/10.1145/3342195.3387543)
* [Unbounded Pipelining in Dynamically Reconfigurable Paxos Clusters](http://tessanddave.com/paxos-reconf-latest.pdf)
* [Revisiting the Paxos Foundations: A Look at Summer Internship Work at VMware Research](https://dl.acm.org/doi/pdf/10.1145/3139645.3139656)

#### Articles & Blog Posts

* [A More Flexible Paxos](http://ssougou.blogspot.com/2016/08/a-more-flexible-paxos.html) - A brief introduction to Flexible Paxos for the systems community, posted on [Tech musings](http://ssougou.blogspot.com) by [Sugu Sougoumarane](https://twitter.com/ssougou)
* [Majority agreement is not necessary for consensus](http://hh360.user.srcf.net/blog/2016/08/majority-agreement-is-not-necessary) - A summary of the key results of the Flexible Paxos paper, posted on [Read, Write and Execute](http://hh360.user.srcf.net/blog/) by [Heidi Howard](https://twitter.com/heidiann360)
* [Flexible Paxos: A new breed of scalable, resilient and performant consensus algorithms is made possible](https://dahliamalkhi.wordpress.com/2016/08/26/flexible-paxos-a-new-breed-of-scalable-resilient-and-performant-consensus-algorithms-is-made-possible/) - [Dahlia Malkhi](https://dahliamalkhi.wordpress.com) describes the story of the Flexible Paxos at [VMware Research](https://research.vmware.com)
* [Distributed Durability in MySQL](http://ssougou.blogspot.com/2016/09/distributed-durability-in-mysql.html) - A proposal to modify the MySQL semi-sync replication process in order to improve the overall consistency, posted on [Tech musings](http://ssougou.blogspot.com) by [Sugu Sougoumarane](https://twitter.com/ssougou)
* [Flexible Paxos: Quorum intersection revisited](https://blog.acolyer.org/2016/09/27/flexible-paxos-quorum-intersection-revisited/) - The popular research blog, the morning paper, covers the Flexible Paxos preprint, posted on [the morning paper](https://blog.acolyer.org) by [Adrian Colyer](https://twitter.com/adriancolyer)
* [The load, capacity, and availability of quorum systems](https://blog.acolyer.org/2016/10/03/the-load-capacity-and-availability-of-quorum-systems/) - Following up from the citation in Flexible Paxos, the morning paper covers Naor & Wool, posted on [the morning paper](https://blog.acolyer.org) by [Adrian Colyer](https://twitter.com/adriancolyer)
* [Modeling Paxos and Flexible Paxos in Pluscal and TLA+](http://muratbuffalo.blogspot.co.uk/2016/11/modeling-paxos-and-flexible-paxos-in.html) - [Murat Demirbas](http://www.cse.buffalo.edu/~demirbas/) details how he model checked Paxos and then Flexible Paxos using Pluscal, posted on [Metadata](http://muratbuffalo.blogspot.co.uk/)
* [Summary of Flexible Paxos: Relaxing the quorum constraint](https://medium.com/designing-distributed-systems/flexible-paxos-relaxing-the-quorum-constraint-89caec294083)
* [Paul Cavallaro on Flexible Paxos](https://paulcavallaro.com/blog/flexible-paxos/#fnref:1)
* [UPaxos and primary-backup replication](https://davecturner.github.io/2017/09/18/upaxos-primary-backup.html)
* [Improved Majority Quorums for Raft](https://basri.dev/posts/2020-07-27-improved-majority-quorums-for-raft/)
* [Paxosmon: Gotta Consensus Them All](https://vadosware.io/post/paxosmon-gotta-concensus-them-all/#honorable-mentions) - Nice summary of the various Paxos variants

#### Talks
* [Distributed consensus: Making impossible possible](http://conferences.oreilly.com/oscon/open-source-eu/public/schedule/detail/54472) - An overview of the key results in the field of distributed consensus. Talk by Heidi Howard at [OSCON London](http://conferences.oreilly.com/oscon/open-source-eu) in 2016. [[Slides]](http://hh360.user.srcf.net/slides/impossible_consensus.pdf)
* [Flexible Paxos: Revisiting quorum intersection using TLA+](https://www.youtube.com/watch?v=LX-WK8EmoFE) - Part of the Dr TLA+ series by Microsoft Research
* [Constructing Scalable, Resilient and Consistent Systems with Flexible Paxos](https://www.youtube.com/watch?v=r6NG_1HM0lA&feature=emb_logo) - Talk by Heidi Howard at Dockercon 2017


#### Code
* [LibFPaxos](https://github.com/fpaxos/fpaxos-lib) - A patch to [LibPaxos3](https://bitbucket.org/sciascid/libpaxos) which exposes quorum size as a configuration parameter.  Licensed under 3-clause BSD.
* [LibFPaxos Benchmarks](https://github.com/fpaxos/fpaxos-test)- Scripts for reproducing the LibFPaxos experiments from the Flexible Paxos paper using [Mininet](http://mininet.org). Licensed under MIT.
* [Flexible Paxos TLA+](https://github.com/fpaxos/fpaxos-tlaplus) - TLA+ specification of single-valued Flexible Paxos. Licensed under MIT.
* [Flexible Raft TLA+](https://github.com/fpaxos/raft.tla) - TLA+ specification of Raft, modified for flexible quorums. Licensed under MIT.
* [LogDevice](https://github.com/facebookincubator/LogDevice) - A distributed log storage systems from Facebook
* [Paxi](https://github.com/ailidani/paxi) - Simulation framework for distributed consensus algorithms which includes prototypes of various algorithms including Flexible Paxos and Fast Flexible Paxos
* [FrankenPaxos](https://github.com/mwhittaker/frankenpaxos) - Another distributed consensus simulator which includes prototypes of various consensus algorithm including Flexible Paxos
* [FlexibleZoo](https://github.com/Max-Meldrum/zookeeper-fpaxos-benchmarks) - Zookeeper fork by [Max Meldrum](https://github.com/Max-Meldrum)
* [FPaxosPython](https://github.com/estensen/fpaxos) - A (naive) implementation of Flexible Paxos

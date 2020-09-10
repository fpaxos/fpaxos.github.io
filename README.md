# Flexible Paxos

Flexible Paxos is the simple observation that it is not necessary to require all quorums in Paxos to intersect. It is sufficient to require that the quorum used by the leader election phase (phase-1) will overlap with the quorums used by previous replication phases (phase-2). Majority quourms are one such way to meet this requirement, but many more exist. Thus, Paxos is just a single point on a broad spectrum of possibilities for safely reaching distributed consensus.

#### Papers

Heidi Howard, Dahlia Malkhi, Alexander Spiegelman
[Flexible Paxos: Quorum intersection revisited](https://arxiv.org/pdf/1608.06696v1.pdf)
20th International Conference on Principles of Distributed Systems (OPODIS 2016)
preprint arXiv:1608.06696 [cs.DC]

#### Blog posts

* [A More Flexible Paxos](http://ssougou.blogspot.com/2016/08/a-more-flexible-paxos.html) - A brief introduction to Flexible Paxos for the systems community, posted on [Tech musings](http://ssougou.blogspot.com) by [Sugu Sougoumarane](https://twitter.com/ssougou) [11/8/2016]
* [Majority agreement is not necessary for consensus](http://hh360.user.srcf.net/blog/2016/08/majority-agreement-is-not-necessary) - A summary of the key results of the Flexible Paxos paper, posted on [Read, Write and Execute](http://hh360.user.srcf.net/blog/) by [Heidi Howard](https://twitter.com/heidiann360) [26/8/2016]
* [Flexible Paxos: A new breed of scalable, resilient and performant consensus algorithms is made possible](https://dahliamalkhi.wordpress.com/2016/08/26/flexible-paxos-a-new-breed-of-scalable-resilient-and-performant-consensus-algorithms-is-made-possible/) - Dalhia Malkhi describes the story of the Flexible Paxos at [VMware Research](https://research.vmware.com), posted by [Dahlia Malkhi](https://dahliamalkhi.wordpress.com) [26/8/2016]
* [Distributed Durability in MySQL](http://ssougou.blogspot.com/2016/09/distributed-durability-in-mysql.html) - A proposal to modify the MySQL semi-sync replication process in order to improve the overall consistency, posted on [Tech musings](http://ssougou.blogspot.com) by [Sugu Sougoumarane](https://twitter.com/ssougou) [6/9/2016]
* [Flexible Paxos: Quorum intersection revisited](https://blog.acolyer.org/2016/09/27/flexible-paxos-quorum-intersection-revisited/) - The popular research blog, the morning paper, covers the Flexible Paxos preprint, posted on [the morning paper](https://blog.acolyer.org) by [Adrian Colyer](https://twitter.com/adriancolyer) [27/9/2016]
* [The load, capacity, and availability of quorum systems](https://blog.acolyer.org/2016/10/03/the-load-capacity-and-availability-of-quorum-systems/) - Following up from the citation in Flexible Paxos, the morning paper covers Naor & Wool, posted on [the morning paper](https://blog.acolyer.org) by [Adrian Colyer](https://twitter.com/adriancolyer) [3/10/2016]
* [Modeling Paxos and Flexible Paxos in Pluscal and TLA+](http://muratbuffalo.blogspot.co.uk/2016/11/modeling-paxos-and-flexible-paxos-in.html) - In this post, Murat details how he model checked Paxos and then Flexible Paxos using Pluscal, posted on [Metadata](http://muratbuffalo.blogspot.co.uk/) by [Murat Demirbas](http://www.cse.buffalo.edu/~demirbas/) [3/10/2016]

#### Talks
* [Distributed consensus: Making impossible possible](http://conferences.oreilly.com/oscon/open-source-eu/public/schedule/detail/54472) - An overview of the key results in the field of distributed consensus. Talk by Heidi Howard at [OSCON London](http://conferences.oreilly.com/oscon/open-source-eu) in 2016. [[Slides]](http://hh360.user.srcf.net/slides/impossible_consensus.pdf)


#### Code
* [LibFPaxos](https://github.com/fpaxos/fpaxos-lib) - A patch to [LibPaxos3](https://bitbucket.org/sciascid/libpaxos) which exposes quorum size as a configuration parameter.  Licensed under 3-clause BSD.
* [LibFPaxos Benchmarks](https://github.com/fpaxos/fpaxos-test)- Scripts for reproducing the LibFPaxos experiments from the Flexible Paxos paper using [Mininet](http://mininet.org). Licensed under MIT.
* [Flexible Paxos TLA+](https://github.com/fpaxos/fpaxos-tlaplus) - TLA+ specification of single-valued Flexible Paxos. Licensed under MIT.
* [Flexible Raft TLA+](https://github.com/fpaxos/raft.tla) - TLA+ specification of Raft, modified for flexible quorums. Licensed under MIT.

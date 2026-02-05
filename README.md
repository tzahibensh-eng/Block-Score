**Introduction**

This repository presents a methodology for estimating the impact of blocking rules between demand (advertisers) and supply (publishers) in a large-scale content distribution or advertising system. In such systems, advertisers may block specific publishers, sections, or placements (and vice versa), at different scopes and levels of granularity. 

These decisions reduce the set of possible supply–demand matches and can have a measurable impact on monetization, delivery efficiency, and marketplace liquidity. However, quantifying that impact is non-trivial, especially when blocking occurs at multiple hierarchical levels and when traffic is highly fragmented.

The metric implemented here aims to address this problem by translating blocking configurations into a continuous impact score. Rather than counting blocks naively, it weights each block by the relative “size” of the affected demand and supply entities, using observed revenue shares as a proxy for scale.

______

**The SQL in this repository is adapted from a production implementation, but table names, column names, and certain details were modified to avoid exposing confidential or proprietary information, while preserving the core logic and methodology.**

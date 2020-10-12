## Abstract

In this thesis, we present an approach for processing event streams online, where events can
carry data values. Events may also appear out of order, that is, the order in which events are
received can be different from the order in which they are generated. Our approach aims at
verifying events streams describing system behavior in real-time against specifications that are
given as formulas in a temporal logic. The novelty of our approach is that we utilize multiple
CPU cores to carry out the monitoring task concurrently and in parallel. To this end, we first
present an architecture that is well suited for online processing event streams in parallel. In a
nutshell, received events are assigned to substreams that are processed separately. Afterwards,
we propose an algorithm based on stateful workers that efficiently aggregate these substreams.
Finally, we report on the outcome of an experimental evaluation of a prototype implementation.
Our evaluation shows that our prototype scales well with respect to the number of CPU cores.
The evaluation also shows that our approach can be more efficient than prior approaches that
process an event stream monolithically.
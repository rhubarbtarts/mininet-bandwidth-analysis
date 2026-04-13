# Bandwidth Measurement using Mininet

## Aim
To measure and compare bandwidth using iperf in different Mininet topologies.

## Tools Used
- Mininet
- iperf
- Ubuntu (WSL2)

## Procedure
1. Start Mininet:
   sudo mn

2. Test connectivity:
   pingall

3. Measure bandwidth:
   h1 iperf -s &
   h2 iperf -c h1

4. Run different topology:
   sudo mn --topo single,3

5. Measure again:
   h1 iperf -s &
   h3 iperf -c h1

## Results
- 2 hosts: 23.7 Gbits/sec
- 3 hosts: 22.5 Gbits/sec

## Conclusion
Bandwidth remains high but varies slightly with topology.

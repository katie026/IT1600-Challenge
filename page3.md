| [Home](README.md) | [Bits & Bytes](page1.md) | [Prefixes](page2.md) | [**Efficiency**](page3.md) | [Compression](page4.md) |

# Efficiency
**Efficiency:** measure of how efficiently a network exchanges information

Information that is to be transferred is placed in packets
- add overhead & reduce efficiency: error detection & correction, requests to resend data that arrived damaged/incomplete, acknowledgements data has been received 

A network that has a bandwidth of 100 Mbps (lets say M = million) can not actually transfer a 100 million bit file in 1 second
- **Throughput:** actual rate that information is transferred; the available bandwidth to transfer information

![badnwidth vs. throughput][image1]
<br></br>

[Bandwidth, Packets Per Second, and Other Network Performance Metrics](https://www.cisco.com/c/en/us/about/security-center/network-performance-metrics.html)

- Other metrics: packets per second (p/s), connections per second (c/s), transactions per second (t/s), and maximum concurrent connections (mcc)
- Connections Per Second (c/s): rate at which a device can establish state parameters for new connections
    - A stateful device must create and manage connection information on all unique IP streams that transit the device
    - device must handle the first packet of a new connection differently than all subsequent packets so that the device can establish the state parameters for the new connection
    - related to factors such as processor (CPU) speed, memory speed, architecture, TCP/IP stack efficiency, etc
    - For packet handling performance: rate at which a device can handle packets when establishing state parameters is usually a small percentage of the rate at which the same device can forward packets in hardware once the state parameters are established
- Maximum Concurrent Connections (mcc): total number of sessions (connections) about which a device can maintain state simultaneously.
    - mainly related to the amount of memory that is dedicated to this task 
        - memory is inexpensive BUT adding memory to support more concurrent connections makes little sense when the c/s rate is low
        - Ex. if enough memory to handle one million concurrent connections but the device had a maximum connection setup rate of 10 c/s, it would take more than 100,000 seconds (or 28 hours) to fully utilize all of this state
- Transactions Per Second (t/s): number of complete actions of a particular type that can be performed per second
    - refers to more than just the processing of a single packet or even the setup of a new connection
    - refers to the completion of a full cycle of a specific action


[image1]: https://cdn.ttgtmedia.com/rms/onlineimages/network_bandwidth_vs_throughput-f_mobile.png
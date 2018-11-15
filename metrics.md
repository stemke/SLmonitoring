---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Metrics collected (Beta)
This topic covers the metrics collected for this beta monitoring application on virtual and bare metal servers.
{:shortdesc}

This topic covers all metrics available through Grafana queries. For more information, see [Creating an advanced monitoring query (Beta)](advanced_query.html). Graphs are available in the user interface for the following metrics only:
* CPU utilization
* Memory Usage
* Disk Read and Write (bytes/seconds and IO per second)
* Disk Read and Write latency
* Public network throughput (in/out)
* Private network throughput (in/out)
* Public network packets (in/out) (Bare metal only)
* Private network packets(in/out) (Bare metal only)
* Public network errors(in/out) (Bare metal only)
* Private network errors (in/out) (Bare metal only)
* Temperature (Bare metal only)


## CPU metrics
  The CPU metrics measure the average percentage of time that a CPU is running instructions during a given time period. The average idle percentage is idle over the addition of user, nice, system, IO Wait, hardware interrupts, and software interrupts.

## Memory metrics
* Bytes used/Average used: The amount of memory being used at a given time, available in both bytes and percentage of the total.
* Swap Bytes used/Average used: The percentage of swap memory being used during a given period. This metric is an indication of how often you have to retrieve data that is not in memory. This metric is available only on bare metal devices.

## Disk metrics

* Disk Total: The total number of bytes available to the disk. This metric should be constant.
* Disk Used (Bytes): The number of bytes being used by the disk at the given time.
* Disk Used (Percentage): The percentage of the total number of bytes being used over the total number of bytes available to the disk.
* Disk Read/Write (bytes per sec): The average amount of data being read/written from/to disk in bytes over a given time period.
* Disk Read/Write (operations per sec): Read/write operations per second
* Disk Read/Write (latency in ms per operation): Latency in ms per read/write

## Network metrics

 * Network Public/Private In: Number of bytes sent by the Public/Private network
* Network Public/Private Out: Number of bytes received by the Public/Private network
* Network Public/Private Packets In: Number of packets received by the network interface on the Public/Private network. This metric is available only on bare metal devices.
* Network Public/Private Packets Out: Number of packets sent by the network interface on the Public/Private network. This metric is available only on bare metal devices.

## Temperature metrics
* Average temperature of the system measured in degrees Celsius. This metric is available only on select bare metal devices.

# Subnetting BEST Method Example 4

## 192.168.1.0/24

### Requirement = 60 Hosts/Subnet

* Hosts / Subnet = 2^X = 2^6\(host bits\) = 64 
* Usable Hosts = 2^n-2 = 2^6-2 = 64-2 = 62
* New Mask = /32 - /6 = /26
* New IP = 192.168.1.0/26

| Subnet 1 | Subnet 2 | Subnet 3 |
| :--- | :--- | :--- |
| 192.168.1.0 \(NID\) | 192.168.1.64 \(NID\) | 192.168.1.128 \(NID\) |
| 192.168.1.1 \(First IP\) | 192.168.1.65 \(First IP\) | 192.168.1.129 \(First IP\) |
| 192.168.1.62 \(Last IP\) | 192.168.1.126 \(Last IP\) | 192.168.1.190 \(Last IP\) |
| 192.168.1.63 \(BID\) | 192.168.1.6127 \(BID\) | 192.168.1.191 \(BID\) |

## Reference:

* [Cisco CCNA 200-301 Exam: Complete Course with practical labs \| Udemy](https://www.udemy.com/course/cisco-ccent-icnd1-100-105-complete-course-sims-and-gns3/learn/lecture/7402450#overview)


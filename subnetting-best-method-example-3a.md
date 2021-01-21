# Subnetting BEST Method Example 3a

## 192.168.1.0/24

### Requirement : 4 Subnets

2^n = 2^2 \(network bits\) = 4 Subnets New Mask = /24+/2 = /26 New IP: 192.168.1.0/26 Hosts bits = /32-/26 = /6 = 64 Hosts/Subnet Usable Hosts/Subnet = 2^n-2 = 2^6 = 64

### 192.168.1.0/26 \(NID\)

#### 192.168.1.1/26 \(First Host IP\)

192.168.1.64/26 \(NID\) 192.168.1.128/26 \(NID\) 192.168.1.192/26 \(NID\)

#### 192.168.1.254 \(Last Host IP\)

#### 192.168.1.255 \(Last BID\)

## Reference:

[Cisco CCNA 200-301 Exam: Complete Course with practical labs \| Udemy](https://www.udemy.com/course/cisco-ccent-icnd1-100-105-complete-course-sims-and-gns3/learn/lecture/18258608#overview)


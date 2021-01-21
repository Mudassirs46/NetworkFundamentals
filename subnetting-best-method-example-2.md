# Subnetting BEST Method Example 2

## 10.128.192.0/18

## Requirement = 30 Subnets \(Max Hosts\)

### Total Number of Subnets = 2^n \(network bits\) \(count bits from Left to Right\)

#### = 2^5

#### = 32 Total Subnets

### New Mask = /18+/5 = /23

### New IP Address = 10.128.192.0/23

### Host bits

/32 - /23 = 9 Hosts bits

### How many Hosts/Subnet = 2^n -2 \(host bits\) \(count bits from Right to Left\)

#### = 2^9 - 2

= 512-2

#### = 510 Hosts/Subnet

### 10.128.192.0/23 \(First NID\)

10.128.192.255/23 \(255 Hosts\) + 10.128.193.255/23 \(255 Hosts\)

### 10.128.194.0/23 \(Second NID\)

#### 10.128.196.0/23 \(Third NID\)

#### 10.128.196.0/23 \(Fourth NID\)

. .

### 10.128.254.0 \(Last NID\)

### 10.128.254.255 \(Last BID\)

10.128.255.255

## Reference:

[Cisco CCNA 200-301 Exam: Complete Course with practical labs \| Udemy](https://www.udemy.com/course/cisco-ccent-icnd1-100-105-complete-course-sims-and-gns3/learn/lecture/6087502#overview)


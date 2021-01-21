# Subnetting BEST Method Example 1

## 10.1.1.0/24

## Requirement = 14 Machines \(14 Hosts\)

### How many Hosts/Subnet = 2^n -2 \(count bits from Right to Left\)

#### = 2^4 - 2

= 16-2

#### = 14 Hosts/Subnet

### Total Number of Subnets = 2^n \(count bits from Left to Right\)

#### = 2^4

#### = 16 Total Subnets

### Masks = 32-4 = /28

## 10.1.1.0/28

10.1.1.240

#### 10.1.1.0/28 \(First NID\)

#### 10.1.1.16/28 \(Second NID\)

#### 10.1.1.32/28 \(Third NID\)

#### 10.1.1.48/28 \(Fourth NID\)

. .

#### 10.1.1.240/28 \(Last NID\)

## Reference:

[Cisco CCNA 200-301 Exam: Complete Course with practical labs \| Udemy](https://www.udemy.com/course/cisco-ccent-icnd1-100-105-complete-course-sims-and-gns3/learn/lecture/6087502#overview)


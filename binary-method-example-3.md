# Binary Method Example 3

### 172.16.129.1/17

## FIRST CONVERT THE CONCERN & THE REMANING OCTET INTO BINARY

172.16.1**0000001.00000001**

#### 1. Network/Subnet Address \(Host portion = 0\)

* 172.16.10000000.00000000
* Network Address = 172.16.128.0

  **2. First Host Address in a Subnet \(Host portion = 0 except the last bit as 1\)**

* 172.16.10000000.00000001
* First Host Address = 172.16.128.1

  **3. Last Host Address in a Subnet \(Host portion = 1 except the last bit as 0\)**

* 172.16.11111111.11111110
* Last Host Address = 172.16.255.254

  **3. Broadcast Address \(Host portion = 1\)**

* 172.16.11111111.11111111
* Broadcast Address = 172.16.255.255

## Reference:

[Cisco CCNA 200-301 Exam: Complete Course with practical labs \| Udemy](https://www.udemy.com/course/cisco-ccent-icnd1-100-105-complete-course-sims-and-gns3/learn/lecture/6087498#overview)


# Binary Method Example 2

### 172.16.35.123/20

## FIRST CONVERT THE CONCERN & THE REMANING OCTET INTO BINARY

172.16.0010**0011.01111011**

#### 1. To workout the Network/Subnet Address

* **Fill the host portion of Address with Binary 0's \(then convert it to Decimal\)**
* 172.16.35.123 - 172.16.0010**0000.00000000**.0

    \(convert Binary into Decimal we get...\)

* **Network Address = 172.16.32.0**

  **2. To workout the First Host Address in a Subnet**

* **Fill the host portion of the Address with Binary 0's except for the last bit which is set to Binary 1 \(then convert it to Decimal\)**
* 172.16.35.123 - 0001**0000.00000001**.0

  \(convert Binary into Decimal we get...\)

* **First Host Address = 172.16.32.1**

  **3. To workout the Last Host Address in a Subnet**

* **Fill the host portion of the Address with Binary 1's except for the last bit which is set to Binary 0 \(then convert it to Decimal\)**
* 172.16.35.123 - 172.16.0010**1111.11111110**

  \(convert Binary into Decimal we get...\)

* **Last Host Address = 172.16.47.254**

  **4. To workout the Broadcast Address**

* **Fill the host portion of the Address with Binary 1's \(then convert it to Decimal\)**
* 172.16.35.123 - 172.16.0010**1111.11111111**

  \(convert Binary into Decimal we get...\)

* **Broadcast Address = 172.16.47.255**

## Reference:

* [Cisco CCNA 200-301 Exam: Complete Course with practical labs \| Udemy](https://www.udemy.com/course/cisco-ccent-icnd1-100-105-complete-course-sims-and-gns3/learn/lecture/6087496#overview)


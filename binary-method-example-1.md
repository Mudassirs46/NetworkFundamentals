# Binary Method Example 1

### 192.168.1.18/24

## FIRST CONVERT THE CONCERN & THE REMANING OCTET INTO BINARY

192.168.1.**00010010**

## THEN ADDRESS INTO BINARY

01000000.10101000.00000001.**00010010**

#### 1. To workout the Network/Subnet Address

* **Fill the host portion of Address with Binary 0's \(then convert it to Decimal\)**
* 192.168.1.18 - 192.168.1.**00000000**

    \(convert Binary into Decimal we get...\)

* **Network Address = 192.168.1.0**

  **2. To workout the First Host Address in a Subnet**

* **Fill the host portion of the Address with Binary 0's except for the last bit which is set to Binary 1 \(then convert it to Decimal\)**
* 192.168.1.18 - 192.168.1.**00000001**

    \(convert Binary into Decimal we get...\)

* **First Host Address Address = 192.168.1.1**

  **3. To workout the Last Host Address in a Subnet**

* **Fill the host portion of the Address with Binary 1's except for the last bit which is set to 0. \(then convert it to Decimal\)**
* 192.168.1.18 - 192.168.1.**11111110**

    \(convert Binary into Decimal we get...\)

* **Last Host Address = 192.168.1.254**

  **4. To workout the Broadcast Address**

* **Fill the host portion of the Addresses with Binary 0's except for the last bit which is set to 1.\(then convert it to Decimal\)**
* 192.168.1.18 - 192.168.1.**00000001**

    \(convert Binary into Decimal we get...\)

* **Broadcast Address = 192.168.1.255**

## Reference:

* [Cisco CCNA 200-301 Exam: Complete Course with practical labs \| Udemy](https://www.udemy.com/course/cisco-ccent-icnd1-100-105-complete-course-sims-and-gns3/learn/lecture/6087496#overview)


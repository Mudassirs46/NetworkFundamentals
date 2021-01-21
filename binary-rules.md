# Binary Rules

## FIRST CONVERT ADD INTO BINARY

### 1. To workout the Network/Subnet Address

* **Fill the host portion of Address with Binary 0's \(then convert it to Decimal\)**

  **2. To workout the First Host Address in a Subnet**

* **Fill the host portion of the Address with Binary 0's except for the last bit which is set to Binary 1 \(then convert it to Decimal\)**

  **3. To workout the Last Host Address in a Subnet**

* **Fill the host portion of the Address with Binary 1's except for the last bit which is set to 0. \(then convert it to Decimal\)**

  **4. To workout the Broadcast Address**

* **Fill the host portion of the Addresses with Binary 0's except for the last bit which is set to 1.\(then convert it to Decimal\)**

#### Why only work on the Host Portion?

* Because mask indicates Number of bits on the Network Side \(already reserved\)
* /24 = 255.255.255.0
* Hence we only work on the Host side

Practical Example:

* [Subnetting Binary Method Example 1](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/binary-method-example-1)
* [Subnetting Binary Method Example 2](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/binary-method-example-2)
* [Subnetting Binary Method Example 3](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/binary-method-example-3)

## Reference:

* [https://www.udemy.com/course/cisco-ccent-icnd1-100-105-complete-course-sims-and-gns3/learn/lecture/6087496\#overview](https://www.udemy.com/course/cisco-ccent-icnd1-100-105-complete-course-sims-and-gns3/learn/lecture/6087496#overview)


## **Introduction**
In the Performance testing test project - I have taken 2 APIs - 
- Restful-Booker: A Books API for load testing and Stress testing
- Dmoney A Website Transaction API for API Chainning (JMeter Collection).
Also,  For Transaction APIs -  I have taken CSV data files to run multiple APIs using Three Threads which are - Deposit Money, SendMoney and Payment in Jmeter

## **Test Case Scenario**
### **Test Cases Scenario - Restful-Booker**
- Create a Collectio of APIs (JMeter Collection) of Login API, Create Booking API and Search API Http requests.
- Perform Load Test and Stress Test. Find the Bottleneck point and Capacity Point.
- Website for APIs - [https://restful-booker.herokuapp.com]
  
### **Test Cases Scenario - DMoney Transaction APIs**
- 5 agents perform deposits for 10 customers.
- 5 customers send money to another 10 customers.
- 5 customers make payments to 2 merchants.
- Withdraw Money applying Boundary Value Analysis (BVA) for the withdrawal amount.
- Set the ramp-up time to 120 seconds in all the above thread configuration.
- Website for APIs - [http://dmoney.roadtocareer.net]

## **How to run?**
## Execute the following steps using JMeter:
- git clone <repo_url>
- Open ApacheJMeter
- From ApacheJMeter open the JMX File
- Finally Run
## Execute the following steps using CLI:
- git clone <repo_url>
- **For Booking APIs JMeter Collection:**
  ```console
    jmeter -n -t .\booking.jmx -l .\booking.jtl -e -o Reports
  ```
- **For DMoney Trabsaction APIs JMeter Collection**:
  ```console
    jmeter -n -t .\dmoney.jmx -l .\dmoney.jtl -e -o Reports
  ```

## **Load and Stress Test Excel Report**

  
## **HTML Report Generate**
### Generated HTML report for Load Test
![image](https://github.com/user-attachments/assets/8db6b91d-0efa-4b0e-9cdb-512168f25d84)


### Generated HTML report for Stree Test
![image](https://github.com/user-attachments/assets/1042fb02-db9c-49e8-ac87-330b4baf41ab)


### Generated HTML report for DMoney Jmeter Collection Test
![image](https://github.com/user-attachments/assets/f881f32e-8ae9-4bcc-9ff9-cc573237bcb5)


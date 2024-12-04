# Project Overview
This repository contains JMeter collections and reports for performance and functional testing of two APIs: **Booking API** and **Dmoney API**. The **Booking API** tests evaluate the system's ability to handle high loads and stress during login, booking creation, and booking search scenarios for up to 120,000 users over 12 hours. The **Dmoney API** tests validate transactions like deposits, money transfers, and payments among agents, customers, and merchants using CSV data files.

# Prerequisites
- JMeter: Apache JMeter installed and added to system PATH.
- Java: JDK 11 or 17 installed.
- Git: Installed to clone the repository.

# How to Run
- Open JMeter and load the respective .jmx file (booking.jmx or dmoney.jmx).
- Ensure the necessary CSV files (deposit.csv, sendMoney.csv, payment.csv) are in the correct path for Dmoney API.
- Configure the thread groups (users, ramp-up, duration) as needed.
- Open the command promt from the folder with the respective .jmx
- Use the following command to run the test in non-GUI mode:
  - jmeter -n -t <path_to_jmx_file> -l <path_to_jtl_file> -e -o <path_to_output_reports_folder>  

# Booking API Test Report
- Load test:
  
![image](https://github.com/user-attachments/assets/57d452d9-0944-4f0b-b2a9-2cd1c415323b)

- Stress test:
  
![image](https://github.com/user-attachments/assets/5619cbb6-5015-44de-85e6-ca0741f1102d)


# Booking API Request Summary and Statistics
- Load test:
  
![image](https://github.com/user-attachments/assets/416aa7af-6847-4610-bd52-9acc842c5fa3)

- Stress test:
  
![image](https://github.com/user-attachments/assets/d6472020-d8e7-4e35-b9aa-0c2b475387c9)

# Dmoney API Request Summary and Statistics

![image](https://github.com/user-attachments/assets/87d5cf6a-1a5b-487c-bd81-8151725654d3)

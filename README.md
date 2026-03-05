# Jmeter-Load-Testing-non-graphical-test-report-demo
Load Testing Sample Project (Non-Graphical Execution)

This repository contains a sample load testing project demonstrating how to perform performance testing using non-graphical (CLI) execution mode for better efficiency and lower resource consumption.

The project simulates concurrent users, executes test scripts through command line, and generates performance test results that can be used to analyze system behavior under load.

The test is designed and executed using Apache JMeter in non-GUI mode, which is recommended for running large-scale performance tests.

**Project Objective:**
Demonstrate basic load testing setup
Execute performance tests using non-graphical mode
Generate test result logs
Analyze system behavior under simulated user load

**Tools Used:**
Apache JMeter
Command Line Interface (CLI)
CSV / JTL result logs

project-root
│
├── plan/
│   └── LoadTest.jmx
│
├── results/
│   └── test_results.jtl
│
├── reports/
│   └── summary_report
│
└── README.md

**How to Run the Test (Non-GUI Mode)**
Install Apache JMeter
Navigate to the project directory.
Run the following command:
\Users\KIBRIA\apache-jmeter-5.6.3\apache-jmeter-5.6.3\bin>jmeter -n -t \Users\KIBRIA\Plan\LoadTest.jmx -l \Users\KIBRIA\Plan\loading.csv

**Where:**
-n → Non-GUI mode
-t → Test plan file
-l → Result log file

**Generate HTML Report:**
Run the following command to generate a performance report:
jmeter -g results/test_results.jtl -o reports/html-report

**Test Result Output**
The test execution generates:
JTL result files
Execution logs
Optional HTML performance reports

These results can be used to analyze:
Response time
Throughput
Error rate
System performance under load


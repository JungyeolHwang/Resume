## 정열 황 (JungYeol Hwang)
Junior Database Engineer 

## 📧 sulum@naver.com | 📍 서울, 대한민국

# 💼 경력

1. 해커스교육그룹 / Database Administrator / 파트장 / 2022.06 ~ 현재
   
   Role : Mysql, MariaDB in OnPremise, AWS Aurora Mysql 백업, 복구, 버전 업그레이드, Query Tunning, Data Modeling 및 검수, 장애 모니터링




2. 카페24 / Backend Developer/ CSD5팀 사원 / 2020.07 ~ 2021.12 (1년 6개월)
   
   Role : LINKED 통합 시스템 개발




3. 시스게이트 / Backend Developer / 대리 / 2019.02 ~ 2020.07 (1년 6개월)
   
   Role : RFID 백업저장매체 관리시스템 리뉴얼, 서버 이전관리시스템 개발




4. 하나금융티아이 / Backend Developer / 은행서비스팀 주임 | 2012.12 ~ 2014.05 (1년 6개월)
   
   Role : 하나캐피탈 차세대 시스템 인사 ERP 개발, 유지보수



# 🏅 자격증

정보처리기사 | 한국산업인력공단 | 2012.08 취득

# 🌐 어학

G-TELP 영어 | 69점 / 2급 / PASS | 2016.03 취득


# 💻 보유 기술

MariaDB, MySQL, Oracle, ElasticSearch, Shell Script, Ansible, Python, JavaScript, Java


**Projects**

**1. Large-Scale MySQL/MariaDB Cloud Migration (2024)**
* Role: Led the migration of over 50 MySQL and MariaDB instances to AWS.
* Skills: MySQL 8.0, MariaDB 10.5, AWS EC2, Xtrabackup
* Description: Implemented real-time data synchronization using Xtrabackup, achieving 99.99% data accuracy. Developed data integrity verification scripts in Python 3.8, validating over 100TB of data with zero data loss.
* Problem Solving: Initially reduced cluster deployment time by 40% using EC2 cold copy method. However, due to binary log replication issues, had to rebuild using Xtrabackup. While this increased migration time per instance from 2 to 3.5 hours, it ensured 100% data consistency.

**2. AI-Based Automated Query Optimization System (2024)**
* Role: Developed a system that automatically optimizes an average of 5,000 slow queries daily.
* Skills: Elasticsearch 7.10, AWS RDS, Aurora MySQL, AWS Lambda, EventBridge, Python 3.9
* Description: Established and automated a systematic query optimization process:
  1. Automated Slow Query Collection
     - Implemented periodic slow query log collection from RDS and Aurora MySQL using AWS EventBridge
     - Developed query normalization and hashing logic using Lambda functions for duplicate query identification
     - Built a pipeline for generating unique hash IDs and loading into Elasticsearch
     - Reduced duplicate query analysis by 90% and optimization target identification time by 75%
  2. Query Structure Optimization
     - Improved student course history query performance by 60% by converting complex correlated subqueries to LATERAL JOINs
     - Reduced course enrollment statistics aggregation time by 45% through subquery-to-JOIN conversion
     - Optimized settlement queries: Added explicit date range comparisons and composite indexes, reducing processing time from 15 to 5 minutes
  3. Index Optimization
     - Eliminated full table scans by designing composite indexes for key search conditions
     - Enhanced join order and table access methods through execution plan analysis
* Problem Solving: 
  1. Query Normalization and Hashing Process
     - Grouped identical query patterns by parameterizing literal values
     - Generated unique IDs for query patterns using hashing algorithms
     - Automated optimization strategy mapping based on normalized query patterns
  2. Optimization Pattern Automation
     - Automated EXPLAIN analysis for generating optimization suggestions
     - Improved index optimization accuracy by incorporating table schema information

**3. Real-Time Database Monitoring System Implementation (2024)**
* Role: Built a real-time monitoring system for over 100 database instances.
* Skills: Grafana 8.3, Prometheus 2.32, PMM 2.25, Slack API, Telegram API
* Description: Implemented a real-time dashboard monitoring eight key performance metrics including CPU, Memory, Disk I/O, and Slow Query Rate. Established threshold settings and alert priority logic for rapid operational response.
* Problem Solving: Reduced daily alert volume by 75% (from 200 to 50) through alert filtering and priority configuration.

**4. Large-Scale Database Backup Automation Project (2024)**
* Role: Implemented automated backup system for 62 database instances (40 MySQL, 22 MariaDB).
* Skills: XtraBackup 8.0, MariaBackup 10.5, Python 3.8
* Description: Rewrote existing shell scripts in Python, implementing code modularization and unit testing. This improved code reusability and reduced maintenance time by 75% (from 20 to 5 hours monthly). Manual operation time decreased by 95% (from 40 to 2 hours weekly).
* Problem Solving: Attempted to reduce processing time by 20% through multi-threading but encountered limitations. Instead, achieved 15% reduction in overall backup time through backup schedule optimization.

**5. Internal Messaging Data Collection and Storage System (2023)**
* Role: Developed an automated system for collecting and storing approximately 5,000 daily internal messages.
* Skills: Python 3.9, AWS Lambda, API Gateway, DynamoDB
* Description: Automated the process of collecting message data using Python scripts, transmitting via API Gateway, and storing in DynamoDB through Lambda functions. Reduced data processing time by 80% compared to the previous system.
* Problem Solving: Implemented batch processing (20 items per batch) to reduce API requests by 90% and increased Lambda function memory from 1024MB to 2048MB, improving processing speed by 50%.

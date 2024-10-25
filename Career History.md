**정열 황 (JungYeol Hwang)**

Junior Database Engineer 📧 [sulum@naver.com](mailto:sulum@naver.com) | 📍 서울, 대한민국

## 대규모 MySQL/MariaDB 클라우드 마이그레이션 (2024)
- Role : 50개 이상의 MySQL 및 MariaDB 인스턴스를 AWS로 마이그레이션하는 작업을 이끌었습니다.
- Skill : MySQL 8.0, MariaDB 10.5, AWS EC2, Xtrabackup, Ansible
- Description: Xtrabackup을 사용해 실시간 데이터 동기화를 구현하여 평균 99.99% 데이터 정확도를 달성했습니다. Python 3.8로 작성한 데이터 무결성 검증 스크립트로 100TB 이상의 데이터를 검증하여 0건의 데이터 손실을 기록했습니다.
- Problem Solving: EC2 콜드 카피 방식으로 클러스터 구축 시간을 기존 대비 40% 단축했으나, 바이너리 로그 복제 문제로 Xtrabackup을 이용해 재구축했습니다. 이 과정에서 마이그레이션 소요 시간이 인스턴스당 평균 2시간에서 3.5시간으로 증가했지만, 데이터 정합성을 100% 보장할 수 있었습니다.

 
 ## AI 기반 자동 쿼리 최적화 시스템 개발 (2024)
- Role: 일일 평균 5000건의 슬로우 쿼리를 자동으로 최적화하는 AI 시스템을 개발했습니다.
- Skill: Elasticsearch 7.10, Filebeat 7.10, Python 3.9
- Description: Filebeat로 수집한 슬로우 로그를 Elasticsearch에 적재하고, Claud AI 모델이 쿼리를 분석하여 최적화 제안을 생성했습니다. 이를 통해 쿼리 실행 시간을 평균 65% 단축했습니다.
Problem Solving: mysqldumpslow를 사용해 로그 중복을 92% 감소시켰고, Python 스크립트로 DDL 정보를 추출하여 AI 모델의 정확도를 기존 대비 25% 향상시켰습니다.

 
 ## 실시간 데이터베이스 통합 모니터링 시스템 구축 (2024)
- Role: 100개 이상의 데이터베이스 인스턴스를 실시간으로 모니터링하는 시스템을 구축했습니다.
- Skill: Grafana 8.3, Prometheus 2.32, PMM 2.25, Slack API, Telegram API
- Description: 약 8개의 핵심 성능 지표를 실시간으로 모니터링하는 대시보드를 구현하고, 중요도에 따라 Slack과 Telegram으로 이중화 알림을 전송하는 시스템을 구축했습니다.
- Problem Solving: 알림 필터링 및 우선순위 설정으로 일일 알림 횟수를 200회에서 50회로 75% 감소시켰습니다.

 
 ## 대규모 데이터베이스 백업 자동화 프로젝트 (2023)
- Role: 총 62개의 데이터베이스 인스턴스(MySQL 40개, MariaDB 22개)에 대한 자동 백업 시스템을 구축했습니다.
- Skill: XtraBackup 8.0, MariaBackup 10.5, Python 3.8
- Description: Python 스크립트로 백업 자동화를 구현하여 수동 작업 시간을 주당 40시간에서 2시간으로 95% 감소시켰습니다. 백업 파일 압축으로 스토리지 사용량을 30% 절감했습니다.
- Problem Solving: 단일 스레드 방식 대비 멀티스레드 구현 시도로 처리 시간을 20% 단축하려 했으나 실패했습니다. 대신 백업 스케줄 최적화로 전체 백업 시간을 15% 단축했습니다.


## 사내 쪽지 데이터 수집 및 자동 저장 시스템 구축 (2024)
- Role: 일일 약 5,000건의 사내 쪽지 데이터를 자동으로 수집 및 저장하는 시스템을 구축했습니다.
- Skill: Python 3.9, AWS Lambda, API Gateway, DynamoDB
- Description: Python 스크립트로 데이터를 수집하고 API Gateway를 통해 전송, Lambda 함수로 처리하여 DynamoDB에 저장하는 프로세스를 자동화했습니다. 이를 통해 데이터 처리 시간을 기존 대비 80% 단축했습니다.
- Problem Solving: 배치 처리(20건씩 묶어 처리)를 도입하여 API 요청을 90% 감소시키고, Lambda 함수의 메모리를 1024MB에서 2048MB로 증가시켜 처리 속도를 50% 향상시켰습니다.

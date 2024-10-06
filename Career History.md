## 정열 황 (JungYeol Hwang)
Junior Database Engineer
📧 sulum@naver.com | 📍 서울, 대한민국

## Professional Summary
대규모 시스템 관리, 클라우드 마이그레이션 및 성능 최적화에서 뛰어난 성과를 보여준 데이터베이스 엔지니어입니다. 최신 데이터베이스 기술을 활용하여 운영 효율성을 높이고, 비용 절감을 실현하는 데 집중하고 있습니다.

## Projects
## 1. 대규모 MySQL/MariaDB 클라우드 마이그레이션 (2024)
- Role : 50개 이상의 MySQL 및 MariaDB 인스턴스를 AWS로 마이그레이션하는 작업을 이끌었습니다.
- Skill : MySQL, MariaDB, AWS EC2, Xtrabackup
- Description: Xtrabackup을 사용해 실시간 데이터 동기화를 설정하고, Python으로 데이터 무결성을 검증하는 스크립트를 작성하여 데이터 손실 및 불일치 문제를 방지했습니다.
- Problem Solving: 인스턴스 구축을 빠르게 하기 위해 EC2에 구축한 향후 마스터로 사용할 인스턴스를 그대로 콜드카피하여 슬레이브로 구축을 시도하여 빠르게 클러스터를 구축하였습니다.하지만 개발팀과 데이터 정합성 TEST시 슬레이브로의 DELETE, UPDATE 의 바이너리로그가 복제가 되지 않는 문제가 발생하여 Xtrabackup으로 재구축 하였습니다. 실제 show slave status 상에서는 I/O, SQL STATUS 모두 정상이었지만 원인을 알수 없어 아쉬움을 남겼습니다.

## 2. AI 기반 자동 쿼리 최적화 시스템 개발 (2024)
- Role : AI 기술을 적용하여 슬로우 쿼리 최적화를 자동화하는 시스템을 설계하고 구현했습니다.
- Skill: Elasticsearch, Filebeat, Python
- Description: Filebeat로 슬로우 로그를 수집하고, Elasticsearch에 적재한 후, AI를 통해 슬로우 쿼리를 자동으로 최적화할 수 있는 시스템을 구축했습니다.
- Problem Solving:
  1. 슬로우 로그의 중복을 제거하는것이 관건이었습니다. 하루동안 쌓인 슬로우 로그를 mysqldumpslow 도구를 이용하여 통계정보와 함께 가공된 슬로우로그로 변환하고 이를 Filebeat가 자동으로 감지하여 ElasticSearch로 전송하게끔 했습니다.
  2. 또하나의 문제는 AI가 튜닝의 퀄리티를 높일 수 있도록 슬로우 쿼리에 존재하는 테이블의 DDL을 뽑아내어 엘라스틱서치에 적재하는것이었습니다. 이를 Python으로 추출하는 스크립트를 작성하여 적재할 수 있도록 했습니다.

## 3. 실시간 데이터베이스 통합 모니터링 시스템 구축 (2024)
- Role : Grafana와 Prometheus를 활용해 실시간 모니터링 시스템을 설계 및 구현했습니다.
- Skill : Grafana, Prometheus, PMM, Slack API, Telegram API
- Description: 실시간 데이터베이스 모니터링 대시보드를 설계하고, Slack과 Telegram API를 연동하여 알림 시스템을 구축했습니다.
- Problem Solving: 초기 과도한 알림 문제를 필터링 및 프로메테우스 우선순위 설정을 통해 해결했습니다.

## 4. 대규모 데이터베이스 백업 자동화 프로젝트 (2023)
- Role : 50개 이상의 데이터베이스 인스턴스에 대해 XtraBackup과 MariaBackup을 사용하여 자동 백업 시스템을 구축했습니다.
- Skill : XtraBackup, MariaBackup, Python
- Description: Python 스크립트를 사용하여 백업 자동화를 구현하고, 스토리지 비용을 절감하기 위해 백업 파일 압축 및 전송을 최적화했습니다.
- Problem Solving: 초기 백업 처리 속도가 느렸던 문제를 해결하기 위해 백업 프로세스를 멀티 스레드 방식으로 개선하여 처리 시간을 단축 시키려 했으나 xtrabackup의 내부동작 문제인지 멀티 스레드로 동작 시키는데 실패하였습니다. 좀더 기술적 깊이가 있었다면 해결할 수 있을것이라 생각되어 아쉬움이 컸습니다.

## 5. 사내 쪽지 데이터 수집 및 자동 저장 시스템 구축 (2024)
- Role : 사내 쪽지 데이터를 Python으로 수집하고, API Gateway로 전송하여 Lambda 함수가 자동 실행되어 DynamoDB에 적재되는 시스템을 설계 및 구현했습니다.
- Skill : Python, AWS Lambda, API Gateway, DynamoDB
- Description: 사내 쪽지 데이터를 수집하고, API Gateway를 통해 전송된 데이터를 Lambda로 처리하여 DynamoDB에 저장하는 프로세스를 자동화했습니다.
- Problem Solving : API 요청 과부하로 인한 타임아웃 문제를 해결하기 위해 요청을 배치로 처리하여 시스템 안정성을 확보했습니다.

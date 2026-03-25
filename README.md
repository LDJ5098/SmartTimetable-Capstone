# 저전력 스마트 표지판

## 프로젝트 개요
교실 앞 종이 시간표를 확인하는 불편함을 해소하기 위한 중앙집중관리 스마트 IoT 시스템입니다.
전자종이 디스플레이(E-Paper)를 활용하여 저전력으로 실시간 강의 정보를 제공합니다.

**개발 기간**: 2024.03 ~ 2024.11 (약 8개월)  
**팀 구성**: 컴퓨터공학 1명, 전기공학 2명, 기계공학 1명

## 프로젝트 미디어 자료
<img src="sample.png" alt="시스템 아키텍처" width="50%">
https://www.youtube.com/watch?v=apCBiD5LA90&list=PL0bpLNgLWNqSEkyhUqsxgQeczZ1ajG5RY&index=9

## 수상 내역
- 교내 캡스톤 경진대회 **대상**
- 2024 창의적 종합설계 경진대회 소재 컨소시엄 예선 **동상**

## 주요 기능
- 웹 기반 중앙집중 관리 시스템
- 실시간 교실 데이터 관리 (CRUD)
- 전력 모니터링 시스템
- 실시간 교실 위치 이동 기능
- 시간표 자동 업데이트

## 기술 스택

### Frontend
- HTML, CSS, JavaScript
- AJAX 비동기 통신

### Backend
- Ubuntu Server 20.04
- Apache2 Web Server
- PHP
- MySQL

### Communication & Protocol
- HTTP Protocol
- TCP/IP
- WiFi (ESP32)
- Web API
- Query String (URL 파라미터 기반 데이터 전송)

### Hardware
- ESP32 (IoT 보드)
- E-Paper Display (전자종이)
- Raspberry Pi 4B (서버)

### Development Tools
- VMware Workstation (테스트 환경)
- SSH (원격 서버 관리)


## 시스템 아키텍처
<img src="Project Architecture.png" alt="시스템 아키텍처" width="50%">

## 주요 성과
- [E2E 자동화] 제조사 프로그램 블랙박스 상태로, 시스템 단절된 구간 발생, 입출력 패턴분석을 통해 극복 및 무중단 자동화 구현
- [빠른 대안 탐색] 단말-DB 통신 결함을 해결하고자 3-Tier 구조, 중계 API를 대안 제시로 빠른 대안 탐색 및 적용
- [데이터 분할 전송] 대용량 데이터 전송 시 종결 식별자 기반의 분할 전송 기법(Chunking) 적용, 타임아웃 및 버퍼 문제 해결
- [반응성 최적화] 부분 비동기(AJAX) 전환으로 사용자 드래그 조작(60FPS)의 네트워크 레이턴시(RTT 10ms) 영향 최적화
- [개발 환경 개선] 하드웨어 의존성을 제거하기 위해 VMware 가상 테스트 환경 구축
- [원격 접속 환경] NAT 환경 포트포워딩과 SSH를 통한 24시간 원격 관리 환경 구축 및 지출 최소화
- [관리자 시스템] 표준 레이아웃 및 도면 시각화를 통해 비전공자도 운영 가능한 중앙집중관리 시스템 구축 및 학습 곡선 및 편의성 확보

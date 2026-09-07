# hks-12
안녕하세요 이번 펩리스 일경험 프르그램에 참가하게된 한규석이라고 합니다



### 1. [Topst nn server](https://github.com/kevin010827-creator/9_hks_topst)

🚀 About Me

🎯 관심 분야: MCU, RTOS, Embedded Linux, System Architecture, Hardware Optimization

🎓 교육 이력:
전자정보공학부 학사 재학 중



💡 목표: 팀원과의 원활한 소통을 바탕으로 효율적이고 검증된 임베디드 소프트웨어 및 하드웨어를 개발하는 엔지니어가 되는 것입니다.

📧 Contact: kevin13895@naver.com |

1. 🥇 [Keil MDK 도구로 이미지 변환을 하기 위한 ARM 코드 최적화] (개인 프로젝트)

기간: 2025.04.28 ~ 2025.06.08

주요 내용: ARM Cortex-A9 및 Keil MDK 환경에서 32-bit RGBA 이미지 데이터를 처리하는 3가지 변환 함수(RGBA별 배치, 색상 반전)를 ARM Assembly로 구현

담당 역할: ARM Assembly 코드 최적화 및 RGBA 이미지 변환 후 처리 속도 개선을 위한 메모리 재배치 알고리즘 설계

주요 성과:

A(Alpha) 값을 제외한 R, G, B 데이터를 각각 별도의 연속된 메모리 영역(R: 0x40010000, G: 0x40012580, B: 0x40014B00)으로 분리 배치하는 알고리즘 적용

4바이트 단위 비연속 접근 방식을 연속 메모리 접근 방식으로 개선하여 수행 시간 축소 (259,207 States / 0.00432s ➔ 230,418 States / 0.00384s)

2. 🥈 [Hand-made MNIST 데이터셋을 이용한 머신러닝 모델 최적화 분석] (팀 프로젝트 - 팀장)

기간: 2025.10.14 ~ 2025.11.24

주요 내용: 노이즈가 포함된 비정형 수기 숫자(Hand-made MNIST) 데이터셋을 활용한 머신러닝 분류 모델 최적화 (Jupyter Notebook / Anaconda 환경)

담당 역할: 팀장으로서 데이터 클리닝(이진화, 중앙 정렬 등) 파이프라인 구축 및 Grid Search를 통한 하이퍼파라미터 튜닝 주도

주요 성과:

임계치(Threshold) 설정을 통한 이미지 이진화(Binarization)로 배경 노이즈 제거 및 숫자 형상 추출

치우친 수기 숫자 데이터를 정중앙 픽셀 위치로 재정렬(Centering)하여 머신러닝 패턴 인식률 극대화

색반전 및 테두리/레이블 오류 데이터 수정 후 혼동 행렬(Confusion Matrix) 기반 높은 분류 정확도 검증

3. 🥉 [Linux 시스템 아키텍쳐 분석] (개인/팀 프로젝트)

기간: 2024.10.30 ~ 2024.12.15

주요 내용: SimpleScalar 시뮬레이터를 활용하여 CPU 프로세서(ALU, Scalar, 분기 예측) 및 캐시 구성(Block Size, Associativity, Replacement Policy) 변화가 시스템 성능에 미치는 영향 정량 분석

담당 역할: Linux 환경에서 SimpleScalar 구조 제어, 연산 장치 및 캐시 구조 변경에 따른 IPC, CPI, Miss Rate 분석

주요 성과:

Anagram, Compress, GCC, Go 벤치마크 프로그램별 Optimal Configuration 도출

Anagram 기준: 8-ALU, 8-Scalar, 3-bit Branch Prediction, 128B Block, 8-way, LRU 조합 시 최고 성능(IPC 2.3111, CPI 0.4327) 달성

Cache Block Size 증가(공간 지역성) 및 Associativity 증가(충돌 미스 감소)에 따른 성능 변화 검증

4. 🏆 [YOLO 객체 인식을 활용한 모터 제어 및 MCU-IPC 연동 구현] 

기간: 2026.08.29 ~ 2026.09.03

주요 내용: AI-G 보드의 YOLO 객체 인식 영상 데이터를 활용하여 VCP-G 보드 연동 모터 제어 및 MCU-IPC 연동 자율주행 파이프라인 구축

담당 역할: 객체 인식 정보 기반 차량 속도 및 LED 제어 로직 구현, CAN 통신 및 MCU-IPC 파이프라인 연결

주요 성과:

주변 차량 위치 인식 결과에 따라 모터 상태를 0, 1, 2 단계로 구분하여 주행 속도 가변 제어

result_pipeline.py ➔ control.py ➔ MCU can_demo.c ➔ gpio_ctrl.c로 이어지는 IPC/CAN 파이프라인 구축

주변 차량과의 거리에 따라 물리적 Blue/Red LED 실시간 점등 제어 구현

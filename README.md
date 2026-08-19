# 👋 안녕하세요! 임베디드 AI & 디지털 회로 설계 엔지니어 김희수입니다.

[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=Gmail&logoColor=white)](mailto:khs99113@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/computerAritist)

---

## 🚀 About Me
- 🎯 **관심 분야**: RTL Design (Verilog), Logic Synthesis & Timing Analysis, Embedded Edge AI, Control Systems
- 💡 **엔지니어링 핵심 강점**:
  - **RTL & Timing Optimization**: Static Timing Analysis 기반 Critical Path 분석 및 Pipelining 기법을 통한 Setup Time Violation 해결
  - **HW/SW & Mechanical Co-Design**: 물리적 환경 제약(중량, 배터리 용량, 무게중심)과 컴퓨팅 파워 간의 Trade-off를 고려한 시스템 최적화
  - **수학적 모델링 기반 제어**: $s$-domain 전달함수 수식화 및 요구 사양(Target Spec) 충족을 위한 PID 제어기 튜닝
  - **체계적인 회로 디버깅**: 아날로그(MOSFET 증폭기) 및 디지털 회로의 오차 원인 분석과 트러블슈팅

---

## 🛠 Tech Stack

### Hardware Design & Development Tools
![Verilog](https://img.shields.io/badge/Verilog_HDL-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Vivado](https://img.shields.io/badge/Xilinx_Vivado-C60000?style=flat-square&logo=xilinx&logoColor=white)
![MobaXterm](https://img.shields.io/badge/MobaXterm-002B49?style=flat-square&logo=mobaxterm&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

### Programming Languages & Frameworks
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=flat-square&logo=mathworks&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)

### Platforms
![NVIDIA Jetson nano](https://img.shields.io/badge/NVIDIA_Jetson_Orin-76B900?style=flat-square&logo=nvidia&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

---

## 📂 Key Projects & Experience

### 1. ⚡ Verilog 기반 8:1 Serializer 설계 및 Synthesis Timing 검증
* **기간**: 2026.05.27 ~ 2026.06.18
* **사용 기술**: `Verilog HDL`, `Synopsys Design Compiler`, `Timing Analysis`
* **주요 내용**: 하드웨어 계층 구조 기반의 8:1 Serializer 및 Clock Divider RTL 설계 및 논리 합성
* **트러블슈팅 & 성과**:
  * **문제 상황**: Logic Synthesis 진행 중 다단계 Combinational Logic의 누적 Propagation Delay로 인해 Setup Time Violation 발생
  * **원인 분석**: Synthesis Report 기반 Critical Path 추적을 통해 Target Clock Period 내 신호 미도달 원인 진단
  * **해결 방안**: 지연 집중 구간에 **Pipeline Register를 배치하는 RTL 구조 개선**을 통해 Clock Margin 확보 및 Timing Closure 달성

---

### 2. 🦯 AI 기반 시각장애인 음성 안내 보조 지팡이 개발
* **기간**: 2025.04.27 ~ 2025.09.26
* **사용 기술**: `NVIDIA Jetson Orin`, `Linux`, `Python`, `YOLOv5`, `PyTorch`, `TTS`
* **주요 내용**: YOLOv5 기반 실시간 객체(음료/장애물 등) 감지 및 사용자 음성 안내 시스템
* **트러블슈팅 & 성과**:
  * **문제 상황**: 보행 시 지팡이를 반복 스윙하는 환경에서 고성능 HW/대용량 배터리로 인한 중량 초과 및 실용성 저하
  * **해결 방안**: 사용자 피로도 최소화를 위한 **배터리 용량·무게 스펙 재산정** 및 하중을 손잡이 쪽으로 유도하는 **무게중심/기구 구조 최적화**
  * **결과**: 물리적 제약 조건(SW/HW Trade-off)을 극복하고 실환경 동작 안정성 및 휴대성 개선

---

### 3. 💡 [Capstone] 스마트 피로도 분석 기반 맞춤형 자동 스탠드 조절 장치 (진행 중)
* **기간**: 2026.XX ~ 진행 중
* **사용 기술**: `Raspberry Pi`, `Python`, `OpenCV`, `MediaPipe Face Mesh`, `회로 설계`
* **주요 내용**: 사용자 얼굴 랜드마크 분석 기반 실시간 피로도 측정 및 조도/색온도/각도 맞춤형 자동 제어 시스템
* **담당 역할 및 진행 상황**:
  * **비전 기반 피로도 판별**: MediaPipe Face Mesh 및 OpenCV를 활용한 눈깜빡임 빈도(EAR) 분석 알고리즘 구현
  * **다차원 피로 최적화 알고리즘 연구 (In Progress)**:
    * 사용자 눈 피로도, 주변 환경 조도(Ambient Light), 스탠드 밝기 및 색온도(CCT)를 3차원($X, Y, Z$) 축 파라미터로 정량화
    * 복합 환경 변수에 대응하여 최적의 시각적 편안함을 제공하는 제어 알고리즘 모델링 및 수식화
  * **하드웨어 제어 회로 구현**: 라즈베리파이 GPIO 인터페이싱, 모터 액추에이터 및 LED 디밍/조색 구동 제어 회로 설계

---

### 4. 🚗 시뮬레이션 기반 자율주행 알고리즘 구현
* **기간**: 2025.04.08 ~ 2025.06.21
* **사용 기술**: `Python`, `OpenCV`, `Autonomous Driving Simulator`
* **주요 내용**: 차선 인식(Hough Transform), 콘(Cone) 탐지 및 장애물 회피 주행 제어 알고리즘 구현
---

## 🔬 Engineering Experiments & Studies

### 📊 제어 시스템 설계 및 시뮬레이션 (MATLAB)
- 물리 시스템의 $s$-domain 전달함수 수식화 및 안정도 해석 (Routh-Hurwitz, Root Locus)
- Target Spec 달성을 위한 **PID 제어기 설계 및 게인 튜닝** (Step Response 시뮬레이션을 통한 Overshoot 및 Settling Time 최적화)

### ⚡ 전자회로 설계 및 트러블슈팅
- **MOSFET 증폭기**: Common Source(CS), Common Gate(CG), Source Follower(SF) 회로 설계 및 소신호 이득/주파수 응답 측정
- **오차 원인 분석**: 실험 데이터 오차 발생 시 기생 성분 및 바이어스 포인트 오차 요인을 체계적으로 분석·재실험하여 Target Spec 달성

---

## 📊 GitHub Stats

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=본인GitHubID&show_icons=true&theme=tokyonight&hide_border=true" alt="GitHub Stats" width="48%" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=본인GitHubID&layout=compact&theme=tokyonight&hide_border=true" alt="Top Languages" width="48%" />
</div>

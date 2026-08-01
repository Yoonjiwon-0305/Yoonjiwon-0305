# 👋 안녕하세요, 윤지원입니다.

**설계한 것이 의도대로 동작함을 증명하는 일에 집중하는 하드웨어 엔지니어입니다.**

한성대학교 전자시스템반도체학과를 졸업하고, 대한상공회의소 서울기술교육센터 **온디바이스 AI 반도체 설계 과정(1기)** 을 수료했습니다.
RTL 설계와 UVM 검증을 중심으로, 실시간 영상 처리와 온디바이스 AI 시스템까지 아우르는 프로젝트를 수행해 왔습니다.

📧 ygw4904@naver.com · 🐙 [@Yoonjiwon-0305](https://github.com/Yoonjiwon-0305)

---

## 💡 Tech Stack

### 🔧 Hardware Design

![SystemVerilog](https://img.shields.io/badge/SystemVerilog-FF6B35?style=for-the-badge&logo=verilog&logoColor=white)
![Verilog](https://img.shields.io/badge/Verilog-FF6B35?style=for-the-badge&logo=verilog&logoColor=white)
![Vivado](https://img.shields.io/badge/Vivado-0071C5?style=for-the-badge&logo=xilinx&logoColor=white)
![Vitis](https://img.shields.io/badge/Vitis-0071C5?style=for-the-badge&logo=xilinx&logoColor=white)

- **Protocols & Interfaces**: AXI4-Lite · AMBA APB · UART · SPI · I2C · SCCB · VGA
- **Platforms**: FPGA (Basys3) · MicroBlaze · STM32F411 · Raspberry Pi · Jetson Orin Nano

### ✅ Verification

![UVM](https://img.shields.io/badge/UVM-4A90E2?style=for-the-badge)
![VCS](https://img.shields.io/badge/VCS-4A90E2?style=for-the-badge)
![Verdi](https://img.shields.io/badge/Verdi-4A90E2?style=for-the-badge)

- **Focus**: Functional Coverage · Testbench Architecture · Constrained Random Verification

### 🤖 Embedded & AI

![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

- **AI Frameworks**: YOLO11 · YOLO Pose · OpenCV · Whisper.cpp · Ollama
- **Hardware Acceleration**: Edge TPU · Jetson Orin Nano

---

## 🎓 Education & Awards

**한성대학교 · 전자시스템반도체학과** | 졸업
디지털 논리 설계 · 마이크로프로세서 설계 · 회로 설계 · FPGA 설계 및 구현
🏆 교내 캡스톤 디자인 경진대회 **은상** — Vision Mandarin

**대한상공회의소 서울기술교육센터 · 온디바이스 AI 반도체 설계 과정 (1기)** | 수료
Verilog HDL & SystemVerilog · ARM AMBA BUS (AXI4-Lite, APB) · 32-bit RISC Processor 설계
UVM Verification & Functional Coverage · 온디바이스 AI 시스템 구축 · 임베디드 시스템

**SPTA · 반도체 구조형성 공정 실습** | 이수
클린룸 입실 실습 — Photolithography · Dry/Wet Etch · Oxidation · Wet Cleaning
제조 공정에 대한 이해가 설계의 완성도와 신뢰성을 높이는 기반임을 체감했습니다.

**Certifications** — TOEIC 700+ · TOEIC Speaking IM2

---

## 📌 Projects at a Glance

| 프로젝트 | 분류 | 핵심 |
|---|---|---|
| [AXI4-Lite SPI/I2C IP + UVM 검증](#1-axi4-lite-기반-spi--i2c-ip-설계-및-uvm-verification) | RTL · 검증 | Functional Coverage 100% |
| [RISC-V RV32I Single Cycle](#2-risc-v-rv32i-single-cycle-processor) | RTL | RV32I 전체 명령어 구현 |
| [RISC-V Multi Cycle & APB BUS](#3-risc-v-multi-cycle-processor--apb-bus) | RTL · 버스 | 주변장치 6종 MMIO 통합 |
| [다중 FPGA 영상 통합 연주 시스템](#4-다중-fpga-영상-통합-연주-시스템-the-bremen-town-musicians) | 영상 · 신호처리 | SPI 대역폭 50% 절감 |
| [UART Stopwatch & Digital Watch](#5-uart-기반-fpga-stopwatch--digital-watch) | RTL · 통신 | UART Rx 직접 설계 |
| [Vision Mandarin](#6-vision-mandarin--ai-기반-귤-자동-선별-시스템-) | 온디바이스 AI | 추론 성능 6.9배 향상 |
| [운전자 졸음 감지 시스템](#7-jetson-orin-nano-기반-운전자-졸음-감지-시스템) | 온디바이스 AI | Head Pose 기반 판단 로직 |

---

## 🔧 RTL Design & Verification

### 1. AXI4-Lite 기반 SPI / I2C IP 설계 및 UVM Verification

**KCCI 캡스톤 · 팀 프로젝트 | 1개월**

> MicroBlaze에 SPI/I2C Master를 AXI4-Lite로 연동하고, UVM 기반 검증 환경으로 기능을 검증

- AXI4-Lite Slave Interface 및 Register Map 설계, SPI/I2C Master FSM 구현
- **UVM Driver / Monitor / Scoreboard / Coverage 환경 전체 구축**
- Constrained Random 기반 256 Transaction, **Functional Coverage 100% 달성** ✅
- C 펌웨어로 레지스터 제어, FPGA 2대 간 SPI/I2C Master-Slave 실통신 검증 완료

**Tech**: `SystemVerilog` `UVM` `AXI4-Lite` `MicroBlaze` `Vivado` `VCS` `Verdi`

🔗 [RTL Repository](https://github.com/Yoonjiwon-0305/AXI) · [UVM Verification](https://github.com/Yoonjiwon-0305/UVM_SPI_I2C)

---

### 2. RISC-V RV32I Single Cycle Processor

**개인 프로젝트 | 1개월**

> RV32I ISA 기반 단일 사이클 프로세서 설계

- Datapath 및 Control Unit 구현 (opcode, funct3, funct7 기반 제어신호 생성)
- R / I / S / B / U / J Type 명령어 전체 구현
- Assembly 프로그램 기반 시뮬레이션 검증

**Tech**: `SystemVerilog` `Vivado` `FPGA (Basys3)`

🔗 [Repository](https://github.com/Yoonjiwon-0305/RISC_V)

---

### 3. RISC-V Multi Cycle Processor & APB BUS

**팀 프로젝트 | 1개월**

> 멀티 사이클 프로세서와 APB 버스 기반 시스템 통합

- **담당: APB Master 및 RAM(APB Slave) 설계**
- Memory-Mapped I/O를 통한 주변장치 6종 통합
- APB Protocol SETUP/ACCESS 타이밍 및 Address Decoder 개선
- C Firmware 기반 메모리 접근 검증

**Tech**: `SystemVerilog` `AMBA APB` `Vivado` `FPGA`

🔗 [Repository](https://github.com/Yoonjiwon-0305/RISC_V)

---

### 5. UART 기반 FPGA Stopwatch & Digital Watch

**개인 프로젝트 | 1개월**

> UART와 FSM을 활용한 PC·보드 통합 제어 스톱워치

- UART 수신기 설계 (4-state FSM, 16배 오버샘플링)
- ASCII Decoder로 PC 입력을 제어 신호로 변환, 보드 입력과 단일 경로로 통합
- FSM 기반 Control Unit (Watch/Stopwatch 모드 전환) 및 FND Controller 구현

**Tech**: `Verilog` `UART` `FSM` `Basys3`

🔗 [Repository](https://github.com/Yoonjiwon-0305/verilog)

---

## 📹 Real-time Video & Signal Processing

### 4. 다중 FPGA 영상 통합 연주 시스템 〈The Bremen Town Musicians〉

**팀 프로젝트 (6인) | 3주** · *OV7670 카메라 및 VGA 출력부는 개인 프로젝트로 선행 구현*

> Master 1대 + Slave 5대 구조로 6대 카메라 영상을 통합하고, 영상 내 표식 위치를 음계로 연주하는 시스템

**개인 선행 구현 — 카메라 입력부터 VGA 출력까지의 데이터 경로**
- **SCCB 컨트롤러 설계**: FSM 기반 카메라 초기화 및 레지스터 시퀀싱
- **VGA Timing Controller**: 640×480@60Hz 표준 타이밍 신호 생성
- **영상 처리 파이프라인**: QVGA(320×240) → VGA 업스케일링, RGB 채널 선택, 그레이스케일 변환
- BRAM 추론 및 ROM 기반 이미지 디스플레이 구현

**팀 프로젝트 담당 — 영상 압축 및 다중 보드 전송**
- **YCoCg Encoder/Decoder 설계**: 48bit RGB 블록(4픽셀)을 24bit 패킷으로 압축
- 부호 있는 색차 데이터를 4bit 필드에 저장하기 위한 offset 기법 적용
- **SPI 전송 대역폭 50% 절감**, 5채널 병렬 영상 전송 안정화
- 니블 정렬 오류로 인한 색 왜곡, GAP 상태 추가로 byte-slip 문제 해결

**Tech**: `SystemVerilog` `OV7670` `SCCB` `VGA` `SPI` `Basys3`

🔗 [OV7670 / VGA Controller](https://github.com/Junbro0608/VGA_CAM_Project/tree/main/Lab00_VGA_OV7670_ctrl) · [Video Processing](https://github.com/Yoonjiwon-0305/Video-Processing)

---

## 🤖 On-device AI

### 6. Vision Mandarin — AI 기반 귤 자동 선별 시스템 🏆

**졸업작품 · 팀 프로젝트 | 교내 캡스톤 경진대회 은상**

> Raspberry Pi4와 Edge TPU를 활용한 실시간 AI 귤 선별 시스템

- **Edge TPU 적용으로 CPU 대비 6.9배 추론 성능 향상** (1.53fps → 10.55fps)
- YOLO11 기반 귤 크기(Small/Medium/Large) 및 불량 여부 실시간 분류
- **담당: 컨베이어·분류기 하드웨어 설계 및 센서/모터 제어 회로 구현**
- 초음파 센서 → DC모터 → 서보모터 자동 분류 파이프라인 구축

**Tech**: `Python` `Raspberry Pi4` `Edge TPU` `YOLO11` `OpenCV` `GPIO`

🔗 [Repository](https://github.com/Yoonjiwon-0305/Graduation-Project)

---

### 7. Jetson Orin Nano 기반 운전자 졸음 감지 시스템

**팀 프로젝트 | 2주**

> AI 기반 실시간 운전자 상태 모니터링 및 음성 안내 시스템

- **담당: Face Detection 모델 학습 및 Head Pose 기반 졸음 판단 알고리즘 구현**
- Debouncing 프레임 누적을 통한 단계별 졸음 경고 로직 설계
- Whisper.cpp · Ollama · gTTS 기반 음성 질의응답 및 안내 시스템 연동
- 화면 중심 거리 기반 운전자 식별로 동승자 오추적 문제 해결

**Tech**: `Python` `YOLOv8` `OpenCV` `Jetson Orin Nano` `Ollama`

🔗 [Repository](https://github.com/Junbro0608/Monitor-drowsy-driving)

---

### 🚧 CNN 기반 제스처 인식 스마트 카메라 *(진행 중)*

**팀 프로젝트**

> FPGA에서 CNN 연산을 수행해 제스처를 인식하는 카메라 시스템

- **담당: Convolution 연산부 RTL 구현**
- 카메라 입력 영상에 대한 실시간 추론 파이프라인 구성

**Tech**: `SystemVerilog` `Vivado` `Python`

🔗 [Repository](https://github.com/Junbro0608/CNN-Based_Gesture_Smart_Camera)

---

**Last Updated**: 2026.08

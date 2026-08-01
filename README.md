# 👋 안녕하세요, 윤지원입니다.

**신뢰성이 곧 경쟁력이라고 믿는 엔지니어. 하드웨어와 소프트웨어의 경계를 넘나들며 완성도 높은 시스템을 설계합니다.**

한성대학교 전자시스템반도체학과를 졸업하고, 대한상공회의소 서울기술교육센터 **온디바이스 AI 반도체 설계 과정(1기)** 을 수료했습니다.
RTL 설계와 UVM 검증을 중심으로, 임베디드 시스템과 온디바이스 AI까지 아우르는 프로젝트를 수행해 왔습니다.

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

- **Focus**: Functional Coverage · Testbench Design · Simulation

### 🤖 Embedded & AI

![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

- **AI Frameworks**: YOLO11 · YOLO Pose · OpenCV · Whisper.cpp · Ollama
- **Hardware Acceleration**: Edge TPU · Jetson Orin Nano

---

## 📚 Featured Projects

### 1. AXI4-Lite 기반 SPI / I2C IP 설계 및 UVM Verification

**KCCI 캡스톤 · 팀 프로젝트 | 1개월**

> MicroBlaze에 SPI/I2C를 AXI4-Lite로 연동하고 UVM으로 검증

- AXI4-Lite Slave Interface 및 Register Map 설계, I2C/SPI Master FSM 구현
- **UVM Driver / Monitor / Scoreboard / Coverage 환경 전체 구축**
- **Functional Coverage 100% 달성** ✅
- FPGA 2대 간 SPI/I2C Master-Slave 통신 검증 완료

**Tech**: `SystemVerilog` `UVM` `AXI4-Lite` `Vivado` `VCS` `Verdi`

🔗 [RTL Repository](https://github.com/Yoonjiwon-0305/AXI) · [UVM Verification](https://github.com/Yoonjiwon-0305/UVM_SPI_I2C)

---

### 2. 다중 FPGA 영상 통합 연주 시스템 〈The Bremen Town Musicians〉

**팀 프로젝트 (6인) | 3주**

> Master 1대 + Slave 5대 구조로 6대 카메라 영상을 통합하고, 영상 내 표식 위치를 음계로 연주하는 시스템

- **담당: YCoCg Encoder/Decoder 설계** — 48bit RGB 블록(4픽셀)을 24bit 패킷으로 압축
- 부호 있는 색차 데이터를 4bit 필드에 저장하기 위한 offset 기법 적용
- **SPI 전송 대역폭 50% 절감**, 5채널 병렬 영상 전송 안정화
- 니블 정렬 오류로 인한 색 왜곡, GAP 상태 추가로 byte-slip 문제 해결

**Tech**: `SystemVerilog` `SPI` `VGA` `OV7670` `Basys3`

---

### 3. RISC-V RV32I Single Cycle Processor

**개인 프로젝트 | 1개월**

> RV32I ISA 기반 단일 사이클 프로세서 설계

- Datapath 및 Control Unit 구현 (opcode, funct3, funct7 기반 제어신호 생성)
- R / I / S / B / U / J Type 명령어 전체 구현
- Assembly 프로그램 기반 시뮬레이션 검증

**Tech**: `SystemVerilog` `Vivado` `FPGA (Basys3)`

🔗 [Repository](https://github.com/Yoonjiwon-0305/RISC_V)

---

### 4. RISC-V Multi Cycle Processor & APB BUS

**팀 프로젝트 | 1개월**

> 멀티 사이클 프로세서와 APB 버스 기반 시스템 통합

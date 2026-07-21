# 👋 안녕하세요, 윤지원입니다.

<div>
  <table>
    <tr>
      <td width="25%" align="center">
        <img src="images/profile.jpg" alt="윤지원" width="180" height="240" style="border-radius: 8px; border: 3px solid #FF6B35;">
      </td>
      <td width="75%">
        <h2>윤지원</h2>
        <p><strong>신뢰성이 곧 경쟁력이라고 믿는 엔지니어. 하드웨어와 소프트웨어의 경계를 넘나들며 완성도 높은 시스템을 설계합니다.</strong></p>
        <p>한성대학교 전자시스템반도체학과를 졸업하였으며, 대한상공회의소 서울기술교육센터 <strong>온디바이스 AI 반도체 설계 과정(1기)</strong>을 수료하면서 RTL 설계, Verification, Embedded System, AI 프로젝트를 수행하며 하드웨어와 소프트웨어를 함께 이해하는 역량을 쌓았습니다.</p>
        <p>📧 <strong>Email</strong>: ygw4904@naver.com</p>
        <p>🐙 <strong>GitHub</strong>: https://github.com/Yoonjiwon-0305</p>
      </td>
    </tr>
  </table>
</div>

---

## 💡 Tech Stack

### 🔧 Hardware Design
![SystemVerilog](https://img.shields.io/badge/SystemVerilog-FF6B35?style=for-the-badge&logo=verilog&logoColor=white)
![Verilog](https://img.shields.io/badge/Verilog-FF6B35?style=for-the-badge&logo=verilog&logoColor=white)
![Vivado](https://img.shields.io/badge/Vivado-0071C5?style=for-the-badge&logo=xilinx&logoColor=white)
![Vitis](https://img.shields.io/badge/Vitis-0071C5?style=for-the-badge&logo=xilinx&logoColor=white)

- **Protocols & Interfaces**: AXI4-Lite · AMBA APB · UART · SPI · I2C · VGA
- **Platforms**: FPGA (Basys3) · STM32F411 · Raspberry Pi · Jetson Orin Nano

### ✅ Verification & Testing
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

### 🏆 1. Vision Mandarin - AI 기반 귤 자동 선별 시스템
**졸업작품 | 은상 수상**

> Raspberry Pi4와 Edge TPU를 활용한 실시간 AI 기반 귤 자동 선별 시스템

- **Key Achievement**: Edge TPU 적용으로 CPU 대비 **6.9배 추론 성능 향상** (1.53fps → 10.55fps)
- YOLO11 기반 귤 크기(Small/Medium/Large) 및 불량 여부 실시간 분류
- 초음파 센서 → DC모터 → 서보모터 자동 분류 파이프라인 구현
- 기어드 모터 최적화로 안정적 분류 달성

**Tech**: `Python` `Raspberry Pi4` `Edge TPU` `YOLO11` `OpenCV` `GPIO`

🔗 [Repository](https://github.com/Yoonjiwon-0305/Graduation-Project)

---

### 2. AXI4-Lite 기반 SPI / I2C IP 설계 및 UVM Verification
**KCCI 과정 캡스톤 | 1개월**

> MicroBlaze에 SPI/I2C를 AXI4-Lite로 연동하고 UVM으로 검증

- AXI4-Lite Slave Interface 및 Register Map 설계
- I2C/SPI Master FSM 구현
- **UVM Driver / Monitor / Scoreboard / Coverage 환경 전체 구축**
- **Functional Coverage 100% 달성** ✅
- FPGA 2대 간 SPI/I2C Master-Slave 통신 검증 완료
- done(Tick) → busy(Level) 신호 개선으로 무한 대기 문제 해결

**Tech**: `SystemVerilog` `UVM` `AXI4-Lite` `Vivado` `VCS` `Verdi`

🔗 [RTL Repository](https://github.com/Yoonjiwon-0305/AXI)

🔗 [UVM Verification](https://github.com/Yoonjiwon-0305/UVM_SPI_I2C)

---

### 3. RISC-V RV32I Single Cycle Processor
**개인 프로젝트 | 1개월**

> RV32I ISA 기반 단일 사이클 프로세서 설계

- RV32I 명령어셋 기반 CPU 아키텍처 설계
- Datapath 및 Control Unit 구현 (opcode, funct3, funct7 기반)
- R / I / S / B / U / J Type 명령어 전체 구현
- Assembly 프로그램 기반 시뮬레이션 검증

**Tech**: `SystemVerilog` `Vivado` `FPGA (Basys3)`

🔗 [Repository](https://github.com/Yoonjiwon-0305/RISC_V)

---

### 4. RISC-V Multi Cycle Processor & APB BUS
**팀 프로젝트 | 1개월**

> 멀티 사이클 프로세서와 APB 버스 기반 시스템 통합

- APB Master 및 RAM(APB Slave) 설계
- Memory-Mapped I/O를 통한 6개 주변장치 통합
- APB Protocol SETUP/ACCESS 타이밍 최적화
- Address Decoder 개선으로 Slave 선택 안정화
- C Firmware 기반 메모리 접근 검증

**Tech**: `SystemVerilog` `APB` `Vivado` `FPGA`

🔗 [Repository](https://github.com/Yoonjiwon-0305/RISC_V)

---

### 5. Jetson Orin Nano 기반 운전자 졸음 감지 시스템
**팀 프로젝트 | 2주**

> AI 기반 실시간 운전자 상태 모니터링 및 음성 안내 시스템

- Face Detection + Head Pose Estimation 통합 분석
- Pose 기반 단계별 졸음 판단 알고리즘 (Debouncing 프레임 누적)
- Whisper.cpp & Ollama 기반 음성 질의응답 시스템
- gTTS 음성 안내 및 Bluetooth 스피커 연동
- 화면 중심 거리 기반 운전자 식별로 동승자 추적 오류 해결

**Tech**: `Python` `YOLOv8` `OpenCV` `Jetson Orin Nano` `Ollama` `Bluetooth`

🔗 [Repository](https://github.com/Junbro0608/Monitor-drowsy-driving)

---

### 6. UART 기반 FPGA Stopwatch & Digital Watch
**개인 프로젝트 | 1개월**

> UART와 FSM을 활용한 PC-보드 통합 제어 스톱워치

- UART 수신기 설계 (16배 오버샘플링, 4-state FSM)
- ASCII Decoder를 통한 PC 입력 → 제어 신호 변환
- FSM 기반 Control Unit (Watch/Stopwatch 모드 전환)
- FND Controller 및 버튼 입력 통합 제어
- 펄스/레벨 신호 및 에지 검출 디버깅 경험 확보

**Tech**: `Verilog` `UART` `FSM` `Basys3`

🔗 [Repository](https://github.com/Yoonjiwon-0305/verilog)

---

### 7. VGA Controller & Image Display
**KCCI 과정 중**

> 640×480@60Hz VGA 타이밍 제어기 및 이미지 디스플레이

- VGA Timing Controller 설계 (표준 타이밍 준수)
- BRAM 추론 및 ROM 기반 이미지 디스플레이
- 이미지 업스케일링 구현

**Tech**: `SystemVerilog` `VGA` `FPGA` `Vivado`

🔗 [Repository](https://github.com/Yoonjiwon-0305/Video-Processing
)

---

### 8. OV7670 기반 실시간 영상 처리 시스템
**개인 프로젝트 | KCCI 과정 중**

> QVGA 저해상도 카메라 영상을 VGA 표준 해상도로 실시간 처리 및 디스플레이

**주요 내용**:
- **OV7670 SCCB 컨트롤러 설계**: FSM 기반 카메라 초기화 (Register Sequencing)
- **OV7670_INIT_ROM**: 카메라 센서 필수 레지스터 주소/값 저장
- **AUTO_SETTING_ADDR_MEM**: 동적 재설정을 위한 레지스터 관리 메모리
- **영상 처리 파이프라인**:
  - QVGA(320×240) → VGA(640×480@60Hz) 업스케일링 (Upscal Filter)
  - RGB 채널 선택 모드 (보드 스위치로 실시간 제어)
  - 그레이스케일 변환 (Gray Filter)
- **VGA 타이밍 컨트롤러**: 표준 VGA 출력 신호 생성 및 동기화

**핵심 학습**:
- SCCB 직렬 통신 프로토콜 구현
- 카메라 센서 제어 및 초기화 시퀀싱
- 실시간 영상 처리 및 필터 파이프라인 설계
- 디지털 필터 (업스케일링, 그레이스케일 변환) 알고리즘 구현

**기술**: `SystemVerilog` `SCCB` `OV7670` `VGA` `FPGA` `Vivado`

🔗 [Repository](https://github.com/Junbro0608/VGA_CAM_Project/tree/main/Lab00_VGA_OV7670_ctrl)

---

## 🏆 Awards & Achievements

| 수상 | 상세 |
|------|------|
| **한성대학교 졸업작품 경진대회 은상** | Vision Mandarin AI 귤 선별 시스템 |
| **KCCI 온디바이스 AI 반도체 설계 과정 수료** | 1기 수료생 |

---

## 🎓 Education

### 한성대학교
**전자시스템반도체학과** | 졸업

- 디지털 논리 설계
- 마이크로프로세서 설계
- 회로 설계
- FPGA 설계 및 구현

### 대한상공회의소 서울기술교육센터
**온디바이스 AI 반도체 설계 과정 (1기)** | 수료

**Core Curriculum**:
- Verilog HDL & SystemVerilog
- FPGA 설계 (Basys3, Vivado)
- ARM AMBA BUS 프로토콜 (AXI4-Lite, APB)
- 32-bit RISC Processor 설계
- UVM Verification & Functional Coverage
- Jetson Orin Nano 기반 AI 시스템 구축
- 임베디드 시스템 (STM32F411, Raspberry Pi)

---

## 🎯 Focus Areas

- ✨ **FPGA 디지털 시스템 설계**
- 🔍 **Hardware Verification (UVM)**
- ⚡ **실시간 임베디드 시스템**
- 🤖 **On-Device AI & Edge Computing**

---

## 📫 Contact & Links

| Channel | Link |
|---------|------|
| 📧 **Email** | ygw4904@naver.com |
| 🐙 **GitHub** | [@Yoonjiwon-0305](https://github.com/Yoonjiwon-0305) |

---

**Last Updated**: 2026.07 | 지속적으로 업데이트 중입니다. 📈

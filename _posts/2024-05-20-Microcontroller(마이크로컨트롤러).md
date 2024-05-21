---
layout: single
title: Microcontroller(마이크로컨트롤러)
categories:
  - Engineering
tags:
  - embedded
  - microprocessor
toc: true
author_profile: true
aliases: 
connected:
  - "[[2024-05-20-Microprocessor-Basics|마이크로프로세서-과목정리]]"
---
## Microcontroller
### **마이크로 컨트롤러 종류**
![](../../files/microcontrollers.png)
### 마이크로 컨트롤러의 주요 구성 요소
1. **중앙 처리 장치(CPU)**
	- 명령어를 실행하고 데이터를 처리
	- 주로 8비트, 16비트, 32비트 프로세스가 사용
2. **메모리:**
	- 플래시 메모리: 프로그램 코드를 저장
	- SRAM(Static RAM): 데이터 저장 및 실행 중인 작업에 사용
	- EEPROM: 비휘발성 메모리로, 데이터 저장에 사용.
3. **입출력 포트(I/O Ports):**
	- 디지털 및 아날로그 신호를 입력받거나 출력하는 역할.
	- 센서, 액추에이터, 디스플레이 등 다양한 외부 장치와 연결
4. **타이머 및 카운터:**
	- 시간 기반 이벤트를 관리하고, 타이밍 기능 제공
	- 주기적 인터럽트 발생, 시간 지연 생성 등에 사용
5. **직렬 통신 인터페이스:**
	- UART(Universal Asynchronous Receiver/Transmitter), SPI(Serial Peripheral Interface), I2C(Inter-Integrated Circuit)등 다양한 통신 프로토콜을 지원하여 다른 장치와 데이터 교환
6. **아날로그-디지털 변환기(ADC):**
	- 아날로그 신호를 디지털 신호로 변환하여 마이크로컨트롤러에서 처리할 수 있게 함.
7. **인터럽트:**
	- 특정 이벤트가 발생하면 CPU의 현재 작업을 중단하고, 우선순위가 높은 작업을 처리하는 메커니즘.

### CPU: Architecture
>Von 

| 특성       | Von Neumann 아키텍처      | Harvard 아키텍처     |
| -------- | --------------------- | ---------------- |
| 메모리 구조   | 단일 메모리 공간             | 분리된 메모리 공간       |
| 버스 시스템   | 단일 버스                 | 이중 버스            |
| 속도 및 효율성 | 버스 병목현상으로 인해 속도 저하 가능 | 병목현상이 줄어들어 더 빠름  |
| 설계 및 구현  | 설계가 간단하고 구현이 용이       | 설계가 복잡하고 구현이 어려움 |
| 메모리 유연성  | 높은 유연성                | 낮은 유연성           |
| 동적 코드 수정 | 가능                    | 불가능 또는 어려움       |


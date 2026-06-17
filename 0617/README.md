# Rotary_Encoder_TIM


## NUCLEO-F103RB 기준 하드웨어 구성:
* Encoder A Phase (CH1): PA6 (TIM3_CH1) ← D12
* Encoder B Phase (CH2): PA7 (TIM3_CH2) ← D11
* USART2 (디버그 출력): PA2(TX), PA3(RX) — 115200 baud
* B1 버튼: PC13 — Encoder count 리셋
* LD2: PA5 — 동작 표시 LED


## 📁 프로젝트 구조
```
C:\work\stm32_rotary_encoder\
└── Core\
    ├── Inc\main.h
    └── Src\main.c
```

##🔌 하드웨어 연결 (NUCLEO-F103RB)

| 신호    | 핀    | TIM3 매핑    | 보드 커넥터 |
|:------:|:------:|:------:|:------:|
| Encoder Phase A    | PA6    | TIM3_CH1    | D12 |
| Encoder Phase B    | PA7    | TIM3_CH2    | D11 |
| USART2 TX    | PA2    | -    | - |
| USART2 RX    | PA3    | -    | - |
| B1 (Reset)    | PC13    | -    | User Button |
| LD2 (LED)    | PA5    | -    | Built-in LED |

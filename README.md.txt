# Servo Motor Angle Control using Potentiometer (STM32F4 + OLED)

## Description
Reads analog value from potentiometer using ADC1 and maps it to servo motor angle (0° to 180°) using PWM (TIM1).  
Current angle is displayed on SSD1306 OLED over I2C.

## Components
- STM32F401RE
- Potentiometer (PA0)
- Servo Motor (PA8 - TIM1_CH1 PWM)
- OLED (PB8 - SCL, PB9 - SDA)

## Output
Servo Angle: 105°
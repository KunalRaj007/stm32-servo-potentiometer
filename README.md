# 🎛️ Potentiometer-Controlled Servo Angle Display System using STM32

This embedded project uses **STM32F401RE**, **Potentiometer**, **Servo Motor**, and **OLED Display (SSD1306 I2C)**.  
It reads analog voltage from the potentiometer using **ADC1**, maps it to a servo angle (0°–180°) using **PWM (TIM1)**, and displays the current angle on the OLED.

---

## 🔧 Components Used

| Component           | Purpose                                      |
|---------------------|---------------------------------------------|
| STM32F401RE         | Main microcontroller                        |
| Potentiometer       | Analog input to control angle               |
| SG90 Servo Motor    | Rotates to specified angle via PWM         |
| SSD1306 OLED (I2C)  | Displays mapped angle                      |
| Jumper Wires        | Connections                                 |
| Power Supply        | 5V for servo + board                        |

---

## ✨ Features

- 🎚️ **Live analog reading** from potentiometer (ADC1)
- 📐 **Maps value** (0–4095) to servo angle (0°–180°)
- ⚙️ **Servo rotation** using TIM1 PWM output
- 🖥️ **OLED display** shows current servo angle
- ✅ STM32 HAL-based clean modular code

---

## 📐 Pin Configuration

| Module        | STM32F401RE Pin | Description              |
|---------------|------------------|--------------------------|
| Potentiometer | PA0 (ADC1 IN0)   | Analog voltage input     |
| Servo Motor   | PA8 (TIM1 CH1)   | PWM output               |
| OLED (I2C)    | PB8 (SCL), PB9 (SDA) | I2C Communication    |

---

## 🧪 Working Logic

1. Potentiometer gives analog voltage (0–3.3V)
2. ADC1 reads value (0–4095)
3. This value is linearly mapped to angle (0°–180°)
4. Servo is rotated using PWM with corresponding duty cycle
5. OLED displays the mapped angle

---

## 🛠️ Project Setup

1. Clone this repo into your STM32CubeIDE workspace  
2. Connect hardware as per above table  
3. Build and flash firmware  
4. Rotate potentiometer knob and observe OLED + Servo  

---

## 📚 Libraries Used

- [SSD1306 OLED I2C Driver](https://github.com/afiskon/stm32-ssd1306) – afiskon  
- STM32 HAL Drivers (CubeMX Generated)  
- TIM1 for PWM generation  
- ADC1 for analog value reading  

---

## 📷 Demo Preview

><img width="237" height="311" alt="image" src="https://github.com/user-attachments/assets/df137be8-30a1-4c12-9e31-b04e14e5d58e" />


---

## 📦 Real-World Applications

- Joystick-based Robotic Arm Control  
- DIY Angle Calibration Tools  
- Servo-based Analog Signal Mapping  
- Smart Control Panels  

---

## 📜 License

This project is open-source and available under the **MIT License**.

---

## 👤 Author

**Kunal Raj**  
Embedded Systems Developer | IoT Enthusiast  
GitHub: [https://github.com/KunalRaj007](https://github.com/KunalRaj007)  
Email: Kunalraj1699.com

---


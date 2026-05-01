Khushil Naishadh Dave  
Socio-technical systems Engineering  
Matrikel-Nr: 6640457  
A portfolio documenting exercises and projects from the Digital Design and Fabrication course at the University of Oldenburg.  
# Exercise 1: Electrical Circuits
Task 1 – LED Control Circuit  

    Task 1.1 - Simple LED Circuit
   <img src="https://github.com/user-attachments/assets/2cea63ba-24dd-4129-8281-e4fb42ce29d7" width="200">
  
 Observation Table:  
 
| Resistor (Ω) | VLED (V) | V1 (V) |
|--------------|--------|----------|
| 220 Ω        | 2.86v  | 2.28v    |
| 1000 Ω       | 2.51v  | 2.77v    |
| 4700 Ω       | 2.31v  | 2.97v    |  

      My experience/observation: 
→ I observed that the brightness of the LED changes depending on the resistor value. With a lower resistance (220Ω), the LED was brighter, while increasing the resistance (1kΩ and 4.7kΩ) made the LED progressively dimmer.  
→ In terms of voltage drop in R1,i observed using a multimeter that the voltage drop across R1 changes when the resistor value is increased. As the resistance increases, the voltage drop across R1 also changes, and I could clearly see this difference in the readings on the multimeter.  
→ In terms of the effect of R1 on the LED, I observed that the value of R1 significantly affected the LED. As we increased the resistor value from 220Ω to 4700Ω, the LED became noticeably dimmer compared to when a lower resistance was used.  
→ One error/mistake i want to admit is that,the circuit was not working initially due to a missing ground connection. After fixing it, the circuit worked properly.  

     Task 1.2 – Switchable LED Circuit  
  <p align="center">
  <img src="https://github.com/user-attachments/assets/1f8ac679-8549-474f-ada8-2c34f64e3fc5" width="200">
  <img src="https://github.com/user-attachments/assets/2a7ae392-6c2e-48a3-b2b5-bcb2189765b4" width="200">
</p>  

    My experience/observation:  
 → When I connected the switch in the both/opposite direction, I did not observe any difference. The circuit behaved the same, and the LED functioned normally in both cases.So,i fell like the switch simply controls the flow of current, regardless of its orientation.  
 
      Task 1.3 – Dimmable LED Circuit
  <p align="center">
  <img src="https://github.com/user-attachments/assets/1692d230-f5c5-43ba-92e4-7b9e197dd42c" width="250">
  <img src="https://github.com/user-attachments/assets/15b6f570-8b9c-4a2d-88bd-4e8fb11a594e" width="250">
</p>  
Obsevation table:  

| Position        | VLED (V) | V2 (V) |
|-----------------|----------|--------|
| a) Full brightness |  3.01v| 3.05v  |
| b) Dimmed          |  2.30v| 4.45v  |
| c) OFF             | 0.005v| 4.50v  |  

    My experience/Observation:
  → Increasing the potentiometer resistance caused the LED to gradually dim and eventually turn OFF.  
  → Moreover,the voltage across the LED (VLED) decreased as the brightness decreased. At the same time, the voltage across the potentiometer (V2) changed accordingly.  
  → However,the relationship is continuous: as resistance increases, current decreases, which reduces the LED brightness.  
  → One more thing,we missed the ground connection on the potentiometer (V2 side), so the LED could not turn fully OFF. After correcting it, the circuit worked properly. 
  
Task 2 – Transistor Switch Circuit  

    Task 2.1 – Switchable LED Strip
<p align="center">
  <img src="https://github.com/user-attachments/assets/b4f4284d-b571-44d1-bc7d-d8dac714ef3d" width="300">
  <img src="https://github.com/user-attachments/assets/d801e5ac-bdf2-4e4e-abe6-f69ecbae37cf" width="300">
</p>  

    My experience/observation:
 → The LED strip turns ON and OFF using the switch. The switch controls the gate voltage (VGS), which turns the MOSFET ON or OFF, allowing current to flow through the LED strip.  
 → As observed,The switch controls the gate voltage (VGS) of the MOSFET.  
→ Principle applied is that: The MOSFET acts as a switch,when a gate voltage is applied, it turns ON and allows current to flow; without gate voltage, it remains OFF and blocks current.  

    Task 2.2 – Dimmable LED Strip
<p align="center">
  <img src="https://github.com/user-attachments/assets/f981d67b-6b11-46d7-9765-f4b7aa5de56b" width="220">
  <img src="https://github.com/user-attachments/assets/90847cae-a11d-4454-b68c-8b2e1765655a" width="220">
  <img src="https://github.com/user-attachments/assets/ed2f5430-3e79-48f3-84bb-9211bb525b1c" width="220">
</p>  
A) In terms of Duty cycle:  

    My Observation:
As the duty cycle increases, the brightness of the LED strip increases.

- Low duty cycle (2%) → LED is very dim  
- Medium duty cycle (75%) → LED is moderately bright  
- High duty cycle (100%) → LED is fully bright
  
→ Moreover,this happens because the LED is ON for a longer time within each cycle as the duty cycle increases.  
→ As well as,this relationship is proportional: higher duty cycle → higher average power → brighter LED.  
→ As i understand,both methods control LED brightness, but dimmable LED circuit (potentiometer) uses analog voltage control, while PWM uses rapid switching.So, PWM is more efficient.  









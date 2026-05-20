Khushil Naishadh Dave  
Socio-technical systems Engineering  
Matrikel-Nr: 6640457  
A portfolio documenting exercises and projects from the Digital Design and Fabrication course at the University of Oldenburg.  
# Exercise 1: Electrical Circuits
### Task 1 – LED Control Circuit  

    Task 1.1 - Simple LED Circuit
   <img src="https://github.com/user-attachments/assets/2cea63ba-24dd-4129-8281-e4fb42ce29d7" width="200">  
   
  
Observation Table:  
 | Resistor (Ω) | VLED (V) | V1 (V) |
|--------------|--------|----------|
| 220 Ω        | 2.86V  | 2.28V    |
| 1000 Ω       | 2.51V  | 2.77V    |
| 4700 Ω       | 2.31V  | 2.97V    |  

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
 → When I connected the switch in the both/opposite direction, I did not observe any difference. The circuit behaved the same, and the LED functioned normally in both cases.I observed that the switch simply controls the flow of current, regardless of its orientation.  
 
      Task 1.3 – Dimmable LED Circuit
  <p align="center">
  <img src="https://github.com/user-attachments/assets/1692d230-f5c5-43ba-92e4-7b9e197dd42c" width="250">
  <img src="https://github.com/user-attachments/assets/15b6f570-8b9c-4a2d-88bd-4e8fb11a594e" width="250">
</p>  
Obsevation table:  

| Position        | VLED (V) | V2 (V) |
|-----------------|----------|--------|
| a) Full brightness |  3.01V| 3.05V  |
| b) Dimmed          |  2.30V| 4.45V  |
| c) OFF             | 0.005V| 4.50V  |  

    My experience/Observation:
  → Increasing the potentiometer resistance caused the LED to gradually dim and eventually turns OFF.  
  → Moreover,the voltage across the LED (VLED) decreased as the brightness decreased. At the same time, the voltage across the potentiometer (V2) changed accordingly.  
  → However,the relationship is continuous: as resistance increases, current decreases, which reduces the LED brightness.  
  → One more thing,we missed the ground connection on the potentiometer (V2 side), so the LED could not turn fully OFF. After correcting it, the circuit worked properly. 
  
### Task 2 – Transistor Switch Circuit  

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
- Medium duty cycle (40-75%) → LED is moderately bright  
- High duty cycle (100%) → LED is fully bright
  
→ Moreover,this happens because the LED is ON for a longer time within each cycle as the duty cycle increases.  
→ As well as,this relationship is proportional: higher duty cycle → higher average power → brighter LED.  
→ As i understand,both methods control LED brightness, but potentiometer uses analog voltage control, while PWM uses rapid switching.So, PWM is more efficient.  

B) In terms of Frequence:
<p align="center">
  <img src="https://github.com/user-attachments/assets/831e0733-5d72-4710-991d-de592663b71c" width="240">
  <img src="https://github.com/user-attachments/assets/42e620f3-46b8-48e5-b8a9-e48db83fae7b" width="240">
</p>

<p align="center">
  <em>f = 5 Hz, D = 50%</em> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <em>f = 45 Hz, D = 50%</em>
</p>  

    My experience/observation:
→ Keeping the duty cycle constant at D = 50%, I observed that the behavior of the LED strip changes with frequency.
- At low frequency (5 Hz), the LED clearly flickers as it turns ON and OFF slowly.
- At medium frequencies (25–45 Hz), the flickering becomes less noticeable.
- At higher frequency (100 Hz), the LED appears stable and continuously ON.

→ Moreover,this happens because the switching becomes too fast for the human eye to detect.  
→ As i observed the flickering effect gradually disappears as the frequency increases and becomes almost unnoticeable around higher frequencies (≈ 45–100 Hz).  
# Exercise 2: Introduction to Arduino  
### Task 2.1 – Connecting the buzzer  
 
https://github.com/user-attachments/assets/aac36e21-9d10-4d4b-8759-7579b1203ca2  


     My experience/observation:  
    
I connected the buzzer to the Arduino and uploaded the test code successfully.The buzzer produced sound according to the HIGH and LOW timing values in the code. By changing the delay values, I observed that the sound pattern and speed changed noticeably.

- Smaller delay → faster beeping
- Larger delay → slower beeping

This helped me understand how timing in Arduino code directly affects hardware behavior.  
### Task 2.2 – Connecting the LCD screen  

<p align="center">
  <img src="https://github.com/user-attachments/assets/7b3a199f-3e35-4104-91d0-e1bd653d3704" width="500">
</p>  

     Small code segment for context:
lcd.init();  
lcd.backlight();  
lcd.setCursor(0,0);  
lcd.print("LCD Testing");  
lcd.setCursor(0,1);  
lcd.print("Hello Khushil!");  


    My experience/observation:   
-> After connecting the LCD screen and installing the required `LiquidCrystal_I2C` library, we successfully displayed text on the LCD using Arduino code.  


-> We also experimented with different text messages, cursor positions, and display arrangements on the LCD screen. By modifying the code, we observed how the text output changed dynamically on the display.  

-> This helped us understand how Arduino communicates with the LCD using the I2C protocol.  
### Task 2.3 - Expanding the setup with a Real Time Clock   
https://github.com/user-attachments/assets/a5d30240-e2eb-4bd5-9990-1216adcd9d7e   

    My experience/observation:

-> In this task, we connected the RTC (Real Time Clock) module with the Arduino using I2C communication.  


-> Using the I2C scanner and Serial Monitor in the Arduino IDE, we successfully identified the address of the RTC module and observed the real-time date and time values.  


-> We also experimented with the RTC module by disconnecting and reconnecting the circuit, and observed that the module continued keeping the correct time because of its backup battery.  


-> This experiment helped us understand how multiple I2C devices can communicate with Arduino using the same communication lines while using different addresses.  
### Task 2.4 -  Using the Push Button  
https://github.com/user-attachments/assets/aedfa003-45f7-4933-a784-ab7128eab55b    

    My experience/observation:  
-> In this task, we connected a push button to the Arduino using the built-in pull-up resistor configuration.  
 

-> When the push button was pressed, the Serial Monitor displayed the message “Pushed”. Releasing the button stopped the message output.  


-> This helped us understand how Arduino reads digital input signals from a push button using the `INPUT_PULLUP` configuration.    

### Task 2.5 - Building an Alarm Clock  

<p align="center">
  <img src="https://github.com/user-attachments/assets/68432047-0bef-4abc-a293-83a00de3ef12" width="350">
  <img src="https://github.com/user-attachments/assets/3e235087-48ff-46a2-a8b2-8ba3c033a0cd" width="350">
</p>  

https://github.com/user-attachments/assets/66f36df7-c88f-4cf8-b2a1-d0fbdfbc3a56  

--> Firstly, we started with a beginner-level alarm clock circuit by combining a push button, LCD screen, RTC module, and buzzer.  


--> The RTC module continuously kept track of the real time, while the LCD displayed the current time. We set the alarm time directly in the Arduino code, and when the current time matched the alarm time, the buzzer started buzzing.  


--> We also added a push button feature so that pressing the button turned the alarm OFF.   

<img width="350" height="350" alt="7b446c91-55a2-468f-b77c-c9898d8af955" src="https://github.com/user-attachments/assets/b44cc93d-fafb-44a0-bf99-36904d5c54f3" />  


https://github.com/user-attachments/assets/4a54ce8a-561f-4bed-ab7b-1ae1427213d8   

--> After successfully building the basic version, we decided to make the alarm clock more advanced by adding two more push buttons.

- The green button was used to select whether to set the hours or minutes.
- The white button was used to increase/change the selected hour or minute value.
- The red button was used to stop the alarm when it started buzzing.

--> This made the alarm clock more interactive and allowed us to control the alarm settings directly using hardware buttons instead of changing the code repeatedly.  

https://github.com/user-attachments/assets/32feefe7-05b7-4eaa-84e4-d2e9dac414fd   

--> To make the project more fun and interactive, we also added a simple math challenge feature to turn OFF the alarm.  


--> When the alarm started buzzing, a math question appeared on the LCD screen. The white button was used to increase the answer value, and the red button was used to submit the answer.  


--> If the entered answer was correct, the alarm stopped successfully. Otherwise, the alarm continued buzzing until the correct answer was submitted.  



















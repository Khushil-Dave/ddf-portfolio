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
→ After connecting the LCD screen and installing the required `LiquidCrystal_I2C` library, we successfully displayed text on the LCD using Arduino code.  


→ We also experimented with different text messages, cursor positions, and display arrangements on the LCD screen. By modifying the code, we observed how the text output changed dynamically on the display.  

→ This helped us understand how Arduino communicates with the LCD using the I2C protocol.  
### Task 2.3 - Expanding the setup with a Real Time Clock   
https://github.com/user-attachments/assets/a5d30240-e2eb-4bd5-9990-1216adcd9d7e   

    My experience/observation:

→ In this task, we connected the RTC (Real Time Clock) module with the Arduino using I2C communication.  


→ Using the I2C scanner and Serial Monitor in the Arduino IDE, we successfully identified the address of the RTC module and observed the real-time date and time values.  


→ We also experimented with the RTC module by disconnecting and reconnecting the circuit, and observed that the module continued keeping the correct time because of its backup battery.  


→ This experiment helped us understand how multiple I2C devices can communicate with Arduino using the same communication lines while using different addresses.  
### Task 2.4 -  Using the Push Button  
https://github.com/user-attachments/assets/aedfa003-45f7-4933-a784-ab7128eab55b    

    My experience/observation:  
→ In this task, we connected a push button to the Arduino using the built-in pull-up resistor configuration.  
 

→ When the push button was pressed, the Serial Monitor displayed the message “Pushed”. Releasing the button stopped the message output.  


→ This helped us understand how Arduino reads digital input signals from a push button using the `INPUT_PULLUP` configuration.    

### Task 2.5 - Building an Alarm Clock  

<p align="center">
  <img src="https://github.com/user-attachments/assets/68432047-0bef-4abc-a293-83a00de3ef12" width="350">
  <img src="https://github.com/user-attachments/assets/3e235087-48ff-46a2-a8b2-8ba3c033a0cd" width="350">
</p>  

https://github.com/user-attachments/assets/66f36df7-c88f-4cf8-b2a1-d0fbdfbc3a56  

→ Firstly, we started with a beginner-level alarm clock circuit by combining a push button, LCD screen, RTC module, and buzzer.  


→ The RTC module continuously kept track of the real time, while the LCD displayed the current time. We set the alarm time directly in the Arduino code, and when the current time matched the alarm time, the buzzer started buzzing.  


→ We also added a push button feature so that pressing the button turned the alarm OFF.   

<img width="350" height="350" alt="7b446c91-55a2-468f-b77c-c9898d8af955" src="https://github.com/user-attachments/assets/b44cc93d-fafb-44a0-bf99-36904d5c54f3" />  


https://github.com/user-attachments/assets/4a54ce8a-561f-4bed-ab7b-1ae1427213d8   

→ After successfully building the basic version, we decided to make the alarm clock more advanced by adding two more push buttons.

- The green button was used to select whether to set the hours or minutes.
- The white button was used to increase/change the selected hour or minute value.
- The red button was used to stop the alarm when it started buzzing.

→ This made the alarm clock more interactive and allowed us to control the alarm settings directly using hardware buttons instead of changing the code repeatedly.  

https://github.com/user-attachments/assets/32feefe7-05b7-4eaa-84e4-d2e9dac414fd   

→ To make the project more fun and interactive, we also added a simple math challenge feature to turn OFF the alarm.  


→ When the alarm started buzzing, a math question appeared on the LCD screen. The white button was used to increase the answer value, and the red button was used to submit the answer.  


→ If the entered answer was correct, the alarm stopped successfully. Otherwise, the alarm continued buzzing until the correct answer was submitted.  

# Exercise 3: Sensors & Actuators  

 ### Task 3.1 – Pneumatic Control System  
 
<p align="center">
  <img src="https://github.com/user-attachments/assets/fa5a7635-f429-4342-a246-d447bcf22af5" width="350">
  <img src="https://github.com/user-attachments/assets/01d8c3aa-15ff-483f-bc01-1ab3ecc8e856" width="350">
</p>  

https://github.com/user-attachments/assets/7561f754-c745-459e-bc64-9403d5f2ac7b   

    My experience/observation:

→ In this, we assembled a pneumatic and electrical control circuit using Arduino, MOSFET modules, pumps, and a valve.  


→ The system was programmed to go through three different phases:

- Inflation phase → the pumps inflated the air pillow.
- Hold phase → the system maintained the pressure for a few seconds.
- Deflation phase → the valve opened and the air was released from the pillow.
 

→ By uploading the Arduino code and testing the setup repeatedly, we observed that the pumps and valve operated according to the programmed timing sequence.  

→ During the setup process, we initially made a mistake while connecting the DC motors because both air tubes were connected to the outlet side. As a result, the airflow did not work correctly. After realizing the issue, we corrected the tube connections and the pneumatic system started functioning properly. 



→ We also encountered some issues in the inflation part of the Arduino code. After correcting the control logic and assigning the proper output pins, the system worked as expected.

    Small code snippet:  
    
```cpp
digitalWrite(PUMP1_PIN, LOW);
digitalWrite(PUMP2_PIN, HIGH);
delay(5000);
```
### Task 3.2 – Integrating the Sensor  
<img width="300" height="300" alt="WhatsApp Image 2026-05-25 at 12 57 53 PM" src="https://github.com/user-attachments/assets/53570289-4e6e-4b70-9f85-e84d075f4ef9" />  

https://github.com/user-attachments/assets/536855be-7b86-49a9-a794-2d6d23c58e7b  

https://github.com/user-attachments/assets/34332c60-f2ad-42d4-a2e3-6a5d991e8092  


    My experience/observation:
→ In this task, we expanded the pneumatic control system by integrating a PIR motion sensor with the Arduino setup.  


→ The motion sensor continuously monitored movement in front of the system. When motion was detected, the Arduino automatically activated the inflation phase by turning ON Pump 2 and closing the valve, causing the air pillow to inflate.  


→ When no motion was detected, the system switched to the deflation phase. Pump 2 turned OFF, the valve opened, and Pump 1 activated to release the air from the system.  


→ We also monitored the system behavior using the Serial Monitor, where messages such as “Motion Detected” and “Area Clear” were displayed according to the sensor readings.  


→ This experiment helped us understand how sensor input can be used to automate pneumatic systems using Arduino and MOSFET-controlled actuators.  

    Small code snippet:
→ This code controls the inflation and deflation behavior based on the PIR motion sensor input.  
```cpp
if (currentMotionState == HIGH) {

  digitalWrite(VALVE_PIN, LOW);
  digitalWrite(PUMP2_PIN, HIGH);

} else {

  digitalWrite(VALVE_PIN, HIGH);
  digitalWrite(PUMP1_PIN, HIGH);
}
```

# Exercise 4: E-Textiles  
 
    Components Used:
→  Conductive thread (copper)  

→  LED 

→  Battery holder 

→  Coin cell battery 

→  Fabric  

→  Sewing needle 

<p align="center">
  <img src="https://github.com/user-attachments/assets/969b94e6-4a53-4d39-9e41-3b86be150af6" width="300">
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/5b9846a6-7707-4b31-ae57-46b5d8cbf537" width="250">
  <img src="https://github.com/user-attachments/assets/01769fd2-6ebc-4df6-bb57-afb9110fda52" width="250">
</p>  
    
    My experience/observation:

→ In this exercise, I created an e-textile project using conductive thread, LEDs, fabric, and a battery holder.  


→ My first design was a flower-shaped fabric with five LEDs. Since sewing was a completely new experience for me, I found it challenging to keep the fabric flat while stitching the conductive thread. As a result, the fabric became wrinkled and compressed, which affected the appearance of the final piece. However, I was pleased that all the LEDs functioned correctly.  


→ To improve the design, I created a second and larger fabric shape. The larger size made sewing easier and helped prevent the fabric from becoming distorted. Initially, I thought the circuit was not working because of a wiring or short-circuit issue, but after troubleshooting, I discovered that the battery had been drained because I had accidentally left it connected for several hours. After replacing the battery, the LEDs worked correctly again.  


→ For my final design, I created a moon-shaped e-textile project, which was both visually cleaner and more reliable. This exercise was a completely new experience for me and helped me learn basic sewing techniques, conductive thread connections, and troubleshooting methods for wearable electronics.  

# Exercise 5: CNC milling  


<p align="center">
  <img src="https://github.com/user-attachments/assets/a4774558-6cc8-43f5-9f0e-4869c4e191f1" width="300">
  <img src="https://github.com/user-attachments/assets/b2b90da8-1a9b-4432-9b3e-14eba5a79928" width="400">
</p>  

    My experience/observation:
→ This exercise introduced me to Inkscape and CNC milling. Since it was my first time using Inkscape, I initially found the software challenging to understand. However, after experimenting with the different tools and following the instructions, I gradually became more comfortable with creating vector shapes and editing designs.  


→ For my design, I created a flower-shaped candle holder. It was interesting to see how a digital sketch could later be converted into toolpaths for CNC machining.  


→ Another highlight of this exercise was seeing a CNC milling machine for the first time. Watching the machine transform a digital design into a physical object was an amazing experience. It helped me understand the connection between digital design and fabrication.  


→ Overall, this exercise was both challenging and enjoyable. It gave me my first experience with vector design software and CNC manufacturing, and I learned a lot about the design-to-production workflow.  

# Exercise 6: Laser Cut Business Cards.  
<p align="center">
  <img src="https://github.com/user-attachments/assets/c11685fa-cb36-4fb6-9a4d-cad69f58b2ba" width="350">
  <img src="https://github.com/user-attachments/assets/fce024ea-e156-4962-b57c-958bf7527602" width="350">
</p>  



https://github.com/user-attachments/assets/e189937a-e3d8-4d1a-8f46-adcc46b99386  





https://github.com/user-attachments/assets/d05fe7b6-2467-442e-b328-1bc181586ede


    My experience/observation:

→ In this exercise, we designed and manufactured a laser-cut business card using Inkscape and a laser cutter. This was the first business card I had ever created, making the experience both interesting and enjoyable.  


→ I designed a simple and clean business card that included my basic contact information, such as my name, phone number, and email address. To make it more useful, I also added a QR code that directly links to my portfolio, allowing anyone to quickly access my work by scanning it with a smartphone.  


→ I first created the design in Inkscape by arranging the layout, text, and vector outlines required for laser cutting. After completing the design, it was sent to the laser cutter, which precisely followed the outlines to cut and engrave the selected material. It was fascinating to see how a digital design was transformed into a physical business card.  


→ I was also surprised by the variety of results that could be achieved using different materials. Even though the designs were similar, the final appearance changed significantly depending on the material used.  


→ During the exercise, I observed that some students experienced problems because the laser cutter could not correctly detect parts of their outlines. As a result, the cutting process stopped before their cards were completed. Fortunately, I did not encounter this issue, and my business card was successfully manufactured on the first attempt. Watching these problems helped me understand the importance of carefully checking vector outlines before laser cutting.  


→ Another exciting part of this exercise was operating a laser cutter for the first time. Watching the machine precisely cut the design was both exciting and enjoyable.  


→ Overall, this exercise improved my Inkscape skills and gave me my first hands-on experience with laser cutting technology.  





# Training Dashboard of CAD Course:  
<img width="1860" height="865" alt="Screenshot 2026-06-21 151046" src="https://github.com/user-attachments/assets/afed59c6-3283-4e1e-ab98-b769d51b5fd1" />






























# Micro:bit Hand Biting Crocodile Tutorial

## 1.Servo

### 1.1 Introduction

Servo is a position control rotary actuator. It mainly consists of a housing, a circuit board, a core-less motor, a gear and a position sensor. Its working principle is that the servo receives the signal sent by MCUs or receivers and produces a reference signal with a period of 20ms and width of 1.5ms, then compares the acquired DC bias voltage to the voltage of the potentiometer and obtains the voltage difference output.

In general, servo has three wires: brown, red and orange. The brown wire is grounded, the red one is a positive pole wire and the orange one is a signal  wire.

![](./media/mb1.png)

The rotation angle of servo is controlled by regulating the duty cycle of PWM (Pulse-Width Modulation) signal. The standard cycle of PWM signal is 20ms (50Hz). Theoretically, the width is distributed between 1ms-2ms, but in fact, it's between 0.5ms-2.5ms. The width corresponds the rotation angle from 0° to 180°. 

![image-20230620134023059](./media/mb2.png)

### 1.2 Specification

Working voltage: DC 3.3V〜5V

Operable angle range: approximately 180° (at 500→2500 μsec)

Pulse width range: 500→2500 μsec

No-load speed: 0.12±0.01 sec/60 (DC 4.8V) 0.1±0.01 sec/60 (DC 6V)

No-load current: 200±20mA (DC 4.8V) 220±20mA (DC 6V)

Stopping torque: 1.3±0.01kg·cm (DC 4.8V) 1.5±0.1kg·cm (DC 6V)

Stop current: ≦850mA (DC 4.8V) ≦1000mA (DC 6V)

Standby current: 3±1mA (DC 4.8V) 4±1mA (DC 6V)

### 1.3 Wiring Diagram

| Expansion Board |    Servo    |
| :-------------: | :---------: |
|       GND       | G（Brown）  |
|       3V3       |  V（Red）   |
|    P1 / io14    | S（Yellow） |

![Servo](./media/mb3.png)

### 1.4 Code

<p style="color:red;">Note: The rotation angle of the servo is 0-180 degrees, but if the crocodile has been assembled, the angle must be rotated between 55-130 degrees, otherwise the servo will get hot and burn out.</p>

**Code File：**

Download link：[Download](./MakeCode/MicrobitBitingCrocodile.zip)

Download the code file and unzip it, then double-click `microbit-1-Servo_Code1.hex `to open the file and upload the code.

![](./media/mb4.png)

**Add code manually：**

1.Tap ![](./media/mb5.png) to add servo library.

![](./media/mb6.png)

2.Input “Servo” and click![](./media/mb7.png) to add Servo library.

![](./media/mb8.png)

3.It is successfully added.

![](./media/mb9..png)

4.Drag ![](./media/mb10.png)into ![](./media/mb11.png)from ![](./media/mb12.png)，and set the pin to P1 and Angle to 55 °.![](./media/mb13.png)

5.Drag![](./media/mb14.png)from ![](./media/mb15.png) and place it under the ![](./media/mb16.png)，and set the delay to 1000ms.

![](./media/mb17.png)

6.Repeat steps 4 and 5 to add the code blocks to set the servo to 90 °  and 110 ° with a delay of 1000ms.

**Complete Code：**

![](./media/mb18.png)



### 1.5 Test Result

After uploading the code, the crocodile will open its mouth for 1s, then close half of its mouth for 1s, and then completely close its mouth. 

### 1.6 Extended Tutorial

Earlier we have controlled the crocodile to open and close its mouth at a wide angle, so how to control the crocodile to slowly close and open its mouth?

#### 1.6.1 Code

**Code File：**

Download link：[Download](./MakeCode/MicrobitBitingCrocodile.zip)

Download the code file and unzip it, then double-click `microbit-1-Servo_Code2.hex`to open the file and upload the code.

![](./media/mb19.png)

**Add code manually：**

1.Click![](./media/mb20.png) in ![](./media/mb21.png) and add a variable named value.

![](./media/mb22.png)

2.Drag![](./media/mb23.png)from ![](./media/mb21.png)into![](./media/mb24.png)，and set the value to 55 in the white box.

![](./media/mb25.png)

3.Drag![](./media/mb26.png)from ![](./media/mb27.png) into![mb11](./media/mb11.png)，and set the repeat times in the white box to 55.

![](./media/mb28.png)

4.Drag![](./media/mb29.png)from ![mb21](./media/mb21.png)into![image-20240411140012957](./media/mb30.png).

![](./media/md31.png)

5.Drag![image-20240411134928930](./media/mb12.png) and from![image-20240411135053755](./media/mb10.png) place it under the![image-20240411134815736](./media/mb29.png)，and set pin to P1.

![image-20240411140622035](./media/mb32.png)

6.Drag![image-20240411140703032](./media/mb54.png)from ![mb21](./media/mb21.png)and place it in the in the white box of  ![image-20240411140727409](./media/mb33.png).

![image-20240411140801321](./media/image-20240411140801321.png)

7.Drag![image-20240411135225827](./media/mb14.png)from ![image-20240411135120617](./media/mb15.png) and place it under the ![image-20240411140848252](./media/mb34.png)，and set the delay to 30ms.

![image-20240411140905994](./media/mb35.png)

9.Right-click![image-20240411140012957](./media/mb30.png)and tap Duplicate”.

![image-20240411140946657](./media/mb36.png)

10.Add the copied code block below ![image-20240411141156778](./media/mb37.png)，then modify  "1" in the white box of ![image-20240411134815736](./media/mb29.png) to "-1".

![image-20240411141318351](./media/mb38.png)

**Complete Code：**

![image-20240411133752416](./media/mb39.png)

#### 1.6.2 Test Result

After uploading the code, the crocodile will slowly open its mouth and then slowly close it.

## 2.Ultrasonic Module

### 2.1 Introduction

The HC-SR04 ultrasonic sensor uses sonar to determine distance to an object like what bats do. It offers excellent non-contact range detection with high accuracy and stable readings in an easy-to-use package. It comes with an ultrasonic transmitter and a receiver.

It is being used in a wide range of electronics projects for creating obstacle detection and distance measuring application as well as various other applications.

### 2.2 Specification

Working voltage:3.3-5V 

Quiescent current: <2mA

Working current: 15mA

Effective angle: <15°

Distance range: 2cm – 400 cm

Accuracy: 0.3 cm

Measuring angle: 30 degrees

Trigger input pulse width: 10 microseconds



![wps3-1687242720835-4](./media/md40.png)

### 2.3 Wiring Diagram

| Expansion Board | Module |
| :-------------: | :----: |
|       GND       |   G    |
|       3V3       |   V    |
|    P8 / io4     |  Trig  |
|   P12 / io15    |  Echo  |

![ultrasonic](./media/mb40.png)

### 2.4 Code

<p style="color:red">Note: The measuring distance of ultrasonic is 2-300cm, but after being assembled on the crocodile, it can only detect 4-30cm. For the ultrasonic receives the bounced signal at a certain angle, but the basswood board of the crocodile body blocks it. As a result, only 30cm can be recognized, but this does not affect our hand biting crocodile tutorial.</p>

**Code File：**

Download link：[Download](./MakeCode/MicrobitBitingCrocodile.zip)

Download the code file and unzip it, then double-click `microbit-2-Ultrasonic_Code.hex`to open the file and upload the code.

![image-20240412082118573](./media/mb41.png)

**Add code manually：**

1.Tap![image-20240411141436376](./media/mb5.png)to add sonar library.

![image-20240411131330336](./media/mb6.png)

2.Input “sonar”and click![image-20240411131603613](./media/mb7.png)to add sonar library.

![image-20240411151421395](./media/mb42.png)

3.The sonar library is added.

![image-20240411151559812](./media/mb43.png)

4.Drag![image-20240411151657614](./media/mb44.png)from ![image-20240411151634760](./media/mb45.png)into ![mb24](./media/mb24.png).

![image-20240411151752157](./media/mb46.png)

5.Click![image-20240411135444604](./media/mb20.png) in ![mb21](./media/mb21.png) and add a variable named value.

![image-20240411135607139](./media/mb22.png)

6.Drag![mb23](./media/mb23.png)from ![mb21](./media/mb21.png)into![mb11](./media/mb11.png).

![image-20240411152209708](./media/mb47.png)

7.Drag![image-20240411152100056](./media/mb48.png)from ![image-20240411152033812](./media/mb49.png) into the white box of ![mb23](./media/mb23.png)，and set trig to P8 pin, echo to P12 pin, unit to CM.![image-20240411152339265](./media/mb50.png)

8.Drag![image-20240411152425981](./media/mb51.png)from ![image-20240411151634760](./media/mb45.png) and place it under the ![image-20240411152456476](./media/mb52.png)，and modify the character in the first white box to "distance=".

![image-20240411152553210](./media/mb53.png)

9.Drag![image-20240411140703032](./media/mb54.png)from ![mb21](./media/mb21.png)and place it into the second white box of![image-20240411152717631](./media/mb55.png).

![image-20240411152816974](./media/mb56.png)

10.Drag![image-20240411135225827](./media/mb14.png)from ![image-20240411135120617](./media/mb15.png)and place it under the ![image-20240411152957623](./media/mb57.png)，and modify the delay to 500ms.



**Complete Code：**

![image-20240411155438811](./media/mb58.png)

### 2.5 Test Result

If you cannot print data in the browser's makecode compilation interface, use CoolTerm software. Details are in the micro bit basic tutorial.

After uploading the code, open the CoolTerm software, click Options, select SerialPort, set the COM port and baud rate to 115200 (after testing, the USB serial communication baud rate of the micro:bit board is 115200), then click OK and Connect.

![image-20240411161642015](./media/mb59.png)

After the setting is completed, we can see the distance sensed by the ultrasonic in the serial port printing area. The serial port printing distance will be printed every 0.5s.

![image-20240411155421424](./media/mb60.png)

## 3.Buttons Control the Crocodile 

### 3.1 Introduction

In this project, we work to control the crocodile to open and close its mouth through the AB buttons on the microbit.

### 3.2 Code

**Code File：**

Download link：[Download](./MakeCode/MicrobitBitingCrocodile.zip)

Download the code file and unzip it, then double-click `microbit-3-Key_controlled_crocodile_Code .hex` to open the file and upload the code.

![image-20240412082159608](./media/mb61.png)

**Add code manually：**

1.Add servo library  then drag![image-20240411134928930](./media/mb12.png)from ![image-20240411135053755](./media/mb10.png)and place it into![mb24](./media/mb24.png)，and set the pin to P1 and the angle to 110°.

![image-20240411163021847](./media/mb62.png)

2.Drag![image-20240411163118548](./media/mb63.png)from ![image-20240411135120617](./media/mb15.png)and place it into![mb24](./media/mb24.png)，and set the dot matrix to display![mb64](./media/mb64.png).

![image-20240411163213565](./media/mb65.png)

3.Drag![image-20240411163257914](./media/mb66.png)from ![image-20240411163233958](./media/mb67.png), then add the set servo to 55 ° code and the dot matrix displays![mb68](./media/mb68.png)code.

![image-20240411163431960](./media/mb69.png)

4.Copy![image-20240411163257914](./media/mb66.png)and alter button to B，then set servo angle to 110°，dot matrix displays![mb64](./media/mb64.png).

![image-20240411163540280](./media/mb70.png)

**Complete Code：**

![image-20240411162817429](./media/mb71.png)

### 3.3 Test Result

After the code is uploaded successfully, press the button A and the crocodile will display ![mb68](./media/mb68.png)and close its mouth. Press the button B and the crocodile will display![mb64](./media/mb64.png)and open its mouth. 

## 4.Hand Biting Crocodile

### 4.1 Introduction

The crocodile opens its mouth. When you put your hand into the crocodile's mouth, the ultrasonic on the crocodile will measure the depth of your hand into the crocodile's mouth. When it reaches the depth we set, the crocodile will bite.

### 4.2 Code

**Code File：**

Download link：[Download](./MakeCode/MicrobitBitingCrocodile.zip)

Download the code file and unzip it, then double-click `microbit-4-Crocodile_Bite_Code.hex ` to open the file and upload the code.

![image-20240412082245262](./media/mb72.png)

**Add code manually：**

1.Add the servo library and the ultrasonic library, and generate variables "distance" and "value".

2.Add ![image-20240416104740404](./media/mb73.png)into![mb24](./media/mb24.png).

![image-20240411165204056](./media/mb74.png)

2.Add![mb23](./media/mb23.png)into![mb11](./media/mb11.png)，and set variable to ‘distance’.

![image-20240411165357924](./media/mb75.png)

3.Add![image-20240411152100056](./media/mb48.png)into![image-20240411165525534](./media/mb76.png)，and set trig to P8 pin, echo to P12 pin, unit to CM.

![image-20240411165615989](./media/mb77.png)

4.Drag![mb78](./media/mb78.png)from ![mb79](./media/mb79.png)and place it under the ![image-20240411165759723](./media/mb80.png).

![image-20240411165825260](./media/mb81.png)

5.Drag![mb82](./media/mb82.png)from ![mb79](./media/mb79.png)and place it under the diamond box of ![mb78](./media/mb78.png).

![image-20240411170008163](./media/mb83.png)

6.Add![image-20240411170057223](./media/mb84.png)to the left box of ![mb82](./media/mb82.png)，![image-20240411170134627](./media/mb85.png)to the right box of![mb82](./media/mb82.png)；distance < value.

![image-20240411170236525](./media/mb86.png)

7.Add![mb23](./media/mb23.png)into ![image-20240411170420122](./media/mb87.png).

![image-20240411170539546](./media/mb88.png)

8.Drag![image-20240411170616999](./media/mb89.png)from ![image-20240411170603994](./media/mb90.png)into![mb23](./media/mb23.png)，and set the value to 3 to 8.

![image-20240411170718826](./media/mb91.png)

9.Add code in![image-20240411171045550](./media/mb92.png)，first, set the servo to 55°，dot matrix displays ![mb68](./media/mb68.png)，and delays 3s，then set the servo to 110°，dot matrix displays![mb64](./media/mb64.png)and delays 1s.

**Complete Code：**

![image-20240411164726559](./media/mb93.png)

### 4.3 Test Result

After the code is successfully uploaded, the crocodile opens its mouth, and the dot matrix displays![mb64](./media/mb64.png). When the distance between the hand and the ultrasonic meets the crocodile's bite conditions, the crocodile bites and the dot matrix displays ![mb68](./media/mb68.png). The crocodile releases its mouth after 3s of bite.  and the dot matrix displays![mb64](./media/mb64.png), the final 1s delay is to prepare for retracting the hand from the crocodile's mouth. After 1s, it enters the next hand-biting process.






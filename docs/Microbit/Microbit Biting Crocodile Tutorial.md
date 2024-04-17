# Hand Biting Crocodile

## 1.Servo

1.1 Introduction

Servo is a position control rotary actuator. It mainly consists of a housing, a circuit board, a core-less motor, a gear and a position sensor. Its working principle is that the servo receives the signal sent by MCUs or receivers and produces a reference signal with a period of 20ms and width of 1.5ms, then compares the acquired DC bias voltage to the voltage of the potentiometer and obtains the voltage difference output.

In general, servo has three wires: brown, red and orange. The brown wire is grounded, the red one is a positive pole wire and the orange one is a signal  wire.

![wps2-1687239587616-2](./media/8532a19f46ac138b6e7ef575a029cf2d.jpg)

The rotation angle of servo is controlled by regulating the duty cycle of PWM (Pulse-Width Modulation) signal. The standard cycle of PWM signal is 20ms (50Hz). Theoretically, the width is distributed between 1ms-2ms, but in fact, it's between 0.5ms-2.5ms. The width corresponds the rotation angle from 0° to 180°. 

![image-20230620134023059](./media/19164a1535c9e77a8e478c4d67d6d464.png)

1.2 Specification

Working voltage: DC 3.3V〜5V

Operable angle range: approximately 180° (at 500→2500 μsec)

Pulse width range: 500→2500 μsec

No-load speed: 0.12±0.01 sec/60 (DC 4.8V) 0.1±0.01 sec/60 (DC 6V)

No-load current: 200±20mA (DC 4.8V) 220±20mA (DC 6V)

Stopping torque: 1.3±0.01kg·cm (DC 4.8V) 1.5±0.1kg·cm (DC 6V)

Stop current: ≦850mA (DC 4.8V) ≦1000mA (DC 6V)

Standby current: 3±1mA (DC 4.8V) 4±1mA (DC 6V)

1.3 Wiring Diagram

| Expansion Board |    Servo    |
| :-------------: | :---------: |
|       GND       | G（Brown）  |
|       3V3       |  V（Red）   |
|    P1 / io14    | S（Yellow） |

![Servo](./media/d53df572132d02ae81dd782d76714163.png)

1.4 Code

<p style="color:red;">Note: The rotation angle of the servo is 0-180 degrees, but if the crocodile has been assembled, the angle must be rotated between 55-130 degrees, otherwise the servo will get hot and burn out.</p>

**Code File：**

Download link：[Download](.\MakeCode\MicrobitBitingCrocodile.zip)

Download the code file and unzip it, then double-click `microbit-1-Servo_Code1.hex `to open the file and upload the code.

![image-20240412081907926](./media/4ab2025eb99fece901650acb4acfd6cb.png)

**Add code manually：**

1.Tap ![image-20240411141436376](./media/d891e4a4266e7cba341cd5f05faba949.png) to add servo library.

![image-20240411131330336](./media/eb3eb6714285cea1d2622c0a33473861.png)

2.Input “Servo” and click![image-20240411131603613](./media/b63121249bc10d1f2a801590eb1ff545.png) to add Servo library.

![image-20240411131510219](./media/376dc2e32d37cecdb2b32a453bfe91d9.png)

3.It is successfully added.

![image-20240411131709253](./media/475d6a3a0e95e5093578815bc3a2c456.png)

4.Drag ![image-20240411134928930](./media/e34514407bdaa5e797e7fb56ee865899.png)into ![image-20240411134958837](./media/4a2b5f2d0205b2887fcca1faa86d78f6.png)from ![image-20240411135053755](./media/cae63144d999699c97ccfec4529a0819.png)，and set the pin to P1 and Angle to 55 °.![image-20240411132040159](./media/62ce0d13aa3222d89264950441a334de.png)

5.Drag![image-20240411135225827](./media/509c1994e221bdc2c080fcaeab14d45a.png)from ![image-20240411135120617](./media/3a5fdc4db0f5eaa5fd6059afd1fff6aa.png) and place it under the ![image-20240411135208381](./media/6d10a45e86dda7267739a31b9bd2aae2.png)，and set the delay to 1000ms.

![image-20240411132624453](./media/56abb3d451a793d6867c3c150f07024d.png)

6.Repeat steps 4 and 5 to add the code blocks to set the servo to 90 °  and 110 ° with a delay of 1000ms.

**Complete Code：**

![image-20240411132800003](./media/e6d983333de62c87238df846e7aa1088.png)



1.5 Test Result

After uploading the code, the crocodile will open its mouth for 1s, then close half of its mouth for 1s, and then completely close its mouth. 

1.6 Extended Tutorial

Earlier we have controlled the crocodile to open and close its mouth at a wide angle, so how to control the crocodile to slowly close and open its mouth?

1.6.1 Code

**Code File：**

Download link：[Download](.\MakeCode\MicrobitBitingCrocodile.zip)

Download the code file and unzip it, then double-click `microbit-1-Servo_Code2.hex`to open the file and upload the code.

![image-20240412082022570](./media/d83a0353a34834c13f54adb802f37f0b.png)

**Add code manually：**

1.Click![image-20240411135444604](./media/f4fe646353fb6d6e44352c227cd4b380.png) in ![image-20240411135423166](./media/b7e60bce1e9efcabf6fcf29418016bb9.png) and add a variable named value.

![image-20240411135607139](./media/e58157f8cd6325eb0e1aa1c4b9833d80.png)

2.Drag![image-20240411135741919](./media/6ce121293517e523528f094d5c37c8a7.png)from ![image-20240411135423166](./media/b7e60bce1e9efcabf6fcf29418016bb9.png)into![image-20240411135755058](./media/feee7d3b9f470b62f6ab6061c72cf87e.png)，and set the value to 55 in the white box.

![image-20240411134206938](./media/b9b4bd79375dcebb8f223a50baf46e0c.png)

3.Drag![image-20240411135850882](./media/5842031640e92466239b02ba666736e6.png)from ![image-20240411135834409](./media/5fe4e169ad2e53135494eab4b21d05d5.png) into![image-20240411134958837](./media/4a2b5f2d0205b2887fcca1faa86d78f6.png)，and set the repeat times in the white box to 55.

![image-20240411134329133](./media/106dd452c7139204527066cc4a7d6367.png)

4.Drag![image-20240411134815736](./media/98e033b73371c648fb142f38e454b025.png)from ![image-20240411135423166](./media/b7e60bce1e9efcabf6fcf29418016bb9.png)into![image-20240411140012957](./media/8c06923d7f1f0721b96b4ab0deb8c8e3.png).

![image-20240411134555038](./media/719562a592dbaa6a21e7496f98bf2eb0.png)

5.Drag![image-20240411134928930](./media/e34514407bdaa5e797e7fb56ee865899.png) and from![image-20240411135053755](./media/cae63144d999699c97ccfec4529a0819.png) place it under the![image-20240411134815736](./media/98e033b73371c648fb142f38e454b025.png)，and set pin to P1.

![image-20240411140622035](./media/e21857c3c0a0aee9911595653e6419e3.png)

6.Drag![image-20240411140703032](./media/1ff8dba8c5e90bf6d705b61977ff5820.png)from ![image-20240411135423166](./media/b7e60bce1e9efcabf6fcf29418016bb9.png)and place it in the in the white box of  ![image-20240411140727409](./media/98408b18af81b40af76d32b179b3caa6.png).

![image-20240411140801321](./media/d5cdf2699dad0403aa3cbf454270499b.png)

7.Drag![image-20240411135225827](./media/509c1994e221bdc2c080fcaeab14d45a.png)from ![image-20240411135120617](./media/3a5fdc4db0f5eaa5fd6059afd1fff6aa.png) and place it under the ![image-20240411140848252](./media/1f680e1caff05d069a44882649fa849e.png)，and set the delay to 30ms.

![image-20240411140905994](./media/bd1747844cfb0455de2a76e64c939885.png)

9.Right-click![image-20240411140012957](./media/8c06923d7f1f0721b96b4ab0deb8c8e3.png)and tap Duplicate”.

![image-20240411140946657](./media/17580a401d009bf01543d15c5dc0dd1f.png)

10.Add the copied code block below ![image-20240411141156778](./media/a2c037d7a150fc45fd1f56ef8c8299d4.png)，then modify  "1" in the white box of ![image-20240411134815736](./media/98e033b73371c648fb142f38e454b025.png) to "-1".

![image-20240411141318351](./media/6c0af7bb20618e3a723aa58f4d89cb15.png)

**Complete Code：**

![image-20240411133752416](./media/650b92ed3dabae360ce0c3997e4cca0a.png)

1.6.2 Test Result

After uploading the code, the crocodile will slowly open its mouth and then slowly close it.

## 2.Ultrasonic Module

2.1 Introduction

The HC-SR04 ultrasonic sensor uses sonar to determine distance to an object like what bats do. It offers excellent non-contact range detection with high accuracy and stable readings in an easy-to-use package. It comes with an ultrasonic transmitter and a receiver.

It is being used in a wide range of electronics projects for creating obstacle detection and distance measuring application as well as various other applications.

2.2 Specification

Working voltage:3.3-5V 

Quiescent current: <2mA

Working current: 15mA

Effective angle: <15°

Distance range: 2cm – 400 cm

Accuracy: 0.3 cm

Measuring angle: 30 degrees

Trigger input pulse width: 10 microseconds



![wps3-1687242720835-4](./media/43ce3e4b06901e3c7d0848770b4e66e3.jpg)

2.3 Wiring Diagram

| Expansion Board | Module |
| :-------------: | :----: |
|       GND       |   G    |
|       3V3       |   V    |
|    P8 / io4     |  Trig  |
|   P12 / io15    |  Echo  |

![ultrasonic](./media/9a5cbc79a4a3a8146ab5e936138480ce.png)

2.4 Code

<p style="color:red">Note: The measuring distance of ultrasonic is 2-300cm, but after being assembled on the crocodile, it can only detect 4-30cm. For the ultrasonic receives the bounced signal at a certain angle, but the basswood board of the crocodile body blocks it. As a result, only 30cm can be recognized, but this does not affect our hand biting crocodile tutorial.</p>

**Code File：**

Download link：[Download](.\MakeCode\MicrobitBitingCrocodile.zip)

Download the code file and unzip it, then double-click `microbit-2-Ultrasonic_Code.hex`to open the file and upload the code.

![image-20240412082118573](./media/1eaa0e4ff2158c482efe05bcce4f5dd8.png)

**Add code manually：**

1.Tap![image-20240411141436376](./media/d891e4a4266e7cba341cd5f05faba949.png)to add sonar library.

![image-20240411131330336](./media/eb3eb6714285cea1d2622c0a33473861.png)

2.Input “sonar”and click![image-20240411131603613](./media/b63121249bc10d1f2a801590eb1ff545.png)to add sonar library.

![image-20240411151421395](./media/20784ae68df1299d3bffb8f3db8dc246.png)

3.The sonar library is added.

![image-20240411151559812](./media/35ca336bdff2c739c68a028822ba655e.png)

4.Drag![image-20240411151657614](./media/77741dbaecdbf6f8b7ef9e7c048d95c8.png)from ![image-20240411151634760](./media/a33ffd3f5adaf9ef6c4096c01d2e3d84.png)into ![image-20240411135755058](./media/feee7d3b9f470b62f6ab6061c72cf87e.png).

![image-20240411151752157](./media/79aa04747c2c12e95049ad62804b112f.png)

5.Click![image-20240411135444604](./media/f4fe646353fb6d6e44352c227cd4b380.png) in ![image-20240411135423166](./media/b7e60bce1e9efcabf6fcf29418016bb9.png) and add a variable named value.

![image-20240411135607139](./media/e58157f8cd6325eb0e1aa1c4b9833d80.png)

6.Drag![image-20240411135741919](./media/6ce121293517e523528f094d5c37c8a7.png)from ![image-20240411135423166](./media/b7e60bce1e9efcabf6fcf29418016bb9.png)into![image-20240411134958837](./media/4a2b5f2d0205b2887fcca1faa86d78f6.png).

![image-20240411152209708](./media/5964dee6821b41eb248d4a3240d1e6e4.png)

7.Drag![image-20240411152100056](./media/e902a0ccca65d21918ead217941cb2db.png)from ![image-20240411152033812](./media/77a03bf0ff8548df73e3fa651f29a0d8.png) into the white box of ![image-20240411135741919](./media/6ce121293517e523528f094d5c37c8a7.png)，and set trig to P8 pin, echo to P12 pin, unit to CM.![image-20240411152339265](./media/b1dcc44ea7d3675f59e3908c54d90d75.png)

8.Drag![image-20240411152425981](./media/16a80310daa9a85274bfd16635be6366.png)from ![image-20240411151634760](./media/a33ffd3f5adaf9ef6c4096c01d2e3d84.png) and place it under the ![image-20240411152456476](./media/96704d3db5bc3ce2042e03fcfc6195ca.png)，and modify the character in the first white box to "distance=".

![image-20240411152553210](./media/0f8e83c1e023a986d1d43908c8992294.png)

9.Drag![image-20240411140703032](./media/1ff8dba8c5e90bf6d705b61977ff5820.png)from ![image-20240411135423166](./media/b7e60bce1e9efcabf6fcf29418016bb9.png)and place it into the second white box of![image-20240411152717631](./media/cb043f37a1ec827ff9ee9b677922a800.png).

![image-20240411152816974](./media/8b37222ecaf43028a16a664d52c69f6a.png)

10.Drag![image-20240411135225827](./media/509c1994e221bdc2c080fcaeab14d45a.png)from ![image-20240411135120617](./media/3a5fdc4db0f5eaa5fd6059afd1fff6aa.png)and place it under the ![image-20240411152957623](./media/982b8d70f9ee968af3619d40a8e5f37e.png)，and modify the delay to 500ms.



**Complete Code：**

![image-20240411155438811](./media/19c5d11ac943f2eb6581332015920d36.png)

2.5 Test Result

If you cannot print data in the browser's makecode compilation interface, use CoolTerm software. Details are in the micro bit basic tutorial.

After uploading the code, open the CoolTerm software, click Options, select SerialPort, set the COM port and baud rate to 115200 (after testing, the USB serial communication baud rate of the micro:bit board is 115200), then click OK and Connect.

![image-20240411161642015](./media/074f9190ad9c291d2ea3a61ec8f68ef2.png)

After the setting is completed, we can see the distance sensed by the ultrasonic in the serial port printing area. The serial port printing distance will be printed every 0.5s.

![image-20240411155421424](./media/10e24fa5330b3d97c14f7dcde69fe123.png)

## 3.Buttons Control the Crocodile 

3.1 Introduction

In this project, we work to control the crocodile to open and close its mouth through the AB buttons on the microbit.

3.2 Code

**Code File：**

Download link：[Download](.\MakeCode\MicrobitBitingCrocodile.zip)

Download the code file and unzip it, then double-click `microbit-3-Key_controlled_crocodile_Code .hex` to open the file and upload the code.

![image-20240412082159608](./media/b4d5b63a1797c61e7ee89ca8ed458351.png)

**Add code manually：**

1.Add servo library  then drag![image-20240411134928930](./media/e34514407bdaa5e797e7fb56ee865899.png)from ![image-20240411135053755](./media/cae63144d999699c97ccfec4529a0819.png)and place it into![image-20240411135755058](./media/feee7d3b9f470b62f6ab6061c72cf87e.png)，and set the pin to P1 and the angle to 110°.

![image-20240411163021847](./media/9af5927e320a0fd77daee8c8c8e835ca.png)

2.Drag![image-20240411163118548](./media/39436bdf11142fcdd68f37be494d1277.png)from ![image-20240411135120617](./media/3a5fdc4db0f5eaa5fd6059afd1fff6aa.png)and place it into![image-20240411135755058](./media/feee7d3b9f470b62f6ab6061c72cf87e.png)，and set the dot matrix to display![image-20240411163149067](./media/af54276130edfd1376f43f1a50fd77ea.png).

![image-20240411163213565](./media/78557784dfaaa594ba34baa0d6577ca5.png)

3.Drag![image-20240411163257914](./media/ad199218a46d2e81cc47175f7fb1efb9.png)from ![image-20240411163233958](./media/54cd51e4a273b1f1ac0fe85d103381cc.png), then add the set servo to 55 ° code and the dot matrix displays![image-20240411163415776](./media/9296f4bbe0c5bf7cbc9a58fc0098795c.png)code.

![image-20240411163431960](./media/e7d73a3a5741862045bdbd01915b0d8b.png)

4.Copy![image-20240411163257914](./media/ad199218a46d2e81cc47175f7fb1efb9.png)and alter button to B，then set servo angle to 110°，dot matrix displays![image-20240411163149067](./media/af54276130edfd1376f43f1a50fd77ea.png).

![image-20240411163540280](./media/eb0743e245941dc1d85de6305b5c1c56.png)

**Complete Code：**

![image-20240411162817429](./media/99636a7c58685f94625938f955ad98d8.png)

3.3 Test Result

After the code is uploaded successfully, press the button A and the crocodile will display ![image-20240411163415776](./media/9296f4bbe0c5bf7cbc9a58fc0098795c.png)and close its mouth. Press the button B and the crocodile will display![image-20240411163149067](./media/af54276130edfd1376f43f1a50fd77ea.png)and open its mouth. 

## 4.Hand Biting Crocodile

4.1 Introduction

The crocodile opens its mouth. When you put your hand into the crocodile's mouth, the ultrasonic on the crocodile will measure the depth of your hand into the crocodile's mouth. When it reaches the depth we set, the crocodile will bite.

4.2 Code

**Code File：**

Download link：[Download](.\MakeCode\MicrobitBitingCrocodile.zip)

Download the code file and unzip it, then double-click `microbit-4-Crocodile_Bite_Code.hex ` to open the file and upload the code.

![image-20240412082245262](./media/28de0b5f15e6f07bca06384859f17e88.png)

**Add code manually：**

1.Add the servo library and the ultrasonic library, and generate variables "distance" and "value".

2.Add ![image-20240416104740404](media/7f7ef96597076d351ba4a501ce9b66fc.png)into![image-20240411135755058](./media/feee7d3b9f470b62f6ab6061c72cf87e.png).

![image-20240411165204056](./media/ab2fa177e44db1459dc3a247e6faede9.png)

2.Add![image-20240411135741919](./media/6ce121293517e523528f094d5c37c8a7.png)into![image-20240411134958837](./media/4a2b5f2d0205b2887fcca1faa86d78f6.png)，and set variable to ‘distance’.

![image-20240411165357924](./media/f0e930ce249fdfebf6fb02d6fdc9d677.png)

3.Add![image-20240411152100056](./media/e902a0ccca65d21918ead217941cb2db.png)into![image-20240411165525534](./media/a521090a7369f879c21dc569b23d08fa.png)，and set trig to P8 pin, echo to P12 pin, unit to CM.

![image-20240411165615989](./media/9f19209f4d4189277724b3611b943171.png)

4.Drag![image-20240411165722484](./media/947567c7d78e72ce485e9f56896dc774.png)from ![image-20240411165643724](./media/a22dfb861ac6a7d69beff361198b6491.png)and place it under the ![image-20240411165759723](./media/70a00807ce0e7b5175f0eced1c2d37d8.png).

![image-20240411165825260](./media/a7dbac06674ff3f82abb7563ed0afe25.png)

5.Drag![image-20240411165906274](./media/0d8b3229e5db2d99ac1ace45d3a49d98.png)from ![image-20240411165643724](./media/a22dfb861ac6a7d69beff361198b6491.png)and place it under the diamond box of ![image-20240411165722484](./media/947567c7d78e72ce485e9f56896dc774.png).

![image-20240411170008163](./media/24f55e1da98ddf950bf2dc8ee839e0bf.png)

6.Add![image-20240411170057223](./media/7fdcae10714008ecb1170ab03541d569.png)to the left box of ![image-20240411165906274](./media/0d8b3229e5db2d99ac1ace45d3a49d98.png)，![image-20240411170134627](./media/60556977be16ba369145d28f27e38551.png)to the right box of![image-20240411165906274](./media/0d8b3229e5db2d99ac1ace45d3a49d98.png)；distance < value.

![image-20240411170236525](./media/94b08eec91eb37655707203762af7bb1.png)

7.Add![image-20240411135741919](./media/6ce121293517e523528f094d5c37c8a7.png)into ![image-20240411170420122](./media/e594343a9d7bb3432498f980be5066ae.png).

![image-20240411170539546](./0a5c8e16dac5242714d92abf02b39b24.png)

8.Drag![image-20240411170616999](./media/4a6633a4eedba5f41adaa766d2923e15.png)from ![image-20240411170603994](./media/3732725f339fc317d1a654d6ccd9e542.png)into![image-20240411135741919](./media/6ce121293517e523528f094d5c37c8a7.png)，and set the value to 3 to 8.

![image-20240411170718826](./media/17adef3d73f632b2f7950f72c76127ff.png)

9.Add code in![image-20240411171045550](./media/ae91c57a47ddab210e1ab71e025235bc.png)，first, set the servo to 55°，dot matrix displays ![image-20240411163415776](./media/9296f4bbe0c5bf7cbc9a58fc0098795c.png)，and delays 3s，then set the servo to 110°，dot matrix displays![image-20240411163149067](./media/af54276130edfd1376f43f1a50fd77ea.png)and delays 1s.

**Complete Code：**

![image-20240411164726559](./media/46cf2fee3611bbd5d95227810730a2e5.png)

4.3 Test Result

After the code is successfully uploaded, the crocodile opens its mouth, and the RGB dot matrix displays a green smile. When the distance between the hand and the ultrasonic meets the crocodile's bite conditions, the crocodile bites and the RGB dot matrix displays a red crying face. The crocodile releases its mouth after 3s of bite. And the RGB dot matrix displays a green smiley face, the final 1s delay is to prepare for retracting the hand from the crocodile's mouth. After 1s, it enters the next hand-biting process.






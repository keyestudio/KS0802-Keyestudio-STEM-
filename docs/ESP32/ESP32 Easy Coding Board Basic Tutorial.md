# ESP32 Easy Coding Board Basic Tutorial

## 1.Development Board

Link：<http://keyestudio-ks5018.readthedocs.io/>

## 2.Kidsblock Software

### 1.1 Installation

#### **Windows System：**

1. Download

   - Download link：[http://xiazai.keyesrobot.cn/KidsBlock.exe](http://xiazai.keyesrobot.cn/KidsBlock.exe)

     

2. After downloading, click  “KidsBlock.exe”![img](./media/an1-1712639258554-18.png)to open it.

3. Tap “**Anyone who uses this computer(all users)**” and “**Next**”.

![](./media/an2-1712639112358-1-1712639258554-19.png)

4. Click “**Browse…**” to choose an installation path of the software, and click “**Install**”.


![img](./media/an3-1712639258554-20.png)

![img](./media/an4-1712639258554-21.png)

5. Click “Finish”.

![img](./media/an5-1712639258554-22.png)

6. If there is a warning on your computer, just click “**Allow access**” to enter the software.

![img](./media/an6-1712639123997-3-1712639258554-23.png)

------



#### MacOS System：

1. Download Kidsblock package： [http://xiazai.keyesrobot.cn/KidsBlock.dmg](http://xiazai.keyesrobot.cn/KidsBlock.dmg)

![img](./media/an7-1712639258554-24.png)

2. After downloading, click **KidsBlock**. And then drag the **KidsBlock Desktop** into **Applications**.

![img](./media/an8-1712639258554-25.png)

3. After installation, you can see the icon of KidsBlock.

   ![img](./media/an9-1712639138551-5-1712639258554-26.png)

4. Open KidsBlock, but it cannot be opened, because Mac devices only allow us to open apps from its App store by default. Thus, we  need to modify some settings. 

   ![img](./media/an9-1-1712639148510-7-1712639258554-27.png)

5. Open settings and enter **Privacy&Security**, tick **App Store and identified developers** in **Security**. And then click **Open Anyway**.

   ![img](./media/an9-2-1712639151503-9-1712639258554-28.png)

6. Click **Open** and the software can be opened.

   ![img](./media/an9-3-1712639154395-11-1712639258554-29.png)

7. Now re-open the Kidsblock.

   ![img](./media/an9-4-1712639157086-13-1712639258554-30.png)

8. Now enjoy your programming!

   ![img](./media/an9-5-1712639160901-15-1712639258554-31.png)

------



### 1.2 Using Tutorial

（**We demonstrate on Windows, and MacOS users may take it as a reference.**）

#### kidsblock Main Interface 1：

![img](./media/an10-1712639258554-32.png)

------



#### Language

Click![img](./media/an11-1712639258555-33.png)to shift languages.

![image-20240409130921782](./media/image-20240409130921782.png)

------



#### Device Driver

**If the driver is already installed on the computer, you do not need to install it again. If not, you need to do the following.**

Click![img](./media/an13-1712639258555-35.png)to choose “**Install driver**”.


![img](./media/an14-1712639258555-36.png)

- Enter **Device Driver Installation Wizard** and click “**Next**”.

![img](./media/an15-1712639258555-37.png)

- Click “**Finish**”.

![img](./media/an16-1712639258555-38.png)

- Click “**Next**”.

![img](./media/an17-1712639258555-39.png)

- Click “**Finish**”.

![img](./media/an18-1712639258555-40.png)

- If a warning appears, just click “**Allow**” and “**Install**”.

![img](./media/an19-1712639258555-41.png)

- Click “**Finish**”.

![img](./media/an20-1712639258555-42.png)

- Click “**Extract**”.

![img](./media/an21-1712639258555-43.png)

- Click “**Next**”.

![img](./media/an22-1712639258555-44.png)

- Click “**I accept this agreement**” and “**Next**”.

![img](./media/an23-1712639258555-45.png)

- Click “**Finish**”.

![img](./media/an24-1712639258555-46.png)

- Click “**INSTALL**”.

![img](./media/an25-1712639258555-47.png)

- Click “**OK**”.

![img](./media/an26-1712639258555-48.png)

------

#### Development Board

##### Connect a board and a port:

- Click![img](./media/an27-1712639258555-49.png)to choose a device.

- Click **Kit** and find **ESP32 Easy Coding Board** to load it. Required sensors and modules are included in it, so you do not need to load them one by one.

  ![img](./media/an28-1712639258555-50.png)

- The following interface will appear, and we need to choose the correct port and click **Connect**.

  ![img](./media/an29-1712639258555-51.png)

- Click **Go to Editor**

  ![img](./media/an30-1712639258555-52.png)

- Main interface:

  ![img](./media/an31-1712639258555-53.png)

------

##### Disconnect

- To disconnect the port，tap![img](./media/an32-1712639258555-54.png)first.

- Then tap **Disconnect**.

  ![img](./media/an33-1712639258555-55.png)

------

#### kidsblock Main Interface 2：

![img](./media/an34-1712639258555-56.png)

------

#### Extensions

**This kit has integrated required sensors and modules. If you want to add them that are not available in the kit, please refer to these steps.**

- Click![img](./media/an35-1712639083027-1-1712639258555-57.png)to choose an extension:

  ![img](./media/an36-1712639258555-58.png)

- For instance, if you want to load a passive buzzer, click it:

  ![img](./media/an37-1712639258555-59.png)

- “When “**Not loaded**” becomes “**Loaded**”, the buzzer module is successfully imported.

  ![img](./media/an38-1712639258555-60.png)

- Click![img](./media/an39-1712639258555-61.png)and you can see a passive buzzer in the blocks:

  ![img](./media/an41-1712639258555-62.png)

- To delete the passive buzzer, click![img](./media/an42-1712639258555-63.png)to select it.

  ![img](./media/an38-1712639258555-60.png)

  When “Loaded” changes into “Not loaded”, the module is removed from blocks.

  ![img](./media/an37-1712639258555-59.png)

  


------

#### Open Code

1. Method 1：

   - Click SB3 file to open it. If you want to open ![](./media/an46-1712639258555-64.png), just double click it. After that, please connect the board and port.

     ![img](./media/an54-1712639258555-65.png)

2. Method 2：

   - Open Kidsblock and click “**file**” to choose “**Load from your computer**”.

     ![img](./media/an47-1712639258555-66.png)	

   - Find and open the SB3 file, like ![img](./media/an46-1712639258531-17.png).

     ![img](./media/an50-1712639258555-67.png)

     ![img](./media/an54-1712639258555-65.png)

------

#### Upload Code and Set Baud Rate

##### Upload Code

- Load code file to Kidsblock.

  ![img](./media/an47-1712639258555-66.png)

- Connect the board to your computer. If there is no port, please install driver first. Choose the correct board and port and click![img](./media/an52-1712639258556-68.png).

  ![img](./media/an54-1712639258555-65.png)

- Wait for uploading.

  ![img](./media/an53-1712639258556-69.png)

------

##### Set Baud Rate

- Click one of ![img](./media/an56-1712639258556-70.png) to set the size of print box.
  - Small ![img](./media/an58-1712639258556-71.png)
  - Large ![img](./media/an59-1712639258556-72.png)
  - None ![img](./media/an60-1712639258556-73.png)

- After opening print box, click ![img](./media/an57-1712639258556-74.png)to set baud rate.

![img](./media/an55-1712639258556-77.png)

After setting the baud rate and uploading the code, “**Hello KidsBlock**” will be printed on the box.

![img](./media/an62-1712639258556-75.png)

------

## 3.ESP32 Easy Coding Board Basic Projects

### 3.1 Heartbeat

![img](./media/1-1712639258556-76.png)

#### 1.Introduction:

This project is easy to conduct with an ESP32 Easy Coding Board, a USB  type-C cable and a computer. The ESP32 Easy Coding Board RGB dot matrix  will display a beating heart. It serves as a start for your entry to the programming world!

#### 2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/2-1712639258556-78.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/3-1712639258556-79.png) |

#### 3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/4-1712639258556-80.png)

#### 4.Test Code：

Please check code in Project 1 file.

![img](./media/5-1712639258557-81.png)

![img](./media/6-1712639258557-82.png)



Find RGB blocks to change its brightness and colors.

![img](./media/7-1712639258557-83.png)



**Build blocks:**

Initialize the RGB.

![img](./media/15-1712639258557-85.png)

![img](./media/8-1712639258557-84.png)

![img](./media/9-1712639258557-86.png)

**Complete code:**

![img](./media/10-1712639258557-87.png)

#### 5.Test Result:

After uploading test code to ESP32 Easy Coding Board and powering on via  USB cable, the RGB dot matrix alternately shows patterns of a small and a large heart.

![img](./media/11-1712639258557-88.png)

![img](./media/12-1712639258557-89.png)

### 3.2 Single RGB Blinking

![img](./media/1-1712639258556-76.png)

#### 1.Introduction:

In this project, we intend to control a certain RGB of the ESP32 Easy Coding Board to be on and off.



#### 2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/2-1712639258556-78.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/3-1712639258556-79.png) |

#### 3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/4-1712639258556-80.png)

#### 4. 5*5 RGB Dot Matrix：

The RGB dot matrix has a total of 25 beads, and we mark them as number 0 to 24 from left to right and from top to bottom.

The serial number is as follows:

![img](./media/13-1712639258557-90.png)

#### 5.Test Code：

**Find code blocks:**

![img](./media/14-1712639258559-93.png)

Initialize RGB

![img](./media/15-1712639258557-85.png)

Set one RGB to light up in a certain color

![img](./media/16-1712639258558-91.png)

Clear all RGB

![img](./media/17-1712639258559-92.png)

Refresh all RGB

![img](./media/18-1712639258559-94.png)

**Build blocks:**

![img](./media/19-1712639258559-95.png)

#### 6.Test Result：

The set RGB will light up once per second.

![img](./media/20-1712639258559-96.png)

### 3.3 RGB Dot Matrix

![img](./media/1-1712639258556-76.png)

#### 1.Introduction:

Dot matrices are very commonplace in daily life, which are widely used in RGB advertisement screens, elevator floor display, bus  stop announcement and so on.

The dot matrix of ESP32 Easy Coding Board contains 25 RGB in a grid.  Previously, we have succeeded in controlling a certain RGB to light by integrating its position value into the test code. Theoretically, we can turn on multiple LEDs at the same time to show patterns, digits and characters.

What’s more, we can also click ”show icon“ to choose the pattern we  like to display. Last but not the least, we can design patterns by ourselves as well.



#### 2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/2-1712639258556-78.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/3-1712639258556-79.png) |

#### 3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/4-1712639258556-80.png)

#### 4.Test Code：

**Find code blocks:**

![img](./media/22-1712639258559-97.png)

**Build blocks:**

We set the icon to an arrow and set its brightness and color.

![img](./media/23-1712639258559-98.png)

Set the brightness and animation time.

![img](./media/24-1712639258559-99.png)

![img](./media/25-1712639258559-101.png)

#### 5.Test Result：

After uploading test code, the dot matrix starts to show arrows in multiple directions, and then it exhibits two animations with full color each 5s.

![img](./media/21-1712639258559-100.gif)

### 3.4 Programmable Touch Buttons 

![img](./media/26-1712639258559-102.png)

#### 1.Introduction:

Buttons can be used to control circuits. In an integrated circuit with a button, the circuit is connected when the button is pressed and if you release the button, the circuit is disconnected.

Capacitive touch detects the user’s operation by measuring changes in capacitance. When you touch the capacitive sensing area, the charge of the human body affects the value of the capacitor, which can be sensed by the module due to this change.

ESP32 Easy Coding Board boasts three buttons: two programmable buttons (marked with A and B), and a reset button at back. By pressing the two programmable buttons, three different signals can be input. When we press button A or B or both,  the LED dot matrix will show A, B  and AB respectively.



#### 2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/2-1712639258556-78.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/3-1712639258556-79.png) |

#### 3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/4-1712639258556-80.png)

#### 4.Test Code 1:

**Find code blocks:**

Find “if…then…” block to determine whether the buttons are pressed.

![img](./media/27-1712639258559-103.png)

![img](./media/28-1712639258559-104.png)



![img](./media/29-1712639258559-105.png)

**Build blocks:**

![img](./media/30-1712639258559-106.png)

#### 5.Test Result 1：

After uploading test code and powering on, the 5x5 dot matrix shows A if button A is pressed, and shows B if button B is pressed, and shows AB if buttons A and B are pressed together. When the touching area is touched, it shows T.

![img](./media/31-1712639258559-109.png)

![img](./media/32-1712639258559-107.png)

![img](./media/32-1-1712639258559-108.png)

#### 6.Test Code 2：

Read the touching area analog values.

**Find code blocks:**

![img](./media/39-1712639258559-110.png)

![img](./media/40-1712639258559-111.png)

**Build blocks:**

![img](./media/41-1712639258559-112.png)

#### 7.Test Result 2：

When you touch this area, the value will reduce to lower than 10.

![img](./media/42-1712639258559-116.png)

### 3.5 Passive Buzzer

![img](./media/60-1712639258559-113.png)

#### 1.Introduction:

The board boasts an built-in passive buzzer, which is a device without an oscillating circuit, so it needs an external driving signal to produce sound.

- **Passive:** Unlike active buzzers, passive buzzers  do not include a built-in oscillator circuit, so an external driving  signal with a certain frequency is required. This is usually done by a  microcontroller or other signal source.
- **Frequency control:** The frequency of the driving  signal determines the frequency at which the buzzer produces sound. By  changing the frequency of the input signals, different tones of sound  can be played.
- **Applications:** Passive buzzers are widely used in various electronic devices to provide audio prompts or alerts, such as  embedded systems, electronic products, alarm systems, etc.
- **Driving:** Due to its passiveness, they have relatively low requirements for external drive signals, so they usually only need to provide enough current and appropriate frequency.



#### 2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/2-1712639258556-78.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/3-1712639258556-79.png) |

#### 3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/4-1712639258556-80.png)

#### 4.Test Code:

**Find code blocks:**

![img](./media/61-1712639258559-114.png)

**Build blocks:**

Play do, re, mi, fa, sol, la, si, or you may compose them by yourself.

![img](./media/62-1712639258559-115.png)

Integrated music and songs:

![img](./media/63-1712639258559-117.png)

**Complete code:**

![img](./media/64-1712639258559-118.png)

#### 5.Test Result：

Play do, re, mi, fa, sol, la, si, and songs.



### 3.6 Microphone

![img](./media/156-1712639258559-119.png)

####  1.Introduction:

Microphone is a device that converts sound into electrical signals,  which is an important part of the audio field. It is widely used in voice recording, communication and audio playback.

Microphones can be divided into many types, including **Dynamic Microphone**, **Condenser Microphone**, **Wireless Microphone**, **USB Microphone** and **Laser Microphone**.

In this project, we use a minimal capacitive microphone.



#### 2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/2-1712639258556-78.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/3-1712639258556-79.png) |

#### 3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/4-1712639258556-80.png)

#### 4.Test Code 1:

**Find code blocks:**

![img](./media/157-1712639258559-120.png)

**Build blocks:**

![img](./media/158-1712639258559-121.png)

#### 5.Test Result 1:

After uploading test code and setting baud rate to 115200, speak to the  ESP32 Easy Coding Board or clap your hands or desks, the louder the sound is, the greater the value will be.



![img](./media/159-1712639258560-124.png)

#### 6.Test Code 2:

We represent the sound on RGB dot matrix, and the louder the sound, the more RGB will light up.

Initialize RGB.

![img](./media/160-1712639258559-122.png)

Determine the sound level and rate it.

![img](./media/161-1712639258559-123.png)

RGB display:

![img](./media/162-1712639258560-125.png)

**Complete code:**

![img](./media/163-1712639258560-126.png)

#### 7.Test Result 2:

Upload test code and power on, and the louder the sound is, the more the RGB will light up.

![img](./media/184-1712639258560-127.png)

![img](./media/185-1712639258560-128.png)

### 3.7 Temperature and Humidity Detection

![img](./media/33-1712639258560-129.png)

#### 1.Introduction:

AHT11 temperature and humidity sensor is equipped on the board, which  outputs digital signals. It uses special analog signal acquisition, conversion technology and temperature and humidity sensing technology to ensure that the sensor features good long-term stability and high reliability. The MCU on the ESP32 Easy Coding Board communicates with it via I2C.



#### 2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/2-1712639258556-78.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/3-1712639258556-79.png) |

#### 3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/4-1712639258556-80.png)

#### 4.Test Code:

**Find code blocks:**

![img](./media/34-1712639258560-130.png)

![img](./media/35-1712639258560-131.png)

![img](./media/36-1712639258560-132.png)

**Build blocks:**

![img](./media/37-1712639258560-133.png)

#### 5.Test Result：

After uploading test code, open the serial monitor and set baud rate,  and the temperature, humidity and dew point value will be printed.

![img](./media/38-1712639258560-134.png)



### 3.8 MPU6050 Accelerometer and Gyroscope

![img](./media/43-1712639258560-135.png)

#### 1.Introduction:

The MPU6050 is a six-axis motion processor that includes a 3-axis gyroscope and a 3-axis accelerometer. The two sensors are integrated on a single chip to detect static and dynamic object motion states, including angular speed, Angle and acceleration.

Its 16-bit ADC can simultaneously read data from six axes to measure diagonal speed and Angle, and infer acceleration information from the object. The MPU6050 also boasts a built-in temperature sensor to measure the temperature of  the chip, helping to monitor the temperature of the sensor during  operation.

In addition, the MPU6050 is equipped with a fast Digital Motion  Processor (DMP), which helps process raw data from the gyroscope and accelerometer to obtain the motion state of the object.



**Typical circuit diagram:**

![img](./media/51-1712639258560-136.png)

|  #   | NAME |                         DESCRIPTION                          |
| :--: | :--: | :----------------------------------------------------------: |
|  1   | GND  |                   Negative interface (0V).                   |
|  2   | VCC  |               Positive interface (3.3V or 5V).               |
|  3   | SDA  |   I2C data line, connected to MCU, used to transmit data.    |
|  4   | SCL  | I2C clock line, connected to MCU, used to synchronize data transmission. |
|  5   | XDA  | I2C data line, connected to external extension sensors, used to transmit data. |
|  6   | XCL  | I2C clock line, connected to external extension sensors, used to synchronize data transmission. |
|  7   | AD0  | I2C Slave address. The sensor address is 0x69 at high and 0x68 at low. |
|  8   | INT  | External interrupt pin, detects the internal interrupt time of the MPU6050. |

- Operating voltage: 3.3V, 5V
- Static current: 5μA
- Rotating current: 3mA
- Maximum rotation speed: 2000°/s
- Acceleration range: ±2g, ±4g, ±8g, ±16g
- Temperature range: –10 ~ +65°C

MPU6050 can be used to measure the attitude of an object. Measurements of three angles are provided: **roll**, **pitch** and **yaw**. It can also provide the acceleration of the object, and obtain the speed and position information of the object through calculation.

**Its three axes:**

![img](./media/52-1712639258560-137.png)

![img](./media/53-1712639258560-138.png)

The corresponding **Euler Angle** indicates the Angle of rotation of the object in three-dimensional space, and its coordinate axis can be adjusted arbitrarily.

Euler Angle consists of three angles, namely **Roll**, **Pitch** and **Yaw**.

|   Roll    |   Rotation Angle with x-axis as rotation axis   |
| :-------: | :---------------------------------------------: |
| **Pitch** | **Rotation Angle with y-axis as rotation axis** |
|  **Yaw**  | **Rotation Angle with z-axis as rotation axis** |

 

![img](./media/54-1712639258560-139.png)

When acquiring Yaw, the gyroscope inside the MPU6050 is automatically calibrated to zero, which causes Yaw to drift to zero.

**Zero drift** means that the detected data will have an accidental small fluctuation, for example, the sensor value will automatically have an accidental small change. Even after a good algorithm, zero drift still exists, as it is limited by hardware.

Solution: add a magnetometer to calibrate the MPU6050.

------

For more details, please refer to the MPU6050 data sheet:

[https://www.invensense.com/wp-content/uploads/2015/02/MPU-6000-Datasheet1.pdf](https://www.invensense.com/wp-content/uploads/2015/02/MPU-6000-Datasheet1.pdf)

[https://www.invensense.com/wp-content/uploads/2015/02/MPU-6000-Register-Map1.pdf](https://www.invensense.com/wp-content/uploads/2015/02/MPU-6000-Register-Map1.pdf)



#### 2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/2-1712639258556-78.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable *1       | ![img](./media/3-1712639258556-79.png) |

#### 3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/4-1712639258556-80.png)

#### 4.Test Code 1:

**Find code blocks:**

![img](./media/34-1712639258560-130.png)

![img](./media/44-1712639258560-140.png)

**Build blocks:**

Initialize serial monitor and MPU6050.

![img](./media/45-1712639258560-141.png)

This block is used to update the data each time it is fetched. 

![img](./media/46-1712639258560-142.png)

![img](./media/47-1712639258560-143.png)

**Complete code:**

![img](./media/48-1712639258560-145.png)

#### 5.Test Result 1：

After uploading code and powering on, Put ESP32 Easy Coding Board flatwise on the desk, press the reset button to initialize MPU6050, and wait 2 or 3 seconds.

When the serial monitor shows values, the initialization is completed; and if values on each axis is less than 10, the initialization is correct; otherwise you need to re-initialize it.

![img](./media/50-1712639258560-144.png)

![img](./media/49-1712639258560-146.png)

### 3.9 Light Intensity

![img](./media/55-1712639258560-147.png)

#### 1.Introduction:

Photoresistors measure light intensity and are commonly used to detect brightness in the surrounding environment.

**Working principle:** This module is designed by the light-sensitive materials. There are two main types: photoresistor and photodiode.

- **Photoresistor:** The resistance of a photoresistor varies with the intensity of ambient light. For one photoresistor, the  stronger the ambient light, the lower the resistance will be.
- **Photodiode:** The current output of a photodiode is proportional to the intensity of the incident light. The electrical signals they produce can be used to measure light brightness.

**Applications:** Photoresistors are widely applied to various fields, including light control systems, lighting systems,  camera exposure control, light monitoring, automatic adjustment of screen brightness, etc.

**Unit of brightness:** They usually measure light intensity in illuminance units (such as Lux). Illuminance represents the luminous flux per unit area.



#### 2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/2-1712639258556-78.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/3-1712639258556-79.png) |

#### 3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/4-1712639258556-80.png)

#### 4.Test Code:

**Find code blocks:**

![img](./media/34-1712639258560-130.png)

![img](./media/56-1712639258560-148.png)

**Build blocks:**

![img](./media/57-1712639258560-149.png)

#### 5.Test Result：

Upload the test code and open the serial monitor. When the light intensity detected by the sensor changes, the sensor values will also change.

![img](./media/58-1712639258560-151.png)

![img](./media/59-1712639258560-150.png)

### 3.10 Read SD Card

![img](./media/66-1712639258560-152.png)

#### 1.Introduction

The SD card module is used in conjunction with the MCU on the ESP32  Easy Coding Board for reading and writing data on the SD (Secure  Digital) card. This module makes it easier to use SD cards to store and access data in projects.

- **Function:** SD card module allows the ESP32 Easy Coding Board to communicate with the SD card to achieve data reading and writing. This is very useful for data logging, file storage, logging,  etc.

- **Interface:** The SD card module usually connects  to the ESP32 Easy Coding Board using the Serial Peripheral Interface  (SPI) interface. It needs to be connected to the corresponding pin of the ESP32 Easy Coding Board, For example, MOSI (Master Out Slave In),  MISO (Master In Slave Out), SCK (Serial Clock), and CS (Chip Select).

- **SD card type:** SD card modules are generally compatible with various types, including standard SD cards, SDHC cards  (High Capacity), and SDXC cards (extended Capacity).

  

#### 2.Components:

| ESP32 Easy Coding Board*1            | ![img](./media/2-1712639258556-78.png)   |
| ------------------------------------ | ---------------------------------------- |
| USB type C  Cable*1                  | ![img](./media/3-1712639258556-79.png)   |
| SD Card*1（not included in the kit） | ![img](./media/65-1712639258560-153.png) |

#### 3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/4-1712639258556-80.png)

Insert the SD card into the slot.

![img](./media/142-1712639258560-154.png)

![img](./media/143-1712639258560-155.png)

#### 4.Test Code:

**Find code blocks:**

![img](./media/139-1712639258560-156.png)

Initialize the serial monitor and SD card.

![img](./media/140-1712639258560-157.png)

Refresh the SD data before using.

![img](./media/141-1712639258560-158.png)



##### Read SD card type

![img](./media/144-1712639258560-159.png)

Serial port output:

![img](./media/145-1712639258561-160.png)

##### Read SD card message

![img](./media/146-1712639258561-161.png)

![img](./media/148-1712639258561-162.png)

Serial monitor output：

![img](./media/147-1712639258561-163.png)

File：

Determine whether there is a ‘’file.txt‘’ file in SD card.

![img](./media/149-1712639258561-164.png)

If there is no ‘’file.txt‘’, create a file and input “hello,world” in a new line.

![img](./media/150-1712639258561-165.png)

After that, read the content in ‘’file.txt‘’.

![img](./media/151-1712639258561-166.png)

Read all list files in SD card, including hidden files.

![img](./media/153-1712639258561-167.png)

Delete this ‘’file.txt‘’.

![img](./media/152-1712639258561-168.png)

**Complete code:**

![img](./media/154-1712639258561-169.png)

Serial monitor output:

![img](./media/155-1712639258561-170.png)

### 3.11 Read ESP32 Easy Coding Board Current

![img](./media/164-1712639258561-171.png)

#### 1.Introduction

ESP32 Easy Coding Board boasts a built-in current measurement module  (only measure USB power supply and PH2.0 interface power supply) to  measure current by a resistive current sensor.

Resistive current sensor is commonly used to monitor the current  value by measuring the voltage drop generated by the current through the resistance. The working principle of such sensors is based on Ohm’s  law, which states that when a current passes through a resistor, the voltage generated at both ends of the resistor is proportional to the current.

![img](./media/165-1712639258561-172.png)

- **Current sensing:** Resistive current sensor contains a current sensing element, usually a resistor. When current passes through this resistor, a voltage drop will be generated at both ends of the resistor, the magnitude of which is proportional to the strength of the current.
- **Voltage output:** By measuring the voltage drop at both ends of the resistor, the sensor can provide a voltage signal that is related to current. This voltage signal can be digitally processed by devices like an analog-to-digital converters (ADC).

Resistive current sensors are widely applied to power system monitoring, power consumption measurement of electronic devices,  electric vehicle current monitoring and so on.



#### 2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/2-1712639258556-78.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/3-1712639258556-79.png) |

#### 3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/4-1712639258556-80.png)

#### 4.Test Code 1:

**Read current value:**

![img](./media/166-1712639258561-173.png)

![img](./media/167-1712639258561-174.png)

#### 5.Test Result 1：

After uploading test code, open the serial monitor and you will see the current value is 0. Because many modules are not working on the board,  so the current is close to 0.

![img](./media/168-1712639258561-175.png)

#### 6.Test Code 2:

Enable RGB dot matrix and then measure the current value.

Initialize the serial monitor and RGB dot matrix.

![img](./media/169-1712639258561-176.png)

First measure 10 RGBs.

![img](./media/170-1712639258561-177.png)

Then measure 18 RGBs.

![img](./media/171-1712639258561-178.png)

Last measure 25 RGBs.

![img](./media/172-1712639258561-179.png)

**Complete code:**

![img](./media/174-1712639258561-180.png)

#### 7.Test Result 2:

Upload test code and you will find that the more the RGB, the larger the current will be.

![img](./media/173-1712639258561-181.png)

#### 8.Test Code 3:

The conversion of current to power: power (P) equals to current (I) times voltage (V).

*P*=*I*×*V*

- *P* is power, unit: Watt(W)
- *I* is current, unit: ampere(A)
- *V* is voltage, unit: volt(V)

This formula is suitable for DC circuits.

For AC circuits, power calculation may require more complex formulas due to power factor.

In a circuit, power describes the conversion of electrical energy.  Input current and voltage values into the above formula and you can get real-time power values.

This is commonly used for energy monitoring, power system management and equipment power consumption evaluation.

The power voltage of ESP32 Easy Coding Board is 3.3V, so we only need to measure the current and multiply it by 3.3 to get the power of the Board at this time.


------

Create variables **P** and **I**.


![img](./media/175-1712639258561-182.png)

![img](./media/176-1712639258561-183.png)

![img](./media/177-1712639258561-184.png)

Assign the read current value to variable I.

![img](./media/178-1712639258561-185.png)

I multiplies by 3.3 is power of the ESP32 Easy Coding Board(the board voltage is 3.3V).

![img](./media/181-1712639258561-186.png)

**Complete code:**

![img](./media/183-1712639258561-187.png)

#### 9.Test Result 3:

Upload code and open serial monitor to set baud rate. The more the RGBs, the greater the current value and power will be.

![img](./media/182-1712639258561-188.png)

### 3.12 Wifi Wireless Communication

ESP32 Easy Coding Board is built with Wi-Fi (2.4G) and Bluetooth (4.2)  to easily connect to a Wi-Fi network and communicate with other devices in the network, so you can use this Board to display web pages in your browser.

![img](./media/124-1712639258561-189.png)

#### ESP32 Easy Coding Board WiFi Function

- **Base mode (STA / Wi-Fi Client mode)**: ESP32 Easy Coding Board is connected to a Wi-Fi hotspot (AP).
- **AP mode (Soft-AP / Wi-Fi hotspot mode)**: Other Wi-Fi devices connect to ESP32 Easy Coding Board.
- **AP-STA mode**: ESP32 Easy Coding Board is both a Wi-Fi hotspot and a Wi-Fi device connected to another Wi-Fi.
- These modes support multiple security modes: WPA, WPA2, WEP, etc.
- Wi-Fi hotspots can be searched (active and passive scanning).
- Support hybrid mode monitoring of IEEE802.11 Wi-Fi packets.

------

For more wifi reference, please visit：[https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/network/esp_wifi.html](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/network/esp_wifi.html)

Espressif Official：[https://www.espressif.com.cn/en/home](https://www.espressif.com.cn/en/home)

![img](./media/125-1712639258561-190.png)

------

#### wifi Web Page

Add an extension of web page editing.

![img](./media/126-1712639258561-191.png)

![img](./media/127-1712639258561-192.png)



![img](./media/128-1712639258561-193.png)

![img](./media/129-1712639258561-194.png)

Connect a Wifi and input your wifi name and passwords. After connecting, the IP address will be printed on the serial monitor.

![img](./media/130-1712639258561-195.png)

![img](./media/131-1712639258561-196.png)

Set up a web component named **temperature** in the unit of ℃.

![img](./media/132-1712639258561-197.png)

![img](./media/133-1712639258562-198.png)

Add a button module named **button**.

![img](./media/134-1712639258562-199.png)

![img](./media/135-1712639258562-200.png)

**Complete code:**

![img](./media/136-1712639258562-201.png)

As long as connecting the Wi-Fi, you may use the Web Server Library of ESP32 Easy Coding Board to provide web page.

In the example, we set up a simple web page to display a certain temperature value.

**Open your browser to check and visit the IP address of ESP32  Easy Coding Board. Herein, you may access to “http://[IP address of  ESP32 Easy Coding Board]” to visit its website.**

**NOTE: When PC, mobile phone and ESP32 Easy Coding Board are connected to one network, this website(your own IP address of ESP32 Easy Coding Board) can be accessed via PC and mobile at the same time.**



PC：

![img](./media/137-1712639258562-202.png)

Mobile：

![img](./media/138-1712639258562-203.png)


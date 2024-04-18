# ESP32 Easy Coding Board Basic Tutorial

## 1.Development Board

Link：<http://keyestudio-ks5018.readthedocs.io/>

## 2.Kidsblock Software

1.1 Installation

**Windows System：**

1. Download

   - Download link：[http://xiazai.keyesrobot.cn/KidsBlock.exe](http://xiazai.keyesrobot.cn/KidsBlock.exe)

     

2. After downloading, click  “KidsBlock.exe”![img](./media/aa89d6fcdb9bcb038b35c13e13d19e4f.png)to open it.

3. Tap “**Anyone who uses this computer(all users)**” and “**Next**”.

![](./media/8ae01ee34f5a3694c2c9e37b7ba26226.png)

4. Click “**Browse…**” to choose an installation path of the software, and click “**Install**”.


![img](./media/1830a79c9170bc563c9344606b1b8eb5.png)

![img](./media/67c631f4c7693fae14dfdf1c60f98217.png)

5. Click “Finish”.

![img](./media/06f8ba928325f1961ece22ef943cbf82.png)

6. If there is a warning on your computer, just click “**Allow access**” to enter the software.

![img](./media/31e0f8000e19073acd66376b178437f8.png)

------



MacOS System：

1. Download Kidsblock package： [http://xiazai.keyesrobot.cn/KidsBlock.dmg](http://xiazai.keyesrobot.cn/KidsBlock.dmg)

![img](./media/d30aea92ba6a5aff9d48f2ec8e7419f4.png)

2. After downloading, click **KidsBlock**. And then drag the **KidsBlock Desktop** into **Applications**.

![img](./media/8a5d7e598e3d23ac7a433713de4ce46e.png)

3. After installation, you can see the icon of KidsBlock.

   ![img](./media/282c7f723d8b8b0bea5bf949c6b7acce.png)

4. Open KidsBlock, but it cannot be opened, because Mac devices only allow us to open apps from its App store by default. Thus, we  need to modify some settings. 

   ![img](./media/f6d9d2910373b38c787556ba7abb4bce.png)

5. Open settings and enter **Privacy&Security**, tick **App Store and identified developers** in **Security**. And then click **Open Anyway**.

   ![img](./media/a48217d60bcc8efef72256832cfbda57.png)

6. Click **Open** and the software can be opened.

   ![img](./media/902141f8671076e3f924bbc29d6a402e.png)

7. Now re-open the Kidsblock.

   ![img](./media/32f68f15c4acea5f9b76cd40a995c696.png)

8. Now enjoy your programming!

   ![img](./media/d0f4763fb4dc20b5d9d27e47f00f0f86.png)

------



1.2 Using Tutorial

（**We demonstrate on Windows, and MacOS users may take it as a reference.**）

kidsblock Main Interface 1：

![img](./media/680c3b0eaf7eb3d467930c553d7de7fa.png)

------



Language

Click![img](./media/04f545ccca87a89060353cc564a9cfc8.png)to shift languages.

![image-20240409130921782](./media/d38b0c729ba108ad2971430d143726bd.png)

------



Device Driver

**If the driver is already installed on the computer, you do not need to install it again. If not, you need to do the following.**

Click![img](./media/73c3a4805aba3635e3eb718b2b5d8a1a.png)to choose “**Install driver**”.


![img](./media/b66194fc67cb7d2428921d3560b669b0.png)

- Enter **Device Driver Installation Wizard** and click “**Next**”.

![img](./media/fdada13a844a24e55ed48cba9288f335.png)

- Click “**Finish**”.

![img](./media/b79e20f4e985da0e20347bcef8e63d38.png)

- Click “**Next**”.

![img](./media/5ecffc2405a21915846b0bc101e39b1a.png)

- Click “**Finish**”.

![img](./media/3078c15bc46dbd345c8a05165319c774.png)

- If a warning appears, just click “**Allow**” and “**Install**”.

![img](./media/235d65419d74f2e3b332bb628bc65049.png)

- Click “**Finish**”.

![img](./media/30c01ca35743aa3f006f635fdd213e21.png)

- Click “**Extract**”.

![img](./media/6951d98e37fd2f2a2f2d91c34d61a502.png)

- Click “**Next**”.

![img](./media/e8e996108095c18e9f1508cf3dc75485.png)

- Click “**I accept this agreement**” and “**Next**”.

![img](./media/33c4335d9455053e4cf2ba89011d6755.png)

- Click “**Finish**”.

![img](./media/d855a13a426a1d36aa0dfae262f21827.png)

- Click “**INSTALL**”.

![img](./media/c67c8443839fbb88f1b6a7a71c73fdeb.png)

- Click “**OK**”.

![img](./media/e9251c41ec093c489111efe2faf4872f.png)

------

Development Board

Connect a board and a port:

- Click![img](./media/8403678060dc2602b342f4bf99daeb33.png)to choose a device.

- Click **Kit** and find **ESP32 Easy Coding Board** to load it. Required sensors and modules are included in it, so you do not need to load them one by one.

  ![img](./media/778acd06b9d296b3034b128faaad012e.png)

- The following interface will appear, and we need to choose the correct port and click **Connect**.

  ![img](./media/c09c9db66c94126d4b85162964c82888.png)

- Click **Go to Editor**

  ![img](./media/3326713c6ceab17917bf3991d090bc93.png)

- Main interface:

  ![img](./media/4c0b872567d86d4cd2290366aadf66d4.png)

------

Disconnect

- To disconnect the port，tap![img](./media/b7cecf81bbe3bbd36bb1c59548165c9a.png)first.

- Then tap **Disconnect**.

  ![img](./media/e2c5c4cc94457e80942c7fadfe7e528b.png)

------

kidsblock Main Interface 2：

![img](./media/1815a966f542fa61fad2f3b787b7b86f.png)

------

Extensions

**This kit has integrated required sensors and modules. If you want to add them that are not available in the kit, please refer to these steps.**

- Click![img](./media/3ed72608cc49997e7798fdcbdbf67e97.png)to choose an extension:

  ![img](./media/79a0694138add048fbb9bf9c6035d661.png)

- For instance, if you want to load a passive buzzer, click it:

  ![img](./media/65463177937533aa865274ee49b5a2d5.png)

- “When “**Not loaded**” becomes “**Loaded**”, the buzzer module is successfully imported.

  ![img](./media/19b19088ed62b6d304dcc8ae4c09e0a1.png)

- Click![img](./media/a2dc87c2feb1d4476fdba1670c9e80ce.png)and you can see a passive buzzer in the blocks:

  ![img](./media/19befcc69743a59e460af656dbc75de1.png)

- To delete the passive buzzer, click![img](./media/3ed72608cc49997e7798fdcbdbf67e97.png)to select it.

  ![img](./media/19b19088ed62b6d304dcc8ae4c09e0a1.png)

  When “Loaded” changes into “Not loaded”, the module is removed from blocks.

  ![img](./media/65463177937533aa865274ee49b5a2d5.png)

  


------

Open Code

1. Method 1：

   - Click SB3 file to open it. If you want to open ![](./media/21f567a32d4f511b4c9c4b243d7d4ff3.png), just double click it. After that, please connect the board and port.

     ![img](./media/e5e8d27a410c4b81e5b5ddbf76876e2d.png)

2. Method 2：

   - Open Kidsblock and click “**file**” to choose “**Load from your computer**”.

     ![img](./media/c523c51500a137ebea82286693023762.png)	

   - Find and open the SB3 file, like ![img](./media/21f567a32d4f511b4c9c4b243d7d4ff3.png).

     ![img](./media/9c52e0b9906c3cd505d2df96cc68c4cc.png)

     ![img](./media/e5e8d27a410c4b81e5b5ddbf76876e2d.png)

------

Upload Code and Set Baud Rate

Upload Code

- Load code file to Kidsblock.

  ![img](./media/c523c51500a137ebea82286693023762.png)

- Connect the board to your computer. If there is no port, please install driver first. Choose the correct board and port and click![img](./media/35244c93ea2ddc2bdd389ace5d7543af.png).

  ![img](./media/e5e8d27a410c4b81e5b5ddbf76876e2d.png)

- Wait for uploading.

  ![img](./media/9d5de91a59629102f82e82a448d1df3f.png)

------

Set Baud Rate

- Click one of ![img](./media/9a1b8dcbbd1328be68b326c7381f7887.png) to set the size of print box.
  - Small ![img](./media/1d820b2f38e244f379d245434cc5792e.png)
  - Large ![img](./media/4669f9818769f8d7dfe8317e18bc56c7.png)
  - None ![img](./media/116bbf77e54df190dfadb6fee7634577.png)

- After opening print box, click ![img](./media/430871c8222322bf6366e70cef8e384f.png)to set baud rate.

![img](./media/4a592a5df595a02d6e2c8c5da087bdb3.png)

After setting the baud rate and uploading the code, “**Hello KidsBlock**” will be printed on the box.

![img](./media/925a7e6d5ea8d875ad9804b26e4f3cdc.png)

------

## 3.ESP32 Easy Coding Board Basic Projects

3.1 Heartbeat

![img](./media/0cf1e7028ce5e6f4f9c9df7d50c4a995.png)

1.Introduction:

This project is easy to conduct with an ESP32 Easy Coding Board, a USB  type-C cable and a computer. The ESP32 Easy Coding Board RGB dot matrix  will display a beating heart. It serves as a start for your entry to the programming world!

2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/4f8ac5efacc04d3f15e4f804abe70fc0.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/26110bd63d838c6377849040b83e3a08.png) |

3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/a4dc84d7f522d094ab4964b4721e0be4.png)

4.Test Code：

Please check code in Project 1 file.

![img](./media/079bbc1db6550b30de5d7708d476f14e.png)

![img](./media/cd24339303faa8efd162100fe9e9fc22.png)



Find RGB blocks to change its brightness and colors.

![img](./media/8105c07199d9d1b8b35e71040496884d.png)



**Build blocks:**

Initialize the RGB.

![img](./media/53f48027e3d08a5ec3e0c4221d47a10a.png)

![img](./media/1713063ff14d71ae06a35e195e227897.png)

![img](./media/f8878b1ea9cf232b86b66d6827c60e4e.png)

**Complete code:**

![img](./media/bfb050d6f17d28fee7f83c022c3cea8d.png)

5.Test Result:

After uploading test code to ESP32 Easy Coding Board and powering on via  USB cable, the RGB dot matrix alternately shows patterns of a small and a large heart.

![img](./media/b28d0c01c7abaeb2cae2bbe204b5ba38.png)

![img](./media/ebcd3d3b7ab3595dfc355a5925e16156.png)

3.2 Single RGB Blinking

![img](./media/0cf1e7028ce5e6f4f9c9df7d50c4a995.png)

1.Introduction:

In this project, we intend to control a certain RGB of the ESP32 Easy Coding Board to be on and off.



2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/4f8ac5efacc04d3f15e4f804abe70fc0.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/26110bd63d838c6377849040b83e3a08.png) |

3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/a4dc84d7f522d094ab4964b4721e0be4.png)

4. 5*5 RGB Dot Matrix：

The RGB dot matrix has a total of 25 beads, and we mark them as number 0 to 24 from left to right and from top to bottom.

The serial number is as follows:

![img](./media/7756ebda7a04fb2f22d291dcd1457623.png)

5.Test Code：

**Find code blocks:**

![img](./media/12bc21c30e6c892da1a17df990d4df25.png)

Initialize RGB

![img](./media/53f48027e3d08a5ec3e0c4221d47a10a.png)

Set one RGB to light up in a certain color

![img](./media/1edbbf615c7db919b572da642bbb59db.png)

Clear all RGB

![img](./media/fd53837d324e63cbb1ff6f6b6cd53314.png)

Refresh all RGB

![img](./media/072e85794e45aa2706bf0de24175ae2e.png)

**Build blocks:**

![img](./media/f19bbdef681cbeea664b49c15a8010ce.png)

6.Test Result：

The set RGB will light up once per second.

![img](./media/f8f71addd63c7c6f09e6e93a3595e46f.png)

3.3 RGB Dot Matrix

![img](./media/0cf1e7028ce5e6f4f9c9df7d50c4a995.png)

1.Introduction:

Dot matrices are very commonplace in daily life, which are widely used in RGB advertisement screens, elevator floor display, bus  stop announcement and so on.

The dot matrix of ESP32 Easy Coding Board contains 25 RGB in a grid.  Previously, we have succeeded in controlling a certain RGB to light by integrating its position value into the test code. Theoretically, we can turn on multiple LEDs at the same time to show patterns, digits and characters.

What’s more, we can also click ”show icon“ to choose the pattern we  like to display. Last but not the least, we can design patterns by ourselves as well.



2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/4f8ac5efacc04d3f15e4f804abe70fc0.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/26110bd63d838c6377849040b83e3a08.png) |

3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/a4dc84d7f522d094ab4964b4721e0be4.png)

4.Test Code：

**Find code blocks:**

![img](./media/4032e017bf8ecb8d7214e6dcf8f6cac6.png)

**Build blocks:**

We set the icon to an arrow and set its brightness and color.

![img](./media/c911a26ceb1d5491c8251bd004c338b8.png)

Set the brightness and animation time.

![img](./media/aa3d90c76b63f910798b5578be65aee1.png)

![img](./media/1da237c79a3a2687ca4f62f361cf6af3.png)

5.Test Result：

After uploading test code, the dot matrix starts to show arrows in multiple directions, and then it exhibits two animations with full color each 5s.

![img](./media/7ab88973db2650f4d25716f9e2d1cc21.gif)

3.4 Programmable Touch Buttons 

![img](./media/695a263fd2704e18d7feed137692f093.png)

1.Introduction:

Buttons can be used to control circuits. In an integrated circuit with a button, the circuit is connected when the button is pressed and if you release the button, the circuit is disconnected.

Capacitive touch detects the user’s operation by measuring changes in capacitance. When you touch the capacitive sensing area, the charge of the human body affects the value of the capacitor, which can be sensed by the module due to this change.

ESP32 Easy Coding Board boasts three buttons: two programmable buttons (marked with A and B), and a reset button at back. By pressing the two programmable buttons, three different signals can be input. When we press button A or B or both,  the LED dot matrix will show A, B  and AB respectively.



2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/4f8ac5efacc04d3f15e4f804abe70fc0.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/26110bd63d838c6377849040b83e3a08.png) |

3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/a4dc84d7f522d094ab4964b4721e0be4.png)

4.Test Code 1:

**Find code blocks:**

Find “if…then…” block to determine whether the buttons are pressed.

![img](./media/07027f9177942e7e922faf412815dd25.png)

![img](./media/1f3529a85a41b4faee21018ca7ac8351.png)



![img](./media/62119eb914fa1b9960867d2e8f68417f.png)

**Build blocks:**

![img](./media/75b1fe72e55ba6278edf5bcab0624f37.png)

5.Test Result 1：

After uploading test code and powering on, the 5x5 dot matrix shows A if button A is pressed, and shows B if button B is pressed, and shows AB if buttons A and B are pressed together. When the touching area is touched, it shows T.

![img](./media/61dbbbdcf9767eb0f067ee35c92c30ea.png)

![img](./media/b694932b7de0048a8a13c51f1a1d43df.png)

![img](./media/9648b166c45be8a72d96ca9b8b4e15fc.png)

6.Test Code 2：

Read the touching area analog values.

**Find code blocks:**

![img](./media/f9f8fe3e08777a55414633b83dc228d5.png)

![img](./media/d276a84f15414743a57ac0c932195693.png)

**Build blocks:**

![img](./media/ae94e955cc4d9659a34de45268a7c265.png)

7.Test Result 2：

When you touch this area, the value will reduce to lower than 10.

![img](./media/7b7ae45b38772f911627890c9dde071e.png)

3.5 Passive Buzzer

![img](./media/9d0c6c49067609427c2e62b5268cf4ee.png)

1.Introduction:

The board boasts an built-in passive buzzer, which is a device without an oscillating circuit, so it needs an external driving signal to produce sound.

- **Passive:** Unlike active buzzers, passive buzzers  do not include a built-in oscillator circuit, so an external driving  signal with a certain frequency is required. This is usually done by a  microcontroller or other signal source.
- **Frequency control:** The frequency of the driving  signal determines the frequency at which the buzzer produces sound. By  changing the frequency of the input signals, different tones of sound  can be played.
- **Applications:** Passive buzzers are widely used in various electronic devices to provide audio prompts or alerts, such as  embedded systems, electronic products, alarm systems, etc.
- **Driving:** Due to its passiveness, they have relatively low requirements for external drive signals, so they usually only need to provide enough current and appropriate frequency.



2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/4f8ac5efacc04d3f15e4f804abe70fc0.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/26110bd63d838c6377849040b83e3a08.png) |

3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/a4dc84d7f522d094ab4964b4721e0be4.png)

4.Test Code:

**Find code blocks:**

![img](./media/895157b81b78c0573b77486bea61daaf.png)

**Build blocks:**

Play do, re, mi, fa, sol, la, si, or you may compose them by yourself.

![img](./media/ffb185bda6ccb840cd17138d6a1959c1.png)

Integrated music and songs:

![img](./media/0f67eb911d018489d810ec67005fa45c.png)

**Complete code:**

![img](./media/53a08e817681a0f9596f105f2da003d2.png)

5.Test Result：

Play do, re, mi, fa, sol, la, si, and songs.



3.6 Microphone

![img](./media/0a220a3a627f88add9a5292e5cda430e.png)

 1.Introduction:

Microphone is a device that converts sound into electrical signals,  which is an important part of the audio field. It is widely used in voice recording, communication and audio playback.

Microphones can be divided into many types, including **Dynamic Microphone**, **Condenser Microphone**, **Wireless Microphone**, **USB Microphone** and **Laser Microphone**.

In this project, we use a minimal capacitive microphone.



2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/4f8ac5efacc04d3f15e4f804abe70fc0.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/26110bd63d838c6377849040b83e3a08.png) |

3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/a4dc84d7f522d094ab4964b4721e0be4.png)

4.Test Code 1:

**Find code blocks:**

![img](./media/8df4223a920199cd763079b8c7a7f5af.png)

**Build blocks:**

![img](./media/98735a71717889cabcad47aeffafa6c1.png)

5.Test Result 1:

After uploading test code and setting baud rate to 115200, speak to the  ESP32 Easy Coding Board or clap your hands or desks, the louder the sound is, the greater the value will be.



![img](./media/ce87537c54e67d3f82ea825e0dd58316.png)

6.Test Code 2:

We represent the sound on RGB dot matrix, and the louder the sound, the more RGB will light up.

Initialize RGB.

![img](./media/aa04be88281b2b8e5fde220ed800e9c1.png)

Determine the sound level and rate it.

![img](./media/9a3ea7bc665ccf9101803ce6db2b5066.png)

RGB display:

![img](./media/d8a385bbc7c63e300a54e4ab113627d5.png)

**Complete code:**

![img](./media/a04e140360a6e353caf4c5d6a6fadd92.png)

7.Test Result 2:

Upload test code and power on, and the louder the sound is, the more the RGB will light up.

![img](./media/cd1e1afcb5b908e9b20bfbf3c91442fd.png)

![img](./media/d520b6c07ec071744fcc3eb7241ec00d.png)

3.7 Temperature and Humidity Detection

![img](./media/16852a0818b5c4cd2bdb481614ea2c43.png)

1.Introduction:

AHT11 temperature and humidity sensor is equipped on the board, which  outputs digital signals. It uses special analog signal acquisition, conversion technology and temperature and humidity sensing technology to ensure that the sensor features good long-term stability and high reliability. The MCU on the ESP32 Easy Coding Board communicates with it via I2C.



2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/4f8ac5efacc04d3f15e4f804abe70fc0.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/26110bd63d838c6377849040b83e3a08.png) |

3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/a4dc84d7f522d094ab4964b4721e0be4.png)

4.Test Code:

**Find code blocks:**

![img](./media/af81635991bc0ed2597f080716945a4c.png)

![img](./media/91ff82be2f6fa43fceddfc6c5a1a2284.png)

![img](./media/2f4cc10ff40c70cdeba51705b05ea5be.png)

**Build blocks:**

![img](./media/09b670f0ef45eeb1574bce2891152ab2.png)

5.Test Result：

After uploading test code, open the serial monitor and set baud rate,  and the temperature, humidity and dew point value will be printed.

![img](./media/a9033da266d51aec79de9c24efeec81d.png)



3.8 MPU6050 Accelerometer and Gyroscope

![img](./media/c782e6004b9ff2dd09a68f0dbe142783.png)

1.Introduction:

The MPU6050 is a six-axis motion processor that includes a 3-axis gyroscope and a 3-axis accelerometer. The two sensors are integrated on a single chip to detect static and dynamic object motion states, including angular speed, Angle and acceleration.

Its 16-bit ADC can simultaneously read data from six axes to measure diagonal speed and Angle, and infer acceleration information from the object. The MPU6050 also boasts a built-in temperature sensor to measure the temperature of  the chip, helping to monitor the temperature of the sensor during  operation.

In addition, the MPU6050 is equipped with a fast Digital Motion  Processor (DMP), which helps process raw data from the gyroscope and accelerometer to obtain the motion state of the object.



**Typical circuit diagram:**

![img](./media/0a2e882d758d9d22bafe32726ca4518f.png)

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

![img](./media/d4ec878ce6579c1fa90ed5b3f7bd4f36.png)

![img](./media/bca124b77cd5d4b1e2555433cea63375.png)

The corresponding **Euler Angle** indicates the Angle of rotation of the object in three-dimensional space, and its coordinate axis can be adjusted arbitrarily.

Euler Angle consists of three angles, namely **Roll**, **Pitch** and **Yaw**.

|   Roll    |   Rotation Angle with x-axis as rotation axis   |
| :-------: | :---------------------------------------------: |
| **Pitch** | **Rotation Angle with y-axis as rotation axis** |
|  **Yaw**  | **Rotation Angle with z-axis as rotation axis** |

 

![img](./media/c4f1a0de73deeefaafc83696ad56621a.png)

When acquiring Yaw, the gyroscope inside the MPU6050 is automatically calibrated to zero, which causes Yaw to drift to zero.

**Zero drift** means that the detected data will have an accidental small fluctuation, for example, the sensor value will automatically have an accidental small change. Even after a good algorithm, zero drift still exists, as it is limited by hardware.

Solution: add a magnetometer to calibrate the MPU6050.

------

For more details, please refer to the MPU6050 data sheet:

[https://www.invensense.com/wp-content/uploads/2015/02/MPU-6000-Datasheet1.pdf](https://www.invensense.com/wp-content/uploads/2015/02/MPU-6000-Datasheet1.pdf)

[https://www.invensense.com/wp-content/uploads/2015/02/MPU-6000-Register-Map1.pdf](https://www.invensense.com/wp-content/uploads/2015/02/MPU-6000-Register-Map1.pdf)



2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/4f8ac5efacc04d3f15e4f804abe70fc0.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable *1       | ![img](./media/26110bd63d838c6377849040b83e3a08.png) |

3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/a4dc84d7f522d094ab4964b4721e0be4.png)

4.Test Code 1:

**Find code blocks:**

![img](./media/af81635991bc0ed2597f080716945a4c.png)

![img](./media/6d4b455db85ed2c550ac1592ac16bd80.png)

**Build blocks:**

Initialize serial monitor and MPU6050.

![img](./media/f115d6971f08e40bedd3a60ce1b913ab.png)

This block is used to update the data each time it is fetched. 

![img](./media/c432dcb1bed8ecf23d15634bc6fc76e2.png)

![img](./media/de113a2dc7f4772b958a038760633838.png)

**Complete code:**

![img](./media/59b490f5d8810ef434eeab9915eab5a5.png)

5.Test Result 1：

After uploading code and powering on, Put ESP32 Easy Coding Board flatwise on the desk, press the reset button to initialize MPU6050, and wait 2 or 3 seconds.

When the serial monitor shows values, the initialization is completed; and if values on each axis is less than 10, the initialization is correct; otherwise you need to re-initialize it.

![img](./media/f76470488f2793026eaa3a9777264b70.png)

![img](./media/4b8d194edc5f4038c774def1b63c87a9.png)

3.9 Light Intensity

![img](./media/db8f895ba85dd2552a29030fc4ab5a3b.png)

1.Introduction:

Photoresistors measure light intensity and are commonly used to detect brightness in the surrounding environment.

**Working principle:** This module is designed by the light-sensitive materials. There are two main types: photoresistor and photodiode.

- **Photoresistor:** The resistance of a photoresistor varies with the intensity of ambient light. For one photoresistor, the  stronger the ambient light, the lower the resistance will be.
- **Photodiode:** The current output of a photodiode is proportional to the intensity of the incident light. The electrical signals they produce can be used to measure light brightness.

**Applications:** Photoresistors are widely applied to various fields, including light control systems, lighting systems,  camera exposure control, light monitoring, automatic adjustment of screen brightness, etc.

**Unit of brightness:** They usually measure light intensity in illuminance units (such as Lux). Illuminance represents the luminous flux per unit area.



2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/4f8ac5efacc04d3f15e4f804abe70fc0.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/26110bd63d838c6377849040b83e3a08.png) |

3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/a4dc84d7f522d094ab4964b4721e0be4.png)

4.Test Code:

**Find code blocks:**

![img](./media/af81635991bc0ed2597f080716945a4c.png)

![img](./media/a34af46f2d6c4adcd279577d384c4140.png)

**Build blocks:**

![img](./media/9b4f562e8a890d3e1dc381beda252483.png)

5.Test Result：

Upload the test code and open the serial monitor. When the light intensity detected by the sensor changes, the sensor values will also change.

![img](./media/d9f8b4dc97dcc96b69404cd6af8eab3d.png)

![img](./media/d4dd0d09cb97e98597d05b8c7dc05f8d.png)

3.10 Read SD Card

![img](./media/dbc96c166250e3277c3d9553eedf0ed6.png)

1.Introduction

The SD card module is used in conjunction with the MCU on the ESP32  Easy Coding Board for reading and writing data on the SD (Secure  Digital) card. This module makes it easier to use SD cards to store and access data in projects.

- **Function:** SD card module allows the ESP32 Easy Coding Board to communicate with the SD card to achieve data reading and writing. This is very useful for data logging, file storage, logging,  etc.

- **Interface:** The SD card module usually connects  to the ESP32 Easy Coding Board using the Serial Peripheral Interface  (SPI) interface. It needs to be connected to the corresponding pin of the ESP32 Easy Coding Board, For example, MOSI (Master Out Slave In),  MISO (Master In Slave Out), SCK (Serial Clock), and CS (Chip Select).

- **SD card type:** SD card modules are generally compatible with various types, including standard SD cards, SDHC cards  (High Capacity), and SDXC cards (extended Capacity).

  

2.Components:

| ESP32 Easy Coding Board*1            | ![img](./media/4f8ac5efacc04d3f15e4f804abe70fc0.png)   |
| ------------------------------------ | ---------------------------------------- |
| USB type C  Cable*1                  | ![img](./media/26110bd63d838c6377849040b83e3a08.png)   |
| SD Card*1（not included in the kit） | ![img](./media/4f70bcfd89ff384a12d0485c91f63c8f.png) |

3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/a4dc84d7f522d094ab4964b4721e0be4.png)

Insert the SD card into the slot.

![img](./media/76163cdf839040406681820aacee0475.png)

![img](./media/80b3aa025cccd44caa354ad0d2956010.png)

4.Test Code:

**Find code blocks:**

![img](./media/c0552cba50bec2bb8e0c8b79016bdca2.png)

Initialize the serial monitor and SD card.

![img](./media/eed2df7b094e85a16d5b6b8ab42b2c38.png)

Refresh the SD data before using.

![img](./media/bd795191701ef148993854501fb3021d.png)



Read SD card type

![img](./media/0b423ee426ccfad1731d395164cbb4dc.png)

Serial port output:

![img](./media/6f69553ae20d4ce1e41df5c0a16399de.png)

Read SD card message

![img](./media/b361a714f678faf06b680a5c97fda77c.png)

![img](./media/532312c650f787990abc6f1b31db8a62.png)

Serial monitor output：

![img](./media/1cf023931e9089a3746e2322aa75c81c.png)

File：

Determine whether there is a ‘’file.txt‘’ file in SD card.

![img](./media/35c090aad4f8f8e7b66be865e22ace57.png)

If there is no ‘’file.txt‘’, create a file and input “hello,world” in a new line.

![img](./media/ad4b85727d676a2577e264cfd0aaee8a.png)

After that, read the content in ‘’file.txt‘’.

![img](./media/f597166b6cac865f382f52e566106a6c.png)

Read all list files in SD card, including hidden files.

![img](./media/10451ce84e7e1dc26f45fcdbd71f9ab0.png)

Delete this ‘’file.txt‘’.

![img](./media/74bde7aecbf49401cdf8f3e2121d9706.png)

**Complete code:**

![img](./media/4a4b43efbbd304584ec05f0fde3a01fd.png)

Serial monitor output:

![img](./media/4bee2f4a6ab0b20ab9f5107984893871.png)

3.11 Read ESP32 Easy Coding Board Current

![img](./media/2da227a2e63416e1f6dd94baa3c9eb4f.png)

1.Introduction

ESP32 Easy Coding Board boasts a built-in current measurement module  (only measure USB power supply and PH2.0 interface power supply) to  measure current by a resistive current sensor.

Resistive current sensor is commonly used to monitor the current  value by measuring the voltage drop generated by the current through the resistance. The working principle of such sensors is based on Ohm’s  law, which states that when a current passes through a resistor, the voltage generated at both ends of the resistor is proportional to the current.

![img](./media/832bba6595b35e2c6b63b43ec42359fb.png)

- **Current sensing:** Resistive current sensor contains a current sensing element, usually a resistor. When current passes through this resistor, a voltage drop will be generated at both ends of the resistor, the magnitude of which is proportional to the strength of the current.
- **Voltage output:** By measuring the voltage drop at both ends of the resistor, the sensor can provide a voltage signal that is related to current. This voltage signal can be digitally processed by devices like an analog-to-digital converters (ADC).

Resistive current sensors are widely applied to power system monitoring, power consumption measurement of electronic devices,  electric vehicle current monitoring and so on.



2.Components:

| ESP32 Easy Coding Board*1 | ![img](./media/4f8ac5efacc04d3f15e4f804abe70fc0.png) |
| ------------------------- | -------------------------------------- |
| USB type C Cable*1        | ![img](./media/26110bd63d838c6377849040b83e3a08.png) |

3.Connection:

Connect the ESP32 Easy Coding Board to your computer via USB cable.

![img](./media/a4dc84d7f522d094ab4964b4721e0be4.png)

4.Test Code 1:

**Read current value:**

![img](./media/6fe6280d99638de85029008a5b0bc120.png)

![img](./media/f1e692b195a31232855914a5917c764c.png)

5.Test Result 1：

After uploading test code, open the serial monitor and you will see the current value is 0. Because many modules are not working on the board,  so the current is close to 0.

![img](./media/5429cd95980c433e8637209a321ef913.png)

6.Test Code 2:

Enable RGB dot matrix and then measure the current value.

Initialize the serial monitor and RGB dot matrix.

![img](./media/11e9caa3dd539f00a8adb12b52c01dec.png)

First measure 10 RGBs.

![img](./media/0bb06d5e3ec3b1fe85c514b87d001a6e.png)

Then measure 18 RGBs.

![img](./media/8de8b3a5f13fe04dc374b54b115eb6d1.png)

Last measure 25 RGBs.

![img](./media/fb92b17a8a6e32f4dd457a6bc4275057.png)

**Complete code:**

![img](./media/4f32fc1463133d03992f0ff3f71996c8.png)

7.Test Result 2:

Upload test code and you will find that the more the RGB, the larger the current will be.

![img](./media/b22d109c823d56aa84006181841386a0.png)

8.Test Code 3:

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


![img](./media/603ba0ec54833da5e008579e80773dd2.png)

![img](./media/bf2925bb49b892ea50f34da98bdaebbf.png)

![img](./media/138d6da2dee2b41bb9ddc40731b4cabf.png)

Assign the read current value to variable I.

![img](./media/28006926353d2e311c5167f2a1fa87d6.png)

I multiplies by 3.3 is power of the ESP32 Easy Coding Board(the board voltage is 3.3V).

![img](./media/4bd35043342c25b0b113c2a7c128641a.png)

**Complete code:**

![img](./media/ba5fe3631c4aaa98011c621395270e2a.png)

9.Test Result 3:

Upload code and open serial monitor to set baud rate. The more the RGBs, the greater the current value and power will be.

![img](./media/2ebecb69f942006aa38d48dc9d15d491.png)

3.12 Wifi Wireless Communication

ESP32 Easy Coding Board is built with Wi-Fi (2.4G) and Bluetooth (4.2)  to easily connect to a Wi-Fi network and communicate with other devices in the network, so you can use this Board to display web pages in your browser.

![img](./media/acc2f14244d38b448897ff5397b2de5d.png)

ESP32 Easy Coding Board WiFi Function

- **Base mode (STA / Wi-Fi Client mode)**: ESP32 Easy Coding Board is connected to a Wi-Fi hotspot (AP).
- **AP mode (Soft-AP / Wi-Fi hotspot mode)**: Other Wi-Fi devices connect to ESP32 Easy Coding Board.
- **AP-STA mode**: ESP32 Easy Coding Board is both a Wi-Fi hotspot and a Wi-Fi device connected to another Wi-Fi.
- These modes support multiple security modes: WPA, WPA2, WEP, etc.
- Wi-Fi hotspots can be searched (active and passive scanning).
- Support hybrid mode monitoring of IEEE802.11 Wi-Fi packets.

------

For more wifi reference, please visit：[https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/network/esp_wifi.html](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/network/esp_wifi.html)

Espressif Official：[https://www.espressif.com.cn/en/home](https://www.espressif.com.cn/en/home)

![img](./media/b4fdfdedf9494c9535fce6a6be913113.png)

------

wifi Web Page

Add an extension of web page editing.

![img](./media/7cb2c9917c343b06bf195888204651dc.png)

![img](./media/77304610624761f9eae57e5580c3d610.png)



![img](./media/d6b277643f8c60696259c8eb4bd9533e.png)

![img](./media/21f70beae826af2028d916eab1a3afa3.png)

Connect a Wifi and input your wifi name and passwords. After connecting, the IP address will be printed on the serial monitor.

![img](./media/d7de9119b64c5894d0c3006c1f3003b6.png)

![img](./media/8e1581c2c9209e3f27b228791621293a.png)

Set up a web component named **temperature** in the unit of ℃.

![img](./media/baa152c1b25963a0c2800f06b7571e44.png)

![img](./media/b18704ff30a7b4a504086c56010e2676.png)

Add a button module named **button**.

![img](./media/21da077c0a0ecd203ac21cc8682dcd0f.png)

![img](./media/a1977b46870d355d0156b640d08fd439.png)

**Complete code:**

![img](./media/20434681f6ce3f6ca772dadf9882d3be.png)

As long as connecting the Wi-Fi, you may use the Web Server Library of ESP32 Easy Coding Board to provide web page.

In the example, we set up a simple web page to display a certain temperature value.

**Open your browser to check and visit the IP address of ESP32  Easy Coding Board. Herein, you may access to “http://[IP address of  ESP32 Easy Coding Board]” to visit its website.**

**NOTE: When PC, mobile phone and ESP32 Easy Coding Board are connected to one network, this website(your own IP address of ESP32 Easy Coding Board) can be accessed via PC and mobile at the same time.**



PC：

![img](./media/a6ae13afc3f26dc52a57ca05a8916a8e.png)

Mobile：

![img](./media/0c04c5513169733e22b726164218bee8.png)


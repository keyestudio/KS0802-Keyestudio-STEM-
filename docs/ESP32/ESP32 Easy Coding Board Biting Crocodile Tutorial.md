# Hand Biting Crocodile

## 1.Servo

### 1.1 Introduction

Servo is a position control rotary actuator. It mainly consists of a housing, a circuit board, a core-less motor, a gear and a position sensor. Its working principle is that the servo receives the signal sent by MCUs or receivers and produces a reference signal with a period of 20ms and width of 1.5ms, then compares the acquired DC bias voltage to the voltage of the potentiometer and obtain the voltage difference output.

In general, servo has three wires: brown, red and orange. The brown wire is grounded, the red one is a positive pole wire and the orange one is a signal  wire.

![wps2-1687239587616-2](./media/wps2-1687239587616-2.jpg)

The rotation angle of servo is controlled by regulating the duty cycle of PWM (Pulse-Width Modulation) signal. The standard cycle of PWM signal is 20ms (50Hz). Theoretically, the width is distributed between 1ms-2ms, but in fact, it's between 0.5ms-2.5ms. The width corresponds the rotation angle from 0° to 180°. 

![image-20230620134023059](./media/image-20230620134023059.png)

### 1.2 Specification

Working voltage: DC 4.8V~6V

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
|      io16       | S（Yellow） |

![Servo](./media/Servo.png)

### 1.4 Code

<p style="color:red;">Note: The rotation angle of the servo is 0-180 degrees, but if the crocodile has been assembled, the angle must be rotated between 55-130 degrees, otherwise the servo will get hot and burn out.</p>

**Code File：**

Download link：[Download](.\Code\BitingCrocodileTutorialCodes.zip)

Download the code file and unzip it, then double-click `1-Servo_Code1.sb3` to open the file and upload the code.

![image-20240409115915246](./media/image-20240409115915246.png)

**Add code manually：**

1.Drag out the `when Arduino begin` module from `Events`.

![image-20240408134535477](./media/image-20240408134535477.png)

2.Drag out the `forever` module from the `Control` and place it under the `when Arduino begin` module.

![image-20240408134844456](./media/image-20240408134844456.png)

3.Tap![an35](./media/an35.png)to find and load servo，then tap “Back”（Details of loading modules are in the development board basic tutorial).

![image-20240408135027322](./media/image-20240408135027322.png)

4.Drag out the servo angle module from the `Servo` , set the pin to IO14, the angle to 110 degrees, and the time to 1000ms, then place it in the `forever` module.

![image-20240408135443465](./media/image-20240408135443465.png)

5.Drag out the servo angle module from `Servo`, set the pin to IO14, the angle to 90 degrees, and the time to 1000ms, and place it below the previous servo angle module.

![image-20240408135542964](./media/image-20240408135542964.png)

6.Drag out the servo angle module from `Servo`, set the pin to IO14, the angle to 55 degrees, and the time to 1000ms, and place it below the previous servo angle module, then tap ![image-20240408135722831](./media/image-20240408135722831.png) to upload the code.

![image-20240408135631602](./media/image-20240408135631602.png)

### 1.5 Test Result

After uploading the code, the crocodile will open its mouth for 1s, then close half of its mouth for 1s, and then completely close its mouth. 

### 1.6 Extended Tutorial

Earlier we have controlled the crocodile to open and close its mouth at a wide angle, so how to control the crocodile to slowly close and open its mouth?

#### 1.6.1 Code

**Code File：**

Download link：[Download](.\Code\BitingCrocodileTutorialCodes.zip)

Download the code file and unzip it, then double-click `1-Servo_Code2.sb3 `to open the file and upload the code.

![image-20240409115949754](./media/image-20240409115949754.png)

**Add code manually：**

1.Drag out the `when Arduino begin` module from `Events`.

![image-20240408134535477](./media/image-20240408134535477.png)

2.Drag out the `forever` module from the `Control` and place it under the `when Arduino begin` module.

![image-20240408134844456](./media/image-20240408134844456.png)

3.Drag out the `repeat` module from `Control` , set the repeat value to 55, then place it in the `forever` module.

![image-20240408140220338](./media/image-20240408140220338.png)

4.Drag out the declare variable module from `Variable Type` , set the variable Type to int, Name to angle, Assigned to to 55, and place it under the `when Arduino begin` module.

![image-20240408140802954](./media/image-20240408140802954.png)

5.Drag out the variable ++ module from  `Variable Type`, set Name to angle, and add it in the `repeat` module.

![image-20240408141034933](./media/image-20240408141034933.png)

6.Drag out the servo angle module from `Servo`, set servo PIN# to IO14, degree to the variable module in the `Variable Type` , variable name to angle, delay to 30 (ms), then place it under the variable ++ .

![image-20240408141235222](./media/image-20240408141235222.png)

7.Click on the `repeat` module, then right-click and click "Duplicate", then place it under the `repeat` module.

![image-20240408141641186](./media/image-20240408141641186.png)

8.Modify the variable ++ module to the variable -- module. Click the ++ area to switch it.

![image-20240408141959921](./media/image-20240408141959921.png)

**Complete Code：**

![KidsBlock Project-1712557255201](./media/KidsBlock%20Project-1712557255201.png)

#### 1.6.2 Test Result

After uploading the code, the crocodile will slowly open its mouth and then slowly close it.

## 2.Ultrasonic Module

### 2.1 Introduction

The HC-SR04 ultrasonic sensor uses sonar to determine distance to an object like what bats do. It offers excellent non-contact range detection with high accuracy and stable readings in an easy-to-use package. It comes complete with an ultrasonic transmitter and receiver modules.

 It is being used in a wide range of electronics projects for creating obstacle detection and distance measuring application as well as various other applications.

### 2.2 Specification

Working voltage:+5V

Quiescent current: <2mA

Working current: 15mA

Effective angle: <15°

Distance range: 2cm – 400 cm

Accuracy: 0.3 cm

Measuring angle: 30 degrees

Trigger input pulse width: 10 microseconds

![wps3-1687242720835-4](./media/wps3-1687242720835-4.jpg)

### 2.3 Wiring Diagram

| Expansion Board | Module |
| :-------------: | :----: |
|       GND       |   G    |
|       3V3       |   V    |
|    P8 / io4     |  Trig  |
|   P12 / io15    |  Echo  |

![ultrasonic](./media/ultrasonic.png)

### 2.4 Code

<p style="color:red">Note: The measuring distance of ultrasonic is 2-300cm, but after being assembled on the crocodile, it can only detect 4-30cm. For the ultrasonic receives the bounced signal at a certain angle, but the basswood board of the crocodile body blocks it. As a result, only 30cm can be recognized, but this does not affect our hand-biting crocodile tutorial.</p>

**Code File：**

Download link：[Download](.\Code\BitingCrocodileTutorialCodes.zip)

Download the code file and unzip it, then double-click `2-Ultrasonic_Code.sb3 `to open the file and upload the code.

![image-20240409120027866](./media/image-20240409120027866.png)

**Add code manually：**

1.Drag out the `when Arduino begin` module from `Events`.

![image-20240408134535477](./media/image-20240408134535477.png)

2.Drag out the `forever` module from the `Control` and place it under the `when Arduino begin` module.

![image-20240408134844456](./media/image-20240408134844456.png)

3.Drag out the serial baudrate module from the `Serial` , set begin baudrate to 9600, and then place it under the `when Arduino begin` module.

![image-20240409094334194](./media/image-20240409094334194.png)

4.Drag out the declare variable module from `Variable Type` , set the variable Type to int, Name to distance, Assigned to to 0, and place it under the begin baudrate module.

![image-20240409094504446](./media/image-20240409094504446.png)

5.Drag out the set variable by module from the `Variable Type`, change the variable name to "distance", and then place it in the `forever` module.

![image-20240409094659743](./media/image-20240409094659743.png)

6.Drag out the read ultrasonic distance module from the `Ultrason`, set the trig pin to IO4, the echo pin to IO15, the read distance to cm, and then place it in the white box of the set variable by module.

![image-20240409095006509](./media/image-20240409095006509.png)

7.Drag out the serial print module from the `Serial` , set the print mode to "warp", and then place it under the set variable by module.

![image-20240409095215543](./media/image-20240409095215543.png)

8.在`Variable Type`栏中拖出`variable`模块，修改变量名为distance，然后放到串口打印模块的白色框中

![image-20240409095334013](./media/image-20240409095334013.png)

9.在`Control`栏拖出拖出延时模块，设置延时为0.3，然后放到串口打印模块下面，这样我们的代码就搭建完成了

![image-20240409093905594](./media/image-20240409093905594.png)

### 2.5 代码结果

上传代码后，如图点击右上角的串口打印区，然后点击有下架的![image-20240409095810773](./media/image-20240409095810773.png)设置波特率为9600（一般默认是9600无需设置)

![image-20240409095718342](./media/image-20240409095718342.png)

设置完成后我们便能在串口打印区看到超声波感应到的距离了，串口打印距离会每个0.3s打印一次

![image-20240409100122569](./media/image-20240409100122569.png)



## 3.按键控制鳄鱼咬合

### 3.1 简介

通过ESP32 Easy Coding Board板载的AB按键控制鳄鱼张嘴与闭嘴。

### 3.2 代码

**代码文件：**

代码文件下载链接：[点击下载代码文件](.\Code\BitingCrocodileTutorialCodes.zip)

下载代码文件后解压，然后双击`3-Key_controlled_crocodile_Code.sb3`打开文件进行上传代码

![image-20240409130125783](./media/image-20240409130125783.png)

**自己动手添加代码：**

1.添加`whrn Arduino begin`模块与初始化RGB点阵与舵机的状态，最开始为张嘴状态

![image-20240409110135033](./media/image-20240409110135033.png)

2.在`Control`栏拖出判断代码块放到`forever`模块中，设置判断条件为按键A是否被按下，并在判断代码块中添加RGB点阵显示红色哭脸的代码和舵机旋转到55度的代码

![image-20240409110800297](./media/image-20240409110800297.png)

3.复制第一个判断模块的代码，然后修改RGB点阵显示绿色笑脸，舵机旋转到110度

![image-20240409111238580](./media/image-20240409111238580.png)

**完整代码：**

![Ultrasonic_Code-1712632430694](./media/Ultrasonic_Code-1712632430694.png)

### 3.3 代码结果

上传代码成功后，按下板载的按键A鳄鱼显示红色哭脸并且鳄鱼嘴巴闭合 ，按下板载的按键B鳄鱼显示绿色微笑并且鳄鱼嘴巴张开。

## 4.鳄鱼咬手

### 4.1 简介

咬手鳄鱼，鳄鱼张开嘴巴当你把手伸进鳄鱼嘴巴的时候鳄鱼上面的超声波会测量手到鳄鱼嘴巴里的深度，当达到我们设置好的深度的时候鳄鱼就会咬下。

### 4.2 代码

**代码文件：**

代码文件下载链接：[点击下载代码文件](.\Code\BitingCrocodileTutorialCodes.zip)

下载代码文件后解压，然后双击`4-Crocodile_Bite_Code.sb3`打开文件进行上传代码

![image-20240409130229411](./media/image-20240409130229411.png)

**自己动手添加代码：**

1.初始化中设置波特率为9600,声明两个int类型变量distance（distance用于存放超声波测量的距离）与item（item用于随机生成数值的存放）其中item的初始值为5，设置舵机角度为110度，RGB点阵显示绿色笑脸

![image-20240409131930068](./media/image-20240409131930068.png)

2.在`forever`中添加将超声波测量的距离赋值给distance变量，然后进行打印使用串口打印模块不换行打印字符进行区分，然后打样数据换行这样就能将字符与数值打印到一行中，颜色0.2s

![image-20240409133354446](./media/image-20240409133354446.png)

3.使用判断模块对distance与item里面的值进行对比如果distance里面的值小于item里面的值则执行判断模块里面的代码。使用随机生成数值模块并设置成随机生成3-9之间的数这样就可以到达鳄鱼咬手的随机性的效果，time初始值是5下一次的值是随机生成。添加RGB点阵显示红色哭脸代码，然后添加舵机选择角度为55度的代码这样鳄鱼就咬合了，延时3秒钟后舵机旋转到110度鳄鱼张嘴，然后RGB点阵显示绿色微笑，在延时1.5s。

![image-20240409133945088](./media/image-20240409133945088.png)

**完整代码：**

![4-Crocodile_Bite_Code](./media/4-Crocodile_Bite_Code.png)

### 4.3代码结果

上传代码成功后鳄鱼张嘴，RGB点阵显示绿色微笑，手往鳄鱼嘴里申当手离超声波的距离满足鳄鱼咬合条件时，鳄鱼咬合RGB点阵显示红色哭脸，咬合3秒钟后鳄鱼松嘴并且RGB点阵显示绿色笑脸，最后的1.5秒延时是为了可以将手从鳄鱼嘴里缩回来准备的。1.5s过后进入下一个咬手过程。




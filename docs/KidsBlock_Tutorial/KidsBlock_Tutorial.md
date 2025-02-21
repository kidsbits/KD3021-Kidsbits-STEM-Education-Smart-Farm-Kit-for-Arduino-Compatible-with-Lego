# KidsBlock Tutorial

## 1. Mainboard_Introduction:

<span style="color: rgb(255, 76, 65);">**Refer to the link：**</span>[http://kd2076-kidsbits-stem-electronic-building-block-programming.readthedocs.io/](http://kd2076-kidsbits-stem-electronic-building-block-programming.readthedocs.io/)

## 2. KidsBlock Development Environment Configuration:


<span style="color: rgb(0, 209, 0);">**Please refer to the link to install and use the KidsBlock software：** </span>
[https://kidsblocksite.readthedocs.io/en/latest/](https://kidsblocksite.readthedocs.io/en/latest/)

<span style="color: rgb(255, 76, 65);">**Note:** The control board used in this kit is the kidsIOT board. For importing the kidsIOT board, libraries and sample codes, please refer to the following content.</span>


1\. Click![Img](media/152.png) to enter the main page, and select the control board needed. In this project, we select the kidsIOT mainboard and click **Connect**, then it is connected. Click Go to Editor to return the code editor. Icon![Img](media/153.png) will change into ![Img](./media/2.png) and ![Img](media/155.png) will change into ![Img](media/156.png). This means the kidsIOT mainboard and ports（COM)are connected.

![5](media/5.png)

![6](media/6.png)

![7](media/7.png)



![image8](media/8.png)

2\. If the kidsIOT mainboard is connected , but icon![Img](media/161.png) doesn’t change into ![Img](media/162.png). You need to click to connect the COM port. Click![Img](media/163.png). Then you will find a page pop up, showing Connected.

![image](media/666.png)

![8](media/8.png)

![9](media/9.png)

To disconnect the port, just click![Img](media/165.png) and Disconnect.

![10](media/10.png)



<span style="color: rgb(255, 76, 65);">Note：If you want to update libraries of KidsBlock, click then Clear cache and restart.</span>

![12](media/12.png)

3\. ![Img](media/172.png)stands for extension libraries of sensors and modules. Click ![Img](media/173.png)to enter the page of extension libraries, click a sensor or module to add. For example, if click the **esp32 passive buzzer** module,**Not loaded** will change into **Loaded**. Then the passive buzzer![Img](media/174.png) is added.                           
![img](media/15.png)

![image](media/16.png)

![image](media/17.png)

Click![Img](media/178.png) to return to the code editor. Then you can view the passive buzzer in the blocks area.

![image](media/18.png)

If you want to delete the **passive buzzer**, click![Img](media/180.png) to select the “**esp32 Passive buzzer**”![Img](media/181.png). Then **Loaded** will change into **Not loaded**. Then the passive buzzer is deleted.

![image](media/17.png)

![image](media/16.png)

The way of deleting other sensors or modules is as same as the passive buzzer.

4\. How to open SB3 type files：

The first method： Double-click SB3 type files to open them. For instance, open![Img](./media/23.png), then we need to double-click it.

![image](media/24.png)

The second method: Open Kidsblock，click **file** and **Load from your computer**，then select the SB3 type file on the computer.（for example![Img](./media/23.png))

![image](media/25.png)

![image](media/26.png)



![image](media/24.png)


## 3. Projects:

### Project 01: Lighting System

![Img](./media/1-0.jpg)

#### 1. Description

As an introductory project for smart farms, lighting up LED is one of the most basic KidsBlock (based on Scratch) practical projects. It is designed to let beginners understand the hardware and software programming of kidsIOT board (based on ESP32) and master basic circuit and programming knowledge.

In this project, you will learn the basic connections and settings of the kidsIOT board in the KidsBlock graphical programming environment, as well as control the digital pin to output level to control the state of LEDs, LED breathing lights, and button control of LEDs, and you can also apply them in your home or lounge. 

#### 2. Components

|![Img](./media/A1.png)|![Img](./media/A8.png)|![Img](./media/A2.png)|
| :--: | :--: | :--: |
|kidsIOT Mainboard×1|White LED Module×1|Button Module×1|
|![Img](./media/A19.png)|![Img](./media/A21.png)|![Img](./media/A29.png)|
|USB Cable×1|Wire×2| Lighting System LEGO Pieces×1 |

![Img](./media/1-1.png)

#### 3. Assembly Steps

##### Step 1:Components Needed

![Img](./media/Z-1-1.png)

##### Step 2: Process

Process 1：

![Img](./media/Z-1-2.png)

Process 2：

![Img](./media/Z-1-3.png)

Process 3：

![Img](./media/Z-1-4.png)

Process 4：

![Img](./media/Z-1-5.png)

Process 5：

![Img](./media/Z-1-6.png)

Process 6：

![Img](./media/Z-1-7.png)

Process 7：

![Img](./media/Z-1-8.png)

Complete

![Img](./media/Z-1-9.png)

#### 4. Wiring Diagram

| Module |kidsIOT Mainboard |
| :--: | :--: |
| White LED Module |No.2 port（control pin is io2） |
|Button Module|No.4 port（control pin is io27）|

Connect the kidsIOT mainboard to your computer via USB cable.

![Img](./media/1-2.png)

#### 5. State of LED

![Img](./media/1-3.png)

##### (1). Knowledge

（1）To keep the light on, the electricity is needed. When we say that  there is electricity, we mean that there is current flowing through an  electrical appliance like a light. Current comes to our home from the  power station via wires. And the generator of a power station is the  power supply, which enables to provide voltage and current. The battery  we usually use is also the power supply. Wires can be used to conduct  electricity, which connect a path for the current to flow. This path is  called a circuit. If we want to make a lamp emit light, both a power supply and a complete circuit are needed.

![img](media/1-4.png)



##### (2). Programming Steps

###### Step 1：Description of the Building Blocks

![Img](./media/1-5.png)

This block indicates that when the kidsIOT board is started, the code will be run.

![image](media/1-6.png)

Set **input** or **output** to the specified pin. **input** means input mode,**output** means output mode. Select **input-pullup** can set the input mode for the pin and make it become high level.

![image](media/1-7.png)

Set **high** or **low** to the specified pin. Select **high** means to set high level for the pin. If there is voltage and current, the LED will be on. Select **low** means to set low level for the pin. If there is no voltage and current, the LED will be off.

![image](media/1-8.png)

This is a delay block. The number 1 can be changed to whatever number of seconds it is delayed.

![image](media/1-9.png)

It will do one thing forever.

###### Step 2：Write the Program

① Open the KidsBlock(based on Scratch)software to select the kidsIOT board and port(COMx).

![Img](./media/1-10.png)

② Drag the instruction block ![Img](media/1-11.png)in the **Events** module to the script area.

![Img](./media/1-12.png)

③ Drag the instruction block ![Img](./media/1-13.png) in the "**Pin**" module to the script area. Since the white LED module is connected to the No. 2 interface on the mainboard (<span style="color: rgb(255, 76, 65);">The control pin is io2</span>) and it is in output mode, so change "**input**" to "**output**".

![Img](./media/1-14.png)

④ Drag the block ![Img](./media/1-15.png) in the "**Control**" module to the script area.

![Img](./media/1-16.png)

⑤ Drag the block ![Img](./media/1-17.png) in the "**Pin**" module to ![Img](./media/1-15.png).

![Img](./media/1-19.png)

⑥ Drag the block ![Img](./media/1-8.png) in the "**Control**" module to ![Img](./media/1-15.png) and set to delay **1** second.

![Img](./media/1-22.png)

⑦ Copy the code block ![Img](./media/1-23.png) into ![Img](./media/1-15.png), and change "**High**" to "**Low**".

![Img](./media/1-25.png)

 

##### (3). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT mainboard. After powering up via the USB cable, the white LED will be on and off for 1s.

We can also realize breathing light effect, flowing water light effect and police light effect via LEDs.

| Level | Function |
| :--: | :---: |
| high | LED lights up |
| low | LED lights off |

#### 6. LED Breathing LED

![Img](./media/1-28.png)

##### (1). Knowledge

The IO port on the kidsIOT mainboard outputs digital signals, which can only output high level and low level. For example, in the lighting up LEDs project, the digital output of the ESP32 is used, which has only two levels: high (3.3V) and low (0V).

Assuming that the high level of the kidsIOT board is 3.3V and the low level is 0V, then if you want to output a voltage between 0 and 3.3V, you need to use PWM (Pulse Width Modulation). PWM can output different voltage values, like a progress bar, which is analog output.

![Img](./media/1-29.png)

PWM uses digital control to generate square waves with different duty cycles (a signal that constantly switches between high level and low level) to control the analog output.

![Img](./media/1-29-1.png)

PWM has three elements: frequency (Hz), period (s) and duty cycle (%)

- **PWM frequency (f):** It refers to the number of PWM cycles in one second.

- **PWM period (T):** Period=1/frequency (T=1/f, where 1 is 1 second), for example: the frequency is 50Hz, which means that one period is 20ms, then one second is 50 PWM cycles.
- **PWM duty cycle:** It refers to the ratio of high level time to the entire cycle time within a pulse cycle. For example: the cycle time is 10ms, the pulse width time is 8ms, then the low level time is 2ms, and the total duty cycle is 8/(8+2)= 80%.

![Img](./media/1-30.png)

PWM can change the effective output voltage by changing the duty cycle in one cycle under the appropriate signal frequency. Among the levels output by the IO port at the specified time, the more high levels, the greater the PWM value and the brighter the LED.

![Img](./media/1-31.png)

##### (2). Programming Steps

###### Step 1：Description of the Building Blocks

The following are "**Variable**" command blocks.

![Img](./media/1-32.png)

This block is used to create "<span style="color: rgb(255, 76, 65);">Variable</span>". You can declare "global" or "local", or set the type, name and value of the variable, item is the variable name.

![Img](./media/1-33.png)

Get variable item.

![Img](./media/1-34.png)

Set the value of variable item.

![Img](./media/1-35.png)

Set the variable item mode to increase item by 1 or decrease item by 1 every time the loop is executed.

![image](media/1-121.png)

Set the string variable item.

![Img](./media/1-37.png)

![Img](./media/1-38.png)

This block is used to set the PWM. You need to set the corresponding pin via the channel (a total of 16 channels (0~15)) and the output value, so that the PWM value can be output.

![Img](./media/1-39.png)

This is a conditional loop control statement that exit the loop when the number of loops is met. For example: 10 means that the loop is executed 10 times. The number 10 can be changed to other numbers.

###### Step 2：Write the Program

① Drag the instruction block ![Img](media/1-11.png)in the **Events** module to the script area.

![Img](./media/1-12.png)

② Drag the instruction block ![Img](./media/1-13.png) in the "**Pin**" module to the script area, change "**input**" to "**output**".

![Img](./media/1-14.png)



③ Drag the block ![Img](./media/1-44.png) in the "**Variable Type**" module to the script area.

![Img](./media/1-45.png)

④ Drag blocks ![Img](./media/1-46.png) and ![Img](./media/1-39.png) in the "**Control**" module to the script area.

![Img](./media/1-48.png)

⑤ Drag the instruction block![Img](./media/1-49.png)in the "**Pin**" module to the script area.

![Img](./media/1-50.png)

⑥ Drag the block![Img](./media/1-33.png)in the "**Variable Type**" module to the script area.

![Img](./media/1-52.png)

⑦ Drag the block![Img](./media/1-53.png)in the "**Variable Type**" module to the script area，"**++**" means that each time the loop is executed, **item** will be increased by **1**.

![Img](./media/1-54.png)

⑧ Drag the block ![Img](./media/1-8.png) in the "**Control**" module to the script area and set the delay to **0.01** second, the repeat **10** to **255**, for the corresponding PWM code block outputs 0~255. In this way, the LED light will slowly turn from dark to bright.

![Img](./media/1-56.png)

⑨  Copy the code block ![Img](./media/1-57.png)，change “**++**” to “**--**”, then LED will slowly turn from bright to dark.

![Img](./media/1-58.png)

⑩ Complete Program

![Img](./media/1-59.png)

##### (3). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT motherboard. After powering up via the USB cable, the LED will gradually brighten and then dim,  like breathing.

#### 7. Read the value of the button module

![Img](./media/1-61.png)

##### (1). Knowledge

The principle of the button module is based on the switch circuit.

When the button is pressed, the switch closes, allowing current to pass through the button to GND, then the digital input pin of the kidsIOT motherboard detects a low level signal.

When not pressed, the switch is in the off state, the pin is pulled high by the pull-up resistor, and the digital input pin detects a high-level signal.

##### (2). Programming Steps

###### Step 1：Description of the Building Blocks

![Img](./media/1-62.png)

The block is used to set serial baud rate(generally, the baud rate 9600 is taken as an example)

![Img](./media/1-63.png)

This block is used to set print mode for the serial port. **warp** means line feed printing, **no-warp** means no line feed printing, **HEX** means hexadecimal printing.

![Img](./media/1-64.png)

It is used to read the digital signal value of the specified pin（0 or 1).

###### Step 2：Write the Program

① Drag the instruction block ![Img](media/1-11.png)in the **Events** module to the script area.

![Img](./media/1-12.png)



② Drag the instruction block![image](media/1-67.png) in the **Serial** module to the script area and take the baud rate 15200 as an example.

![Img](./media/1-68.png)

③ Drag the block ![Img](./media/1-69.png) in the "**Pin**" module to the script area. Since the button module is connected to No. 4 port ( <span style="color: rgb(255, 76, 65);">the control pin is io27</span>) , so change pin IO2 to IO27.

![Img](./media/1-70.png)

④ Drag the block ![Img](./media/1-44.png) in the "**Variable Type**" module to the script area, then change item to “<span style="color: rgb(255, 76, 65);">Button</span>”.

![Img](./media/1-72.png)

⑤ Drag the block ![Img](./media/1-15.png) in the "**Control**" module to the script area.

![Img](./media/1-74.png)

⑥ Drag the block ![Img](./media/1-75.png) in the "**Variable Type**" module to the script area, then change item to “<span style="color: rgb(255, 76, 65);">Button</span>”.

![Img](./media/1-76.png)

⑦ Drag the block ![Img](./media/1-77.png) in the "**Pin**" module to the script area, then change pin IO2 to IO27.

![Img](./media/1-78.png)

⑧ Drag the instruction block![image](media/1-79.png) in the **Serial** module to the script area. 

![Img](./media/1-80.png)

⑨ Drag the block ![Img](./media/1-81.png) in the "**Variable Type**" module to the script area, then change item to “<span style="color: rgb(255, 76, 65);">Button</span>”.

![Img](./media/1-82.png)

⑩Drag the block ![Img](./media/1-8.png) in the "**Control**" module to the script area and set the delay to **0.1** second.

![Img](./media/1-84.png)

⑪ Complete Program

![Img](./media/1-85.png)

##### (3). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT motherboard. After powering up via the USB cable, click ![Img](./media/1-87.png) in the serial monitor and set the baud rate to 15200. When the button is not pressed, the serial monitor prints the digital signal 1, when pressed, the digital signal 0 is printed.

![Img](./media/1-88.png)

#### 8. Self-locking button function

![Img](./media/1-89.png)

##### (1). Knowledge

Self-locking button: It locks when pressed and will not automatically pop up. It will pop up only when pressed again, which is very similar to a switch. The switch can be turned on and off using self-locking buttons. If it is controlled by the kidsIOT mainboard, this operation can also be achieved via software.

##### (2). Programming Steps

###### Step 1：Description of the Building Blocks

![Img](./media/1-90.png)

It is a conditional statement code executing if-then function: If the logical judgment statement in ![Img](media/338.png) is satisfied, the code statement below **then** is executed.

![Img](./media/1-92.png)



It is a conditional statement: If the logical judgment statement in ![image](media/99999.png)is satisfied, the loop will be executed continuously. If not, the loop will be terminated.

![Img](./media/1-93.png)

It is a conditional statement code executing if-then-else function: If the logical judgment statement in ![Img](media/338.png) is satisfied, the code statement below **then** is executed, otherwise, the code below **else** is executed.

###### Step 2：Write the Program

① First define a Value to get the button status, and then define a Button. At the same time, select the serial baud rate to 15200 and the control button pin IO27 to "**input**" mode.

![Img](./media/1-94.png)

②Assign the read button value to "<span style="color: rgb(255, 76, 65);">Value</span>".

![Img](./media/1-95.png)

③ Determine whether the button is pressed. When pressed, change the value of "<span style="color: rgb(255, 76, 65);">Button</span>" and print it.

![Img](./media/1-96.png)

<span style="color: rgb(255, 76, 65);">**Description**：</span>

![Img](./media/1-97.png)

The delay of 0.01 seconds is the button anti-shake function.
After detecting that the button is closed, a delay program is executed, with a delay of 5ms ～ 10ms (depending on the mechanical characteristics). After the jitter disappears, the button status is detected again. If the closed state level is still maintained, then a button is pressed.

When it is released, a delay of 5ms ～ 10ms is also required. Only after the jitter disappears can the button processing program be transferred.
When the button is pressed once, the button becomes 1, when pressed again, it becomes 0.


④ Complete Program

![Img](./media/1-98.png)

##### (3). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT motherboard. After powering up via the USB cable, click ![Img](./media/1-87.png) in the serial monitor and set the baud rate to 15200. When the button is pressed, the serial monitor prints the number 1, and when pressed again, the monitor prints the number 0, so as to achieve the self-locking function of buttons.

![Img](./media/1-100.png)

#### 9. Lighting control system

![Img](./media/1-101.png)

##### (1). Programming Steps

###### Step 1：Flow Chart

![Img](./media/1-102.png)

###### Step 2：Write the Program

① Based on the code of the self-locking button above, add the relevant blocks for turning the LED on and off.

![Img](./media/1-103.png)

② Complete Program

![Img](./media/1-104.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT motherboard, then power up via the USB cable. When the button is pressed for the first time, the LED is turned on. When pressed for the second time, the LED is turned off. When pressed for the third time, the LED is turned on again..., which is consistent with the LED switch in real life.

![Img](./media/1-107.jpg)

#### 10. Common Problems

##### Q1: There are errors in kidsIOT board programming program

A: Please check whether the board type is correct.

Please check whether the USB port number is selected correctly.

##### Q2: The LED does not light up after burning the code

A: Please confirm whether the pins in the code are consistent with the actual wiring. If there is an error, please wire correctly according to the pins in the code.

##### Q3: Are the buttons insensitive? Sometimes it can be detected, sometimes not?

A: Modify the button delay time and set it to an appropriate delay.

![Img](./media/1-106.png)


### Project 02: Light Controlled System

![Img](./media/2-0.jpg)

#### 1. Description

This light controlled system is composed of a photoresisitor, a LED and a kidsIOT mainboard, which can realize intelligent lighting control, saving energy and improving usage efficiency.

It empowers to automatically detect day and night as well as light intensity, making the entire system more intelligent and energy-saving.

When the ambient brightness is lower than the set value, the photoresisitor will detect a signal and automatically turn on the LED; when higher than the set value, it will send another signal to turn off the LED.

#### 2. Components

|![Img](./media/A1.png)|![Img](./media/A5.png)|![Img](./media/A8.png)|
| :--: | :--: | :--: | 
|kidsIOT Mainboard×1|Photoresistor×1|White LED Module×1|
|![Img](./media/A21.png)|![Img](./media/A19.png)|![Img](./media/A30.png)|
|Wire×2|USB Cable×1| Light Controlled System LEGO Pieces×1 |

![Img](./media/2-1.png)

#### 3. Assembly Steps

##### Step 1：Components Needed

![Img](./media/Z-2-1.png)

##### Step 2：Process

Process 1：

![Img](./media/Z-2-2.png)

Process 2：

![Img](./media/Z-2-3.png)

Process 3：

![Img](./media/Z-2-4.png)

Process 4：

![Img](./media/Z-2-5.png)

Process 5：

![Img](./media/Z-2-6.png)

Complete

![Img](./media/Z-2-7.png)

(<span style="color: rgb(255, 76, 65);">Note: Do not dismantle it, it will still be used in project 10.</span>)

#### 4. Wiring Diagram

| Module |kidsIOT Mainboard |
| :--: | :--: |
| White LED Module |No.2 port（control pin is io2） |
|Photoresistor|No.4 port（control pin is io39）|


Connect the kidsIOT mainboard to your computer via USB cable.

![Img](./media/2-2.png)

#### 5. Read the value of the photoresistor

![Img](./media/2-3.png)

##### (1). Programming Steps

###### Step 1：Description of the Building Blocks

![Img](./media/2-4.png)

It is used to read the analog signal value of the specified pin.

###### Step 2：Write the Program

① Set the baud rate to 15200.

![Img](./media/1-68.png)

② Set the pin IO39 connected to the photoresistor ( <span style="color: rgb(255, 76, 65);">control pin io39</span>) to the "**input**" mode.

![Img](./media/2-6.png)

③ Define a "<span style="color: rgb(255, 76, 65);">Photosensor</span>" variable to store the value of the photoresistor.

![Img](./media/2-7.png)

④ Store the read value of the photoresistor in the "<span style="color: rgb(255, 76, 65);">Photosensor</span>" variable.

![Img](./media/2-8.png)

⑤ Complete Program

![Img](./media/2-9.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT motherboard. After powering up via the USB cable, click ![Img](./media/1-87.png) in the serial monitor and set the baud rate to 15200. Then the serial monitor will print the value read by the photoresistor. When the light detected by the photoresistor is brighter, the monitor prints a larger value, otherwise, the monitor prints a smaller value.

![Img](./media/2-12.png)

#### 6. Light Controlled System

![Img](./media/2-13.png)

##### (1). Programming Steps

###### Step 1：Flow Chart

![Img](./media/2-14.png)

###### Step 2：Write the Program

① Delete the "<span style="color: rgb(255, 76, 65);">Wait 0.5 seconds</span>" block in the complete program above, and then drag "**Set pin IO2 mode input**" block from the "**Pin**" module to the script area. Change "**input**" to "**output**".

![Img](./media/2-15.png)

② Determine the value read by the photoresistor. When the value is less than or equal to 700, the LED will turn on, otherwise, the LED will turn off.

![Img](./media/2-16.png)

③ Complete Program

![Img](./media/2-17.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT motherboard, then power up via the USB cable. When the light is strong during the day and the value of  the photoresistor is greater than 700, the LED will turn off. After dark, when the value is less than or equal to 700, the LED will automatically turn on.

![Img](./media/2-19.jpg)

#### 7. Common Problems　

##### Q1: The value detected by the photoresistor cannot be 0?

A: Because in actual operation, even if all the lights are turned off and the room is very dark, the value is only close to 0.

##### Q2: After burning the sample code, why can’t the LED light up even when the lights are turned off in the room?

A: You can set the value read by the photoresistor to be larger. The value in the sample code is 700, which can be adjusted to 1000 or even larger.



### Project 03:  Automatic Feeding System

![Img](./media/3-0.webp)

#### 1. Description

The automatic feeding system is composed of a kidsIOT main board, an ultrasonic sensor and a servo. The ultrasonic sensor is used to detect the distance of pets in the feeding area. When the pet approaches the food bowl, the sensor detects that the distance is getting closer. After triggering the signal, it controls the servo to open the feed box and automatically feed the animals.

#### 2. Components

|![Img](./media/A1.png)|![Img](./media/A6.png)|![Img](./media/A7.png)|![Img](./media/A14.png)|
| :--: | :--: | :--: | :--: |
|kidsIOT Mainboard×1|Ultrasonic Adapter Board×1|Ultrasonic Sensor×1|Servo×1|
|![Img](./media/A21.png)|![Img](./media/A19.png)|![Img](./media/A32.png)| |
|Wire×1|USB Cable×1| Automatic Feeding System LEGO Pieces×1 | |

![Img](./media/3-1.png)

#### 3. Assembly Steps

##### Step 1：Components Needed

![Img](./media/Z-3-1.png)

##### Step 2：Process

Process 1：

![Img](./media/Z-3-2.png)

Process 2：

![Img](./media/Z-3-3.png)

Process 3：

![Img](./media/Z-3-4.png)

Process 4：

![Img](./media/Z-3-5.png)

Process 5：

![Img](./media/Z-3-6.png)

Process 6：

![Img](./media/Z-3-7.png)

Process 7：

![Img](./media/Z-3-8.png)

Process 8：

![Img](./media/Z-3-9.png)

Process 9：

![Img](./media/Z-3-10.png)

Process 10：

![Img](./media/Z-3-11.png)

Process 11：

![Img](./media/Z-3-12.png)

Process 12：

![Img](./media/Z-3-13.png)

Process 13：

![Img](./media/Z-3-14.png)

Process 14：

![Img](./media/Z-3-15.png)

Process 15：

![Img](./media/Z-3-16.png)

Process 16：Initialize the servo angle

Wiring of servo
![Img](./media/Z-3-17.png)

First write the following code in KidsBlock software and upload the code to the kidsIOT mainboard, then the servo will rotate 190° . (<span style="color: rgb(255, 76, 65);">Note: If the servo can not rotate, you can press the RESET button on the kidsIOT board.</span>)

![Img](./media/Z-3-18.png)

Process 17：

![Img](./media/Z-3-19.png)

Process 18：

![Img](./media/Z-3-20.png)

Process 19：

(<span style="color: rgb(255, 76, 65);">Note: Do not twist the servo</span>)

![Img](./media/Z-3-21.png)

Process 20：

![Img](./media/Z-3-22.png)

Process 21：

![Img](./media/Z-3-23.png)

Complete

![Img](./media/Z-3-24.png)

#### 4. Wiring Diagram

| Module |kidsIOT Mainboard |
| :--: | :--: |
| Ultrasonic Adapter Board |No.9 port（Trig--io18，Echo--io19） |
|Servo|G/V/io33 port（Brown→G，Red→V，Orange→io33）|



| Ultrasonic Sensor | Ultrasonic Adapter Board |
| :--: | :--: |
| Vcc | VCC |
| Trig | Trig |
| Echo | Echo |
| Gnd | GND |

Connect the kidsIOT mainboard to your computer via USB cable.

![Img](./media/3-2.png)

#### 5. Servo rotation

![Img](./media/3-3.png)

##### (1). Programming Steps

###### Step 1：Description of the Building Block

![Img](./media/1-38.png)

Set the servo's channel and output (rotation) angle to the specified PWM pin.

###### Step 2：Write the Program

① Set the pin IO33 (<span style="color: rgb(255, 76, 65);">control pinio33</span>) connected to the servo to "**Output**" mode.

![Img](./media/3-5.png)

② Initialize the control channel of the servo to CH2 (LT1) and the initial angle to <span style="color: rgb(255, 76, 65);">190°</span>, with a delay of 0.5 seconds.

![Img](./media/3-6.png)

③ The servo rotates from 190° to 120° and then to 60° every 0.5 seconds.

![Img](./media/3-7.png)

④ Complete Program

![Img](./media/3-8.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT motherboard, then power up via the USB cable, then servo will rotate.

#### 6. Read the Value of Ultrasonic Sensor

![Img](./media/3-10.png)

##### (1). Programming Steps

###### Step 1：Add the Ultrasonic Sensor

Tap the “Sensor” module in the “Extension” , then select “**Ultrasonic Sensor**” and click ![Img](media/781.png)to return to the programming interface.

![Img](./media/3-13.png)

![Img](./media/3-14.png)

![Img](./media/3-15.png)

###### Step 2：Description of the Building Block

![Img](./media/3-16.png)

This block is used to measure distance to the specified pin, and the distance unit can be cm or inch.

###### Step 3：Write the Program

① Set the baud rate to 15200.

![Img](./media/1-68.png)

② Set the Trig pin of the ultrasonic sensor <span style="color: rgb(255, 76, 65);">IO18</span> to "**output**" mode, and the Echo pin <span style="color: rgb(255, 76, 65);">IO19</span> to "**input**" mode.

![Img](./media/3-18.png)

③ Set Trig to <span style="color: rgb(255, 76, 65);">IO18</span> and Echo to <span style="color: rgb(255, 76, 65);">IO19</span>, and the serial port prints the distance value detected by the ultrasonic sensor at 0.1 second intervals.

![Img](./media/3-19.png)

④ Complete Program

![Img](./media/3-20.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT motherboard. After powering up via the USB cable, click ![Img](./media/1-87.png) in the serial monitor and set the baud rate to 15200. Move your hand in front of the ultrasonic sensor. When you are close to it, the displayed distance value becomes smaller. When you move away from it, the value becomes larger.

![Img](./media/3-23.png)

#### 7. Automatic Feeding System

![Img](./media/3-24.png)

##### (1). Programming Steps

###### Step 1：Flow Chart

![Img](./media/3-25.png)

###### Step 2：Programming Steps

① Set the baud rate to 15200, the Trig pin of the ultrasonic sensor <span style="color: rgb(255, 76, 65);">IO18</span> to "**output**" mode, and the Echo pin <span style="color: rgb(255, 76, 65);">IO19</span> to "**input**" mode.

![Img](./media/3-26.png)

② Set the pin IO33 connected to the servo to "**Output**" mode, initialize the control channel of the servo to CH2 (LT1) and the initial angle to <span style="color: rgb(255, 76, 65);" >190°</span>, delay 0.5 seconds.

![Img](./media/3-27.png)

③ Define a "<span style="color: rgb(255, 76, 65);">Distance</span>" global variable to store the distance value detected by the ultrasonic sensor.

![Img](./media/3-28.png)

④ Set the Trig pin and Echo pin of the ultrasonic sensor, and print the read distance value of the ultrasonic sensor on the serial port.

![Img](./media/3-29.png)

⑤ Determine the distance detected by the ultrasonic sensor. If 2cm < distance value < 7cm, the feed box will be opened; otherwise, it will be closed.

![Img](./media/3-30.png)

⑥ Complete Program

![Img](./media/3-31.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT motherboard. After powering up via the USB cable, click ![Img](./media/1-87.png) in the serial monitor and set the baud rate to 15200. If an animal is detected within 2cm-9cm, the feed box will be opened  to feed the animal.

![Img](./media/3-34.jpg)

#### 8. Common Problems　

##### Q1: Why doesn’t the servo work?

A: It may be stuck. Before assembling the servo, use the code to adjust it to 80°.

##### Q2: Why is the detection distance inaccurate when using the ultrasonic sensor?

A: Measurement should be started from the transmitting head of the ultrasonic sensor. This module is not a high-precision ultrasonic distance detection module and may exist errors.

![Img](./media/3-34.png)

### Project 04: Anti-theft Alarm System

![Img](./media/4-0.jpg)

#### 1. Description

The anti-theft alarm system is composed of a PIR motion sensor, a buzzer, a LED and a kidsIOT mainboard. When programming via the KidsBlock, you are able to judge whether someone is moving by reading the digital signal detected by the PIR motion sensor. If someone is moving, the buzzer will sound an alarm and the LED will flash to alert the user that someone has entered the area. Thus, a low-cost anti-theft alarm system can be realized, which is suitable for homes or offices.



#### 2. Components

|![Img](./media/A1.png)|![Img](./media/A4.png)|![Img](./media/A10.png)|![Img](./media/A14.png)|
| :--: | :--: | :--: | :--: |
|kidsIOT Mainboard×1|PIR Motion Sensor×1|Passive Buzzer×1|Servo×1|
|![Img](./media/A21.png)|![Img](./media/A19.png)|![Img](./media/A31.png)|  |
|Wire×2|USB Cable×1| Anti-theft Alarm System LEGO Pieces×1 |  |

![Img](./media/4-1.png)

#### 3. Assembly Steps

##### Step 1：Components Needed

![Img](./media/Z-4-1.png)

##### Step 2：Process

Process 1：

![Img](./media/Z-4-2.png)

Process 2：

![Img](./media/Z-4-3.png)

Process 3：

![Img](./media/Z-4-4.png)

Process 4：

![Img](./media/Z-4-5.png)

Process 5：

![Img](./media/Z-4-6.png)

Process 6：Initialize the servo angle

Wiring of  servo(it is the same as project 03)

![Img](./media/Z-4-7.png)

First write the following code in KidsBlock software and upload the code to the kidsIOT mainboard, then the servo will rotate 180° . (<span style="color: rgb(255, 76, 65);">Note: If the servo can not rotate, you can press the RESET button on the kidsIOT board.</span>)

![Img](./media/Z-4-8.png)

Process 7：(Place the three Lego boxes on the same side, then assemble the four gears.)

![Img](./media/Z-4-9.png)

Process 8：

![Img](./media/Z-4-10.png)

Process 9：

![Img](./media/Z-4-11.png)

Process 10：

![Img](./media/Z-4-12.png)

Complete 1：

![Img](./media/Z-4-13.png)

Process 11：Share the LEGO board with project 03

![Img](./media/Z-4-14.png)

Complete 2：

![Img](./media/Z-4-15.png)


#### 4. Wiring Diagram

| Module |kidsIOT Mainboard |
| :--: | :--: |
| PIR Motion Sensor |No.4 port（control pin is io27） |
|Passive Buzzer|No.6 port（control pin is io23）|
|Servo|G/V/io33 port（Brown→G，Red→V，Orange→io33）|

Connect the kidsIOT mainboard to your computer via USB cable.

![Img](./media/4-2.png)

#### 5. Passive buzzer makes sound

![Img](./media/4-3.png)

##### Method 1

###### (1). Knowledge

The passive buzzer is driven by square waves. Let's simulate the square waves below.
The high and low levels of the pin can simulate a square wave: keeping the high level for 1000us and the low level for 1000us can make the buzzer sound.

![Img](./media/4-4.png)

Changing the time of high and low level can change the sound volume of the buzzer. You can try changing it to 1500us, 2000us, 3000us...

###### (2). Write the Program

① Initialize the buzzer's pin **IO23** and "**Output**" mode.

![Img](./media/4-5.png)

② Set the buzzer pin **IO23** to "**High**" and "**Low**". Here we take the delay of 0.001 second (1000 microseconds) as an example to make the buzzer emit sound.

![Img](./media/4-6.png)

The delay function is a microsecond delay, which means the time delay is 1000 microseconds.

<span style="color: rgb(255, 76, 65);">Note: The conversion relationship between seconds, milliseconds and microseconds is: 1 second = 1000 milliseconds = 1000000 microseconds. </span>


By f=1/T, changing high and low levels in 1000us, we can know that the frequency of such a square wave is 1000Hz (that is, the number of high and low level changes per second is 1000 times).

③ Complete Program

![Img](./media/4-7.png)

###### (3). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT motherboard. After powering up via the USB cable, the passive buzzer will make sound.

##### Method 2

###### (1). Knowledge

Use the "passive buzzer" code block to drive.
The "passive buzzer" code block can generate a fixed-frequency PWM signal to drive the passive buzzer to sound. The sounding time length (beat) and sounding frequency can be controlled via parameters.

![Img](./media/4-9.png)

###### (2). Add “passive buzzer” 

Tap the “Actuator” module in the “Extension” , then select “**<span style="color: rgb(255, 76, 65);">esp32 Passive buzzer</span>**” and click ![Img](media/781.png)to return to the programming interface.

![Img](./media/3-13.png)

![Img](./media/4-13.png)

![Img](./media/4-14.png)

###### (3). Description of the Building Block

![Img](./media/4-9.png)

Set the frequency and beat of the passive buzzer to the specified pin.

![Img](./media/4-16.png)
Set the passive buzzer to play specific music to the specified pin.

![Img](./media/4-17.png)

Set the passive buzzer to make no sound to the specified pin.

###### (4). Write the Program

① Initialize the buzzer's pin **IO23** and "**Output**" mode.

![Img](./media/4-5.png)

② Set the sound pin, frequency and beat can be selected by yourself.

![Img](./media/4-19.png)

③ Produce different tones.

![Img](./media/4-20.png)

④ Complete Program

![Img](./media/4-21.png)

###### (5). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT motherboard. After powering up via the USB cable, the passive buzzer will make sounds with different tones.

#### 6. Passive buzzer plays music

![Img](./media/4-23.png)

###### (1). Write the Program
① The buzzer pin is <span style="color: rgb(255, 76, 65);">**IO23**</span>, and then select a piece of music (we take **Birthday** as an example here) .

![Img](./media/4-24.png)

② Complete Program

![Img](./media/4-25.png)

###### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT mainboard. After powering up via the USB cable, the passive buzzer will play a "Happy Birthday" music.



#### 7. Read the value of PIR Motion Sensor

![Img](./media/4-27.png)

###### Step 1：Write the Program

① Set the baud rate to 15200.

![Img](./media/1-68.png)

② Set the pin IO27 connected to the PIR motion sensor to "**input**" mode.

![Img](./media/4-29.png)

③ Define a "<span style="color: rgb(255, 76, 65);">PIR_motion_sensor</span>" global variable to store the value of the sensor.

![Img](./media/4-30.png)

④ Store the read value of the sensor in the <span style="color: rgb(255, 76, 65);">"PIR_motion_sensor</span>" variable and print it on the serial port.

![Img](./media/4-31.png)

⑤ Complete Program

![Img](./media/4-32.png)

###### Step 2：Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT motherboard. After powering up via the USB cable, click ![Img](./media/1-87.png) in the serial monitor and set the baud rate to 15200. 

When the sensor detects movement of a person or animal, the serial monitor window prints 1, and the red LED on the sensor will be off; otherwise, the monitor prints 0, and the red LED on the sensor will be on.

<span style="color: rgb(255, 76, 65);">Note: The sensor does not have penetrating capabilities. When detecting human movement, please do not block it.</span>


![Img](./media/4-35.png)

#### 8. Anti-theft Alarm System

![Img](./media/4-36.png)

##### (1). Programming Steps

###### Step 1：Flow Chart

![Img](./media/4-37.png)

###### Step 2：Write the Program

①Set the baud rate to 15200, the IO27 pin of PIR motion sensor to "**input**" mode.

![Img](./media/4-29.png)

② Set the pin IO33 connected to the servo to "**Output**" mode, initialize the control channel of the servo to CH2 (LT1) and the initial angle to <span style="color: rgb(255, 76, 65);" >90°</span>, delay 0.5 seconds.

![Img](./media/4-39.png)

② Define a "<span style="color: rgb(255, 76, 65);">PIR_motion_sensor</span>" global variable to store the value of the PIR motion sensor.

![Img](./media/4-40.png)

③ Store the read value of the sensor in the <span style="color: rgb(255, 76, 65);">"PIR_motion_sensor</span>" variable.

![Img](./media/4-41.png)

④ Judge whether the sensor detects that a person or animal is moving. When someone or an animal is moving, the buzzer sounds, the servo rotates to close the door, and the serial monitor prints "Someone"; otherwise, the buzzer does not sound, the servo rotates to open the door, and the monitor prints " No one".

![Img](./media/4-42.png)

⑤ Complete Program

![Img](./media/4-43.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT mainboard. After powering up via the USB cable, click ![Img](./media/1-87.png) in the serial monitor and set the baud rate to 15200. 

When the sensor detects that someone or an animal is moving, the buzzer sounds, the servo rotates to close the door, and the serial monitor prints "Someone"; otherwise, the buzzer does not sound, the servo rotates to open the door, and the monitor prints "No one".

![Img](./media/4-46.png)

![Img](./media/4-47.jpg)

#### 9. Common Problems　

##### Q1: The tone of the passive buzzer is not accurate to the actual tone?

A: The tones simulated by ordinary passive buzzers cannot meet the requirements of professional tones. If you need accurate tones, you need to use a more professional passive buzzer.

##### Q2: Does the PIR motion sensor make false alarms?

A: ① Non-professional PIR motion sensor.

② The requirements for the sensor to avoid false alarms are as follows:
Within the detection range, avoid objects that are caused by the wind, such as curtains, clothing, flowers, etc.
Avoid interference from strong light within the detection range, such as sunlight, car lights, spotlights, lighting and other light sources.


### Project 05：Rainwater Control System

<span style="color: rgb(255, 76, 65);">Note: Sprinkling water on other sensors will cause a short circuit and device failure. Sprinkling water on batteries will cause heating and explosion. Please be careful when using the device, especially when used by young children, it must be under the supervision of parents. To ensure safe operation of the device, please follow relevant usage guidelines and safety regulations.</span>


![Img](./media/5-0.jpg)

#### 1. Description

This project explains how to use a steam sensor, a passive buzzer and a kidsIOT board to make a rain detection system. When the sensor detects rain, it sends a signal to the kidsIOT mainboard to trigger various actions. 

For example, the buzzer can be used to sound an alarm to alert the user that it is raining. This system is able to monitor rainfall in gardening, agriculture, and detect leaks in roofs or buildings. The sensor can be easily connected to the kidsIOT motherboard to form a simple rain detection system.


#### 2. Components

|![Img](./media/A1.png)|![Img](./media/A3.png)|![Img](./media/A10.png)|
| :--: | :--: | :--: |
|kidsIOT Mainboard×1|Steam Sensor×1|Passive Buzzer×1 |
|![Img](./media/A21.png)|![Img](./media/A19.png)|![Img](./media/A33.png)|
|Wire×2|USB Cable×1| Rainwater Control System LEGO Pieces×1 |

![Img](./media/5-1.png)

#### 3. Assembly Steps

##### Step 1：Components Needed



![Img](./media/Z-5-1.png)

##### Step 2：Process

Process 1：

![Img](./media/Z-5-2.png)

Process 2：

![Img](./media/Z-5-3.png)

Process 3：

![Img](./media/Z-5-4.png)

Process 4：

![Img](./media/Z-5-5.png)

Process 5：

![Img](./media/Z-5-6.png)

Process 6：

![Img](./media/Z-5-7.png)

Process 7：

![Img](./media/Z-5-8.png)

Process 8：

![Img](./media/Z-5-9.png)

Process 9：

![Img](./media/Z-5-10.png)

Complete：

![Img](./media/Z-5-11.png)

#### 4. Wiring Diagram

| Module |kidsIOT Mainboard |
| :--: | :--: |
| Steam Sensor |No.6 port（control pin is io36） |
|Passive Buzzer|No.8 port（control pin is io5）|

Connect the kidsIOT mainboard to your computer via USB cable.

![Img](./media/5-2.png)

#### 5. Read the analog value of the steam sensor

![Img](./media/5-3.png)

###### Step 1：Write the Program

① Set the baud rate to 15200.

![Img](./media/1-68.png)

② Set the pin IO36 connected to the steam sensor to "**input**" mode.

![Img](./media/5-5.png)

③ Define a "<span style="color: rgb(255, 76, 65);">Steam_sensor</span>" global variable to store the analog value of the steam sensor.

![Img](./media/5-6.png)

④ Store the read analog value of the sensor in the "<span style="color: rgb(255, 76, 65);">Steam_sensor</span>" variable and print it on the serial port.

![Img](./media/5-7.png)

⑤ Complete Program

![Img](./media/5-8.png)

###### Step 2：Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT motherboard. After powering up via the USB cable, click ![Img](./media/1-87.png) in the serial monitor and set the baud rate to 15200. 

Then the serial monitor will print the value(range：0~4095) read by the steam sensor. Touch the detection area on the sensor with a moistened finger, the larger the area, the greater the value!

![Img](./media/5-11.png)

#### 6. Rainwater Control System

![Img](./media/5-12.png)

##### (1). Programming Steps

###### Step 1：Flow Chart

![Img](./media/5-13.png) 

###### Step 2：Add “passive buzzer” 

![Img](./media/5-14.png) 

###### Step 3：Write the Program
①Set the baud rate to 15200, the IO36 pin of steam sensor to "**input**" mode.

![Img](./media/5-15.png)

② Define a "<span style="color: rgb(255, 76, 65);">Steam_sensor</span>" global variable to store the analog value of the steam sensor.

![Img](./media/5-16.png) 

③  Receive analog value of the sensor and print it on the serial port.

![Img](./media/5-17.png)

④ Determine the received analog value of the sensor. When 800≤analog value<2000, the buzzer will sound alarm 1.

![Img](./media/5-18.png)

⑤ Determine the received analog value of the sensor. When 2000≤analog value<4000, the buzzer will sound alarm 2.

![Img](./media/5-19.png)

⑥ Determine the received analog value of the sensor. When analog value≥4000, the buzzer will sound alarm 3.

![Img](./media/5-20.png)

⑦ Complete Program

![Img](./media/5-21.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT mainboard. After powering up via the USB cable, when the rain value detected by the sensor is larger, the buzzer alarm sound will be louder.

![Img](./media/5-23.jpg)

#### 7. Common Problems　

##### Q1: Is the steam sensor waterproof?

A: The detection area can be exposed to water, but when detecting water, please be careful not to use too much water.

##### Q2: After the sensor detects water, the alarm still sounds after a long time?

A: The passive buzzer keeps alarming because there are still water stains in the detection area of the sensor. Just clean it.



### Project 06：Temperature and Humidity Control System

![Img](./media/6-0.png)

#### 1. Description

This project introduces how to use a kidsIOT mainboard, a temperature and humidity sensor, a fan and an OLED display to build an intelligent temperature and humidity control system.

The system can measure ambient temperature and humidity and control fans to cool down and dehumidify based on demand. When the temperature or humidity exceeds the set threshold, it will automatically turn on the fan to reduce the temperature or humidity in the environment below the set value to protect the animals and plants on the farm. 

What's more, it enables to adjust the ambient temperature and humidity and display them on the OLED display.


#### 2. Components

|![Img](./media/A1.png)|![Img](./media/A11.png)|![Img](./media/A12.png)| ![Img](./media/A21.png)|![Img](./media/A20.png)|
| :--: | :--: | :--: |:--: |:--: |
|kidsIOT Mainboard×1|Motor×1|Temperature and Humidity Sensor×1|Wire×2|Battery Holder×1|
|![Img](./media/A27.png)|![Img](./media/A19.png)|![Img](./media/A34.png)|![Img](./media/A28.png) | |
|Fan×1|USB Cable×1| Temperature and Humidity System LEGO Pieces×1 | AA Battery（<span style="color: rgb(255, 76, 65);">Not provide</span>）×6 | |

![Img](./media/6-1.png)

#### 3. Assembly Steps

##### Step 1：Components Needed

![Img](./media/Z-6-1.png)

##### Step 2：Process

Process 1：

![Img](./media/Z-6-2.png)

Process 2：

![Img](./media/Z-6-3.png)

Process 3：

![Img](./media/Z-6-4.png)

Process 4：

![Img](./media/Z-6-5.png)

Complete：

![Img](./media/Z-6-6.png)

#### 4. Wiring Diagram

| Module |kidsIOT Mainboard |
| :--: | :--: |
| Temperature and Humidity Sensor |No.6 port（control pin is io23） |
|Motor|No.9 port（IN+control pin is io18，IN-control pin is io19）|

Connect the kidsIOT mainboard to your computer via USB cable, connect the external power supply and turn the DIP switch on the mainboard to ON end.

![Img](./media/6-2.png)

#### 5. OLED Display

![Img](./media/6-3.png)

##### (1). Programming Steps

###### Step 1：Description of the Building Block

![Img](./media/6-4.png)

This block is used to initialize the OLED’s width, height and an I2C address.

![Img](./media/6-5.png)

This is a command block for drawing a straight line from the initial position x0:0 y0:0 to the final position x1:32 y1:16. The number in the  block can be changed.

![Img](./media/6-6.png)

This is a command block that draws a recta with a width of 32 and a  height of 16 from the initial position x:0 y:0, the numbers can be  changed.

![Img](./media/6-7.png)

This is a command block that draws a rectangle with a width of 32 and a  height of 16 from the initial position x:0 y:0, the numbers can be  changed.

![Img](./media/6-8.png)

This is the command block that draws a circle with a radius of 8 starting from the initial position x:16 y:16.

![Img](./media/6-9.png)

This is the command block that fills a circle with a radius of 8 starting at an initial position of x:16 y:16.

![Img](./media/6-10.png)

This is the command block that draws a round rectangle with width 32,  height 16, and radius 4 starting from an initial position of x:16 y:16.

![Img](./media/6-11.png)

This is the command block that fills a round rectangle with width 32,  height 16 and radius 4 starting from initial position x:16 y:16.

![Img](./media/6-12.png)

This is the command block to draw a triangle from three positions x0:0 y0:0, x1:16 y1:0 and x2:8 y2:16.

![Img](./media/6-13.png)

This is the command block that fills the triangle between the three positions x0:0 y0:0, x1:16 y1:0 and x2:8 y2:16.

![Img](./media/6-14.png)

This is a command block for setting text size and color and background color.

![Img](media/6-15.png)

This is the command block that sets the cursor position.

![Img](./media/6-16.png)

This is a command block for setting the way of printing strings on the OLED screen. “**warp”** means newline printing, “**no-warp**” means no newline printing.

![Img](./media/6-17.png)

This is the command block to set the OLED display pattern.

![Img](./media/6-18.png)

This is the command block to clear the OLED screen.

![Img](./media/6-19.png)

This is the command block to refresh the OLED screen and display the next content.

![Img](./media/6-20.png)

This is a command block that sets strings to start scrolling in a certain direction.

![Img](./media/6-21.png)

This is the command block to set stop scrolling.

###### Step 2：Write the Program

① Initialize the OLED with width 128, height 64 and I2C address 0x78 (0x3c).

![Img](./media/6-22.png)

② Set the text size displayed on the OLED to 6x8, the text color to white and the background color to black.

![Img](./media/6-23.png)

③ OLED displays straight lines.

![Img](./media/6-24.png)

④ The OLED displays the straight line and delays 1 second.

![Img](./media/6-25.png)

⑤ The OLED displays rectangle and delays 1 second.

![Img](./media/6-26.png)

⑥ The OLED displays fill rectangle and delays 1 second.

![Img](./media/6-27.png)

⑦ The OLED displays circle and delays 1 second.

![Img](./media/6-28.png)

⑧ The OLED displays fill circle and delays 1 second.

![Img](./media/6-29.png)

⑨ The OLED displays round rectangle and delays 1 second.

![Img](./media/6-30.png)

⑩ The OLED displays fill round rectangle and delays 1 second.

![Img](./media/6-31.png)

⑪ The OLED displays triangle and delays 1 second.

![Img](./media/6-32.png)

⑫ The OLED displays fill triangle and delays 1 second.

![Img](./media/6-33.png)

⑬ The OLED displays smile face and delays 1 second.

![Img](./media/6-34.png)

⑭The OLED displays angry face and delays 1 second.

![Img](./media/6-35.png)

⑮ The OLED displays cry face and delays 1 second.

![Img](./media/6-36.png)

⑯ The OLED displays “↑” and delays 1 second.

![Img](./media/6-37.png)

⑰ The OLED displays “↓” and delays 1 second.

![Img](./media/6-38.png)

⑱ The OLED displays “←” and delays 1 second.

![Img](./media/6-39.png)

⑲ The OLED displays “→” and delays 1 second.

![Img](./media/6-40.png)

⑳ The OLED displays “❤” and delays 1 second.

![Img](./media/6-41.png)

㉑ Set the cursor position of the OLED to display the "Hello, KidsBlock" string at x:0 y:30 with a delay of 1 second.

![Img](./media/6-42.png)

㉒ Complete Program

![Img](./media/6-43.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT motherboard. After powering up via the external power supply, the OLED display on the kidsIOT board displays various patterns and English letters.


#### 6. Fan rotates

![Img](./media/6-45.png)

##### (1). Programming Steps

###### Step 1：Add “DC Motor” 

Tap ![Img](./media/6-46.png), click the “Actuator” module in the “Extension” , then select “**<span style="color: rgb(255, 76, 65);">DC Motor for esp32</span>**” and click ![Img](media/781.png)to return to the programming interface.

![Img](./media/6-48.png)

![Img](./media/6-49.png)

![Img](./media/6-50.png)

###### Step 2：Description of the Building Block

![Img](./media/6-51.png)

Set the high and low level states of the motor INA pin and INB pin.

![Img](./media/6-52.png)

Set the high and low level status of the motor INA pin and the analog output value of the INB pin in certain channels.
If the INA pin is in a high-level state, the smaller the INB analog output value, the faster the fan rotates; and if the INA pin is in a low-level state, the larger the INB analog output value, the faster the fan rotates.

###### Step 3：Write the Program

① The pin INA of the motor module is IO18, the level is low, the INB pin is IO19, the channel is CH0 (LT0), and the analog output value is 0, then the motor does not rotate.

![Img](./media/6-53.png)

② Set the motor pin INA to low level and the analog output value of the INB pin to different values, then the motor rotates clockwise at different speeds.

![Img](./media/6-54.png)

③ Set the motor to stop rotating for 3 seconds.

![Img](./media/6-55.png)

④ Set the motor pin INA to high level and the analog output value of the INB pin to different values, then the motor rotates anticlockwise at different speeds.

![Img](./media/6-56.png)

⑤ Set the motor to stop rotating for 3 seconds.

![Img](./media/6-57.png)

⑥ Complete Program

![Img](./media/6-58.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT motherboard. After powering up via the external power supply, the motor rotates clockwise at different speeds and stops for 3 seconds, and then rotates counterclockwise at different speeds and stops for 3 seconds.

#### 7. Read data from the temperature and humidity sensor

![Img](./media/6-60.png)

##### (1). Programming Steps

###### Step 1：Add “temperature and humidity sensor” 

Tap ![Img](./media/6-46.png), click the “Sensor” module in the “Extension” , then select “**<span style="color: rgb(255, 76, 65);">DHT sensor for esp32</span>**” and click ![Img](media/781.png)to return to the programming interface.

![Img](./media/6-63.png)

![Img](./media/6-64.png)

![Img](./media/6-65.png)

###### Step 2：Description of the Building Block

![Img](./media/6-66.png)

Initialize the pin and mode of the temperature and humidity sensor (dht11, dht21 or dht22).

![Img](./media/6-67.png)

Read the temperature and humidity from the temperature and humidity sensor.

###### Step 3：Write the Program

① Set the baud rate to 15200.

![Img](./media/1-68.png)

② Initialize pin IO23 of the temperature and humidity sensor, and select the dht11 mode.

![Img](./media/6-69.png)

③ The serial port prints the read temperature and humidity in the current environment every 1 second.

![Img](./media/6-70.png)

④ Complete Program

![Img](./media/6-71.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT mainboard. After powering up via the USB cable, click ![Img](./media/1-87.png) in the serial monitor and set the baud rate to 15200. Then the serial port prints the temperature and humidity in the current environment.

![Img](./media/6-74.png)

#### 8. Temperature and Humidity Control System

![Img](./media/6-75.png)

##### (1). Programming Steps

###### Step 1：Flow Chart

![Img](./media/6-76.png)

###### Step 2：Write the Program
①Initialize pin IO23 of the temperature and humidity sensor, and select the dht11 mode.

![Img](./media/6-77.png)

② Initialize the width, height, I2C address, text size and color as well as background color of the OLED display.

![Img](./media/6-78.png)

③ Set the strings "Temper:" and "Humid:" to be displayed on the OLED.

![Img](./media/6-79.png)

④ Define variables "**temperature**" and "**humidity**".

![Img](./media/6-80.png)

⑤ Store the read <span style="color: rgb(255, 76, 65);">temperature data</span> into the "temperature" variable. The read <span style="color: rgb(255, 76, 65);">humidity data</span> is stored in the "humidity" variable.

![Img](./media/6-81.png)

⑥  Display <span style="color: rgb(255, 76, 65);">temperature data</span> and <span style="color: rgb(255, 76, 65);">humidity data</span> at the corresponding position on the OLED.

![Img](./media/6-82.png)

⑦ Determine the temperature and humidity value in the environment detected by the temperature and humidity sensor. When the temperature is greater than 29°C, or the humidity is greater than 80%RH, the fan will be turned on.

![Img](./media/6-83.png)

⑧ Complete Program

![Img](./media/6-84.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT mainboard. After powering up via the external power, the OLED displays the temperature and humidity in the current environment. 

When the temperature reaches 29°C or the humidity reaches 80%RH, the motor will turn on to dissipate heat or dehumidify (the fan simulates heat dissipation and dehumidification, and the heat dissipation and dehumidification effect is average); otherwise, the motor will turn off to achieve automatic farm temperature  and humidity control effect.

![Img](./media/6-86.jpg)

#### 9. Common Problems　

##### Q1: Is the temperature and humidity sensor waterproof?

A: The sensor detects the temperature and humidity in the air, which is not waterproof. Please do not put the module into water.

##### Q2: Does the rotation of the motor cause the kidsIOT mainboard to reset?

A: When the motor rotates, it requires a larger current than other sensors, which will cause voltage and current fluctuations in the circuit. Especially when the motor rotates forward and reverse, the voltage and current fluctuations are too large, causing the voltage and current of the kidsIOT mainboard to be too low, thus causing a reset.




### Project 07：Soil Moisture Detection System

<span style="color: rgb(255, 76, 65);">Note: Do not allow water to overflow from sinks and soil troughs when using the device. Sprinkling water on other sensors will cause a short circuit and device failure. Sprinkling water on batteries will cause heating and explosion. Please be careful when using the device, especially when used by young children, it must be under the supervision of parents. To ensure safe operation of the device, please follow relevant usage guidelines and safety regulations.</span>


![Img](./media/7-0.png)

#### 1. Description

This project introduces how to use a kidsIOT mainboard, a soil moisture sensor, a passive buzzer and an OLED display to make an intelligent soil moisture detection system.
The system can display the value of the soil moisture sensor in real time through the OLED display. When the soil moisture is lower than the set value, the buzzer will sound an alarm to remind you that it is time to water the land.

#### 2. Components

|![Img](./media/A1.png)|![Img](./media/A15.png)|![Img](./media/A16.png)|![Img](./media/A10.png)|
| :--: | :--: | :--: |:--: |
|kidsIOT Mainboard×1|Water Level Sensor×1|Soil Moisture Sensor×1|Passive Buzzer×1|
|![Img](./media/A13.png)|![Img](./media/A9.png)|![Img](./media/A17.png)|![Img](./media/A22.png)|
|GPIO Shield×1|Relay Module×1|Water Pump×1| Wire×3 |
|![Img](./media/A20.png)|![Img](./media/A25.png)|![Img](./media/A24.png)|![Img](./media/A23.png) |
|Battery Holder×1|Slotted Screwdriver×1|M-F DuPont Wires|F-F  DuPont Wires|
|![Img](./media/A18.png)|![Img](./media/A35.png) |![Img](./media/A28.png) |![Img](./media/A26.png) |
| Water Pipe×1 |Soil Moisture/Water Level/Automatic Irrigation System LEGO Pieces×1|AA Battery（<span style="color: rgb(255, 76, 65);">Not provide</span>）×6|Sink×2 |

![Img](./media/7-1.png)

#### 3. Assembly Steps

##### Step 1：Components Needed

![Img](./media/Z-7-1.png)

##### Step 2：Process

Process 1：

![Img](./media/Z-7-2.png)

Process 2：

![Img](./media/Z-7-3.png)

Process 3：

![Img](./media/Z-7-4.png)

Process 4：

![Img](./media/Z-7-5.png)

Process 5：

![Img](./media/Z-7-6.png)

![Img](./media/Z-7-7.png)

Process 6：

![Img](./media/Z-7-8.png)

Process 7：

![Img](./media/Z-7-9.png)

Process 8：

![Img](./media/Z-7-10.png)

Process 9：

![Img](./media/Z-7-11.png)

Process 10：

![Img](./media/Z-7-12.png)

![Img](./media/Z-7-13.png)

Process 11：

![Img](./media/Z-7-14.png)

Process 12：

![Img](./media/Z-7-15.png)

Process 13：

![Img](./media/Z-7-16.png)

Process 14：

![Img](./media/Z-7-17.png)

Complete：

![Img](./media/Z-7-18.png)

#### 4. Wiring Diagram

| Module |GPIO Shield| kidsIOT Mainboard |
| :--: | :--: | :--: |
| Soil Moisture Sensor |G→G，V→V，S→S3|No.4 port（control pin of S3 is io27）|
|Passive Buzzer| |No.8 port（control pin is io5）|

Connect the kidsIOT mainboard to your computer via USB cable.


![Img](./media/7-2.png)

#### 5. Read the value of soil moisture sensor

![Img](./media/7-3.png)

##### (1). Write the Program

① Set the baud rate to 15200.

![Img](./media/1-68.png)

② Set the pin IO27 connected to the soil moisture sensor to "**input**" mode.

![Img](./media/7-5.png)

③ Define a "<span style="color: rgb(255, 76, 65);">Soil_humidity_sensor</span>" global variable to store the analog value of the soil moisture sensor.

![Img](./media/7-6.png)

④ Store the read analog value of the soil moisture sensor in the "<span style="color: rgb(255, 76, 65);">Soil_humidity_sensor</span>" variable and print it on the serial port.

![Img](./media/7-7.png)

⑤ Complete Program

![Img](./media/7-8.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT board. After powering up via the USB cable, click ![Img](./media/1-87.png) in the serial monitor and set the baud rate to 15200. 

Insert the soil moisture sensor into the soil (or touch the sensor with wet hands), then the serial monitor will print the analog value of the soil moisture sensor (range: 0~4095). The greater the soil moisture (or the wetter the hand), the greater the value!

![Img](./media/7-11.png)

#### 6. Soil Moisture Detection System

![Img](./media/7-12.png)

##### (1). Programming Steps

###### Step 1：Flow Chart

![Img](./media/7-13.png)

###### Step 2：Add “passive buzzer” 

![Img](./media/5-14.png)

###### Step 3：Write the Program

① Set the pin IO27 connected to the soil moisture sensor to "**input**" mode.

![Img](./media/7-15.png)

② Initialize the width, height, I2C address, text size and color as well as background color of the OLED display.

![Img](./media/7-16.png)

③ Define a "<span style="color: rgb(255, 76, 65);">Soil_humidity_sensor</span>" global variable to store the analog value of the soil moisture sensor.

![Img](./media/7-17.png)

④ Store the read analog value of the soil moisture sensor in the "<span style="color: rgb(255, 76, 65);">Soil_humidity_sensor</span>" variable and display it on the OLED.

![Img](./media/7-18.png)

⑤ Determine the analog value of the sensor. If it is less than 500, the buzzer will sound an alarm; otherwise, the buzzer will not sound.

![Img](./media/7-19.png)

⑥ Complete Program

![Img](./media/7-20.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT mainboard. After powering up via the USB cable, insert the soil moisture sensor into the soil (or touch the sensor with wet hands), when the sensor detects that the moisture of the soil (or the moisture of your hands) is less than the set threshold, the buzzer will sound an alarm.

![Img](./media/7-22.jpg)

#### 7. Common Problems　

##### Q: Is the sensor waterproof?

A: The detection area of the soil moisture sensor is waterproof. Exceeding the detection area will cause a short circuit.



### Project 08：Water Level Detection System

<span style="color: rgb(255, 76, 65);">Note: Do not allow water to overflow from sinks and soil troughs when using the device. Sprinkling water on other sensors will cause a short circuit and device failure. Sprinkling water on batteries will cause heating and explosion. Please be careful when using the device, especially when used by young children, it must be under the supervision of parents. To ensure safe operation of the device, please follow relevant usage guidelines and safety regulations.</span>


![Img](./media/8-0.jpg)

#### 1. Description

This project introduces how to use a kidsIOT mainboard, a water level sensor, a passive buzzer and an OLED display to make an intelligent automatic water level detection system. It is able to monitor water level changes, detect problems in time and take measures to avoid disasters, and is widely used in water conservancy projects, urban drainage as well as environment monitoring.

#### 2. Components

|![Img](./media/A1.png)|![Img](./media/A15.png)|![Img](./media/A10.png)|![Img](./media/A13.png)|![Img](./media/A22.png)|
| :--: | :--: | :--: |:--: |:--: |
|kidsIOT Mainboard×1|Water Level Sensor×1|Passive Buzzer×1|GPIO Shield×1|Wire×2|
|![Img](./media/A19.png)|![Img](./media/A35.png)|![Img](./media/A23.png)|![Img](./media/A26.png) | |
|USB Cable×1| Soil Moisture/Water Level/Automatic Irrigation System LEGO Pieces×1 |F-F DuPont Wires|Sink×1 | |

![Img](./media/8-1.png)

#### 3. Assembly Steps

<span style="color: rgb(255, 76, 65);">It shares the same structural shape with **Project 07**. If the assembly parts of **Project 07** have finished, there is no need to assemble it again.</span>


#### 4. Wiring Diagram

| Module |GPIO Shield| kidsIOT Mainboard |
| :--: | :--: | :--: |
| Water Level Sensor |G→G，V→V，S→S4|No.4 port（control pin of S4 is io39）|
|Passive Buzzer| |No.8 port（control pin is io5）|

Connect the kidsIOT mainboard to your computer via USB cable.


![Img](./media/8-2.png)

#### 5. Read the value of water level sensor

![Img](./media/8-3.png)

##### (1). Write the Program

① Set the baud rate to 15200.

![Img](./media/1-68.png)

② Set the pin IO39 connected to the water level sensor to "**input**" mode.

![Img](./media/8-5.png)

③ Define a "<span style="color: rgb(255, 76, 65);">Water_level_sensor</span>" global variable to store the analog value of the water level sensor.

![Img](./media/8-6.png)

④ Store the read analog value of the water level sensor in the "<span style="color: rgb(255, 76, 65);">Water_level_sensor</span>" variable and print it on the serial port.

![Img](./media/8-7.png)

⑤ Complete Program

![Img](./media/8-8.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT mainboard. After powering up via the USB cable, click ![Img](./media/1-87.png) in the serial monitor and set the baud rate to 15200. 

Insert the water level  sensor in the water (or touch the sensor with wet hands), then the serial monitor will print the analog value of the sensor (range: 0~4095). The greater the water level, the greater the value!

![Img](./media/8-11.png)

#### 6. Water Level Detection System

![Img](./media/8-12.png)

##### (1). Programming Steps

###### Step 1：Flow Chart

![Img](./media/8-13.png)

###### Step 2：Add “passive buzzer” 

![Img](./media/5-14.png)

###### Step 3：Write the Program

① Set the pin IO39 connected to the water level sensor to "**input**" mode.

![Img](./media/8-15.png)

② Initialize the width, height, I2C address, text size and color as well as background color of the OLED display.

![Img](./media/8-16.png)

③ Define a "<span style="color: rgb(255, 76, 65);">Water_level_sensor</span>" global variable to store the analog value of the water level sensor.

![Img](./media/8-17.png)

④ Store the read analog value of the  sensor in the“<span style="color: rgb(255, 76, 65);">Water_level_sensor</span>” variable and display it on the OLED.

![Img](./media/8-18.png)

⑤ Determine the analog value of the sensor. If it is greater than 2000, the buzzer will sound an alarm; otherwise, the buzzer will not sound.

![Img](./media/8-19.png)

⑥ Complete Program

![Img](./media/8-20.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT mainboard. After powering up via the USB cable, insert the water level sensor in the water (or touch the sensor with wet hands), when the sensor detects that the water level (or the moisture of your hands) is greater than the set threshold, the buzzer will sound an alarm.

![Img](./media/8-22.jpg)

#### 7. Common Problems　

##### Q: Is the sensor waterproof?

A: The detection area of the sensor is waterproof. Exceeding the detection area will cause a short circuit.




### Project 09：Automatic Irrigation System

<span style="color: rgb(255, 76, 65);">Note: Do not allow water to overflow from sinks and soil troughs when using the device. Sprinkling water on other sensors will cause a short circuit and device failure. Sprinkling water on batteries will cause heating and explosion. Please be careful when using the device, especially when used by young children, it must be under the supervision of parents. To ensure safe operation of the device, please follow relevant usage guidelines and safety regulations.</span>

![Img](./media/9-0.jpg)

#### 1. Description

This project introduces how to use a kidsIOT mainboard, a soil moisture sensor, a water level sensor, a passive buzzer, an OLED display, a relay and a water pump to build an automatic irrigation system.

We will read the analog values of the soil moisture sensor and water level sensor by writing code to control the relay and the water pump.

When the soil is too dry, the relay will be turned on to control the water pump to irrigate the plants, when too low, the water pump will not be started and the buzzer will alarm. 

At the same time, the OLED display will display the dryness of the soil and the water level, thus realizing automated plant watering and water level control, improving production efficiency while reducing the time and energy costs of manual operations.

#### 2. Components

|![Img](./media/A1.png)|![Img](./media/A15.png)|![Img](./media/A16.png)|![Img](./media/A10.png)|
| :--: | :--: | :--: |:--: |
|kidsIOT Mainboard×1|Water Level Sensor×1|Soil Moisture Sensor×1|Passive Buzzer×1|
|![Img](./media/A13.png)|![Img](./media/A9.png)|![Img](./media/A17.png)|![Img](./media/A22.png)|
|GPIO Shield×1|Relay Module×1|Water Pump×1| Wire×3 |
|![Img](./media/A20.png)|![Img](./media/A25.png)|![Img](./media/A24.png)|![Img](./media/A23.png) |
|Battery Holder×1|Slotted Screwdriver×1|M-F DuPont Wires|F-F  DuPont Wires|
|![Img](./media/A18.png)|![Img](./media/A35.png) |![Img](./media/A28.png) |![Img](./media/A26.png) |
| Water Pipe×1 |Soil Moisture/Water Level/Automatic Irrigation System LEGO Pieces×1|AA Battery（<span style="color: rgb(255, 76, 65);">Not provide</span>）×6|Sink×2 |

![Img](./media/9-1.png)

#### 3. Assembly Steps

<span style="color: rgb(255, 76, 65);">It shares the same structural shape with **Project 07**. If the assembly parts of **Project 07** have finished, there is no need to assemble it again.</span>

#### 4. Wiring Diagram

| Module |GPIO Shield| kidsIOT Mainboard |
| :--: | :--: | :--: |
| Soil Moisture Sensor |G→G，V→V，S→S3|No.4 port（control pin of S3 is io27）|
| Water Level Sensor |G→G，V→V，S→S4|No.4 port（control pin of S4 is io39）|
|Passive Buzzer| |No.8 port（control pin is io5）|
|Relay Module| |No.2 port（control pin is io2）|


<span style="color: rgb(61, 167, 66);">**Note：** You need to use a slotted screwdriver to loosen the screws at the NO port and COM port of the relay module. Use a m-f DuPont wire to connect the COM port on the module to V on the GPIO shield, and connect the red wire of the water pump to the NO port of the relay module, the black wire of the water pump and the f--f Dupont wire are connected to G of the GPIO shield. After connecting the wires, use the screwdriver to tighten the screws at the NO port and COM port. </span>


Connect the kidsIOT mainboard to your computer via USB cable, connect the external power supply and turn the DIP switch on the mainboard to ON end.


![Img](./media/9-2.png)

#### 5. Pumping System

![Img](./media/9-3.png)

##### (1). Write the Program

① Set the pin IO2 connected to the relay module to "**input**" mode.

![Img](./media/9-4.png)

② Set the relay module to close for 0.5 seconds and then disconnect, controlling the water pump to pump water for 0.5 seconds.

![Img](./media/9-5.png)

③ Complete Program

![Img](./media/9-6.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT mainboard. After powering up via the USB cable, the relay module will control the water pump to pump water.

#### 6. Automatic Irrigation System

![Img](./media/9-8.png)

##### (1). Programming Steps

###### Step 1：Flow Chart

![Img](./media/9-9.png)

###### Step 2：Add “passive buzzer” 

![Img](./media/5-14.png)

###### Step 3：Write the Program

① Initialize pin IO27 of the soil moisture sensor and pin IO39 of the water level sensor to "**input**" mode.

![Img](./media/9-11.png)

② Initialize pin IO2 of the relay module and pin IO5 of the passive buzzer to "**Output**" mode.

![Img](./media/9-12.png)

③ Initialize the width, height, I2C address, text size and color as well as background color of the OLED display.

![Img](./media/9-13.png)

④ Define a "<span style="color: rgb(255, 76, 65);">Soil_humidity_sensor</span>" global variable to store the analog value of the soil moisture sensor and a "<span style=" color: rgb(255, 76, 65);">Water_level_sensor</span>" global variable to store the analog value of the water level sensor.

![Img](./media/9-14.png)

⑤ Assign sensor data to variables.

![Img](./media/9-15.png)

⑥Display the sensor data at the corresponding position on the OLED display.

![Img](./media/9-16.png)

⑦ Judgment: When the water level is less than 1000, or the soil moisture is less than 500, the buzzer will sound an alarm.

![Img](./media/9-17.png)

⑧ When the soil moisture is less than 500 and the water level in the sink is greater than 1000, the relay will drive the water pump for automatic irrigation.

![Img](./media/9-18.png)

⑨ Complete Program

![Img](./media/9-19.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT mainboard. After powering up via the USB cable, the OLED displays current soil moisture and sink water level information.

When the soil moisture is lower than the set threshold, then the soil is too dry, the buzzer will sound an alarm. At this time, the pumping system will automatically irrigate the soil.
When the water level in the sink is lower than the set threshold, the pumping system will not work and the buzzer will sound an alarm to indicate that there is insufficient water in the sink.

![Img](./media/9-21.jpg)

#### 7. Common Problems　

##### Q1: Is the sensor waterproof?

A: The relay is not waterproof.

##### Q2: Does the rotation of the water pump cause the kidsIOT board to reset?

A: When the water pump rotates, it requires a larger current than other sensors, which will cause voltage and current fluctuations in the circuit. Excessive voltage and current fluctuations will cause the voltage and current of the kidsIOT mainboard to be too low, causing the kidsIOT mainboard to reset.




### Project 10 ：WiFi Web Page Controls Smart Farm System

<span style="color: rgb(255, 76, 65);">Note: Do not allow water to overflow from sinks and soil troughs when using the device. Sprinkling water on other sensors will cause a short circuit and device failure. Sprinkling water on batteries will cause heating and explosion. Please be careful when using the device, especially when used by young children, it must be under the supervision of parents. To ensure safe operation of the device, please follow relevant usage guidelines and safety regulations.</span>


![Img](./media/10-0.png)

#### 1. Description

In today's era of rapid technological development, unified control of intelligent devices via mobile phones has gradually gained people's favor. This method uses a microcontroller to establish a connection between a mobile phone and an intelligent device through a WiFi module and the Internet network to achieve remote control of the intelligent device.

In this project, we will focus on the WiFi infrastructure of ESP32 and control the smart farm system via WiFi web page.

#### 2. Components

|![Img](./media/A1.png)|![Img](./media/A15.png)|![Img](./media/A16.png)|![Img](./media/A10.png)|
| :--: | :--: | :--: |:--: |
|kidsIOT Mainboard×1|Water Level Sensor×1|Soil Moisture Sensor×1|Passive Buzzer×1|
|![Img](./media/A8.png)|![Img](./media/A5.png)|![Img](./media/A12.png)|![Img](./media/A11.png)|
|White LED Module×1|Photoresistor×1|Temperature and Humidity Sensor×1|Motor×1|
|![Img](./media/A17.png)|![Img](./media/A13.png)|![Img](./media/A9.png)|![Img](./media/A27.png)|
|Water Pump×1| GPIO Shield×1 |Relay Module×1|Fan×1|
|![Img](./media/A23.png)|![Img](./media/A26.png)|![Img](./media/A20.png)|![Img](./media/A24.png) |
|F-F DuPont Wires|Sink×2 |Battery Holder×1|M-F DuPont Wire×1|
|![Img](./media/A18.png)|![Img](./media/A28.png) | ![Img](./media/A25.png) |![Img](./media/A22.png) |
|Water Pipe×1 |AA Battery（<span style="color: rgb(255, 76, 65);">Not provide</span>）×6 | Slotted Screwdriver×1 | Wire×7 |

#### 3. Assembly Steps

<span style="color: rgb(255, 76, 65);">Just put the structural shapes assembled in Project 02, Project 06 and Project 07 together . </span>


![Img](./media/10-1.jpg)

#### 4. Wiring Diagram

| Module |GPIO Shield| kidsIOT Mainboard |
| :--: | :--: | :--: |
| Water Level Sensor |G→G，V→V，S→S4|No.4 port（control pin of S4 is io39）|
| Soil Moisture Sensor | |G/V/io33 port（G→G，V→V，S→io33）|
|Photoresistor| |No.6 port（control pin is io36）|
|Temperature and Humidity Sensor| |No.8 port（control pin is io5）|
|White LED Module| |No.7 port（control pin is io16）|
|Passive Buzzer| |No.2 port（control pin is io2）|
|Motor| |No.9 port（IN+control pin is io18，IN-control pin is io19）|
|Relay Module| |No.3 port（control pin is io26）|


<span style="color: rgb(61, 167, 66);">Note：You need to use a slotted screwdriver to loosen the screws at the NO port and COM port of the relay module. Use a m-f DuPont wire to connect the COM port on the module to V on the GPIO shield, and connect the red wire of the water pump to the NO port of the relay module, the black wire of the water pump and the f--f Dupont wire are connected to G of the GPIO shield. After connecting the wires, use the screwdriver to tighten the screws at the NO port and COM port. </span>


Connect the kidsIOT mainboard to your computer via USB cable, connect the external power supply and turn the DIP switch on the mainboard to ON end.


![Img](./media/10-2.png)

#### 5. WiFi Web Page Display

![Img](./media/10-3.png)

##### (1). Knowledge

![Img](./media/10-4.png)

The Wi-Fi library supports configuring and monitoring ESP32 Wi-Fi networking functions. Supported configurations:

- station mode (STA mode or Wi-Fi client mode), at this time the ESP32 is connected to the access point (AP).
- AP mode (Soft-AP mode or Access Point mode), at this time the base station is connected to the ESP32.
- station/AP coexistence mode (ESP32 is both an access point and a base station connected to another access point).
- Various security modes for the above mentioned modes (WPA, WPA2, WPA3, etc.).
- Scan access points (including active scanning and passive scanning).
- Monitor IEEE802.11 Wi-Fi packets using promiscuous mode.

For details about wifi, tap it：[https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/network/esp_wifi.html](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/network/esp_wifi.html)

Espressif official website：[https://www.espressif.com.cn/en/home](https://www.espressif.com.cn/en/home)

##### (2). Programming Steps

###### Step 1：Add the “Web Page Editing PRO” library

Tap ![Img](./media/6-46.png), click the “communication” module in the “Extension” , then select “**<span style="color: rgb(255, 76, 65);">Web Page Editing PRO</span>**” and click ![Img](media/781.png)to return to the programming interface.

![Img](./media/3-13.png)

![Img](./media/10-9.png)

![Img](./media/10-10.png)

###### Step 2：Description of the Building Block

![Img](./media/10-11.png)

Enter the WiFi name and password to connect to the WiFi hotspot.

![Img](./media/10-12.png)

Read the WiFi IP address.

![Img](./media/10-13.png)

Set up a card on the web page, and its card label,  card unit and card type correspond one to one.

![Img](./media/10-14.png)

Add a button card to the web page.

###### Step 3：Write the Program

① Change the WiFi name and password in the code to your own WiFi name and password, and connect to the WiFi hotspot.

![Img](./media/10-15.png)

② Display the WiFi IP address on the OLED.

![Img](./media/10-16.png)

③ Set a card on the web page, the card label is "Temperature", the card type is "Temperature", the card unit is "℃", the card ID is 1, and the temperature value is 30.

![Img](./media/10-17.png)

![Img](./media/10-18.png)

④Set up a card on the web page. The card label is "Air humidity", the card type is "Humidity", the card unit is "%RH", the card ID is 2, and the temperature value is 60.

![Img](./media/10-19.png)

![Img](./media/10-20.png)

⑤ Complete Program

![Img](./media/10-21.png)

##### (3). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT mainboard and power on. Once connected to WiFi, the OLED on the board will display the corresponding IP address (<span style="color: rgb(255, 169, 0);">Here we take the IP address: 192.168.0.48 as an example</span> ).

![Img](./media/10-23.jpg)

<span style="color: rgb(255, 76, 65);">**Note: When the PC, mobile phone and kidsIOT mainboard are connected to the same network, this webpage can be opened on the PC and mobile phone at the same time. Here is the IP address displayed on the OLED on your own kidsIOT board**</span>



You can enter "<span style="color: rgb(0, 209, 0);">**http://[IP address displayed on the OLED display]**</span>" in the browser to view the web page . In this way, you will create a simple web page that displays a fixed temperature information and a fixed humidity information:

**PC：**

![Img](./media/10-24.png)

**Mobile phone：**

![Img](./media/10-25.png)

#### 6. WiFi Web Page Controls Smart Farm System

![Img](./media/10-26.png)

##### (1). Programming Steps

###### Step 1：Flow Chart

![Img](./media/10-27.png)

###### Step 2：Add "Passive Buzzer", "DC Motor", "Temperature and Humidity Sensor" and "Web Page Editing PRO" libraries

Tap ![Img](./media/6-46.png), click "<span style="color: rgb(255, 76, 65);">Actuator</span>" and find "<span style="color: rgb(255, 76, 65);">esp32 Passive buzzer</span>” and “<span style="color: rgb(255, 76, 65);">DC Motor for esp32</span>” . Click "<span style="color: rgb(255, 76, 65);">Sensor</span>" and find "<span style="color: rgb(255, 76, 65);">DHT sensor for ESP32</span>" .

Click the “communication” , then select “**<span style="color: rgb(255, 76, 65);">Web Page Editing PRO</span>**” and click ![Img](media/781.png)to return to the programming interface.

![Img](./media/3-13.png)

![Img](./media/10-31.png)

![Img](./media/6-64.png)

![Img](./media/10-9.png)

![Img](./media/10-34.png)

###### Step 3：Write the Program

① Change the WiFi name and password in the code to your own WiFi name and password, and connect to the WiFi hotspot.

![Img](./media/10-35.png)

② Display the WiFi IP address on the OLED.

![Img](./media/10-36.png)

③ Initialize pin IO5 of the temperature and humidity sensor, and select the mode dht11.

![Img](./media/10-37.png)

④ Initialize the pin IO33 of the soil moisture sensor, the pin IO39 of the water level sensor, and the pin IO36 of the photoresistor, and set them to "**Input**" mode.

![Img](./media/10-38.png)

⑤ Initialize the pin IO16 of the LED module, the pin IO26 of the relay module and the pin IO2 of the passive buzzer, and set them to "**Output**" mode.

![Img](./media/10-39.png)

⑥ Define four global variables, namely "<span style="color: rgb(255, 76, 65);">Val1</span>", "<span style="color: rgb(255, 76, 65) ;">Val2</span>", "<span style="color: rgb(255, 76, 65);">Val3</span>" and "<span style="color: rgb(255, 76, 65);">Val4</span>".

![Img](./media/10-41.png)

⑦ Set up multiple cards of the web page, namely Temperature，Air humidity，Soil humidity，Water level and Brightness.

![Img](./media/10-42.png)

⑧ Set the button card to control LED on and off.

![Img](./media/10-43.png)

⑨ Set the button card  to control the fan on and off.

![Img](./media/10-44.png)

⑩ Set a button card to control the relay's on and off, thereby controlling whether the water pump pumps water.

![Img](./media/10-45.png)

⑪ Set the button card for playing music.

![Img](./media/10-47.png)

⑫ Complete Program

![Img](./media/10-48.png)

##### (2). Test Result

Click![Img](./media/1-27.png) to upload the above complete code to the kidsIOT mainboard and power on. Once connected to WiFi, the OLED on the board will display the corresponding IP address. You can enter "<span style="color: rgb(255, 76, 65);">**http://[IP address displayed on the OLED]**</span>" in the browser to view the web page . The sensor data can be viewed on the web page, and LEDs and fans can also be controlled.

![Img](./media/10-52.jpg)

**PC：**

![Img](./media/10-50.png)

**Mobile phone：**

![Img](./media/10-51.png)

|   Sensor data   |   Control   |
| :------------: | :--------: |
|  Ambient temperature(℃)  |  LED on/off  |
| Ambient humidity(%RH) |  Fan on/off  |
|    Soil moisture    | Water pump on/off |
|    water level of sink    |   Play music   |
|  Light(0~4095)  |             |

#### 7. Common Problems　

##### Q1：You can’t connect the WiFi?

A: Please move the kidsIOT board to the vicinity of the router, press the reset button on the board to restart kidsIOT, and wait patiently for the connection. If you still can't connect, please check whether the WiFi name and password are filled in correctly.


##### Q2：When remotely operating other sensors on the web page, the response is very slow?

A: Reasons:

- When multiple people are connecting it, the router's CPU resources are insufficient. Restart the router and reconnect to the network.
- The router system has been used for too long. Restart the router.
- When wireless interference occurs and the wireless signal is unstable, please do not use it through the wall.

For router related knowledge, please search on **google** yourself.



























　
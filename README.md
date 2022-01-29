# C# Arduino System Information
See your system information on LCD with Arduino, but with C#!

You can see RAM usage, and CPU usage.
## Requirements:
- An Arduino Board. **[ You can use all type of Arduino types *(Leonardo, UNO, Mega etc.)* ]**
- A 16X2 *(Minimum)* LCD Shield **with or without I2C**
- .Net in your computer (?)

**If you have an LCD Without I2C, you need:**
- A 10K potentiometer 
- A 220 Ohm resistor 


## How to use?
1. Download/Clone this repo.
2. If you have I2C, upload the code named `systeminfoI2C.ino`, else `systeminfo.ino` to your board.
3. Connect pins. Look under for this. And connect your board to your computer.
4. Write your COM port to code:
```cs
SerialPort port = new SerialPort("COM3", 9600, Parity.None, 8, StopBits.One);
```
6. And finaly, compile. And you can see your System Info on LCD.
Working image:
![image](https://user-images.githubusercontent.com/70021050/147857017-f1ea1fb9-cfdc-4139-93a1-c50da9da4bb0.jpg)

Circuit of Project for **NOT I2C**:
![tinkercad](https://user-images.githubusercontent.com/70021050/147857009-69643cf9-e338-4abb-81e5-e55f44b51196.png)

**For I2C**:
![image](https://user-images.githubusercontent.com/70021050/147857874-e9ff53cb-1a57-4f7c-a34b-258d9aaa5340.png)

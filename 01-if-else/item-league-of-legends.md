# “WELCOME TO THE LEAGUE OF LEGENDS!”

วินเซนต์ในช่วงหน้าร้อน ช่างว่างเสียจริงๆ ดังนั้น เขาจึงเริ่มหาอะไรทำแก้เบื่อ  เขาเลือกเล่นเกม LEAGUE OF LEGENDS ซึ่งเป็นเกมแนว moba ประเภทหนึ่ง แต่ถึงจะเคยเล่นเกมแนวนี้มาก่อนแล้ว แต่เรื่องการซื้อไอเทมตอนต้นเกมเนี่ย ก็ยังงงๆอยู่นะ ดังนั้นเขาจึงบังคับให้โปรแกมเมอร์นางหนึ่งเขียนโค้ดเพื่อประกอบการตัดสินใจขึ้นมา โค้ดดังกล่าว จะเริ่มต้นด้วย การให้เลือกเลนที่จะไป ซึ่งมี **4 เลน** ด้วยกัน นั่นคือ 

* **Top** เลนบน 
* **Jungle** เลนป่าเพื่อรอเข้าไปช่วยเลนอื่น 
* **Mid** เลนกลาง 
* **Bot** เลนล่าง 

จากนั้นจะให้เลือกบทบาทที่จะเล่น ซึ่งประกอบไปด้วย Tank ที่มีพลังชีวิตสูง Magician หรือ Ap ใช้เวทย์เป็นหลัก Adc เป็นตัวทำดาเมจยิงไกล Support คอยช่วยสนับสนุน และปกป้อง adc และ Assassin เป็นตัวทำดาเมจหลัก ซึ่งเมื่อเราเลือกเลนแล้ว จะมีบทบาทให้เราเลือก ตามเลนนั้นๆ เมื่อเราเลือกเลนและบทบาทเสร็จสิ้น ระบบจะทำการโชว์ไอเทมเริ่มต้นที่เราควรจะซื้อ แต่ถ้าหากใส่คำตอบนอกเหนือจากตัวเลือก ระบบจะโชว์ "Wow error 'w'" และหยุดการทำงาน

## ตัวอย่าง Input/Output ##

**ตัวอย่างที่ 1**

```
WELCOME TO THE LEAGUE OF LEGENDS 
YOU CAN GO 
TOP    : 1 
JUNGLE : 2 
MIDDLE : 3
BOTTOM : 4
Choose your lane : 1
OK, you will go Top lane
ASSASSIN    : 1
MAGICIAN    : 2
TANK        : 3
ADC-CARRY   : 4
Now, Choose your roles : 3
Your first item is Doran's Shield.
```
**ตัวอย่างที่ 2**
```
WELCOME TO THE LEAGUE OF LEGENDS
YOU CAN GO
TOP    : 1
JUNGLE : 2
MIDDLE : 3
BOTTOM : 4
Choose your lane : 4
OK, you will go Bot lane
ADC-CARRY : 1
SUPPORT   : 2
TANK      : 3
Now, Choose your roles : 2
Your first item are Spellthief's Edge or Ancient Coin or Relic Shield.
```
**ตัวอย่างที่ 3**
```
WELCOME TO THE LEAGUE OF LEGENDS
YOU CAN GO
TOP    : 1
JUNGLE : 2
MIDDLE : 3
BOTTOM : 4
Choose your lane : 3
OK, you will go MID lane
ASSASSIN : 1
MAGICIAN : 2
SUPPORT  : 3
Now, Choose your roles : 1
Your first item are Doran's Blade or Long Sword.
```
**ตัวอย่างที่ 4**
```
WELCOME TO THE LEAGUE OF LEGENDS
YOU CAN GO
TOP    : 1
JUNGLE : 2
MIDDLE : 3
BOTTOM : 4
Choose your lane : 5
Wow error 'w'
```
**ตัวอย่างที่ 5**
```
WELCOME TO THE LEAGUE OF LEGENDS
YOU CAN GO
TOP    : 1
JUNGLE : 2
MIDDLE : 3
BOTTOM : 4
Choose your lane : 4
OK, you will go Bot lane
ADC-CARRY : 1
SUPPORT   : 2
TANK      : 3
Now, Choose your roles : 8
Wow error 'w'
```

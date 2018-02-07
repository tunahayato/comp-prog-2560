# Kapop's Coffee Shop

โปรแกรมสั่งกาแฟ โดยร้านนี้จะมีสมาชิก 2 แบบ คือ แบบ Normal และแบบ Premium โดยสมาชิกแต่ละประเภทจะได้รับส่วนลด 15% และ 25% ตามลำดับ (จากราคาทั้งหมดของแก้วนั้นรวมราคาขนาดแก้วแล้ว) และถ้าไม่ได้เป็นสมาชิกจะไม่ได้รับส่วนลดใดๆ 

## ตัวอย่างรหัสสมาชิก(มี 4 หลัก)
* แบบ **Normal** รหัสสมาชิกจะเป็นเลขคู่ (EX : 0022)
* แบบ **Premium** รหัสสมาชิกจะเป็นเลขคี่ (EX : 0035)
* **ไม่ได้เป็นสมาชิก** รหัสสมาชิกจะเป็น 0000

**หมายเหตุ** : ผู้ใช้ไม่จำเป็นต้องพิมพ์เข้ามาทั้ง 4 หลัก สามารถพิมพ์แค่เลขท้ายได้ เช่น รหัสสมาชิกคือ 0004 ผู้ใช้ สามารถพิมพ์แค่ 4 ได้ โดยโปรแกรมจะเปลี่ยนให้และแสดงว่ารหัสสมาชิกคือ 0004 ก่อนที่ผู้ใช้จะเริ่ม

## ราคาของน้ำแต่ละแก้ว
* Coffee   \_ (20 บาท)
* Tea      \_ (25 บาท)
* Cocoa    \_ (30 บาท)
* Ovaltine \_ (30 บาท)
* Smoothie \_ (35 บาท)

**หมายเหตุ** : โดยถ้าใส่ประเภทเครื่องดื่มผิด จะขึ้นข้อความว่า **Please select again.** และโปรแกรมจะบังคับให้ใส่ใหม่จนกว่าจะถูก

## ราคาตามขนาดแก้ว
* ขนาด **Small** ไม่บวกราคาเพิ่ม
* ขนาด **Large** บวกราคาเพิ่ม 10 บาท

**หมายเหตุ** : โดยถ้าใส่ขนาดผิด จะขึ้นข้อความว่า **Please select again.** และโปรแกรมจะบังคับให้ใส่ใหม่จนกว่าจะถูก

**ตัวอย่าง Input/Output**

1. **Input**
```
----- Welcome to Kapop's coffee shop -----
Please enter your member code (EX : 0000) : 4

You are normal member :)
Your code is 0004

================
 TYPE OF DRINKS
================
- Coffee(1)
- Tea(2)
- Cocoa(3)
- Ovaltine(4)
- Smoothie(5)
Please select type of drink :1

================
 SIZE OF DRINKS
================
- small(1)
- large(2)
Please select type of drink :1
```
**Output**
```
Total : 17.00
Thank you :)
```

2. **Input**
```
----- Welcome to Kapop's coffee shop -----
Please enter your member code (EX : 0000) : 0

You are not member :)

================
 TYPE OF DRINKS
================
- Coffee(1)
- Tea(2)
- Cocoa(3)
- Ovaltine(4)
- Smoothie(5)
Please select type of drink :5

================
 SIZE OF DRINKS
================
- small(1)
- large(2)
Please select type of drink :4

Please select agian.

================
 SIZE OF DRINKS
================
- small(1)
- large(2)
Please select type of drink :2
```
**Output**
```
Total : 45.00
Thank you :)
```

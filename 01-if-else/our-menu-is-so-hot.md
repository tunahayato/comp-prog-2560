# ไก่อร่อยเกินไป
เนื่องจากในช่วงงานเกษตรแฟร์ ชมรมนิสิตมุสลิมได้ออกร้านขายอาหารหลากชนิด ซึ่งในช่วงเวลาที่ใกล้กับมื้ออาหารนั้นไก่ย่างและชาชักขายดีเป็นพิเศษ เนื่องจากรสชาติที่อร่อยและราคาที่ถูกจนทำให้เกิดปัญหาไม่พอขายขึ้น เนื่องจากที่เราเป็นโปรแกรมเมอร์และไม่อยากให้ลูกค้ายืนรอนานๆ จึงได้เขียนโปรแกรมสั่งจองไก่ย่างและชาชักขึ้น  
### ซึ่งมีตัวเลือกดังนี้  
1. grilled chicken  
    * BBQ flavour
    * Original flavour
    * sticky rice
2. tea tarik
    * low sweet ?
3. both  
### ราคาสินค้า
ไม่ต้องแสดงในโปรแกรมเนื่องจากหน้าร้านนั้นมีราคาบอกอยู่แล้ว
1. grilled chicken 10 baht.
2. sticky rice 5 baht.
3. tea tarik 35 baht.

  
## input
* รับชนิดของเมนูอาหารเข้ามาโดยรับ input เป็นตัวอักษรแรกของเมนูนั้น
* ถามจำนวนอาหารในชนิดที่ลูกค้าสั่ง
## output
* สรุปรายการอาหารที่สั่งซื้อทั้งหมด
* ไม่ต้องแสดงรายการอาหารที่ไม่ได้ซื้อ
* หากสั่ง tea tarik แบบ low sweet ให้ต่อท้ายตอนสรุปว่า " with low sweet "
* สรุปราคาอาหารทั้งหมดที่สั่งซื้อ (หากราคาเกินหลักร้อยมา 5 baht. เราจะลดให้)
* หาก input ผิดพลาดให้แสดงข้อความ "Please choose only our menu or use lower characters"
  
## ตัวอย่าง input output
### example 1
\*\*\*Welcome to Nisit Muslim, please choose your order***  
[g]rilled chicken.   
[t]ea tarik.  
[b]oth.  
Your order is: a  
Please choose only our menu or use lower characters  
* เนื่องจาก input ผิดพลาดจึงแสดงผลดังกล่าว
  
### example 2
\*\*\*Welcome to Nisit Muslim, please choose your order***  
[g]rilled chicken.  
[t]ea tarik.  
[b]oth.  
Your order is: b  
\*\*\*grilled chicken.***  
BBQ flavour: 6  
Original flavour: 0  
Sticky rice: 2   
\*\*\*tea tarik.***  
How many: 1  
Low sweet? [y/n] :n  
\*\*\*Your order is***  
grilled chicken.  
BBQ flavour: 6  
Sticky rice: 2  
tea tarik: 1    
Total cost = 100 Baht.  
\*\*\*thank you***  
* เนื่องจากไม่มีการสั่ง original flavuor จึงไม่แสดงในช่วงสรุปเมนู และราคารวมนั้นมีราคา 105 baht. จึงลดเหลื่อ 100 baht.

### example 3
\*\*\*Welcome to Nisit Muslim, please choose your order***  
[g]rilled chicken.  
[t]ea tarik.  
[b]oth.  
Your order is: t  
\*\*\*tea tarik.***  
How many: 2  
Low sweet? [y/n] :y  
\*\*\*Your order is***  
tea tarik: 2 with low sweet  
Total cost = 70 Baht.  
\*\*\*thank you***  
* เนื่องจากเลือก tea tarik แค่เมนูเดียวจึงสรุปเพียงเมนูเดียว
* เนื่องจากเลือก low sweet ในช่วงสรุปจึงต่อท้ายด้วย with low sweet


#DECODE
ให้เขียนโปรแกรมรับรหัสเข้ามาซึ่งรหัสจะเป็นตัวอักขระทั้งหมดไม่มากกว่า 20 ตัว
 โดยไม่เว้นวรรคและจะมีข้อความภาษาอังกฤษแทรกอยู่ก็คือรหัสลับ 
ซึ่งนอกจากข้อความภาษาอังกฤษอักขระที่เหลือจะไม่ใช่ตัวอักษรภาษาอังกฤษ 
เช่น 0645!@r#!ach(*at(*a$ จะถอดรหัสได้เป็น rachata 
กำหนดให้
Input prompt คือ YOUR CODE : 
Output prompt คือ Decode is : 

หมายเหตุ :ถ้ากรอกชุดรหัสมากกว่า20 จะคิดแค่ถึง20เท่านั้น ที่เหลือจะไม่นำมาคิด

---

* **ข้อมูลนำเข้า** นำเข้าชุดรหัสลับ
* **ข้อมูลออก**แสดงผลคำที่ถอดจากรหัสลับ

---

**ตัวอย่างของ Input/Output**

1.**input** YOUR CODE : !@$@!g%*$&%)$u$(%*n) 	   	**output** Decode is : gun
2.**input** YOUR CODE : !@$ra@c!h%a*t&a)$(%)  	   	**output** Decode is : rachata
3.**input** YOUR CODE : GradA 				**output** Decode is : GradA
4.**input** YOUR CODE : abcdefghijklmnopqrstuvwxyz 	**output** Decode is : abcdefghijklmnopqrst

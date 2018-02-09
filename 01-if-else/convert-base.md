## การแปลงเลขระหว่างฐาน

**โจทย์ปํญหา**

ให้ผู้ใช้เขียนโปแกรมเพื่อทำการสร้างเมนู และทำการแปลงเลขฐาน 2 จำนวน 8 หลัก เป็นฐาน 8 10 และ 16 ตามที่ผู้ใช้เลือก พร้อมทั้งตรวจสอลเลขฐาน 2 ที่ผู้ใช้ป้อนจะต้องเป็น 0 หรือ 1 เท่านั้น

**ข้อมูลเข้า**

1. เลือก choice ว่าต้องการจะแปลงเป็นเลขฐานใด
2. ใส่เลขฐานที่ต้องการจะแปลง

**ข้อมูลออก**

1. เลขฐาน 8 หลักที่ผู้ใช้ป้อนเข้าไป (จะไม่แสดงเมื่อผู้ใช้ป้อนเลขอื่นนอกจาก 0 และ 1)
2. เลขฐานต่างๆที่ผู้ใช้เลือกที่จะแปลง

**ตัวอย่าง Input/Output**

ตัวอย่างที่ 1
```
1. Convert Binary to Decimal  
2. Convert Binary to Octal
3. Convert Binary to Hexadecimal
4. Exit
Choose a choice : 1
Input Binary number (8 digits) : 10101010
Binary Number is 10101010
Decimal is 170
```

ตัวอย่างที่ 2
```
1. Convert Binary to Decimal
2. Convert Binary to Octal
3. Convert Binary to Hexadecimal
4. Exit
Choose a choice : 3
Input Binary number (8 digits) : 11001010
Binary Number is 11001010
Hexadecimal is CA
```

ตัวอย่างที่ 3
```
1. Convert Binary to Decimal
2. Convert Binary to Octal
3. Convert Binary to Hexadecimal
4. Exit
Choose a choice : 2
Input Binary number (8 digits) : 12345678
Error! digit must be 1 or 0
```

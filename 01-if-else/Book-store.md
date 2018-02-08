# Book-Store
ร้านเช่าหนังสือแห่งหนึ่ง มีหนังสือ 2 ประเภท คือ
1. Fiction (หนังสือนิยาย) ค่าเช่าเล่มละ 20 บาทจะเช่าได้ 3 วัน
2. Comics (หนังสือการ์ตูน) ค่าเช่าเล่มละ  10 บาท เช่าได้ 2 วัน

และถ้าคืนช้าทางร้านจะคิดค่าปรับ วันละครึ่งราคาเช่าต่อเล่ม คุณจะต้องเขียนโปรแกรมเพื่อคำนวณค่าเช่าหนังสือของร้านนี้

**ข้อมูลเข้า**
* ประเภทหนังสือที่จะเช่า ถ้าคำตอบอยู่นอกเหนือคำถามให้แสดงข้อความ “ERROR”
* จำนวนหนังสือที่ยืม เป็นจำนวนเต็มมากกว่า 0 เท่านั้น ถ้าไม่ใช่ให้แสดงข้อความ “ERROR”
* จำนวนวันที่ยืม เป็นจำนวนเต็มตั้งแต่ 0 ขึ้นไป ถ้าไม่ใช่ให้แสดงข้อความ “ERROR”

**ข้อมูลออก**
* ค่าเช่าหนังสือทั้งหมด

**ตัวอย่าง Input/Output**

    Enter type of book(1=Fiction, 2=comic): 1
    Enter number of book: 2
    Enter days: 2
    Your cost is 40 Baht.
---
**ตัวอย่าง Input/Output**

    Enter type of book(1=Fiction, 2=comic): 2
    Enter number of book: 5
    Enter days: 0
    ERROR
---
**ตัวอย่าง Input/Output 2**

    Enter type of book(1=Fiction, 2=comic): 2
    Enter number of book: 2
    Enter days: 5
    Your cost is 80 Baht.
---

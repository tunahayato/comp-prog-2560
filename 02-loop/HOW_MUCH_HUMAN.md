#HOW_MUCH_HUMAN
จงเขียนโปรแกรมให้ท่านยมบาลรับค่าช่วงของวันที่ต้องการโดยรับสามค่าคือวันเริ่ม(Start Day) 
วันสุดท้าย(Last day) และ วันเริ่มต้นเป็นวันอะไร(Start Day Is ) 
ให้หาผู้ตายในช่วงของวันนี้โดยบังเอิญของบังเอิญที่วันจันทร์จะมีผู้ตาย1คนและเพิ่มที่ละ1ในวันถัดไป
โดยจะครบวันอาทิตย์จะตาย7คนและเมื่อเริ่มวันจันทร์ก็จะกลับมาตาย1คนเสมอและแทนวันนั้นๆ
ด้วยตัวเลขในวงเล็บหลังวันดังตาราง 
หมายเหตุ : พิมพ์ ERROR เมื่อ	
1.วันเริ่มต้นน้อยกว่า0หรือมากกว่า31
2.วันสุดท้ายน้อยกว่า0หรือมากกว่า31
3.วันสุดท้ายน้อยกว่าวันเริ่มต้น
4.จำนวนวันน้อยกว่า1หรือมากกว่า7


| Days    |   จำนวนผู้ตาย |
| -------- | -------- | 
|Monday(1)   |1       |
|Tuesday(2)   |2    | 
|  Wednesday(3)|3   | 
|  Thursday(4)|4  | 
| Friday(5)|5 | 
| Saturday(6)|6 | 
|  Sunday(7)|7  | 

---
* **ข้อมูลนำเข้า**  นำเข้าวันที่แรกวันที่สุดท้ายและวันอะไรตามลำดับโดยมี input prompt คือ (Start Day : ),(Last Day: ) และ (Start Day Is : ) ตามลำดับ
* **ข้อมูลออก** แสดงจำนวนคนที่อยู่ในช่วงที่รับ input มาโดย มี output prompt คือ (Number of deaths is : ) และ "ERROR" ในกรณีกรอกข้อมูลผิด

---
**ตัวอย่างของ Input/Output**

1.**input** Start Day : 4 , Last Day : 20, Start Day Is : 4 **output** Number of deaths is : 71

2.**input** Start Day : 1 , Last Day : 30, Start Day Is : 5 **output** Number of deaths is : 123

3.**input** Start Day : 0 , Last Day : 29, Start Day Is : 2 **output** ERROR

4.**input** Start Day : 5 , Last Day : 4, Start Day Is : 2 	**output** ERROR

5.**input** Start Day : 7 , Last Day : 8, Start Day Is : 8 	**output** ERROR

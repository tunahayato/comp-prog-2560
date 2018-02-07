#Automatic Air Conditioner
บ้านหลังหนึ่งมีระบบเปิด-ปิดแอร์อัตโนมัติ เนื่องจากเจ้าของบ้านเป็นคนนี้มีความประหยัดมาก จึงได้ตั้งเวลาเปิดไว้ตั้งแต่เวลา 18.00-5.30 น. ของทุกวัน เพราะเจ้าของบ้านนี้กลับมานอนที่บ้านทุกวัน แต่หากอุณหภูมิสูงเกิน 35 องศาในวันหยุด(วันเสาร์ – วันอาทิตย์)แอร์จะเปิดเมื่อเจ้าของบ้านอยู่บ้าน  
จงเขียนโปรแกรมควบคุมระบบเปิด-ปิดแอร์อัตโนมัติของบ้านหลังนี้ โดยรับข้อมูล วัน เวลา อุณหภูมิ และมีคนอยู่บ้านหรือไม่ ตามลำดับ  
**หมายเหตุ** : ข้อมูลที่รับเข้ามาเป็นจำนวนเต็ม และมีความถูกต้องเสมอ
##ตัวอย่าง Input / Output
```
1 Monday
2 Tuesday
3 Wednesday
4 Thursday
5 Friday
6 Saturday
7 Sunday
What day is today? (Please enter number.): 1
What time is it?
-Hours: 18
-Minutes: 00
Air conditioner is ON.
```

```
1 Monday
2 Tuesday
3 Wednesday
4 Thursday
5 Friday
6 Saturday
7 Sunday
What day is today? (Please enter number.): 7
What time is it?
-Hours: 18
-Minutes: 01
Air conditioner is ON.
```

```
1 Monday
2 Tuesday
3 Wednesday
4 Thursday
5 Friday
6 Saturday
7 Sunday
What day is today? (Please enter number.): 7
What time is it?
-Hours: 17
-Minutes: 52
What Temperature is it? (Celsius): 35
Air conditioner is OFF.
```

```
1 Monday
2 Tuesday
3 Wednesday
4 Thursday
5 Friday
6 Saturday
7 Sunday
What day is today? (Please enter number.): 6
What time is it?
-Hours: 17
-Minutes: 52
What Temperature is it? (Celsius): 36
Do you have someone at home? (Yes = 1/No = 0): 1
Air conditioner is ON.
```

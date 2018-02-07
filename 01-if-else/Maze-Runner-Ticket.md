# Maze Runner Ticket.

วันหนึ่งนิสิตภาควิชาวิทยาการคอมพิวเตอร์ของมหาวิทยาลัยย่านบางเขนคนหนึ่งอยากไปดูหนังเรื่อง Maze runner 3 ที่โรงหนังแห่งหนึ่งจึงทำการเข้าไปเช็ครอบหนังของแต่ละเรื่อง โดยมีเวลาฉายของแต่ละรอบเป็นดังนี้

![enter image description here](https://lh3.googleusercontent.com/xRs66BBmUMeJOjAWZ_q-wVvGVYw-NSLTTeRZh1NEy78qMOr0E6U3EoaLFQpTJWokoMY9ohMfDnU)

และโรงหนังแห่งนี้มีระบบสมัครสมาชิกอยู่ 2 แบบด้วยกันซึ่งแต่ละชนิดจะมีสิทธิพิเศษดังนี้ ได้แก่
![enter image description here](https://lh3.googleusercontent.com/X1jxry6Eg8Qbl8UrCogPLh4qs8tK1loyUQClbOkaE1-bK86APadv2kBBicnxgx3RBe-CW8_KIjo)

**ให้นิสิตทำการเขียนโปรแกรมที่ :**
1. บรรทัดแรกรับประเภทของหนังเป็นจำนวนเต็ม
* 1 คือ (3D)
- 2 คือ (4DX)
2. บรรทัดที่สอง รับชนิดของSoundtrack เป็นจำนวนเต็ม
- 1 คือ (thai)
- 2 คือ (subthai)
3. บรรทัดที่สาม รับเวลาของรอบหนังที่เลือก (1 / 2 / 3) เป็นเลขจำนวนเต็ม
4. บรรทัดที่สี่ รับชนิดของการเป็นสมาชิกโรงหนังเป็นจำนวนเต็ม
* 1 คือ (Movie pass)
* 2 คือ (M generator)
5. บรรทัดที่ห้าให้ปริ้นท์ในรูปแบบชนิดของสมาชิกและสิทธิพิเศษ
6. บรรทัดที่หกให้ปริ้นท์จำนวนเงินที่ต้องจ่ายเป็นจำนวนเต็ม
โดยการันตีว่า input ที่เข้ามาจะมีเพียงรูปแบบที่ดังที่ให้ไว้เท่านั้น

ปล.หากเลือกช่วงเวลาที่ไม่มีรอบหนังฉายให้ทำการปริ้นท์  “Didn’t have movie in this time.” แค่บรรทัดเดียว

### Test Case I
```
**Input**
Select type movie 1 (3D) or 2 (4DX): 2
Select soundtrack 1 (thai) or 2 (subthai): 2
Select show time of movie (1, 2, 3): 2
Select your member card 1 (Movie pass) or 2 (M generator): 2

**Output**
Didn’t have movie in this time.
```
### Test Case II
```
**Input**
Select type movie 1 (3D) or 2 (4DX): 1
Select soundtrack 1 (thai) or 2 (subthai): 1
Select show time of movie (1, 2, 3): 1
Select your member card 1 (Movie pass) or 2 (M generator): 1
**Output**
Member card: Movie pass / Your Privilege : free!!
Price = 0
```


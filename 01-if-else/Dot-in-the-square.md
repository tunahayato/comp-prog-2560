# **โจทย์ปัญหา if-else** 
## **ชื่อโจทย์ : จุดอยู่ในสี่เหลี่ยมหรือไม่ ? และสี่เหลี่ยมอะไร ? \(Dot in the square?\)**
### ให้รับพิกัดของจุดที่เป็นมุมของสี่เหลี่ยมโดยที่มุมที่รับเป็นมุมบน-ซ้าย \(x, y\) ของสี่เหลี่ยม และรับระยะทางจากจุดมุมบน-ซ้ายของสี่เหลี่ยมไปทางทิศตะวันออกและทิศใต้ ตามแนวฉาก \(Eastern and Southern\) ของสี่เหลี่ยม และรับพิกัดจุดจุดหนึ่ง \(a, b\) แล้วให้แสดงผลว่าจุดที่รับค่ามานั้นอยู่ในพื้นที่สี่เหลี่ยมหรือไม่ และเป็นสี่เหลี่ยมผืนผ้า \(rectangle\) หรือสี่เหลี่ยมจัตุรัส \(square\)
#### \*\*หมายเหตุ\*\*  พิกัดที่รับค่าระยะทางไปทางทิศตะวันออกและทิศใต้ตามแนวฉากต้องมีค่ามากกว่า 0 ทั้งสองค่าเสมอ ถ้าพิกิดที่รับค่าระยะทางไม่เป็นไปตามหมาย เหตุให้แสดงข้อความ  Input is not rectangle or square\.
---
>1)  **ความต้องการของโปรแกรม** คือ **ตรวจสอบจุด \(a, b\) ที่รับค่ามาว่าอยู่ในพิกัดสี่เหลี่ยมผืนผ้าหรือจัตุรัสหรือไม่ โดยพิกัดจะกำหนดโดยมีจุดมุมบน-ซ้ายของสี่เหลี่ยมและระยะทางไปทางทิศตะวันออกและทิศใต้ตามแนวฉากของสี่เหลี่ยม**
>
>2) **ข้อมูลนำเข้า \(Input\)** คือ **พิกัดสี่เหลี่ยมผืนผ้าหรือจัตุรัส และจุดหนึ่งจุด**
>
>3) **ข้อมูลออก \(Output\)** คือ **จุดอยู่ในสี่เหลี่ยมผืนผ้าหรือจัตุรัส หรือ จุดไม่ได้อยู่ในสี่เหลี่ยมผืนผ้าหรือจัตรัส**
>
>4) **ตัวอย่างของ Input/Output ดังนี้**

                    Enter the rectangle or square:
    Input square:   ~~ x-axis: 5
                    ~~ y-axis: 5
                    ~~ Eastern: 0
                    ~~ Southern: 0
                    Enter a coordinate: 
    Input dot:      Input x-axis: 1
                    Input y-axis: 2
    Output:         Input is not rectangle or square.
---
                    Enter the rectangle or square:
    Input square:   ~~ x-axis: 5
                    ~~ y-axis: 5
                    ~~ Eastern: 5
                    ~~ Southern: 5
                    Enter a coordinate:
    Input dot:      Input x-axis: 6
                    Input y-axis: 4
    Output:         ~ (6,4) is inside the square.
--- 
                    Enter the rectangle or square:
    Input square:   ~~ x-axis: 4
                    ~~ y-axis: 6
                    ~~ Eastern: 3
                    ~~ Southern: 10
                    Enter a coordinate:
    Input dot:      Input x-axis: 8
                    Input y-axis: -7
    Output:         ~ (8,-7) is not inside the rectangle.
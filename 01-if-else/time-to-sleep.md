# กฏการนอน 90 นาที

         คือ วิธีนอนไม่ให้ตื่นมางัวเงีย นอนให้ครบรอบ90นาที ทางฝรั่งวิจัยแล้วยืนยันได้ผลจริง เพราะร่างกายมีวงจรการหลับ ช่วงหลับลึก/ฝัน รวม90นาที ว่าง่ายๆ คือ ทุกๆ90นาทีสามารถตื่นโดยไม่ง่วงแม้นอนน้อย 

         โดยโปรแกรมนี้จะคำนวณเวลาที่คุณควรจะนอน โดยให้คุณกรอกว่าจะต้องการ ‘ตื่น’ กี่โมง และให้คุณเลือก level ระยะเวลาการ ‘นอน’ ซึ่งมีให้เลือกถึง 10 ระดับ
        
1. Level 1 1 hours 30 minutes
2. Level 2 3 hours 0  minutes
3. Level 3 4 hours 30 minutes
4. Level 4 6 hours 0 minutes
5. Level 5 7 hours 30 minutes
6. Level 6 9 hours 0  minutes
7. Level 7 10 hours 30 minutes
8. Level 8 12 hours 0 minutes
9. Level 9 13 hours 30 minutes
10. Level 10 15 hours 0 minutes

         และบอกเวลาที่เหมาะสมกับอายุของคุณ

        0-3 months sleep range 14-17 hours.
        14-17 months sleep range 12-15 hours.
        1-2 years sleep range 11-14 hours.
        3-5 years sleep range 10-13 hours.
        6-13 years sleep range 9-11 hours.
        14-17 years sleep range 8-10 hours.
        18-25 years sleep range 7-9 hours.
        26-64 years sleep range 7-9 hours.
        65+ years sleep range 7-8 hours.

 **ข้อมูล Input**
<br/>รับค่าอายุที่เป็นจำนวนเต็ม
<br/>รับค่าเวลาที่ต้องการตื่น แยกเป็นชั่วโมงกับนาที
<br/>เลือกเลเวลที่ต้องการจะนอน

 **ข้อมูล Output**
<br/>จะบอกว่าคุณควรจะนอนกี่โมง
<br/>บอกว่าคุณนอนมากหรือน้อย และอายุของคุณควรนอนกี่ชั่วโมง

**Example 1**
<br/>How old are you?(years) : 0
<br/>How old are you?(months) : 2

What time do you want to wake up ?
<br/>Enter hours (0-23) : 1
<br/>Enter minutes (0-59) : 0
<br/> Time is 01:00

Level to sleep (1 - 10) : 10
<br/> Time to sleep 10:00
<br/>You sleep well

**Example 2**
<br/>How old are you?(years) : 67
<br/>How old are you?(months) : 6

What time do you want to wake up ?
<br/>Enter hours (0-23) : 4
<br/>Enter minutes (0-59) : 4
<br/> Time is 04:04

Level to sleep (1 - 10) : 7
<br/> Time to sleep 17:34
<br/>You sleep so much.
<br/>You should sleep range 7-8 hours.

**Example 3**
<br/>How old are you?(years) : 37
<br/>How old are you?(months) : 2

What time do you want to wake up ?
<br/>Enter hours (0-23) : 2
<br/>Enter minutes (0-59) : 45
<br/> Time is 02:45

Level to sleep (1 - 10) : 4
<br/> Time to sleep 20:34
<br/>You sleep less.
<br/>You should sleep range 7-9 hours.

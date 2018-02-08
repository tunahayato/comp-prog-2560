# Traffic in Bangkok
**จงเขียนโปรแกรมรายงานการจราจรในกรุงเทพ**
1. รับค่าวันที่ออกเดินทาง โดย
- วันจันทร์ = 1 
- วันอังคาร = 2
- วันพุธ = 3
- วันพฤหัส = 4
- วันศุกร์ = 5
- วันเสาร์ = 6
- วันอาทิตย์ = 7
2. รับค่าเวลาที่ออกเดินทางโดยประมาณเป็นชั่วโมง โดย เที่ยงคืน = 0 ตีหนึ่ง = 1 ไปเรื่อยๆ...จนถึง 5 ทุ่ม = 23
3. รับค่าว่าเป็นวันหยุดหรือไม่ โดย
- วันปีใหม่ = 1
- วันสงกรานต์ = 2
- วันลอยกระทง = 3
- วันหยุดนักขัตฤกษ์อื่นๆ = 4
- และถ้าไม่ใช่วันหยุด = 0
4. และรับค่าว่าฝนตกหรือไม่ ถ้าฝนตก = 1 ถ้าฝนไม่ตก = 2
#### โดย output ที่ออกมามี 3 แบบ คือ ***Very Traffic jam.***(รถติดมาก), Traffic jam.(รถติด) และ Traffic is good.(รถไม่ติด)
- โดยกรณีที่รถติดมาก(***Very Traffic jam.***) มีดังนี้
    - ไม่ว่าจะเป็นวันอะไรถ้าฝนตกจะรถติดมาก
    - ในกรณีที่ฝนไม่ตก ถ้าเป็นวันสงกรานต์หรือวันลอยกระทง รถจะติดมาก
    - ในกรณีที่ฝนไม่ตก และไม่เป็นวันหยุด ถ้าเป็นวันจันทร์เช้า(6โมงถึง9โมง) และวันศุกร์เย็น(4โมงเย็นถึง2ทุ่ม) รถจะติดมาก
- โดยกรณีที่รถติด(Traffic jam.) มีดังนี้
    - ทุกวันที่ไม่ใช่วันเสาร์อาทิตย์ ตอนเช้า(6โมงถึง9โมง) และเย็น(4โมงเย็นถึง2ทุ่ม) รถจะติดเพราะเป็นเวลาไปทำงานและเป็นเวลาเลิกงาน
- โดยกรณีที่รถไม่ติด(Traffic is good.) มีดังนี้
    - ถ้าเป็นวันปีใหม่รถจะไม่ติดเพราะคนกลับต่างจังหวัดกันหมด และวันหยุดนักขัตฤกษ์อื่นๆรถจะไม่ติด
    - ทุกกรณีนอกเหนือจากกรณีด้านบน
#### และถ้าข้อมูลไม่ถูกต้องให้พิมพ์ ERROR
**ตัวอย่าง Input/Output**
####
         Monday = 1
         Tuesday = 2
         Wednesday = 3
         Thursday = 4
         Friday = 5
         Saturday = 6
         Sunday = 7
    What day do you leave home?: 5
    What time do you leave home? (0-23 0'clock): 8
         New Year Day = 1
         Songkran Day = 2
         Loi Kra Thong Day = 3
         Holiday = 4
    What day is New Year Day/Songkran Day/Loi Kra Thong Day/Holiday? (0 = No): 3
    Is it rainny? (Y = 1/N = 2): 2
    ***Very Traffic jam.***

####
         Monday = 1
         Tuesday = 2
         Wednesday = 3
         Thursday = 4
         Friday = 5
         Saturday = 6
         Sunday = 7
    What day do you leave home?: 4 
    What time do you leave home? (0-23 0'clock): 19
         New Year Day = 1
         Songkran Day = 2
         Loi Kra Thong Day = 3
         Holiday = 4
    What day is New Year Day/Songkran Day/Loi Kra Thong Day/Holiday? (0 = No): 0
    Is it rainny? (Y = 1/N = 2): 2
    Traffic jam.

####
         Monday = 1
         Tuesday = 2
         Wednesday = 3
         Thursday = 4
         Friday = 5
         Saturday = 6
         Sunday = 7
    What day do you leave home?: 7
    What time do you leave home? (0-23 0'clock): 10
         New Year Day = 1
         Songkran Day = 2
         Loi Kra Thong Day = 3
         Holiday = 4
    What day is New Year Day/Songkran Day/Loi Kra Thong Day/Holiday? (0 = No): 0
    Is it rainny? (Y = 1/N = 2): 2
    Traffic is good.

####
         Monday = 1
         Tuesday = 2
         Wednesday = 3
         Thursday = 4
         Friday = 5
         Saturday = 6
         Sunday = 7
    What day do you leave home?: 6
    What time do you leave home? (0-23 0'clock): -3
         New Year Day = 1
         Songkran Day = 2
         Loi Kra Thong Day = 3
         Holiday = 4
    What day is New Year Day/Songkran Day/Loi Kra Thong Day/Holiday? (0 = No): 0
    Is it rainny? (Y = 1/N = 2): 1
    ERROR
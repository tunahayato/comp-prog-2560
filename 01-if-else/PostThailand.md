# ไปรษณีย์ไทย
เขียนโปรแกรมสำหรับการคำนวณเงินที่ต้องใช้ในการส่งพัสดุ บอกประเภทที่ควรจัดส่งพัสดุ และค่าประกันสิ่งของที่ทำการส่ง จากข้อมูลนำเข้าทั้งหมด 

**การคำนวณเงินที่ใช้ในการจัดส่ง**

    ราคาของรูปแบบกล่องที่ใช้ + ราคาของรูปแบบซองจดหมายที่ใช้ + ค่าจัดส่งตามประเภทที่จัดส่ง + ไปรษณีย์ตอบรับ 

**ราคาของกล่องจดหมายที่ใช้ในการส่งพัสดุ**
| ชนิดของกล่องจดหมาย | ราคา |
| --------- | ---------- |
|  กล่องจดหมำยรูปแบบ A (14 x 20 x 6 cm.)    |    9 บาท|
|  กล่องจดหมำยรูปแบบ B (17 x 25 x 9 cm.)   |    12 บาท|
|  กล่องจดหมำยรูปแบบ C (20 x 30 x 11 cm.)   |    12 บาท|

**ราคาของซองจดหมายที่ใช้ในการส่งพัสดุ**
| ชนิดของซองจดหมาย | ราคา |
| --------- | ---------- |
|  ซองจดหมำยรูปแบบ A (114 x 162 mm.)     |    1.5 บาท|
|  ซองจดหมำยรูปแบบ B (110 x 220 mm.)   |    2 บาท|

**ประเภทของการส่ง**
1.  **ประเภทลงทะเบียน (REGISTRATION)** ประเภทนี้จะใช้เวลาในการทำการส่งคือ 3-7 วัน ค่ารับประกันสินค้าอยู่ที่สูงสุดแค่ 300 บาทโดยมูลค่าสินค้ามีค่าน้อยกว่า 300 บาทจะจ่ายตามมูลค่าของสินค้า แต่ถ้ามากกว่า 300 บาทจะได้สูงสุดที่ 300 บาทเท่านั้นน้ำหนักที่จะสามารถส่งได้ต้องไม่เกิน 2 กิโลกรัม โดยอัตราค่าส่งอยู่ที่ 10 บาท 
2.  **ประเภท EMS** ประเภทนี้จะใช้เวลาในการทำการส่ง 1-2 วัน ค่ารับประกันสินค้าอยู่ที่สูงสุด 1000 บาทโดยถ้ามูลค่าสินค้ามีค่าน้อยกว่า 1000 บาท จะจ่ายตามมูลค่าของสินค้า แต่ถ้ามากกว่า 1000 บาทจะได้สูงสุดที่ 1000 บาทเท่านั้น น้ำหนักที่สามารถส่งได้ต้องไม่เกิน 30 กิโลกรัม
โดยอัตราค่าส่งอยู่ที่ถ้าน้ำหนักน้อยกว่าเท่ากับ 15 กิโลกรัม อัตราค่าส่ง 30 บาทถ้าน้ำหนักมากกว่า 15 กิโลกรัม อัตราส่งอยู่ที่ 60 บาท 

**ไปรษณีย์ตอบรับ**
*   ส่งแบบลงทะเบียนเสียเงิน 8 บาท
*   ส่งแบบ EMS เสียงเงิน 12 บาท 

**ถ้าเกิดข้อมูลนำเข้าเกิดข้อผิดพลาด**

จะแสดงผลตามข้อมูลนำเข้าที่ผิดพลาด และประเภทการส่งเป็น none ค่าใช้จ่ายทั้งหมดที่ใช้ในการส่งและค่าประกันสินค้ามีค่าเป็น 0 ถ้าเกิดข้อผิดพลาดหลายจุดจะแสดงผลทั้งหมดที่ผิดพลาด ยกเว้น น้ำหนักของสินค้าไม่สัมพันธ์กับวันที่ต้องการส่ง จะพิมแค่อันเดียวเท่านั้น ข้อความที่แสดงเมื่อเกิดข้อผิดพลาด มีดังนี้

*   รูปแบบกล่องผิดพลาด แสดงข้อความ "ERROR : your input (product:box) is not correct"
*   รูปแบบซองจดหมายผิดพลาด แสดงข้อความ "ERROR : your input (product:envelope) is not correct."
*   น้ำหนักสิ่งของผิดพลาด แสดงข้อความ "ERROR : your input (weight) is not correct."
*   จำนวนวันที่ส่งผิดพลาด แสดงข้อความ "ERROR : your input (times) is not correct."
*   มูลค่าของสิ่งของผิดพลาด แสดงข้อความ "ERROR : your input (price of thing) is not correct."
*   ต้องการไปรษณีย์ตอบรับผิดพลาด แสดงข้อความ "ERROR : your input (advice) is not correct."
*   น้ำหนักของสินค้าไม่สัมพันธ์กับวันที่ต้องการส่ง แสดงข้อความ "ERROR : It’s can’t delivery."
    

#### ข้อมูลนำเข้า
1.  แสดงข้อความ "Enter your box size:    "   และรับจำนวนเต็มของรูปแบบกล่องที่ใช้ส่ง
2.  แสดงข้อความ "Enter your envelope size:   "   และรับจำนวนเต็มของรูปแบบซองจดหมายที่ใช้ส่ง
3.  แสดงข้อความ "Enter your weight of parcel post (1-30 kg.):    " และรับจำนวนเต็มของน้ำหนักสิ่งของที่ต้องการส่ง
4.  แสดงข้อความ "Enter times do you need to deliver (1-7 day):"  และรับจำนวนเต็มของจำนวนวันที่ต้องการทำการจัดส่งให้ถึงมือผู้รับ
5.  แสดงข้อความ "Enter your price of thing:  "   และรับจำนวนเต็มของมูลค่าของสิ่งของที่ทำการส่งพัสดุ
6.  แสดงข้อความ "Do you want a advice of delivery (Yes = 1,No = 0):  "   และรับจำนวนเต็มของความต้องการใช้บริการตอบรับ
#### ข้อมูลที่นำออก
1. แสดงข้อความ "Types of deliver : "   ตามด้วยประเภทของการส่ง
2. แสดงข้อความ "Totals expenses : "   ตามด้วยค่าใช้จ่ายทั้งหมดที่ใช้ในการส่งพัสดุ
3. แสดงข้อความ "Price guarantee of parcel: " ค่าประกันสินค้า

## ตัวอย่าง Input/Output 

                    *THAILAND POST CO.,LTD.*
    --------------------------------------------------------
    Boxes's sizes : - Type A = 1
                    - Type B = 2
                    - Type C = 3
                    - None = 0
    --------------------------------------------------------
    Envelopes's sizes : - Type A = 1
                        - Type B = 2
                        - None = 0
    --------------------------------------------------------
    Enter your box size: 4
    Enter your envelope size: 3
    Enter your weight of parcel post (1-30 kg.): 0
    Enter times do you need to deliver (1-7 day): 0
    Enter your price of thing: 0
    Do you want a advice of delivery (Yes = 1,No = 0): 2
    ---------------------------------------------------------
    ERROR : your input (product:box) is not correct.
    ERROR : your input (product:envelope) is not correct.
    ERROR : your input (weight) is not correct.
    ERROR : your input (times) is not correct.
    ERROR : your input (price of thing) is not correct.
    ERROR : your input (advice) is not correct.
    Types of deliver : None
    Totals expenses : 0.00 baths.
    Price guarantee of parcel : 0.00 baths.

##

                    *THAILAND POST CO.,LTD.*
    --------------------------------------------------------
    Boxes's sizes : - Type A = 1
                    - Type B = 2
                    - Type C = 3
                    - None = 0
    --------------------------------------------------------
    Envelopes's sizes : - Type A = 1
                        - Type B = 2
                        - None = 0
    --------------------------------------------------------
    Enter your box size: 2
    Enter your envelope size: 0
    Enter your weight of parcel post (1-30 kg.): 2
    Enter times do you need to deliver (1-7 day): 7
    Enter your price of thing: 500
    Do you want a advice of delivery (Yes = 1,No = 0): 1
    ---------------------------------------------------------
    Types of deliver : REGISTRATION
    Totals expenses : 30.00 baths.
    Price guarantee of parcel : 300.00 baths.

##
                    *THAILAND POST CO.,LTD.*
    --------------------------------------------------------
    Boxes's sizes : - Type A = 1
                    - Type B = 2
                    - Type C = 3
                    - None = 0
    --------------------------------------------------------
    Envelopes's sizes : - Type A = 1
                        - Type B = 2
                        - None = 0
    --------------------------------------------------------
    Enter your box size: 0
    Enter your envelope size: 0
    Enter your weight of parcel post (1-30 kg.): 25
    Enter times do you need to deliver (1-7 day): 3
    Enter your price of thing: 5000
    Do you want a advice of delivery (Yes = 1,No = 0): 1
    ---------------------------------------------------------
    ERROR : It's can't delivery.
    Types of deliver : None
    Totals expenses : 0.00 baths.
    Price guarantee of parcel : 0.00 baths.

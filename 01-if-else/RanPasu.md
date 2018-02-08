**ตู้เติมเงินมือถือป้าสุ**

ป้าสุมีตู้บริการเติมเงินโทรศัพท์มือถือออนไลน์โดยป้าสุจะได้กำไรจากการเติมจากลูกค้าแต่ละครั้งเท่ากับ 3.5% ทุกเครือข่าย เมื่อลูกค้ามาใช้บริการ ลูกค้าจะต้องกรอกหมายเลขโทรศัพท์, จำนวนเงินที่เหลืออยู่ และเลือก
เครือข่าย โดยกำหนดให้ DTAC เป็นเครือข่ายที่ 1, AIS เป็นเครือข่ายที่ 2, TRUE เป็นเครือข่ายที่ 3  
ถ้าลูกค้ากรอกเบอร์โทรผิดระบบจะแจ้งว่า “Sorry, the number you have pressed is incorrect.”  
แต่ถ้าลูกค้ากรอกเบอร์โทรศัพท์ถูก ระบบจะคำนวณต่อ โดยถามว่าต้องการเติมเงินเท่าไหร่ และคำนวณออกมาให้ผู้ใช้ทราบจำนวน
เงินหลังเติมแล้ว หลังจากผู้ใช้เสร็จสิ้นการใช้งาน ระบบจะส่งผลกำไรให้ป้าสุผ่าน SMS จงเขียนโปรแกรมตู้เงินป้าสุ
เพื่อคำนวณเงินของลูกค้า และกำไรของป้าสุหลังลูกค้าเสร็จสิ้นการใช้งาน

**ตัวอย่าง Input/Output 1**

    Welcome to Ran Pasu :D
    Your number: (+66)123456
    Sorry, the number you have pressed is incorrect.

**ตัวอย่าง Input/Output 2**

    Welcome to Ran Pasu :D
    Your number: (+66)123456789
    What's your balance currently (baht): 50
    Please choose your system.
    DTAC press 1 | AIS press 2 | TRUE press 3
    Answer: 1
    Top Up amount: 275
    Pasu has just topped up your phone (DTAC) by 275.00 baht.
    Your balance is currently 325.00 baht.
    Please check your SMS to make sure that the balance is correctly.
    *-*-*-*-*-*-Thank you for chooseing us-*-*-*-*-*-*
    -----------------------------------------------------------------
    Pasu's income is 11.38 baht.

# Formatting Message
## Problem

แสดงข้อความจากข้อมูลที่ผู้ใช้ส่งเข้าไปโดยใช้เงื่อนไขดังนี้

- Message
    - คือข้อความหลักที่ผู้ใช้ส่งเข้าไป
    - หากเลือกเปิด block offensive word option ข้อความที่มี offensive word จะไม่แสดงผล (ในที่นี้สมมติเป็นคำว่า ‘fack’ ทั้งอักษรตัวใหญ่ทุกตัว ตัวเล็กทุกตัว และตัวใหญ่ตัวเล็กปนกัน)
    - หากเลือกปิด block offensive word option ข้อความจะแสดงผลในทุกกรณี
- Date
    - คือวันที่ส่งข้อความ
    - รับข้อมูลโดยใช้ 3 ตัวแปร ได้แก่ day เก็บจำนวนเต็มวันที่ month เก็บจำนวนเต็มเดือน year เก็บจำนวนเต็มปี
    - กำหนดให้ปีที่ถูกต้องคือปี 1980-1985 เท่านั้น
    - หากวันที่ เดือน หรือปีไม่ถูกต้อง จะแสดงข้อความบอกจุดที่ข้อมูลไม่ถูกต้องทุกจุดเรียงต่อกันในข้อความเดียว
    - หากข้อมูลที่รับมาทั้งหมดถูกต้อง จะแสดงผลในรูปแบบ day/month/year
- Time
    - คือเวลาที่ส่งข้อความ
    - รับข้อมูลโดยใช้ 3 ตัวแปร ได้แก่ hour เก็บจำนวนเต็มชั่วโมง minute เก็บจำนวนเต็มนาที second เก็บจำนวนเต็มวินาที
    - หากชั่วโมง นาที หรือวินาทีไม่ถูกต้อง จะแสดงข้อความบอกจุดที่ข้อมูลไม่ถูกต้องทุกจุดเรียงต่อกันในข้อความเดียว
    - หากข้อมูลที่รับมาทั้งหมดถูกต้อง จะแสดงผลในรูปแบบ hour:minute:second
- Sender
    - คือชื่อผู้ส่งข้อความ
    - หากชื่อตรงกับชื่อ admin จะมี (Admin) ต่อท้ายชื่อ (ในที่นี้สมมติว่า admin ชื่อ Chorn)
    - หากเป็นชื่ออื่นจะแสดงผลชื่อนั้นตามปกติ

## Input/Output
- Input
    - message (string)
    - sending day (int)
    - sending month (int)
    - sending year (int)
    - sending hour (int)
    - sending minute (int)
    - sending second (int)
    - sender name (string)
    - block offensive word (int, 0=no or 1=yes)
- Output
    - ข้อความและรายละเอียดของข้อความที่ถูกจัดรูปแล้ว ได้แก่ sender, date, time, message บรรทัดละหัวข้อ

## Test case
- Test case #1

    ```
    //Input
    --------------------
    Welcome user!
    --------------------
    Enter message here (max 99 chars, no space): What-the-FacK
    Enter sending day here: 5
    Enter sending month here: 5
    Enter sending year here: 1985
    Enter sending hour here: 1
    Enter sending minute here: 1
    Enter sending second here: 56
    Enter sender name here (max 99 chars, no space): gg
    Block message that contains offensive word? (1 = Yes, 0 = No): 1

    //Output
    --------------------
    Result
    --------------------
    Sender: gg
    Date: 5/5/1985
    Time: 1:1:56
    Message: This message has been blocked due to containing an offensive word(s)!
    ```

- Test case #2

    ```
    //Input
    --------------------
    Welcome user!
    --------------------
    Enter message here (max 99 chars, no space): message
    Enter sending day here: 5
    Enter sending month here: 5
    Enter sending year here: 1984
    Enter sending hour here: 5
    Enter sending minute here: 5
    Enter sending second here: 5
    Enter sender name here (max 99 chars, no space): Chorn
    Block message that contains offensive word? (1 = Yes, 0 = No): 1

    //Output
    --------------------
    Result
    --------------------
    Sender: Chorn (Admin)
    Date: 5/5/1984
    Time: 5:5:5
    Message: message
    ```

- Test case #3

    ```
    //Input
    --------------------
    Welcome user!
    --------------------
    Enter message here (max 99 chars, no space): fackky
    Enter sending day here: 5
    Enter sending month here: 5
    Enter sending year here: 1983
    Enter sending hour here: 25
    Enter sending minute here: 60
    Enter sending second here: 61
    Enter sender name here (max 99 chars, no space): tt
    Block message that contains offensive word? (1 = Yes, 0 = No): 1

    //Output
    --------------------
    Result
    --------------------
    Sender: tt
    Date: 5/5/1983
    Time: Error - Invalid hour. Error - Invalid minute. Error - Invalid second.
    Message: This message has been blocked due to containing an offensive word(s)!
    ```

- Test case #4

    ```
    //Input
    --------------------
    Welcome user!
    --------------------
    Enter message here (max 99 chars, no space): s
    Enter sending day here: 5
    Enter sending month here: 5
    Enter sending year here: 1987
    Enter sending hour here: 5
    Enter sending minute here: 5
    Enter sending second here: 5
    Enter sender name here (max 99 chars, no space): d
    Block message that contains offensive word? (1 = Yes, 0 = No): 1

    //Output
    --------------------
    Result
    --------------------
    Sender: d
    Date: Error - Invalid year -> This year is 1985. You must have a time machine!!! Error - Couldn't validate day due to an error of year and/or month.
    Time: 5:5:5
    Message: s
    ```

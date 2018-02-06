# ขนมปังเหลี่ยมบนจานกลม

> เด็กชายคนหนึ่งรู้สึกหิวมาก เลยวิ่งไปซื้อขนมปังที่ Seven Eleven หน้าปากซอย มาปิ้งกินที่ บ้าน หลังจากปิ้งในเตาอบเสร็จแล้ว เด็กชายคนนี้ก็ได้เอาจานขนาด 100 x 100 หน่วยมา เพื่อที่จะมาใส่ขนมปังไปกินหน้าคอมพิวเตอร์ของเขา แต่ว่าการที่จะใส่ขนมปังลงในจานโดยไม่ หล่นออกจากจานเป็นเรื่องยากมาก ดังนั้นเด็กชายคนนี้จึงเริ่มเขียนโปรแกรมคํานวนการวาง ขนมปังบนจาน ว่าขนมปังจะตกออกนอกจานหรือไม่

- **ข้อมูลนำเข้า** -
กําหนดให้รับ Input 4 ค่าคือ x1, y1, x2, y2 เป็นพิกัดจุด มุมบน และมุมล่างของ ขนมปัง

- **ข้อมูลออก** -
 ถ้าหากขนมปังวางบนจานโดยไม่มีส่วนใดเกินออกมา ให้แสดงข้อความว่า BREAD IS IN THE PLATE แต่ถ้าไม่อยู่ในพื้นที่จานให้แสดงข้อความออกมาว่า BREAD IS NOT IN THE PLATE ถ้าหาก Input มีค่าเกิน 100 หรือน้อยกว่า 0 ให้แสดงค่า INPUT ERROR

## ทดสอบชุดคําสั่ง (Test Case)
<center>
<img src="https://image.ibb.co/hbh3mH/Screen_Shot_2561_02_06_at_16_17_06.png">

<table>
    <thead>
        <tr>
            <td>INPUT</td>
            <td>OUTPUT</td>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                Enter position 1 (X): 10<br>
                Enter position 1 (Y): 10<br>
                Enter position 2 (X): 50<br>
                Enter position 2 (Y): 50<br>
            </td>
            <td>
                BREAD IS NOT IN THE PLATE
            </td>
        </tr>
        <tr>
        <td>
            Enter position 1 (X): 30<br>
            Enter position 1 (Y): 30<br>
            Enter position 2 (X): 70<br>
            Enter position 2 (Y): 70<br>
        </td>
        <td>
            BREAD IS IN THE PLATE
        </td>
        </tr>
    </tbody>
</table>
</center>


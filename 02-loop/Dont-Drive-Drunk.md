# Don't Drive Drunk

ถ้าคุณต้องการที่จะไปดื่มสังสรรค์กับเพื่อนแต่ไม่รู้ว่าที่คุณดื่มไปนั้นมีแอลกอฮอล์เท่าไหร่ และ คุณจะสามารถขับรถกลับบ้านได้หรือไม่  โดยร้านที่คุณดื่มนั้นมีเครื่องดื่มอยู่ 3 ชนิด โดยแต่ละชนิดมีปริมาณแอลกอฮอล์ต่อแก้วไม่เหมือนกัน ดังนี้

1. เบียร์ มีแอลกอฮอล์ 10 mg%
2. ไวน์ มีแอลกอฮอล์ 12 mg%
3. สุรา มีแอลกอฮอล์ 13 mg%

ตามที่กฎหมายได้กำหนดไว้ว่า ถ้าแอลกอฮอร์ในร่างกายมีค่าเกินกว่า 50 mg% จะถือว่าเมาตามกฎหมาย และไม่สามารถขับรถได้ แต่ถ้าหากคุณเลือกที่จะนอนพักก่อน แอลกอฮอล์ในร่างกายจะลดลงไป 1 mg% ต่อชม.

ให้เขียนโปรแกรมเพื่อรับค่าว่าเราดื่มอะไรไปบ้าง โดยถ้าใส่ค่า 1 คือ beer ,2 คือ wine ,3 คือ liquor , -1 คือ ไม่ได้ดื่ม
    Ex. What do you drink? (beer=1/wine=2/liquor=3/not drink=-1):

โดยเมื่อเราใส่ว่าเราดื่มอะไรแล้ว ให้ถามว่าเราดื่มไปกี่แก้ว แล้วจะวนลูปมาถามว่าเราดื่มไรอีก
    โดยถ้าเลือก beer   ให้แสดงว่า “How many glasses of beer?:”
    โดยถ้าเลือก wine   ให้แสดงว่า “How many glasses of wine?:”
    โดยถ้าเลือก liquor ให้แสดงว่า “How many glasses of liquor?:”

เมื่อใส่ -1 แล้วออกจากลูปจะขึ้นถามว่านอนพักมั้ย  “What to nap?(yes=1,no=0):” ถ้าใส่ 1 จะ ถามต่อว่า “How many hour?:” แต่ถ้าใส่ 0 จะไม่ถามและขึ้นค่าแอลกอฮอล์ว่า “You have alcohol …. mg%” โดยถ้าค่าแอลกอฮอล์เกิน 50 จะขึ้น “You can not drive.” ถ้าไม่เกินจะขึ้น “You can drive.”

หมายเหตุ: ถ้าใส่ค่าติดลบตรงที่ถามว่า ดื่มกี่แก้วจะขึ้น ERROR

***
##### ตัวอย่างที่ 1
	What do you drink? (beer=1/wine=2/liquor=3/not drink=-1): 2
	How many glasses of wine?: 3
	What do you drink? (beer=1/wine=2/liquor=3/not drink=-1): -1
	Want to nap?(yes=1,no=0): 1
	How many hour?: 3
	You have alcohol 33 mg%
	You can drive.

---
##### ตัวอย่างที่ 2
	What do you drink? (beer=1/wine=2/liquor=3/not drink=-1): 1
	How many glasses of beer?: 2
	What do you drink? (beer=1/wine=2/liquor=3/not drink=-1): 2
	How many glasses of wine?: 2
	What do you drink? (beer=1/wine=2/liquor=3/not drink=-1): 3
	How many glasses of liquor?: 2
	What do you drink? (beer=1/wine=2/liquor=3/not drink=-1): -1
	Want to nap?(yes=1,no=0): 0
	You have alcohol 70 mg%
	You can not drive.

---
##### ตัวอย่างที่ 3
	What do you drink? (beer=1/wine=2/liquor=3/not drink=-1): 1
	How many glasses of beer?: -1
	ERROR

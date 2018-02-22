# Check diabetes case

ณ โรงพยาบาลแห่งหนึ่งคุณหมอต้องทำการตรวจน้ำตาลในเลือดของคนไข้  และอยากที่จะเก็บค่าน้ำตาลในเลือดของคนไข้ไว้และค่อยมาเช็คดูเคสที่ต้องการจะดูว่ามีคนไข้มีน้ำตาลในเลือดเท่าไหร่ โดยถ้าน้ำตาลในเลือดมี 70-100 mg/dL จะถือว่าปกติ แต่ถ้ามีมากกว่า 100-126 จะเสี่ยงต่อการเป็นเบาหวาน และ มากกว่า 126 คือเป็นเบาหวาน แต่ถ้าต่ำกว่า 70 ลงไปจะขาดน้ำตาลในเลือด

หมอสามารถรับคนไข้ได้ไม่เกิน 20 คนถ้ามากกว่า 20 หรือน้อยกว่าเท่ากับ 0 จะพิมพ์ ERROR

เขียนโปรแกรมรับจำนวนคนไข้ “How many patients?: ”

จากนั้นวนลูปเก็บค่าน้ำตาลในเลือดของคนไข้ เช่น คนที่1 “Enter blood sugar of you patients(1)”

จากนั้นให้เลือกว่าจะเช็คคนที่เท่าไหร่ “Check case number: ” ถ้าค่าน้อยกว่าหรือมากกว่า จำนวนคนไข้จะพิมพ์ “ERROR” และไม่ทำงานต่อ

สุดท้ายบอกค่าว่า  “FBS …..  mg/dL is …………. ” หลัง FBS คือค่าน้ำตาลในเลือดของ เคสที่เลือก และ หลัง is คือ ข้อความที่บอกถึงน้ำตาลในเลือด โดยแต่ละค่าจะเป็นข้อความดังนี้

1. ถ้าเคสที่เลือกค่าน้ำตาลน้อยกว่า 0 ให้พิมพ์แค่ “Mistake.”
1. น้อยกว่า 70 “ hypoglycemia.”
1. มากกว่าหรือเท่ากับ 70 และ น้อยกว่าหรือเท่ากับ 100 “ normal.”
1. มากกว่า 100 และ น้อยกว่าหรือเท่ากับ 126 “diabetes risk.”
1. มากกว่า 126 “diabetes.” 	

***
##### ตัวอย่างที่ 1
	How many patients?: 3
	Enter blood sugar of you patients(1): 70
	Enter blood sugar of you patients(2): 126
	Enter blood sugar of you patients(3): 130
	check case number: 3
	FBS 130 mg/dL is diabetes.
---
##### ตัวอย่างที่ 2
	How many patients?: 3
	Enter blood sugar of you patients(1): -70
	Enter blood sugar of you patients(2): -126
	Enter blood sugar of you patients(3): -130
	check case number: 1
	Mistake.
---
##### ตัวอย่างที่ 3
	How many patients?: 3
	Enter blood sugar of you patients(1): 70
	Enter blood sugar of you patients(2): 126
	Enter blood sugar of you patients(3): 130
	check case number: 4
	ERROR.

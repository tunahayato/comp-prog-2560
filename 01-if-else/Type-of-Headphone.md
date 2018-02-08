# Type of Headphone
ในการเลือกหูฟังชนิดหนึ่งจะมีปัจจัยที่กำหนดอยู่สามอย่างด้วยกันคือราคา ประเภทของหูฟัง
จงเขียนโปรแกรมที่จะทำการเลือกชนิดของหูฟังที่เหมาะกับผู้ซื้อ ทำการคำนวนเงินทอน
กำหนดราคาหูฟังแต่ละชนิดตามตารางต่อไปนี้

|      ชื่อ	       |   ประเภท	  |ราคา |
|----------------|--------------|-----|
|ATH IM 50	     |In ear	    |2990 |
|ATH LS70i	     |In ear 	    |4990 |
|SONY WH-H800	 |On ear	    |7990 |
|Beats EP	     |On ear 	    |4400 |
|SONY MDR H600A	 |Full size	    |5790 |
|AKG 701	     |Full size	    |7500 |
|Yuri Pk3	     |Earbud	    |1190 |
|Yuri Pk2	     |Earbud	    |1990 |

# Input/output

Input
- budget (int)
- type (int)

Output
- ชื่อของหูฟังที่ได้ และ ประเภทของเงินทอน

# Test case
Test case 1

    welcome to Headphone store
    -----------------------------------------------------------
    Put you budget: 4400
    Put you type of your ear phone: 1=Inear,2=Full size,3=Earbud,4=On ear: 5
    -----------------------------------------------------------
    Error
    -----------------------------------------------------------
    Thank you


Test case 2

    welcome to Headphone store
    -----------------------------------------------------------
    Put you budget: 7500
    Put you type of your ear phone: 1=Inear,2=Full size,3=Earbud,4=On ear: 2
    -----------------------------------------------------------
    You get AKG 701
    -----------------------------------------------------------
    You change is 0 baht
    1000 :0
    500 :0
    100 :0
    50 :0
    20 :0
    10 :0
    5 :0
    1 :0
    Thank you

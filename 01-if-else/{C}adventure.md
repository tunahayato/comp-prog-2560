# {C}adventure
ให้นิสิตเติมโค้ดให้โปรแกรมเกมภาษาซีนี้สมบูรณ์เพื่อสามารถรันเกมตอบคำถาม{C}adventure ได้โดยเกมนี้จะมีคำถามให้ 5 คำถามเป็นคำถามที่เกี่ยวกับภาษาซี โดยหวังว่าผู้ใช้โปรแกรมนี้จะได้ประโยชน์จากการทบทวนบทเรียนไปในตัว โดยใช้ if/else, Relation Operators และ/หรือ Logical Operators ในการแก้ปัญหา นิสิตต้องมีความรอบคอบในการแก้ปัญหานี้
```
#include <stdio.h>
void main ()
{
	char name[10], yesno, answer;
	int ____, ____;

	_____("Enter your name: ");
	____f("%s", name);
	____f("Welcome to the game {C}adventure >>>%s<<<. <3<3<3\n", name);
	p____f("This game is about learning c language.\n\n");
	p____f(">>>Now you have level <0>.\n");
	p____f("Want to start a game. [y:n]?");
	scanf("%s", &yesno);
	if (yesno=='y'|| yesno=='Y'){
		printf("Start Question\n");
		p____f("1.What is the file extension of the C language?\n");
		printf("a. .CPP\nb. .C\nc. .OBJ\nd. .BAS\n>>>>>Answer is? ");
		s__nf("%s",&answer);
		sum += 1;
		if (answer == 'b'){
		  level += 1;
		  printf("<<<<<Perfect>>>>>\n>>>>>>>>>>Level UP!!!<<<<<<<<<<\n");
		}else if(answer=='a' || answer=='c' || answer=='d'){
		  ______("<<<<<Unlucky>>>>>\n");
		}else{
		  p______________________________-\n");
		}printf("----------------------------------------------------------------------------------------------\n");
		printf("2.Which of the following describes how the program works?\n");
		printf("a. Pseudo-codes\nb. Flowchart\nc. Editor\nd. a. and b.\n>>>>>Answer is? ");
		s___f("%s", &answer);
		s__ += 1;
		if (answer == 'd'){
		  level += 1;
		  p______________________________________________________\n");
		}else if (answer == 'a' || answer == 'b' || answer == 'c'){
		  printf("<<<<<Unlucky>>>>>\n");
		}else{
		  printf(">>>>>>>>>>ERROR<<<<<<<<<<\n");
		}p___f("---------------------------------------------------------------------------------------------\n");
		printf("3.What words must have in every program in language c?\n");
		printf("a. int\nb. main\nc. var\nd. printf\n>>>>>Answer is? ");
		scanf("%s", &answer);
		sum += 1;
		if (answer == 'b'){
		  level += 1;
		  p____f("<<<<<Perfect>>>>>\n>>>>>>>>>>Level UP!!!<<<<<<<<<<\n");
		}else if (answer == 'a' || answer == 'c' || answer == 'd'){
		  printf("<<<<<Unlucky>>>>>\n");
		}else{
		  printf(">>>>>>>>>>ERROR<<<<<<<<<<\n");
		}printf("----------------------------------------------------------------------------------------------\n");
		printf("4.Command of the program in the C language. Must be within any marker.?\n");
		printf("a. ( )\nb. [ ]\nc. { }\nd. /* */\n>>>>>Answer is? ");
		scanf("%s", &answer);
		sum += 1;
		if (answer == 'c'){
		  level += 1;
		  p______________________________________________________\n");
		}else if (answer == 'a' || answer == 'b' || answer == 'd'){
		  p___________________________\n");
		}else{
		  printf(">>>>>>>>>>ERROR<<<<<<<<<<\n");
		}____tf("----------------------------------------------------------------------------------------------\n");
		printf("5.Use function printf(); What is wrong?\n");
		p___tf("a. printf(\"THAILAND\");\nb. printf(\"12345\");\nc. printf(\"5 + 2 = 7\");\nd. printf('COMPUTER');\n>>>>>Answer is? ");
		scanf("%s", &answer);
		sum += 1;
		if (answer == 'd'){
		  le__l += 1;
		  printf("<<<<<Perfect>>>>>\n>>>>>>>>>>Level UP!!!<<<<<<<<<<\n");
		}else if (answer == 'a' || answer == 'b' || answer == 'c'){
		  _____f("<<<<<_______>>>>>\n");
		}else{
		  printf(">>>>>>>>>>______<<<<<<<<<<\n");
		}
	}else if (yesno=='n' || yesno=='N'){
	  printf(">>>>>>>>>>GAME OVER!!!<<<<<<<<<<\n");
	}else{
	  printf(">>>>>>>>>>ERROR<<<<<<<<<<\n");
	}___________________________________________________________________________________________-\n");
	printf(">>>>>>>>>>Ranking<<<<<<<<<<\n");
	p____f("You got %d/%d.\n", level, sum);
	 if(level==1){
	  p____f("You are a human!!!?");
	}else if(level==2){
	  printf("You are Challenger!!!");
	}else if(level==3){
	  p____f("You are Master!!!!");
	}else if(level==4){
	  printf("You are Legend!!!!!");
	}else if(level==5){
	  ______("You are Champion!!!!!!!");
	}else{
	  _____f("You are a baby boy!!??");
	}
}
```
Test case:
เมื่อใส่อะไรที่ไม่ใช่ y,Y/N,n ต้องเป็นตามรูปนี้
```
Enter your name:  tae
Welcome to the game {C}adventure >>>tae<<<. <3<3<3
This game is about learning c language.

>>>Now you have level <0>.
Want to start a game. [y:n]? u
>>>>>>>>>>ERROR<<<<<<<<<<
---------------------------------------------Finis---------------------------------------------
>>>>>>>>>>Ranking<<<<<<<<<<
You got 0/0.
You are a baby boy!!??   
```


เมื่อจะไม่เล่นเกมนี้ก็ใส่ n,N จะได้ผลตามรูปนี้
```
Enter your name:  tae
Welcome to the game {C}adventure >>>tae<<<. <3<3<3
This game is about learning c language.

>>>Now you have level <0>.
Want to start a game. [y:n]? n
>>>>>>>>>>GAME OVER!!!<<<<<<<<<<
---------------------------------------------Finis---------------------------------------------
>>>>>>>>>>Ranking<<<<<<<<<<
You got 0/0.
You are a baby boy!!??   
```



เมื่อต้องการเล่นเกมนี้ก็ใส่ y,Y และเมื่อตอบถูกจะได้คะแนนและขึ้นตามรูปนี้
```
Enter your name:  tae
Welcome to the game {C}adventure >>>tae<<<. <3<3<3
This game is about learning c language.

>>>Now you have level <0>.
Want to start a game. [y:n]? y
Start Question
1.What is the file extension of the C language?
a. .CPP
b. .C
c. .OBJ
d. .BAS
>>>>>Answer is?  
```




เมื่อตอบอะไรมาก็ไม่รู้ ไม่มีอยู่ในตัวเลือกก็จะขึ้นแบบนี้
```
Enter your name:  tae
Welcome to the game {C}adventure >>>tae<<<. <3<3<3
This game is about learning c language.

>>>Now you have level <0>.
Want to start a game. [y:n]? y
Start Question
1.What is the file extension of the C language?
a. .CPP
b. .C
c. .OBJ
d. .BAS
>>>>>Answer is?  o
>>>>>>>>>>ERROR<<<<<<<<<<<<<
```

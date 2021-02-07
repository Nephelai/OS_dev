## NASK

Nask는 NASM이란 assembler를 바탕으로 최적화가 이루어진 assembler

### DB (Data Byte)

1byte를 직접 쓰는 CMD

문자열을 사용할 경우 문자에 해당하는 데이터를 채워준다.

### RESB (Reserved Byte)

<RESB 10> 처럼 쓰이며 해당 byte 만큼 reserved 처리, 해당 부분을 0x00으로 채운다.

### DW (Data Word), DD (Data Double-Word)

각각 2btye, 4byte를 의미

### $

앞에 총 몇바이트가 있는지 알려주는 변수

<RESB 200 - $> 처럼 쓰이며, 앞에는 건드리지 않으며 200 byte까지 0x00으로 채운다.

### ORG

이 기계어가 실행 시에 PC의 메모리 내 어디에 Loading이 되는지를 nask에 알려주기 위한 CMD

$의 의미 또한 ORG 사용시 달라진다. 시작이 ORG의 지정한 부분이 된다.

### JMP (jump)

goto CMD, 메모리 점프

### Label

Label이란 CMD가 아니라. <entry: > 처럼 쓰인다.

### MOV

대입 CMD <MOV A, B> 'A에 B를 넣어라' 라는 의미

---

### 
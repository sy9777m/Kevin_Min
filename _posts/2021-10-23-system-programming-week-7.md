---
toc: true
layout: post
description: Soongsil University 2-2 System Programming week 7.
categories: [markdown]
title: System Programming week 7
---
# System Programming week 7

## Memory layout

![image-20211023220301091](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023220301091.png)

이런 주소들은 사실 가상 메모리 주소

![image-20211023220633873](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023220633873.png)

![image-20211023220710523](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023220710523.png)

## Buffer overflow

![image-20211023220819305](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023220819305.png)

![image-20211023221014528](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023221014528.png)

### Such problems are a big deal

![image-20211023221327278](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023221327278.png)

### String library code

![image-20211023221442145](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023221442145.png)

### Vulnerable buffer code

![image-20211023221721448](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023221721448.png)

### Buffer overflow disassembly

![image-20211023221812079](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023221812079.png)

### Buffer overflow stack

![image-20211023221849264](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023221849264.png)

![image-20211023222129261](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023222129261.png)

![image-20211023222138610](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023222138610.png)

00은 문자열의 끝을 표시

![image-20211023222145796](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023222145796.png)

![image-20211023222201006](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023222201006.png)

![image-20211023222326923](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023222326923.png)

### Code injection attacks

![image-20211023222345731](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023222345731.png)

### Exploits based on buffer overflows

![image-20211023222531305](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023222531305.png)

### Example: the original internet worm

![image-20211023222647027](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023222647027.png)

### Example: IM War

![image-20211023222748812](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023222748812.png)

![image-20211023222905522](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023222905522.png)

### Aside: Worms and Viruses

![image-20211023223020111](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023223020111.png)

## What to do about buffer overflow attacks

### Avoid overflow vulnerabilities  in code

![image-20211023223131350](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023223131350.png)

### System-level protections can help

![image-20211023223159861](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023223159861.png)

![image-20211023223329811](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023223329811.png)

### Stack canaries can help

![image-20211023223446845](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023223446845.png)

![image-20211023223621936](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023223621936.png)

#### Setting up canary

![image-20211023223636524](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023223636524.png)

![image-20211023223817021](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023223817021.png)

### Return-oriented programming attacks

![image-20211023223827063](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023223827063.png)

## Attack lab

![image-20211023224310021](/Kevin_Min/images/2021-10-23-system-programming-week-7/image-20211023224310021.png)

## Attack Lab

**1. 1****단계 문제** 

   (1) 문제 기술 

함수가 실행될 때 메모리는 정해진 역할에 따라 구획을 나눈다. 이 때 return address를 담을 공간을 할당하고 padding을 두고 local data를 쌓을 stack의 시작점을 지정한다. 함수가 실행되면서 local data는 쌓이고, stack은 return address를 향해 자란다. (작은 주소에서 큰 주소로 자란다) 그러나 이 padding보다 큰 길이의 local data가 쌓일 경우 다른 용도로 할당된 메모리 공간(return address가 담길 자리)을 침범하면서 segmentation fault, buffer overflow가 발생한다.

이번 문제는 stack에 할당된 padding보다 긴 데이터를 받아 buffer overflow를 발생시키고, 그 데이터에 실행하고자 하는 함수(touch 1)의 주소를 담아 return address를 담기로 할당했던 메모리에 해당 함수의 memory address를 담아 실행하는 문제이다.

   (2) 해답 

  ![그림입니다.  원본 그림의 이름: CLP000066c80002.bmp  원본 그림의 크기: 가로 679pixel, 세로 183pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp67BF.jpg)  

   (3) 분석 

  ![그림입니다.  원본 그림의 이름: CLP000066c80003.bmp  원본 그림의 크기: 가로 580pixel, 세로 132pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp67D0.jpg)  

objdump를 통해 assembly 코드를 확인해본 결과 %rsp에 24(0x18)bytes만큼의 padding을 설정하고(sub $0x18, %rsp), %rdi를 %rsp에 할당해주고, Gets 함수를 호출한다. 따라서 %rdi에 24bytes 만큼의 stack이 할당됐고, buffer overflow를 발생시키기 위해서는 24bytes 초과의 dummy 데이터를 Gets를 통해 전달하면 된다.

  ![그림입니다.  원본 그림의 이름: CLP000066c80011.bmp  원본 그림의 크기: 가로 734pixel, 세로 165pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp67D1.jpg)  

touch1 함수를 실행하는 것이 목적이므로 return address 담는 %rsp에 touch1 함수의 memory address(00000000004017e6)를 주면 된다. 따라서 24bytes 크기의 dummy data로 padding을 가득 채우고, 이후 touch 1의 memory address를 삽입하여 데이터를 구성했다.

Gets 함수는 해당 데이터를 읽으면서 padding을 dummy data로 가득 채우게 되고, %rsp(return address가 담길 공간)을 침범하여 해당 공간에 touch1 함수의 memory address를 담게 된다. 따라서 getbuf 함수가 값을 return할 때 %rsp를 참조하게 되면서 touch1 함수가 실행된다.

dummy data는 00 24개로 구성했고, little endian을 감안하여 dummy data 이후 줄 바꿈을 하고 memory address를 역순으로 삽입했다.

  ![그림입니다.  원본 그림의 이름: CLP000066c80002.bmp  원본 그림의 크기: 가로 679pixel, 세로 183pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp67E1.jpg)  

   (4) 실행결과 

  ![그림입니다.  원본 그림의 이름: CLP000066c80002.bmp  원본 그림의 크기: 가로 679pixel, 세로 183pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp67E2.jpg)  

**2. 2****단계 문제** 

   (1) 문제 기술

1단계와 마찬가지로 buffer overflow를 통해 원하는 코드를 실행하여 결과를 얻는 문제다. 차이는 바로 원하는 코드를 바로 실행하는 것이 아니라 중간 작업을 하고 난 뒤에 함수를 실행하는 것이다. buffer overflow를 통해 중간 작업(comparison 통과를 위한 값을 cookie로 할당)을 수행하고, touch2를 실행하여 comparison 연산을 통과하는 것이다.

   (2) 해답 

  ![그림입니다.  원본 그림의 이름: CLP000066c8000c.bmp  원본 그림의 크기: 가로 571pixel, 세로 49pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp67F3.jpg)  

   (3) 분석 

1단계는 return 받는 값을 내가 원하는 함수의 주소로 설정해서 해당 함수를 실행하는 것이라면, 2단계는 return 받는 값을 내가 원하는 함수를 실행하기 전에 해야 작업을 하는 주소로 설정해서 해당 작업을 끝내면 내가 원하는 함수가 실행하도록 하는 문제다.

1단계: buffer overflow -> touch1 실행

2단계: buffer overflow -> 작업 -> touch2 실행

해야 하는 작업은 touch2에서 진행되는 input argument와 cookie 값의 비교연산을 통과하기 위해 input argument를 cookie 값으로 바꿔주는 것이다.

먼저 cookie의 값을 확인했다.

  ![그림입니다.  원본 그림의 이름: CLP000066c80012.bmp  원본 그림의 크기: 가로 155pixel, 세로 32pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp6804.jpg)  

buffer overflow를 통해 return address 자리에는 해당 작업을 수행하는 함수의 주소를 넣어줘야 한다. 그러나 그 작업이 함수를 호출하는 형태로 구현되지 않는다. buffer overflow를 일으키기 위해 stack에 해당 작업을 수행하는 코드를 담아서, buffer overflow가 일어난 getbuf 함수가 반환하는 return의 값이 stack의 맨 처음으로 돌아가도록 구현한다. 이 때 맨 처음으로 돌아가면 우리가 원하는 중간작업을 수행하게 되고, 그 작업이 끝나면 touch2 함수를 실행하는 것이다.

  ![그림입니다.  원본 그림의 이름: CLP000066c80006.bmp  원본 그림의 크기: 가로 898pixel, 세로 410pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp6805.jpg)  

2단계를 pass하기 위해서는 중간에 있는 비교연산을 통과해야 한다. (cmp %edi, 0x202cfc(%rip)) edi값을 cookie 값으로 바꿔줘야 한다. 이는 attck lab instruction(pdf)을 따라 수행했으며 다음과 같이 작성했다. (2-1의 코드와 섞여있다.)

  ![그림입니다.  원본 그림의 이름: CLP000066c80007.bmp  원본 그림의 크기: 가로 456pixel, 세로 100pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp6815.jpg)  

%edi에 쿠키 값을 할당해야 했으므로 쿠키 값인 0x754e7ddd를 %edi에 할당하는 코드를 작성했다.

중간작업이 끝나면 touch2 함수를 실행해야 한다. touch2 함수의 memory address를 return 해야 하므로 pushq $0x401812와 retq를 작성했다. 이 해결방법은 구글링과 수업자료, attack lab instruction에서 해답을 찾았다.

  ![그림입니다.  원본 그림의 이름: CLP000066c80008.bmp  원본 그림의 크기: 가로 650pixel, 세로 319pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp6826.jpg)  

  ![그림입니다.  원본 그림의 이름: CLP000066c80005.bmp  원본 그림의 크기: 가로 586pixel, 세로 209pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp6827.jpg)  

![그림입니다.  원본 그림의 이름: CLP000066c80013.bmp  원본 그림의 크기: 가로 1546pixel, 세로 491pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp6837.jpg)  

pushq를 통해 %rbx를 stack의 최상단에 넣고, ret 전에 popq로 %rbx를 빼낸다. return 값이 따로 없으므로 ret 명령어가 실행되도 stack에서 별도의 return address를 받지 않고 다음으로 넘어간다.

  ![그림입니다.  원본 그림의 이름: CLP000066c80007.bmp  원본 그림의 크기: 가로 456pixel, 세로 100pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp6858.jpg)  

pushq를 이용해서 return하고자 하는 값(touch2의 address, 0x401812)을 stack의 최상단에 넣고, retq는 해당 값을 pop하고 바로 그 address로 이동한다.

이렇게 작성한 assembly 코드를 컴파일 한 뒤 objdump로 disassemble하여 실행코드를 생성했다.

  ![그림입니다.  원본 그림의 이름: CLP000066c8000a.bmp  원본 그림의 크기: 가로 507pixel, 세로 182pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp6868.jpg)  

그리고 이 코드를 ans2.txt에 삽입했다. 1단계와 마찬가지로 24개의 dummy와 return address 영역에 buffer overflow로 들어갈 코드를 입력해야 했다. return address 영역에 넣어줄 코드는 다시 stack의 처음(%rdi)으로 돌아와야 하기 때문에 해당 주소를 넣어야 했는데, 실행 때마다 메모리가 동적으로 할당되어 %rdi에 있는 값과 주소가 계속 바뀌므로 Gets 함수 실행 직전의 %rdi 주소를 알아내야 했다.

gdb를 통해 debug를 진행했고, 아래와 같이 알아냈다.

  ![그림입니다.  원본 그림의 이름: CLP000066c8000b.bmp  원본 그림의 크기: 가로 624pixel, 세로 497pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp6879.jpg)  

getbuf 함수에 breakpoint를 걸고, ni로 함수 내부까지 한 줄 한 줄 실행해서 내려가면서 Type string:을 힌트로 이 때 Gets 함수가 호출되었음을 확인했다. 그리고 info reg rdi 명령어를 통해 이 때의 rdi address를 알아냈다. 이 주소를 buffer overflow를 통해 segmentation fault를 낼 return address 자리에 넣어줬다.

  ![그림입니다.  원본 그림의 이름: CLP000066c8000c.bmp  원본 그림의 크기: 가로 571pixel, 세로 49pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp687A.jpg)  

그렇게 실행하여 테스트에 통과했다.

   (4) 실행결과 

  ![그림입니다.  원본 그림의 이름: CLP000066c8000d.bmp  원본 그림의 크기: 가로 688pixel, 세로 185pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp688B.jpg)  

**2. 2_1****단계 문제** 

   (1) 문제 기술 

2단계 문제와 모든 것이 같으나 차이점은 cookie와 비교하는 것이 아니라 내가 두 값을 할당해서, 두 값을 비교하는 것이다.

   (2) 해답 

  ![그림입니다.  원본 그림의 이름: CLP000066c8000e.bmp  원본 그림의 크기: 가로 570pixel, 세로 49pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp689B.jpg)  

   (3) 분석 

2단계에서는 cookie와 비교연산을 했고, 그 비교를 위한 argument를 내가 할당하는 방식이었다. 이번 2_1단계에서는 내가 두 값을 모두 할당해야 하고, 비교연산이 일어나는 레지스터가 무엇인지 알아내 두 값을 똑같은 값으로 할당하도록 코드만 변경하면 된다.

  ![그림입니다.  원본 그림의 이름: CLP000066c8000f.bmp  원본 그림의 크기: 가로 803pixel, 세로 385pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp689C.jpg)  

comp %esi, %edi 연산을 확인하고, 2단계를 해결한 코드 (shell.s)에서 %esi에 값을 할당하는 연산을 추가하여 disassemble 과정을 통해 코드를 추출하고, 해당 코드를 똑같이 getbuf의 stack에 쌓아주어 실행하였다.

  ![그림입니다.  원본 그림의 이름: CLP000066c80007.bmp  원본 그림의 크기: 가로 456pixel, 세로 100pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp68AD.jpg)  

  ![그림입니다.  원본 그림의 이름: CLP000066c8000a.bmp  원본 그림의 크기: 가로 507pixel, 세로 182pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp68AE.jpg)  

  ![그림입니다.  원본 그림의 이름: CLP000066c8000e.bmp  원본 그림의 크기: 가로 570pixel, 세로 49pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp68BE.jpg)  

   (4) 실행결과

  ![그림입니다.  원본 그림의 이름: CLP000066c80010.bmp  원본 그림의 크기: 가로 699pixel, 세로 182pixel](/Kevin_Min/images/2021-10-23-system-programming-week-7/tmp68BF.jpg)  

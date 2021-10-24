---
toc: true
layout: post
description: Soongsil University 2-2 System Programming week 7.
categories: [markdown]
title: System Programming week 7
---
# System Programming week 7

## Memory layout

![image-20211023220301091](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023220301091.png)

이런 주소들은 사실 가상 메모리 주소

![image-20211023220633873](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023220633873.png)

![image-20211023220710523](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023220710523.png)

## Buffer overflow

![image-20211023220819305](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023220819305.png)

![image-20211023221014528](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023221014528.png)

### Such problems are a big deal

![image-20211023221327278](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023221327278.png)

### String library code

![image-20211023221442145](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023221442145.png)

### Vulnerable buffer code

![image-20211023221721448](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023221721448.png)

### Buffer overflow disassembly

![image-20211023221812079](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023221812079.png)

### Buffer overflow stack

![image-20211023221849264](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023221849264.png)

![image-20211023222129261](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023222129261.png)

![image-20211023222138610](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023222138610.png)

00은 문자열의 끝을 표시

![image-20211023222145796](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023222145796.png)

![image-20211023222201006](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023222201006.png)

![image-20211023222326923](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023222326923.png)

### Code injection attacks

![image-20211023222345731](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023222345731.png)

### Exploits based on buffer overflows

![image-20211023222531305](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023222531305.png)

### Example: the original internet worm

![image-20211023222647027](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023222647027.png)

### Example: IM War

![image-20211023222748812](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023222748812.png)

![image-20211023222905522](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023222905522.png)

### Aside: Worms and Viruses

![image-20211023223020111](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023223020111.png)

## What to do about buffer overflow attacks

### Avoid overflow vulnerabilities  in code

![image-20211023223131350](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023223131350.png)

### System-level protections can help

![image-20211023223159861](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023223159861.png)

![image-20211023223329811](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023223329811.png)

### Stack canaries can help

![image-20211023223446845](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023223446845.png)

![image-20211023223621936](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023223621936.png)

#### Setting up canary

![image-20211023223636524](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023223636524.png)

![image-20211023223817021](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023223817021.png)

### Return-oriented programming attacks

![image-20211023223827063](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023223827063.png)

## Attack lab

![image-20211023224310021](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-10-23-system-programming-week-7\image-20211023224310021.png)


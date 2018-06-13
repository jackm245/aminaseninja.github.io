---
title: Base 10, Base2 and Base 15
layout: post
author: jack.morgan2
permalink: /base-10,-base2-and-base-15/
source-id: 1j45vPdddArArbeX5tdacHAfVam1ehwsRzCm5HxT8nz4
published: true
---
In the third lesson of the Computer Science GCSE course, I have taken a step into converting our decimal (Base 10) to the computer methods of counting, binary (Base 2) and hexadecimal (Base 16).

We were looking at how each of the bases can be converted between each other and the usefulness of counting in Binary.

The reason computers use binary is because they operate on the basis of an electrical signal being on(1) or off(0).

Converting Binary to decimal is a matter of multiplying each 1 or 0 by 128,64,32,16,8,4,2,1 as an eight digit binary number reads from left to right. If the binary was less than eight digits long, you would adjust so that the last digit is multiplied by 1.

Converting Decimal to binary means working out which of 128,64,32,16,8,4,2,1 add together to get the decimal number. If you need one of the numbers from the list, you mark its position in the list with a 1. If you don't need it, mark it with a 0

Converting Hex to decimal means multiplying the first number of the Hex number by 16 and the second number by 1

Converting Decimal to hex means dividing the decimal by 16 and writing that as the first number and writing the remainder (in Hex) as the second number.

One thing you will notice is that 1 0 in any base is the base number. For example 10 in Base 10 is 10, 10 in base 2 is 2, 10 in base 273 is 273.


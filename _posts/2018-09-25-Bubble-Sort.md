---
title: Bubble Sort
layout: post
author: jack.morgan2
permalink: /bubble-sort/
source-id: 1c1yg9AJ5Xi80QhGGXkb1pqzidknI2c0Sg0sacAQMJeI
published: true
---
from colorama import Fore

swap = 1

index = 0

sort_list = []

my_list=[1,2]

for i in my_list:

 while True:

   new_number = input(Fore.WHITE + "please enter a number:")

   try:

     a = int(new_number)

     sort_list.append(a)

     break

   except ValueError:

     print (Fore.RED + "enter a number this time!")

while sort_list[len(sort_list)-1] != 000:

   while True:

     new_number = input(Fore.WHITE + "and another, or 000 to finish:")

     try:

       a = int(new_number)

       sort_list.append(a)

       break

     except ValueError:

       print (Fore.RED + "enter a number this time!")

del (sort_list[len(sort_list) -1])

while swap == 1:

 swap = 0

 for i in sort_list:

   if sort_list[index] > sort_list[index+1]:

     (sort_list[index],sort_list[index+1])=(sort_list[index+1],sort_list[index])

     swap  =1

   index +=1

   if index == len(sort_list) -1:

     index = 0

print (Fore.WHITE + "in ascending order :")

for x in sort_list:

 print (x,end=" ")


---
title: Cryptography Lesson 2
layout: post
author: jack.morgan2
permalink: /cryptography-lesson-2/
source-id: 1Hp_dHe0uOWvo8K1GjVV5zirXILYZVOWQfRDi5SCoP0w
published: true
---
<table>
  <tr>
    <th class="orange">Title</th>
    <td>Cryptography Lesson 2</td>
    <th class="orange">Date</th>
    <td>15/11/17</td>
  </tr>
</table>


<table>
  <tr>
    <th class="orange">Starting point:</th>
    <td>I have created a simple caesar cipher </td>
  </tr>
  <tr>
    <th class="orange">Target for this lesson?</th>
    <td>To add a "breakout" section to my spreadsheet.</td>
  </tr>
  <tr>
    <th class="orange">Did I reach my target? 
</th>
    <td>Yes, I have completed my task, perfected it, debugged it and advanced onto some extension work</td>
  </tr>
</table>


<table>
  <tr>
    <th class="orange">Lesson Review</th>
  </tr>
  <tr>
    <th class="orange">Lesson Recap</th>
  </tr>
  <tr>
    <td>"What is cryptography?" We started talking about different types of ciphers like the Caesar Cipher. This is where every letter is shifted along the alphabet by 5. So instead of going “ABC” it would become “FGH” or” Hello” would become “Mjqqt”. We also looked briefly at the enigma code. The enigma code was a code that changed every day, so therefore, it was hard to break. However, if you look for the three most common letters in the alphabet : e t and a , then it becomes easier to try and crack a code. 
<br>
If you still do not understand what cryptography is, then here is a video from the Scishow on youtube about it:</td>
  </tr>
  <tr>
    <th class="orange">How did I learn? What strategies were effective? </th>
  </tr>
  <tr>
    <td>
Our lesson today was to create a part to our spreadsheet where we type in a sentence into 1 cell. We then have to separate each letter into a separate cell. Then we encode these cells into an encrypted message. We then have to translate this. We then take this translation and turn a 20 cell code (1 letter per cell) and combine these cells into a sentence into one cell.
<br>
We started off by making a plain text cell, this is where the user types in their code that they want encrypted.  I then use the len() function to determine the length of the sentence. Underneath this, I use the left() and right() function. This allows the computer to put each letter in its own cell. However, there is a problem with this. This problem is that the last letter always repeats itself. This is a problem. Therefore, my code looks like this : =if(E$16+1>$J$13, "", RIGHT(left($F$13,E$16+1),1)), The first part shows that if the bx number is more than the length of the text, then put nothing. This stops the last letter from repeating. The second part is about finding the right letter to put in the cell. To fix this repeating problem, I had to use a lot of logical thinking and perseverance. I personally find it very hard to fix problems ny my code, so this was a really big achievement for me. 
<br>
Below this, we have a “Cipher text” section. This encodes the user's message into a caesar cipher shift of 7. My code for this section looks as follows: =if(iserror(vlookup(E$17, OriginalText, 2, false)),"",VLOOKUP(E$17, OriginalText, 2, false)). This may look very complicated, but if you take your time and break it down, then it looks a lot less scary or overwhelming. It basically says, If there is an error , like the user entered in a character that is not in my list, then return nothing. It then looks in my OriginalText range of cells and translate what the user put in.
<br>
 I then concatenate the cells where the encoded text is written. For this, I use the =Concatenate() function. This then puts all of the cells with the encrypted message and puts all of the characters into 1 cell. 
<br>
For example,  ( the [ and ] mark the cell), If I had [h] [e] [l] [l] [o] in 5 cells, It would bring them together to make [hello]. This then makes it easier to read and understand. 

<br>
I think that this lesson, I had to use a lot of logical thinking to overcome the  problems with my code. I also used a lot of perseverance because when I got something wrong, I did not give up, I kept on trying. 

<br>

Here is my spreadsheet so far:
<br>



</td>
  </tr>
  <tr>
    <th class="orange">What limited my learning? Which habits do I need to work on? </th>
  </tr>
  <tr>
    <td>My learning was not limited this lesson, I got on and did all of the set work, and even went beyond that.</td>
  </tr>
  <tr>
    <th class="orange">What will I change for next time? How will I improve my learning?</th>
  </tr>
  <tr>
    <td>I am going to keep on challenging myself and keeping up the good work. 
<br>
Instead of using a Jekyll Blog, I am going to try and create a JQuery blog.</td>
  </tr>
</table>



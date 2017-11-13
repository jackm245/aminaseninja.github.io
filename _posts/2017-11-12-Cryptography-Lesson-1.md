---
title: Cryptography Lesson 1
layout: post
author: jack.morgan2
permalink: /cryptography-lesson-1/
source-id: 1UBCDm8oAy-DMoQUeiBDVlzDsNKEj-1XQiT3Kk0t_Kz4
published: true
---
<table>
  <tr>
    <td>Title</td>
    <td>Cryptography Lesson 1</td>
    <td>Date</td>
    <td>8/11/17</td>
  </tr>
</table>


<table>
  <tr>
    <td>Starting point:</td>
    <td>Before this lesson, I knew that cryptography was about codes and ciphers. However, I didn't know how to create or decipher them</td>
  </tr>
  <tr>
    <td>Target for this lesson?</td>
    <td>To start a spreadsheet where I am to create a caesar cipher.</td>
  </tr>
  <tr>
    <td>Did I reach my target? 
</td>
    <td>Yes, I  have written a code so that you can change the number of shifts, type in a message, and te it gives the encoded version and the decoded version</td>
  </tr>
</table>


<table>
  <tr>
    <td>Lesson Review</td>
  </tr>
  <tr>
    <td>How did I learn? What strategies were effective? </td>
  </tr>
  <tr>
    <td>
We started of this lesson by asking : "What is cryptography?" We started talking about different types of ciphers like the Caesar Cipher. This is where every letter is shifted along the alphabet by 5. So instead of going “ABC” it would become “FGH” or” Hello” would become “Mjqqt”. We also looked briefly at the enigma code. The enigma code was a code that changed every day, so therefore, it was hard to break. However, if you look for the three most common letters in the alphabet : e t and a , then it becomes easier to try and crack a code. 

If you still do not understand what cryptography is, then here is a video from SciShow on youtube about it:


<iframe width="560" height="560" src="https://www.youtube.com/embed/-yFZGF8FHSg" frameborder="0" allowfullscreen></iframe> 

However, our task was to create a cryptography spreadsheet. We started of by making three columns on the left hand side of our spreadsheet. The first column was the Letter that the user typed in. It went from a-z. It was called “Letter”.  The next column was labeled “Ciphertext” in a shift of 7. It started at G, then went all the way to z and then went from a-f. It was in this order: G H I J K L M N O P Q R S T U V W X Y Z A B C D E F. The third column was then again from a-z, it was called “Original”. I then made a named range of the columns Letter and ciphertext and I called  it “CipherText”. I then made a named range of columns “Ciphertext” and “Original” and I called it “OriginalText”. 

I made a row called “Original Text”.I the left a free row under this where the user will type the text that they would like to get encoded. Under this, I made a row called “Cipher text” and again, I left a free row under this where the encoded message will be displayed. And finally, I made a row underneath this where the decoded message will be displayed. 

I have left the “OriginalText' row free because this row is for the user. However, I did add code to the row under that: “CipherText.” I wrote this: “=if(iserror(vlookup(E$4, CipherText, 2, false)),"",VLOOKUP(E$4, CipherText, 2, false)) .” It basically says, If there is an error, then put nothing, and if they put a certain letter, then shift it by 7. 

However, I have thought of another way on how to encode and then decode a message. It uses a character table or ascii table: where every character is given a number. I then let the user enter the number of shifts, and then I add the number of shifts to the original character number. This then gets a new encoded message. You can then subtract the number of shifts from the encoded version to get the original or deciphered text.

I keep the original text row free, I then add : ”=if(iserror(vlookup(E$4, CypherText, 2, false)),"",VLOOKUP(E$4, CypherText, 2, false))” To the encoded row to get the encoded version. I then type: “=if(G17 = "", "", char(code(G17)-G$14) )” To get the decoded version.

On another note, our fabulous teacher had marked our blogs. On the new 1-9 GCSE scale, I was given an 8, the highest in my class. Here was my feedback: “Superb effort in the blogs, well written and lovely design. 
Spreadsheet shows effort and attention to detail. Really well done.” I am really proud of myself and am going to try and keep up the good work.

My improvement point was to create a new Jquery Blog. This is a big challenge, but I hope to complete my task.

Here is my spreadsheet so far:


<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSItZFenbdUkqMxR76Vzmz5hakCE_R96Fum207sZxjcHCRtNGZn1H1gfL3WsllXWb6NVpyuxBKJatqq/pubhtml?widget=true&amp;headers=false" height="400" width="675"></iframe>

</td>
  </tr>
  <tr>
    <td>What limited my learning? Which habits do I need to work on? </td>
  </tr>
  <tr>
    <td>My learning was not limited this lesson, I got on and did all of the set work, and even went beyond that.</td>
  </tr>
  <tr>
    <td>What will I change for next time? How will I improve my learning?</td>
  </tr>
  <tr>
    <td>I am going to keep on challenging myself and keeping up the good work.</td>
  </tr>
</table>



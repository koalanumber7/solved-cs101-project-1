Download Link: https://assignmentchef.com/product/solved-cs101-project-1
<br>
For this project you will read words from a given file into your program. Each word consists strictly of the letters A-Z and a-z. Any whitespace, punctuation, digit, etc. will separate words. An example would be this!is A&amp;Word. This text would represent the 4 words this, is, A, and Word. Each word should be converted to lower case so that only lower case letters remain.

Once you have read all of the words, you should output the total number of words read. Your next task is to determine how many distinct words appear in the file and output that value. Finally, you will prompt the user to enter a word and report how many occurrences of the given word are in the file. You will continue to prompt the user until they enter the EOF character.

When the user enters a word to search for, a ‘?’ character may be present as some of the letters for the search. This special character represents the ability to match any character, including the empty character. For example, colo?r matches both “color” and “colour”. This query should report every word that matches.

Keep in mind that the ? character in the source input file is not a wildcard match.  In the original source, it is just another non-letter character.

<table width="602">

 <tbody>

  <tr>

   <td colspan="3" width="602">There will be no more than 10,000 distinct words in the source file, and when multiple words</td>

  </tr>

  <tr>

   <td colspan="2" width="575">match a query, the results should appear in the order that the result words appear in the</td>

   <td rowspan="2" width="27"> </td>

  </tr>

  <tr>

   <td width="81">original text.</td>

   <td width="494"> </td>

  </tr>

  <tr>

   <td width="81"></td>

   <td width="494"></td>

   <td width="27"></td>

  </tr>

 </tbody>

</table>




<h1>Requirements</h1>

Please carefully read the following requirements:

<ul>

 <li>You must supply a makefile. We will discuss makefiles in class (1/25)</li>

 <li>You must use C++ streams for all I/O</li>

 <li>You must format your output as shown in the example below.</li>

 <li>You must do your own work, you must not share code.</li>

 <li>You must submit your project in a zipfile as specified under submission</li>

</ul>




<h1>Example</h1>

Here is an example document “sample.txt”

Cryptography is both the practice and study of the techniques used to communicate and/or store information or data privately and   securely, without being intercepted by third parties. This can include processes such as encryption, hashing, and steganography. Until the modern era, cryptography almost exclusively referred to encryption, but now cryptography is a broad field with applications in many critical areas of our lives.

You must be able to run the program as shown below and get the identical output

$ make

g++ -Wall -std=c++11 main.c -o project1

$ ./project1 sample.txt

The number of words found in the file was 64

The number of unique words found in the file was 52




Please enter a word: of

The word of appears 2 times in the document




Please enter a word: is

The word is appears 2 times in the document




Please enter a word: or

The word or appears 2 times in the document




Please enter a word: a?d

The word and appears 4 times in the document




Please enter a word: a??

The word and appears 4 times in the document

The word as appears 1 time in the document

The word a appears 1 time in the document




Please enter a word: ^C

$

We highly recommend that you create your own tests to make sure you have covered all possibilities. Those students that do not test their code have a higher chance of having errors during grading.



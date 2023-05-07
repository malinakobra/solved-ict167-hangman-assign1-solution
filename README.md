Download Link: https://assignmentchef.com/product/solved-ict167-hangman-assign1-solution
<br>
Hangman is a game that can be played between two players. One player thinks of a word and the other tries to guess it by suggesting letters. The word to guess is represented by a row of dashes, giving the number of letters in the word. If the guessing player suggests a letter which occurs in the word, the other player writes it in all its correct positions. See <em><a href="https://en.wikipedia.org/wiki/Hangman_(game)" rel="nofollow">http://en.wikipedia.org/wiki/Hangman_(game)</a></em> for further details).

Design, write in Java, test and document a program which will allow a user to play a simplified version of the hangman game. The program will display the secret word in its disguised form (a row of question marks (?), and invite the user to enter an alphabetic letter. If the letter occurs in the secret word, the program will display it in all its correct positions and ask the user to enter another letter as a guess. The process continues until the user guesses the word correctly! The program will also display a running total of the number of guesses made and the number of wrong guesses.

The program will have two classes – a class that could be used to play a simplified version of the hangman game (as described in the above paragraph) and a client class that uses the hangman class.

The hangman class will have at least the following attributes:

<ul>

 <li>The secret word or phrase (a String, which may include embedded white spaces and punctuation characters)</li>

 <li>The disguised word, in which each unknown alphabetic letter in the secret word is replaced with a question mark (?). When an unknown letter is guessed correctly, it will replace the corresponding question mark(s) in the disguised word. For example, if the secret word is <em>abracadabra</em> and the letters <em>a</em> and <em>b</em> have been guessed, the disguised word would be <em>ab?a?a?ab?a</em>.</li>

 <li>The number of guesses made.</li>

 <li>The number of incorrect guesses.</li>

</ul>

The hangman class will have at least the following methods:

<ul>

 <li>makeGuess(ch) guesses that character ch is in the word.</li>

 <li>getDisguisedWord returns a String containing correctly guessed letters in their correct positions and unknown letters replaced with <em>?</em>.</li>

 <li>getSecretWord returns the secret word.</li>

 <li>getGuessCount returns the number of guesses made.</li>

 <li>isFound returns true if the hidden word has been discovered.</li>

</ul>

Devise any additional methods and attributes that are needed in the class and are not listed above. Note that when treating letters of the alphabet, case is not important (i.e., the uppercase and lowercase forms of the same letter are to be treated the same).

Write a client class that tests the hangman class. The client class should allow the user to play three games of hangman. The client class will have the three secret words (or phrases) built into it as String variables. Note that the client class only needs to have the main method which creates an object of the hangman class, sets the secret word and passes control to the hangman class.

<strong>Do not use arrays in this program.</strong>

The test results from the program should be submitted as part of your external documentation.

Your program should also include a method (eg, StudentInfo( )) to output your student details (name, student number, mode of enrolment, tutor name, tutorial attendance day and time) at the start of program output.

Here is some sample output (the user input is in <strong>bold</strong>):

Let’s play a round of hangman.

We are playing hangman

The disguised word is &lt;???????&gt; Guess a letter: <strong>a</strong>

Correct. Guesses made 1 with 0 wrong

The disguised word is &lt;?a?????&gt; Guess a letter:

<strong>7</strong>

Sorry, your guess must be an alphabet character from a to z

Guesses made 1 with 0 wrong

The disguised word is &lt;?a?????&gt; Guess a letter:

<strong>p</strong>

Incorrect. Guesses made 2 with 1 wrong

The disguised word is &lt;?a?????&gt; Guess a letter:

<strong>ha</strong>

Sorry, bad guess. Need a single letter.

Guesses made 2 with 1 wrong

The disguised word is &lt;?a?????&gt; Guess a letter: <strong>h</strong>

Correct. Guesses made 3 with 1 wrong

The disguised word is &lt;ha?????&gt; Guess a letter: <strong>r</strong>

Incorrect. Guesses made 4 with 2 wrong

The disguised word is &lt;ha?????&gt; Guess a letter:

<strong>l</strong>

Correct. Guesses made 5 with 2 wrong

The disguised word is &lt;hal????&gt; Guess a letter:

<strong>s</strong>

Incorrect. Guesses made 6 with 3 wrong

The disguised word is &lt;hal????&gt; Guess a letter: <strong>n</strong>

Correct. Guesses made 7 with 3 wrong

The disguised word is &lt;hal???n&gt; Guess a letter:

<strong>0</strong>

Sorry, your guess must be an alphabet character from a to z

Guesses made 7 with 3 wrong

The disguised word is &lt;hal???n&gt; Guess a letter: <strong>o</strong>

Correct. Guesses made 8 with 3 wrong

The disguised word is &lt;hal??on&gt; Guess a letter: <strong>b</strong>

Incorrect. Guesses made 9 with 4 wrong

The disguised word is &lt;hal??on&gt; Guess a letter: <strong>c</strong>

Correct. Guesses made 10 with 4 wrong

The disguised word is &lt;halc?on&gt; Guess a letter: <strong>y</strong>

Correct. Guesses made 11 with 4 wrong

Congratulations, you found the secret word: halcyon

***************************************************

Let’s play a second round of hangman.

We are playing hangman

The disguised word is &lt;?’?? ?? ????.&gt; Guess a letter: <strong>b</strong>

Correct. Guesses made 1 with 0 wrong

The disguised word is &lt;?’?? b? b???.&gt; Guess a letter:

<strong>9</strong>

Sorry, your guess must be an alphabet character from a to z

Guesses made 1 with 0 wrong

The disguised word is &lt;?’?? b? b???.&gt; Guess a letter:
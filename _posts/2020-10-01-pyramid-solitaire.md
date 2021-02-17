---
layout:     post
title:      Pyramid Solitaire
author:     Zoheb Aziz
categories: Projects
---
![Basic](/assets/BPS.png)

<!--excerpt-->

## About Pyramid Solitaire
Pyramid Solitaire is a an alteration on the ruleset of the original solitaire
game. This project was created in JAVA using the Model-View-Controller design
pattern for my Object Oriented Design course. This iteration of Pyramid Solitaire
has a text based display and interacts with the user through text based inputs
read from the console.
## Features
Pyramid Solitaire project offers 3 different game modes each with its unique
style. Different game mods can be chosen upon launch of application through
command line arguments\
\
<Strong>Basic Pyramid Solitaire</Strong>:\
The classic pyramid solitaire rule set and gameplay. The goal is to remove all of
the cards from the pyramid. The size of the pyramid and the number of draw cards
at the disposable of the player is customizable via command line arguments.\
\
<Strong>Relaxed Pyramid Solitaire</Strong>:\
A variation on the Basic ruleset that offers a more beginner friendly experience
for the user. The game allows the user to remove cards even if they are 'partially
exposed' rather than having to fully expose a card in order to remove it from the
pyramid.\
\
<Strong>Multipyramid Solitaire</Strong>\
This is a variation on the view of the game. There are 104 cards in play rather
than the standard 52 and there are now three 'peaks' to the pyramid rather than just
one. This spinoff game mode allows for some variation in the classic display of
the game as well as a tougher variation for pyramid solitaire veterans.\
\
![Multipyramid](/assets/MPS.png)
## Creation
Pyramid Solitaire was created using JAVA in the Intellij IDE. I used the Model-
View-Controller design pattern as the mane outline for this project. The Basic
model and standard view were the first parts I created. The controller was then
added and supports any Readable and Appendable to pass inputs into although
the game is best enjoyed using a System console. Next the other two game modes
were implemented through the use of a second model and a second view. Lastly a
factory class and a main class were implemented so that the application would
support command line arguments and be runnable as a .jar application.
## Key Takeaways
* MVC Pattern
* Factory Classes
* Command Line Arguments
* Testing and Debugging  

## Try It Out + How to Play
A downloadable .jar file of the game is included [here](/assets/pyramidsolitaire.jar).
One of 3 game modes can be selected using any of the following as the first
command line argument:
<ul>
  <li>basic</li>
  <li>relaxed</li>
  <li>multipyramid</li>
</ul>
Optionally 2 more arguments may be given. The first will change the number of
rows of the pyramid to create (up to 7) and the second will change the number
of draw cards visible at a time.\
A ruleset of how to play Pyramid Solitaire can be found at:\
<a href="https://www.thesprucecrafts.com/pyramid-solitaire-card-game-rules-412478">
https://www.thesprucecrafts.com/pyramid-solitaire-card-game-rules-412478</a>\
The commands to play the game are:
<ul>
  <li>rm1 xpos ypos</li>
    <ul>
      <li>Removes a single card at the position x and y position given</li>
    </ul>
  <li>rm2 card1xpos card1xpos card2xpos card2ypos y</li>
    <ul>
      <li>Removes 2 cards at the x and y positions given</li>
    </ul>
  <li>rmwd drawcardnumber xpos ypos</li>
    <ul>
      <li>Uses a draw card to remove a card at the draw index and the x and y positions given</li>
    </ul>
  <li>dd drawcardnumber</li>
    <ul>
      <li>Discards a draw card at the draw index given</li>
    </ul>
  <li>q</li>
    <ul>
      <li>Quits game</li>
    </ul>
</ul>
\
Have fun playing!\
\
Source code is available here:\
<a href="https://github.com/zohebaziz/PyramidSolitiare">https://github.com/zohebaziz/PyramidSolitiare</a>

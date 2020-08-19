# Game : Number Guesser
Simple Game for beginners
 
## Inspiration
This app is based on courses by Brad Traversy from Udemy

## What I Did To Make The Project Even Better

## What I learned
* method: parseInt, reload, math.floor, math.random
* property: textContent

- textContent : property of the Node interface represents the text content of the node and its descendants
- reload: method reloads the current URL, like the Refresh button

## Game Function:
- Player must guess a number between a min and a max
- Player gets a certain amount of guesses
- Notify player of guesser remaining
- Notify the player of the correct answer if loose
- Let player choose to play again

## How to build
<strong> [ Step 1. UI & Add Task Items ] </strong>


[ step1. Validation & Winning Case ]

1. define Game values
variable initialize variable min= 1, max -=10, winning Num=2, guessesLeft = 3

(rename class:guess-value -> guess-btn) 
2. UI Elements : define variable 
id:game,  guess-btn, guess-input
class:min-num, max-num, message

3. Assign UI min and max


4.Listen for guess
GuessBtn = add event, after 'click' call function
define guess which is value of guessInput 

if it's not a number or less than min or greater than max
load function setMessage  
: argument are please enter a number between min and max , red


5.define function setMessage
argument are msg, color
assigning - color, msg

6.Check if won
* if guess is equal winningNum
* then, Disable input 
* then, change border color : green
* then, call function set message : winningNum is correct, YOU WIN, green

[step2. Lose Case & Game Over ]
1. else
* guessesLeft = guessesLeft - 1
* if guessesLeft is strict equality (Game Over)
* then, disable input
* then, change border color : red
* then, call function set message : Game Over, you lost. The correct number was winningNum, red
* otherwise, 
  then, change bborder color - red
  then, clear input
  then, call function set message :  guess is not correct, guessesLeft guesses left, red
 2. define function gameOver : argument are won, msg
* paste some codes from if won and change some part
* set text color 
* declare variable color
 - tenary operator: if won is strict equality boolean true 
 then color is green else color is red

* fix codes when won
 - call gameOver: boolean, setMsg: winningNum is correct, YOU WIN
* fix codes woen lost
 - call gameOver: boolean, setMsg: Game Over, you lost. The correct number was winningNum

[step 3. Play again]
1. value of guessBtn is 'play-again'
 - add class 'Play-Again'
* add event - game , after mousedown call function 
  - IF statement
     : if add class 'play-again' at event target 
        then, reloads the current URL
2. set winningNum is equal with function getWinningNum
* define getRandomNum argument are min, max






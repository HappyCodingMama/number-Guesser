ebs생활영어 쉐도잉

let : statement declares a block-scoped local variable, optionally initializing it to a value
textContent : property of the Node interface represents the text content of the node and its descendants
parseInt : function parses a string argument and returns an integer of the specified radix

- radix :  the base of a number system or of logarithms

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
if guess is equal winningNum
then, Disable input 
then, change border color : green
then, call function set message : winningNum is correct, YOU WIN, green

[step2. Lose Case & Game Over ]



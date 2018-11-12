# Psychic-Game
//Variables ====================================

I added the array to hold all the possible letters to be guessed.

Created variables that grab the HTML elements by their Id's.

Added counter variables to keep track of current wins, losses, and guesses. There's a variable with an empty array for letters guessed.
The computerGuess variable will = a letter when the function randomLetter is called.

//Functions ====================================

randonLetter() picks a random letter by running the length of the alphabet array.

resetValues() sets the values back to it's starting default and is called when the player either wins or loses.

A random letter is picked before the game starts.

In the HTML, the start button will call the function called start().

Inside, the document.onkeyup will run the event, which has a variable to define the userInput.

//Main code ====================================

When a key is pressed, it runs the if logic:

If the key pressed is = to the letter the computer guessed, increase the win variable by 1, reset the counter variables, and pick a new random letter

If the key pressed does not equal to the computer guess, subtract 1 from the guesses remaining.

If the number of guess reaches 0, increase loss by 1, reset values, and pick new random letter

Else, push the keys pressed into the variable with the empty array.

The .textContent updates the values before the end of the function.
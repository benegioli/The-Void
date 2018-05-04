# The-Void
All of the files for my website, probably.
<!--
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width">
    <title>(Game)</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
<div class="nav-bar">
    <a class="active" href="index.html">Home     <img src="https://78.media.tumblr.com/84d37feb6eb1701ffb3199fa99c04c64/tumblr_p74rfqc2P31vgxtsho1_1280.png" height="16px"> </a>
    <a href="places-to-visit.html">Places To Visit</a>
    <a href="where-to-eat.html">Where To Eat</a>
    <a href="must-do.html"> Must Do</a>
    <a href="curiosities.html"> Curiosities</a>
    <a href="game.html">(Game)</a>
    <br>
    <br>
    <br>
    <br>
<div class="main">
<div id="guess_display"></div>
<form id="guess_form">
    <br>
    <br>
    <label>Guess a letter:
        <input type="text" id="guess_input">
    </label>
</form>
<div id="guess_status"></div>
<script>
    // Store DOM elements in variables
    var guessForm = document.getElementById("guess_form");
    var guessDisplay = document.getElementById("guess_display");
    var guessInput = document.getElementById("guess_input");
    var guessStatus = document.getElementById("guess_status");
    // Initialize game state variables
    var secretWord = "stracciatella";
    var guessedWord = [];
    var guessedLetters = [];
    for (var i = 0; i < secretWord.length; i++) {
        guessedWord[i] = "_";
    }
    // Returns true if its a correct guess -
    //  if the letter is anywhere in the word
    // Also updates guessedWord and guessedLetters
    var checkLetterGuess = function(letter) {
        var bool = false;
        for (var i = 0; i < secretWord.length; i++) {
            if (secretWord.charAt(i) === letter) {
                guessedWord[i] = letter;
                bool = true;
            }
            guessedLetters.push(letter);
        }
        return bool;
    };
    // Returns true if they guessed the whole word
    var hasWon = function() {
        for (var i = 0; i < secretWord.length; i++) {
            if (secretWord.charAt(i) === guessedWord[i]) {/*return true;*/
            }
        }
    };
    var displayGuessedWord = function() {
        guessDisplay.innerHTML = guessedWord.join(" ");
    };
    guessForm.addEventListener("submit", function(event) {
        event.preventDefault();
        var foundLetter = checkLetterGuess(guessInput.value);
        if (foundLetter) {
            guessStatus.innerHTML = "Yay you got one :)";
        } else {
            guessStatus.innerHTML = "Nope, try again :)";
        }
        if (hasWon()) {
            guessStatus.innerHTML += "WOOO WINNER WINNER!";
        }
        displayGuessedWord();
        guessInput.value = "";
    });
    displayGuessedWord();
    // Step 0: Read through the code and understand it
    // Step 1: Implement guessLetter
    // Step 2: Implement hasWon
    // Bonus Steps:
    // - Randomly generate a word for each game
    //   by pulling from an array
    // - Come up with a scoring mechanism --
    //    you can declare game over in a # of guesses
    //    or just track number of guesses and display it
    // - Display the letters they've already guessed
    // - Implement error checking for duplicate guesses
    // - Make way cooler win and lose states!
</script>
</div>
</div>
</body>
</html>
-->

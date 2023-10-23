# Pumpkin Puzzler Game

## Game Objective and Rules

Pumpkin Puzzler is a word-guessing game based on the classic "hangman" concept, designed to be both fun and educational. The objective of the game is to guess the hidden word by selecting letters. Here are the rules:

1. You have seven chances to guess the word.
2. Each incorrect guess erases one obstacle between the "pumpkin" and the "trophy."
3. If you guess all the correct letters before running out of chances, you win the game and the pumpkin doesn't claim the trophy.
4. If you guess incorrectly seven times, the pumpkin claims the trophy, and you lose the game.

## Technology Stack Used

The game is built using the following technologies:

- HTML
- CSS
- JavaScript

### Frameworks, Libraries, Programmes and Tools
 - [Balsamiq](https://balsamiq.com/) to design the wireframes
 - The fonts used in the project are imported from [Google Fonts](https://fonts.google.com/)
 - [Eye Dropper](https://eyedropper.org/) extension for Chrome to pick and generate colours for the project
- [Coolors](https://coolors.co/) to generate a colour palette/see how colours worked beside each other
- [Webaim Contrast Checker](https://webaim.org/resources/contrastchecker/) to check the contrast for the colour choices 
- [Adobe Illustrator](https://www.adobe.com/ie/products/illustrator.html) to create the 'monster', trophy and 'obstacle' graphics
- [Font Awesome](https://fontawesome.com/) for the icons used throughout
- Git for version control, using the [Gitpod](https://www.gitpod.io/) terminal to commit to Git and push to GitHub
- [GitHub](https://github.com/) to store the project code and host the live project
- [Chrome Dev Tools](https://developer.chrome.com/docs/devtools/) during development and testing to fix issues with the code and check for responsiveness/different device sizes
- [W3C HTML validator](https://validator.w3.org/) to validate the HTML code
- [W3C CSS Validator](https://jigsaw.w3.org/css-validator/) to validate the CSS code
- [JSHint](https://jshint.com/) to check the quality of and check for errors in the JavaScript code
- [Am I Responsive](http://ami.responsivedesign.is/) to generate the mockup image showing the project on different devices
- [RealFaviconGenerator](https://realfavicongenerator.net/) to convert the PNG graphic into ICO for the favicon


## Testing
### Code Validation
The [W3C Markup Validation Service](https://validator.w3.org/) was used to validate the HTML on every page of the project. There was an error in relation to using `aria-label="hidden"` instead of `aria-hidden="true"`, this was as a result of human error and was rectified. After fixing this error the code validates with no issue.
>
The [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/) was used to validate the CSS file used for the project. There were no errors found.
>
[JSHint](https://jshint.com/) was used to check the quality of the JavaScript code and check for errors. Apart from `Missing semicolon` errors which were rectified, there was one error:
> 	`Expected an assignment or function call and instead saw an expression` 

The code causing the error was in `script.js` in `function checkLetter()`:
>`isWrongGuess ? handleIncorrectGuess(keyPressed) : handleCorrectGuess(keyPressed);`

This was amended to the `if/else statement` shown below and there is no longer any error.
>`if (wordToGuess.indexOf(keyPressed.innerHTML) === -1) {
        handleIncorrectGuess(keyPressed);
    } else {
        handleCorrectGuess(keyPressed);
    }`


## Setup and Deployment Instructions

The user just needs to access the link which also present in the github directory and paste in the browser. And he can start the game.

To play the Word Monster game, follow these steps:

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/your-username/word-monster-game.git
   ```

2. Open the `index.html` file in your web browser.

3. Start playing the game. Select letters to guess the word and try to beat the monster.

You can also access the live version of the game on [GitHub Pages](https://your-username.github.io/word-monster-game/).

## Credits for Third-Party Assets and Code

The Word Monster game incorporates the following third-party assets and code:

- Fonts imported from [Google Fonts](https://fonts.google.com/)
- Icons provided by [Font Awesome](https://fontawesome.com/)
- Color palette generated with [Coolors](https://coolors.co/)
- Graphics created using [Adobe Illustrator](https://www.adobe.com/products/illustrator.html)

## Reflection :

Pumpkin Puzzler is an educational and nostalgic twist on the classic hangman game. It aims to enhance vocabulary and spelling skills for children, while also providing a fun, retro game experience for adults.

The core mechanics align with hangman, but introduce a friendly Pumpkin character and obstacles rather than a scaffold. This lighthearted approach appeals to both kids and nostalgic adults.

For children, the goal is to learn spelling, expand vocabulary, and get mental exercise through an enjoyable game. For adults, it allows escaping into nostalgia and sharpening language skills.

The simple, one-player format fosters accessibility and collaboration. Users of all ages can grasp the gameplay quickly and participate at their own level.

By balancing educational value and entertainment, Pumpkin Puzzler caters to different user goals. Kids practice spelling and learn new words, while adults stimulate their mind and reminisce.

In summary, creative choices in Pumpkin Puzzler's design make it engaging for both children and nostalgic adults. The game innovates on a classic formula to provide an experience that is both fun and fulfilling for a wide audience.
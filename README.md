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

 - The fonts used in the project are imported from [Google Fonts](https://fonts.google.com/)
 - [Eye Dropper](https://eyedropper.org/) extension for Chrome to pick and generate colours for the project
- [Coolors](https://coolors.co/) to generate a colour palette/see how colours worked beside each other
- [Webaim Contrast Checker](https://webaim.org/resources/contrastchecker/) to check the contrast for the colour choices 
- [Adobe Illustrator](https://www.adobe.com/ie/products/illustrator.html) to create the 'monster', trophy and 'obstacle' graphics
- [Font Awesome](https://fontawesome.com/) for the icons used throughout
- Git for version control.
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
   git clone https://github.com/nsurve180/pumpkin-puzzler.git
   ```

2. Open the `index.html` file in your web browser.

3. Start playing the game. Select letters to guess the word and try to beat the monster.

You can also access the live version of the game on [GitHub Pages](https://github.com/nsurve180/pumpkin-puzzler.git).


## Credits for Third-Party Assets and Code

The Word Monster game incorporates the following third-party assets and code:

- Fonts imported from [Google Fonts](https://fonts.google.com/)
- Icons provided by [Font Awesome](https://fontawesome.com/)
- Color palette generated with [Coolors](https://coolors.co/)
- Graphics created using [Adobe Illustrator](https://www.adobe.com/products/illustrator.html)

## Reflection 

The design and development of the Pumpkin Puzzler game was a rewarding experience that brought with it a set of challenges and valuable lessons. The game's concept, a blend of nostalgia and education, posed both creative and technical hurdles that required a careful balance to curate a positive user experience. 
One of the main challenges we faced during the design and development process was finding the right balance between educational value and entertainment. We wanted Pumpkin Puzzler to be a game that not only enhanced children's vocabulary and spelling skills, but also provided a fun and engaging experience for adults. Striking this balance was imperative, as we did not want the game to feel overly educational and difficult to interpret, nor did we want it to be too simplistic for adults.
To address this challenge, we decided to maintain the core mechanics of the classic hangman game, a game many adults fondly remember playing during their childhood. To make the game different, we introduced a friendly Pumpkin character and obstacles instead of the traditional scaffold, intertwining a lighthearted and visually appealing twist for the game. This approach allowed us to create a game that appealed to both kids and nostalgic adults. It was a critical decision that worked well, as it combined the familiarity of hangman with a fresh perspective and engaging aesthetic.
The design process involved making sure that the game was accessible to users of all ages. We designed a simple, one-player format, ensuring that anyone could quickly grasp the gameplay and participate without any specialty training. The instructions are also provided in the game for player’s reference. This approach worked effectively in making the game more inclusive and user-friendly. The user experience was of paramount importance, and simplicity in design greatly contributed to this. 
The technical development of Pumpkin Puzzler, however, was not without its challenges. Ensuring that the game ran smoothly across various devices and platforms required meticulous attention to detail. We had to optimize graphics and performance to provide a seamless experience. This developed into a colorful and interactive screen display (UX/UI component) and mimics the season of the year–Halloween.
One aspect that worked exceptionally well in the design and development process was our commitment to user goals. We recognized that different age groups had different motivations for playing the game. For children, it was important to incorporate ways to learn and improve their spelling and vocabulary, while adults were looking for a nostalgic experience and mental challenge. By understanding and catering to these distinct goals, we were able to create a game that gave a broad appeal.
One crucial lesson we learned throughout the process was the value of feedback. We conducted several iterations between the group members to determine if the difficulty of word-guessing and hints was simple yet challenging enough for children and adults. This strategy also helped us identify areas that needed improvement, whether it was game difficulty, user interface design, or the overall user experience. Listening to each team members’ feedback and making necessary adjustments was integral to the game's development.
In conclusion, designing and developing Pumpkin Puzzler was a fulfilling journey that required us to navigate the delicate balance between uniqueness, usability and ease of interpretation. We believe the game's unique approach, blending a classic game with a friendly Pumpkin character, will be a successful strategy in appealing to both children and nostalgic adults. Ensuring accessibility and simplicity in design, coupled with responsive user feedback, were key factors that contributed to the game's completion. This project helped enforce the importance of understanding user goals and the significance of user feedback in creating a game that is not only engaging but also valuable in terms of learning and reminiscence.

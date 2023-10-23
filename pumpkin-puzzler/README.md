# Pumpkin  Puzzler
---

[View the live website here]

## Purpose
---
Monster Mash is a game based on the classic 'hangman' game, where the user has to figure out a word by guessing one letter at a time. The game is over when the user has guessed incorrectly 7 times, or when they have revealed the word by guessing all the correct letters. For this version, instead of drawing part of the hangman for each wrong guess (as is the case for the classic version of the game), there is a 'monster' character with obstacles between it and the trophy. Each wrong guess erases an obstacle and the monster claims the trophy on the seventh wrong guess. The reason for using this character instead of the classic hangman is to make it a bit more friendly and light-hearted, bearing in mind the target audience. 

The game is aimed at school-age children as a fun way of helping them to learn words and how they are spelled. It is also designed to appeal to adults in a nostalgic way, since many played hangman as children and the style of the game is reminiscent of old video games.

### User’s goals:
- the game's users want to practice their spelling
- they want to improve their vocabulary
- they want to exercise their brain in a fun way
- they want a fun, nostalgic game to divert attention for a few minutes of their day

### Site owner’s goal:
- the goal of the website is to provide a game for use by school-age children to help with learning the correct spelling of words, and to improve their vocabulary by exposing them to different words in the game. 
- And to provide a game for adults who want to brush up on their spelling and/or vocabulary, or just want to exercise their brain a little bit, or play the game for a few minutes of distraction from daily life.

## User Experience (UX)
---
### User stories
Note: there is no login or registered users on this site so each user story is from the point of view of a visiting user.
1. As a visiting user, I want to find out how to play the game so that I can start to play
2. As a visiting user, I want to be able to select the category from which the random word will be chosen so that I know which type of word it is to help guide my guesses
3. As a visiting user, I want to know how many letters are in the word to be guessed so that I can make a decision on which letters might be in the word
4. As a visiting user, I want to know which letters I have already guessed when playing the game so that I can decide my next guess
5. As a visiting user, I want to know if my guess was correct or not so that I can plan my next guess
6. As a visiting user, I want to see the correctly guessed letters displayed in the correct place in the word, so that I can plan my next guess
7. As a visiting user, I want to know how many chances I have left to guess incorrectly so that I can try to avoid losing the game
8. As a visiting user, I want to be able to get a hint to help me guess the word
9. As a visiting user, I want to know what the word was, if I lose the game, so that I can learn the word or see how it is spelled
10. As a visiting user, I want to know the meaning of the word at the end of the game, regardless of whether I won or lost, so that I can add the word to my vocabulary 
11. As a visiting user, I want to know how many games I have won during this session of playing.
12. As a visiting user, I want to be able to contact the site owners if I come across any issues, have questions on the game or suggestions for improvement.

### Design
The design of the Word Monster site and game takes inspiration from 'old-school' arcade video games like Pac-Man and Space Invaders. The simplicity of the 'hangman' style game is reflected in using the same style of simple graphics from these 80s video games. It also brings a sense of nostalgia for older visitors to the site, who may remember both these old video games, as well as playing the paper and pencil version of 'hangman' when they were children. For children, the simple graphics and bright colours should appeal and stand out in a world of realistic graphics and animations! The design of the game will reflect this through the use of colour, typography and graphics. 
The monster graphic is based on and reminiscent of the characters from Space Invaders and Pac-Man.

 
### Wireframes
  - Desktop/tablet wireframes:
    - [Homepage](docs/wireframes/home-desktop-tablet.png)
    - [Instructions](docs/wireframes/instructions-desktop-tablet.png)
    - [Game in progress](docs/wireframes/game-in-play-desktop.png)
     - [Game over - user won game](docs/wireframes/game-over-won-desktop.png)
    - [Game over - user lost game](docs/wireframes/game-over-lost-desktop.png)
    - [Contact Form](docs/wireframes/contact-form-desktop.png)

  - Mobile wireframes:
    - [Homepage - game not started](docs/wireframes/home-mobile.png)
    - [Instructions](docs/wireframes/instructions-mobile.png)
    - [Game in progress](docs/wireframes/game-in-play-mobile.png)
    - [Game over - user won game](docs/wireframes/game-over-won-mobile.png)
    - [Game over - user lost game](docs/wireframes/game-over-lost-mobile.png)
    - [Contact Form](docs/wireframes/contact-form-mobile.png)
  - [View all wireframes in pdf here.](docs/wireframes/wireframes-all.pdf)
  - Changes from Original Wireframe Designs:
    - In the Header, the Score and Instructions are represented by icons only at smaller screen sizes. 
    - Previous versions of wireframes showed a 2 column layout for the game at larger screen sizes. This layout was developed accordingly, however folowing feedback from my mentor and others, it was decided to keep the one column layout for the game at all screen sizes
    - Originally the website was one page and did not contain a Contact Form. This was added as a feature later in the project and Wireframes were updated. At this point Session Storage was introduced as a feature also, so that Score could be retained when moving between pages.

## Features
---
### Existing Features
- #### Header
  - Top of the page, contains game name on the left, Score and Instructions on the right.
  - Fixed to the top of the page so that score is always visible
  - Instructions: when clicked displays the instructions on how to play the game, X in top right corner to close and return to game page
  - Score: displays a number indicating to the user how many games they have won during this session of playing. Display only, not clickable.
  - Since there is more than one page, session storage to be used to retain the user's score when moving between the Game and the Contact Form/Form Success pages
- #### Game area:
  - Consists of three sections: Monster/guesses section; Word section; Keyboard section. The features of each vary depending on which stage the game is in: not-started, in-play, or over.
  - the full game area should always be visible on the screen without having to scroll down, where possible. This is especially important for mobile screens viewing, for supported devices.
- #### Game area - 'Monster/guesses remaining' section:
  - At the 'not-started' stage of the game there is a 'monster' character and 6 obstacles between it and the trophy icon
  - During the 'in-play' stage, wrong guesses are represented visually by this monster character getting closer to the trophy icon
  - For each wrong guess, one obstacle disappears and the monster moves into its place, thereby getting closer to the trophy
  - On the seventh wrong guess, the trophy disappears, meaning the game has been lost. The game is now in the 'over' state and a message is displayed: "Game Over. You Lost"
  - If the user guessed the letters correctly before the monster gets to the trophy, the game also enters the 'over' state and a message is displayed: "Game Over! You Won the Trophy!". 
- #### Game area - 'Word' section:
  - This subsection contains a text box and a button area, again these change depending on the stage of the game
  - At the 'not-started' stage of the game, the text box instructs user to choose a category from the two buttons below it - Adjective or Verb. These are the word categories from which the random word will be chosen.
  - Once one of these buttons is pressed/clicked on, the game starts and is in the 'in-play' stage
  - The text box now displays the chosen word category, and underneath this it shows a number of dashes representing the letters in the word to be guessed. 
  - When letters are guessed correctly, these are shown in the relevant place in the word, above the dash
  - A Hint button is shown underneath the word to be guessed
  - When the Hint button is clicked, it displays a hint to help the user determine what the word might be. The hint then remains displayed on the page until the game is over
  - When the game enters the 'over' stage, the text box shows a message confirming what the word was and its meaning. 
  - The button is now a "Play Again" button, which re-sets the game back to the 'not-started' stage so that the user can select a category to play a new game
- #### Game area - 'Keyboard' section:
  - This section is below the word to be guessed and contains a keyboard of letters from A to Z
  - The user guesses a letter by pressing/clicking on one of the letters
  - Once a letter has been guessed it cannot be pressed/clicked on again, and it visually displays a different color to show if it was correct or incorrect
  - The keyboard letters are always displayed but are only active when the game is in the 'in-play' stage 
  - *Note:* The use of this keyboard on screen instead of using the keyboard of the device serves two purposes: allowing the keyboard to be enabled or disabled at different stages of the game, and visually displaying the already guessed letters during the game.
- #### Footer:
  - contains the social media links: Facebook, Instagram and Twitter, represented by icons. 
  - on the home page, contains the Contact Us link to the Contact Form page. This link is not shown while the game is in the in-play stage, because leaving the main page would lose progress in the game. 
  - on the Contact Form page and Form Success page, footer contains Back to Game link in place of the Contact Us link


### Future Features
- Extend the range of available word categories to choose from 
- An option to choose the level of difficulty before selecting a category so that harder words are included as the difficulty level increases
- Possibly retrieve the random words from an external resource so that there is a greater selection of words. Not in scope currently due to level of experience of the developer.
- The option for a user to register with a username and have a user profile where they can see their score among other things
- The option to have a Scoreboard showing different user's scores in particular categories/difficulty levels
- The option for a user to be awarded with a 'badge' on successful completion of a certain number of games in a particular difficulty level and particular category. The badge would be added to their profile.
- Add a timer to the game so that it has to be completed in a certain time. Higher scores could be awarded for winning the game in a shorter amount of time

## Content Requirements
---
- Graphic representing the guesses available:
  - pumpkin character
  - icon representing the guesses
  - trophy icon


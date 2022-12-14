# PP3 - Hangman in Python

![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

![Hm logo](favicon.ico)

## About

Hangman Python3 Command Line application. It's a guessing game where the User tries to guess a random  word in a certain number of guesses.

The last update to this file was: **August 22, 2022**

[You can find the live project here](https://hangman-pp3-py.herokuapp.com/)

## Responsiveness

<details><summary>Am i responsive?</summary>

![Am i responsive](readme_images/Am_i_responsive.webp)
</details>

## How to use the App

After the user has registered or logged-in in the main menu the user is brought to the game. A random word from a word bank is generated every new game. The aim is to guess a secret word before spending the 7 lives given. If the user guesses the word before that he/she wins the game, if not the user dies and losses. Find out more about hangman in [wikipedia](https://en.wikipedia.org/wiki/Hangman_(game))

## User Experience (UX)

<details><summary>User stories - as user I want to able to:</summary>

- easy navigate the application

- register and login into the application

- be greeted by my chosen username

- exit the app during registration or login process if I chose so

- be challenged with a different word every time I play the game

- see feedback of my progress during the game

- play again without having to login again

</details>

## Features

<details><summary>Main menu</summary>

- The main menu is displayed when the application starts. Simple an easy to to understand: 1. New user registration  , 2. User login , 3. Exit.

![main menu](readme_images/main_menu.webp)

- Validation message if user enters other that 1,2 or 3.

![main menu validation](readme_images/main_menu_validation.webp)
</details>

<details><summary>Registration </summary>

- User is prompted to enter username and password that meets the requirements.

- Validation message appears if invalid input is entered.

![registration validation](readme_images/register_validation.webp)

- Validation for username already taken.

![username already taken](readme_images/username_already_taken.webp)

</details>

<details><summary>Login</summary>

- The user is prompted to enter his/her login credentials.

![login](readme_images/successful_login.webp)

- User credentials validation

![login validation](readme_images/invalid_login.webp)

</details>

<details><summary>Game menu</summary>

- The user is prompted if he/she wants to play of to quit.

![game menu](readme_images/game_menu.webp)

</details>

<details><summary>Hangman game</summary>

- Features: random word, validates right input, lives countdown, display already guessed words, graphics.

![hangman screenshot](readme_images/hangman.webp)

</details>

## Design

<details><summary>Flow charts</summary>

- ![application flow chart](readme_images/app_flowchart.webp)
- ![game flow chart](readme_images/game_flowchart.webp)

</details>

## Technologies

<details><summary>Languages, External Libraries and Programs Used</summary>

- [Python 3](https://www.python.org/)
  - High level language used to build this project version 3.8.11
- [Random](https://docs.python.org/3/library/random.html?highlight=random%20choice#random.choice)
  - Return a random element from the non-empty sequence.
- [String](https://docs.python.org/3/library/string.html?highlight=string#module-string)
  - The uppercase letters 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'.
- [Time](https://docs.python.org/3/library/time.html?highlight=time%20sleep#time.sleep)
  - From time this app uses sleep to pause between screens.
- [Gspread](https://docs.gspread.org/en/latest/index.html)
  - gspread is a Python API for Google Sheets.
- [Sys](https://docs.python.org/3/library/sys.html?highlight=sys#module-sys)
  - System-specific parameters and functions.
- [Github](https://github.com/)
  - GitHub is the site used to store the source code for the Website.
- [Git](https://git-scm.com/)
  - Git is the  version control software used to commit and push code to the GitHub repository where the source code is stored.
- [Visual Studio Code](https://code.visualstudio.com/)
  - VS Code for short is the integrated development environment (IDE) software used to build the website.
- [Lucid chart](https://www.lucidchart.com/pages/)
  - Lucid chart was used to create flowcharts of the project.
- [Heroku](https://id.heroku.com)
  - Used to deploy the application and provides an environment where the code can be executed.
- [Image converter](https://www.simpleimageresizer.com/)
  - Used to resize the images used in the project.

</details>

## Testing

[PEP8 validator online check](http://pep8online.com)

<details>

<summary> Result for run.py</summary>

- ![PEP8_run.py](readme_images/pep8-run-py.webp)

</details>

<details><summary>Testing table</summary>

- ![testing table](readme_images/test_table1.webp)

- ![testing table](readme_images/test_table2.webp)

</details>

## Bugs

<details><summary>Solved bugs</summary>

- Problem: Registration of the same username multiple times.
  - Fix: Added function that validates if username already exits.
- Problem: Username validation not triggered.
  - Fix: Syntax error in list comprehension.
- Problem: Infinite loop during registration and login.
  - Fix: Add a quit command to exit the loop.
- Problem: Accidentally pushed the users CSV database to Github,
  but the accounts whose passwords were on Github were test accounts.
  - Fix: They have so far been removed.
- Problem: Unable to retrieve CSV users data from Github to Heroku.
  - Fix: Implement Google sheet API as database.

</details>

## Deployment

### How to deploy to Heroku

<details>

<summary>Steps taken to deploy</summary>

- Create an account if necessary and log in.

- Once in the [Heroku](https://id.heroku.com) dashboard, click on New dropdown menu button (top right side) and Create new App.

- On the Create New App page, enter a name for the application and select your region. Then click Create app.

- You will then be brought to the Application Configuration page for your new app.

- Scroll down the Settings page to Buildpacks:
  - Click Add buildpack, select Python from the pop up window and click on Save changes.
  - Click Add buildpack again, select Node.js click on Save changes. It is important that is done in that order Python first, then Node.js beneath.
  - Click on the Deploy tab on the Application Configuration page.
  - Select GitHub as the Deployment Method.
  - Enter your Github username and your Github repository name (in this case [https://github.com/JoseMGuerra/hangman-pp3-py](https://github.com/JoseMGuerra/hangman-pp3-py)) and click on Connect to link up the Heroku app to the GitHub repository code.

- Scroll down the page and there are to options, either Automatically Deploy each time changes are pushed to GitHub, or Manually deploy - for this project Automatic Deploy was selected.

- The application can be run by clicking on the Open App button at the top of the Application Configuration page.

- The live link for this project is [https://hangman-pp3-py.herokuapp.com](https://hangman-pp3-py.herokuapp.com)

</details>

## Resources / Credits / Inspiration

- [Python documentation](https://docs.python.org/3/)
- [Free code camp](https://www.freecodecamp.org/)
- [Stack over flow](https://stackoverflow.com/questions/16060899/alphabet-range-in-python)
- [W3Schools documentation](https://www.w3schools.com/python/default.asp)
- [Geeks for Geeks](https://www.geeksforgeeks.org/python-programming-language/?ref=shm)
- [Love sandwiches project](https://food-market-stock.herokuapp.com/)

## Acknowledgments

- Thank you to my mentor Brian Macharia for guiding me and for his invaluable advice.

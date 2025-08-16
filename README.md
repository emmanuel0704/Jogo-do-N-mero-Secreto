# Secret Number Game

This project is a simple JavaScript game called **"Secret Number Game"**, where the goal is to guess a random number between 1 and 100. The player has several attempts to find the number, and the game provides hints on whether the correct number is higher or lower than the guess. Once the player guesses correctly, they can restart the game.

## Project Structure

The project consists of three main files:

1. **index.html**: Contains the basic layout of the webpage.  
2. **style.css**: Defines the visual styling of the page.  
3. **app.js**: Contains the game logic, such as random number generation and attempt control.  

### index.html
- Main HTML structure with a form that allows the player to input a number.  
- Includes links to Google Fonts, a voice library (ResponsiveVoice.js) for spoken feedback, and the CSS styling file.  
- Two main buttons:  
  - **"Guess"**: To submit a number attempt.  
  - **"New Game"**: To restart the game, disabled until the player guesses the correct number.  

### style.css
- Responsive design with visual adjustments for different screen sizes.  
- Dark gradient background colors.  
- Styled buttons, fonts, and input boxes for a modern interface.  
- Background images with transparency and shadows for a smooth visual effect.  

### app.js
- **Main functions**:  
  - `ExibirMensagemInicial()`: Displays the game title and instructions.  
  - `verificarChute()`: Checks if the entered number matches the secret number. If incorrect, a hint is shown (whether the number is higher or lower). If correct, a success message is displayed and the restart button is enabled.  
  - `gerarNumeroAleatorio()`: Generates the random secret number and ensures the same number is not repeated while the game is active.  
  - `limparCampo()`: Clears the input field after each attempt.  
  - `reiniciarJogo()`: Resets the game with a new secret number and disables the "New Game" button until the next number is guessed correctly.  

## How to Play

1. Enter a number between 1 and 100 in the input field.  
2. Press the **Guess** button to check if you got it right.  
3. If wrong, a hint will be provided indicating whether the secret number is higher or lower.  
4. Keep guessing until you find the number.  
5. Once correct, the **New Game** button will be activated, allowing you to start a new round.  

## Requirements

- A modern browser that supports JavaScript, HTML5, and CSS3.  
- Internet connection to load fonts and the voice library.  

## Customization

- The maximum number value can be changed by modifying the `numeroLimite` variable in the `app.js` file.  
- The design and appearance can be customized in the `style.css` file as needed.  

## Running the Project

Open the `index.html` file in a browser to start playing. The game will run locally without requiring installation or additional dependencies.  

---

This game is a simple and fun way to practice JavaScript, DOM manipulation, and CSS styling.  

Project developed during Alura’s programming logic course.  

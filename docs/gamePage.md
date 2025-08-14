# this is pseudocodes about Rock Paper Scissors Game.

BEGIN

    // 1. Define an object constructor.
    // This object holds the player's choice and the result for one round.
    CONSTRUCTOR GameRound(playerChoice):
        this.playerChoice = playerChoice
        this.computerChoice = null
        this.result = null
    END CONSTRUCTOR

    // 2. Start the main function.
    FUNCTION main():
    
        // Set up the variables.
        DEFINE choices = ["Rock", "Paper", "Scissors"]
        DEFINE userChoice

        // 3. Get a correct input from the user.
        LOOP WHILE userChoice is not one of ("Rock", "Paper", "Scissors"):
            DISPLAY "Enter Rock, Paper, or Scissors:"
            GET userChoice from user

            // 4. Check if the input is correct.
            IF userChoice is not one of ("Rock", "Paper", "Scissors") THEN
                DISPLAY "Invalid input. Please try again."
            END IF
        END LOOP

        // 5. Create a new round for the game.
        DEFINE currentRound = NEW GameRound(userChoice)
        
        // Decide the computer's choice randomly.
        currentRound.computerChoice = random choice from choices

        // Call the function to check who won.
        currentRound.result = determineWinner(currentRound.playerChoice, currentRound.computerChoice)

        // 6. Show the result.
        DISPLAY "You chose: " + currentRound.playerChoice
        DISPLAY "Computer chose: " + currentRound.computerChoice
        DISPLAY "Result: You " + currentRound.result + "!"
        
    END FUNCTION


    // A separate function to decide the winner.
    FUNCTION determineWinner(player, computer):
        IF player == computer THEN
            RETURN "draw"
        ELSE IF (player == "Rock" AND computer == "Scissors") OR 
                (player == "Scissors" AND computer == "Paper") OR 
                (player == "Paper" AND computer == "Rock") THEN
            RETURN "win"
        ELSE
            RETURN "lose"
        END IF
    END FUNCTION

    // Call the main function to start the game.
    CALL main()

END
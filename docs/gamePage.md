# this is pseudocodes about Rock Paper Scissors Game.

Begin
1. Make variables:Rock Paper Scissors
   - "choices" = ["Rock", "Paper", "Scissors"]
   - "yourChoice" = User's input (Rock Paper Scissors)
   - "npcChoice" = Randomly selected choice from choices
   - "result" = output of the game
   
2. Rules:
    - Rock is stronger than Scissors
    - Scissors is stronger than Paper
    - Paper is stronger than Rock
  
3. Ask the user to select one:Rock Paper Scissors. - save the user's choice in a variable: "yourChoice"

4. Use a random method to decides one choice for computer. - save the computer's choice in a variable: "npcChoice"
   
5. Check if the user lose, draw, or win.And store your result into a variable "result"
   - If ("yourChoice" == "Rock" and "npcChoice" == "Scissors") OR 
  ("yourChoice" == "Scissors" and "npcChoice" == "Paper") OR 
  ("yourChoice" == "Paper" and "npcChoice" == "Rock") then "result" ="win"
   - Else if "yourChoice" == "npcChoice", then "result" = "draw"
   - Else, "result" = "lose"

6. Display your result
   - Show "yourchoice", "npcChoice" and "result"

End